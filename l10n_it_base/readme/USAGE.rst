In other addons to depend it, it's important to inherit l10n_it_base.mixin model and use in view something like these:

::
   <field name="is_company_it" invisible="1" />
   <field name="custom_field_it" attrs="{'invisible': [('is_company_it','=', False)]}" />
