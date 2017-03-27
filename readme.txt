<record model="ir.ui.view" id="wizard_form_view">
            <field name="name">wizard.form</field>
            <field name="model">test.wizard</field>
            <field name="arch" type="xml">
                <form string="Add Attendees">
                    <group>
                        <field name="session_id"/>
                        <field name="attendee_ids"/>
                    </group>
                    <footer>
                        <button name="subscribe" type="object"
                                string="Subscribe" class="oe_highlight"/>
                        or
                        <button special="cancel" string="Cancel"/>
                    </footer>
                </form>
            </field>
        </record>
        <act_window id="launch_session_wizard"
                    name="Add Attendees"
                    src_model="test.session"
                    res_model="test.wizard"
                    view_mode="form"
                    target="new"
                    key2="client_action_multi"/>111222
