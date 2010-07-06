How to use
==========

Place lib/proxy.rb in your project and require it somewhere from your code.

Usage:
------

require 'lib/proxy'

items = [1, 2, 3, 4]

items_paginator = Pagination::Proxy.new 400, 1, 4
items_paginator.subject = items

items.current_page
==> 1

items.per_page
==> 4

items.next_page
==> 2

items.previous_page
==> nil

items.total_pages
==> 100

etc. Enjoy.
