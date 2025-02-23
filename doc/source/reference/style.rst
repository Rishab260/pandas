{{ header }}

.. _api.style:

=====
Style
=====
.. currentmodule:: pandas.io.formats.style

``Styler`` objects are returned by :attr:`pandas.DataFrame.style`.

Styler constructor
------------------
.. autosummary::
   :toctree: api/

   Styler
   Styler.from_custom_template

Styler properties
-----------------
.. list-table::
   :widths: auto

   * - :attr:`Styler.index` : Index
     - Index of the DataFrame.
   * - :attr:`Styler.columns` : Index
     - Columns of the DataFrame.
   * - :attr:`Styler.env` : jinja2.Environment
     - Jinja2 Environment for template rendering.
   * - :attr:`Styler.template_html` : jinja2.Template
     - Jinja2 Template for rendering `Styler` objects as HTML output.
   * - :attr:`Styler.template_html_style` : jinja2.Template
     - Jinja2 Template for the `<style>` section in the HTML output.
   * - :attr:`Styler.template_html_table` : jinja2.Template
     - Jinja2 Template for rendering HTML tables.
   * - :attr:`Styler.template_latex` : jinja2.Template
     - Jinja2 Template for LaTeX output.
   * - :attr:`Styler.template_typst` : jinja2.Template
     - Jinja2 Template for Typst output.
   * - :attr:`Styler.template_string` : jinja2.Template
     - Jinja2 Template for string representation.
   * - :attr:`Styler.loader` : jinja2.BaseLoader
     - Jinja2 Loader for templates.

Style application
-----------------
.. autosummary::
   :toctree: api/

   Styler.apply
   Styler.map
   Styler.apply_index
   Styler.map_index
   Styler.format
   Styler.format_index
   Styler.format_index_names
   Styler.relabel_index
   Styler.hide
   Styler.concat
   Styler.set_td_classes
   Styler.set_table_styles
   Styler.set_table_attributes
   Styler.set_tooltips
   Styler.set_caption
   Styler.set_sticky
   Styler.set_properties
   Styler.set_uuid
   Styler.clear
   Styler.pipe

Builtin styles
--------------
.. autosummary::
   :toctree: api/

   Styler.highlight_null
   Styler.highlight_max
   Styler.highlight_min
   Styler.highlight_between
   Styler.highlight_quantile
   Styler.background_gradient
   Styler.text_gradient
   Styler.bar

Style export and import
-----------------------
.. autosummary::
   :toctree: api/

   Styler.to_html
   Styler.to_latex
   Styler.to_typst
   Styler.to_excel
   Styler.to_string
   Styler.export
   Styler.use
