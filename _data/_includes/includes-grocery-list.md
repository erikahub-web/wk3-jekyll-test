<!-- display an unordered list of the grocery list data -->
<ul>
{% for item in wk3-jekyll-test.data.grocery-list-data %}
  <li><strong>{{ item.name }}</strong> has type {{ item.type }}</li>
{% endfor %}
</ul>

<!-- display a table of the grocery list data -->
    <thead><th>Item</th><th>Type</thead>
    <tbody>
        {% for item in wk3-jekyll-test.data.grocery-list-data %}
        <tr>
            <td>{{ item.name }}</td>
            <td>{{ item.type }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>