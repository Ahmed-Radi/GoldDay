#GoldDay

### Files structure
    css
        |css.css
        |mediaquery.css
    images
        |eg-flag
        |logo
    index.html

![navbar](https://user-images.githubusercontent.com/52893501/159471539-8d8b6cfa-0d35-4a81-89a1-b7ffd3f60d66.png)

##### Navbar `HTML`

```
<div class="invoice-header">
            <div class="row">
                <div class="col-lg-6 col-md-6 col-sm-12">
                    <div class="invoice-header__left">
                        <i class="invoice-header__left-icon fa-solid fa-arrow-left-long"></i>
                        <h2>Invoice Browser</h2>
                    </div>
                </div>
                <div class="col-lg-6 col-md-6 col-sm-12 invoice-header__right">
                    <form action="">
                        <label class="form-from" for="from">
                            <span class="form-label">from: </span>
                            <input type="date" id="from" />
                        </label>
                        <label class="form-to" for="to">
                            <span class="form-label">to: </span>
                            <input type="date" id="to" />
                        </label>
                        <button class="submit-btn">submit</button>
                    </form>
                </div>
            </div>
        </div>

```

##### Navbar `CSS`

```
/* Start Navbar */
.navbar {background: var(--navbar-background);}
.navbar-nav {flex-direction: row !important;}
.navbar-nav .nav-item {
    padding-left: 5px;
    display: flex;
}
.navbar-light .navbar-nav .nav-link {
    color: var(--white-color) !important;
}
.navbar-nav .nav-item .nav-link {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
.navbar-nav .nav-item .nav-link span {
    color: var(--white-color);
    font-size: 8px;
}
/* Start user Info */
.left-side {
    display: flex;
    padding-right: 6%;
}
/*Start Menu*/
.navbar-menu {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 5px;
    width: 20px;
    height: 20px;
    cursor: pointer;
    transition: all .5s ease-in-out;
    flex-direction: column;
}
.navbar-menu__btn {
    width: 100%;
    height: 3px;
    background: var(--white-color);
    border-radius: 5px;
    transition: all .5s ease-in-out;
    margin-top: 5px;
}
/*End Menu*/
.user-info {
    display: flex;
    flex-direction: column;
}
.user-info__name {color: var(--white-color);}
.user-info__id {
    color: var(--gray-color);
    font-size: 10px;
}
/*End user Info*/
.nav__icon {
    color: var(--white-color);
    border: 3px var(--border-gold-color) solid;
    border-radius: 50%;
    padding: 5px;
    transition: background 0.9s ease;
}
.nav__icon:hover {
    background-color: var(--background-gold-color);
    transition: background 0.9s ease;
}
.nav__icon-ball {
    color: var(--border-gold-color);
    font-size: 20px;
    padding: 5px;
}
.nav__icon-notification {position: relative;}
.nav__icon-notification::after {
    content: "";
    position: absolute;
    right: -18px;
    top: -31px;
    background-color: red;
    height: 10px;
    width: 10px;
    border-radius: 50%;
}
/* End Navbar */

```

![header-invocation](https://user-images.githubusercontent.com/52893501/159471629-a33bf9cb-e259-49c5-b744-61a7dfba51c9.png)

##### invoice information `HTML`

```
        <div class="tables-container">
            <div class="table-data">
                <table class="table table-data__info">
                    <thead class="table-thead">
                        <tr>
                            <th>Invoice Number</th>
                            <th>Date</th>
                            <th>Transaction Type</th>
                            <th>Metal</th>
                            <th>Quantity in Grams</th>
                            <th>Gross Price/Gram</th>
                            <th>Net Price/ Gram</th>
                            <th>Net Amount</th>
                            <th>Open Invoice*</th>
                        </tr>
                    </thead>
                    <tbody class="table-tbody">
                        <tr>
                            <td>Mark</td>
                            <td>2022-03-16 12:14:53</td>
                            <td>@mdo</td>
                            <td>Mark</td>
                            <td>Otto</td>
                            <td>@mdo</td>
                            <td>Mark</td>
                            <td>Otto</td>
                            <td>@mdo</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <div class="table-data">
                <table class="table table-data__info">
                    <thead class="table-thead">
                        <tr>
                            <th>Invoice Number</th>
                            <th>Date</th>
                            <th>Transaction Type</th>
                            <th>Metal</th>
                            <th>Quantity in Grams</th>
                            <th>Gross Price/Gram</th>
                            <th>Net Price/ Gram</th>
                            <th>Net Amount</th>
                            <th>Open Invoice*</th>
                        </tr>
                    </thead>
                    <tbody class="table-tbody">
                        <tr>
                            <td>Mark</td>
                            <td>2022-03-16 12:14:53</td>
                            <td>@mdo</td>
                            <td>Mark</td>
                            <td>Otto</td>
                            <td>@mdo</td>
                            <td>Mark</td>
                            <td>Otto</td>
                            <td>@mdo</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>

```
##### invoice information `CSS`

```
#main-content {
    margin-top: 20px;
    margin-bottom: 20px;
    padding: 10px 20px;
    border: 1px var(--border-gold-color) solid;
    border-radius: 5px;
    overflow: hidden;
}
.invoice-header {
    text-transform: capitalize;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-bottom: 10px;
}
.invoice-header__left {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding-left: 5px;
}
.invoice-header__left-icon {
    color: #fff;
    border: 3px var(--border-gold-color) solid;
    border-radius: 50%;
    padding: 5px;
    margin-right: 10px;
    transition: background 0.9s ease;
    cursor: pointer;
}
.invoice-header__left-icon:hover {
    background-color: var(--background-gold-color);
    transition: background 0.9s ease;
}
.invoice-header__left h2 {
    color: var(--font-gold-color);
    position: relative;
    margin-left: 4px;
    margin-bottom: 0;
}
.invoice-header__left h2::before {
    content: '';
    height: 80%;
    width: 4px;
    margin-left: -8px;
    position: absolute;
    left: 0;
    top: 5px;
    background-color: #ffffff;
}
.invoice-header__right {
    display: flex;
    justify-content: end;
    align-items: center;
}
.form-from input,
.form-to input {
    background-color: transparent;
    border: none;
    color: var(--white-color);
}
.form-label {
    color: var(--font-gold-color);
    font-weight: bold;
}
input#from, input#to {
    width: 140px;
    outline: none;
}
.submit-btn {
    background: transparent;
    color: var(--white-color);
    border: 1px var(--border-color) solid;
    border-radius: 5px;
    padding: 5px 10px;
    text-transform: capitalize;
    transition: background 0.9s ease;
}
.submit-btn:hover {
    background-color: var(--background-gold-color);
    transition: background 0.9s ease;
}
/* tables info section */
.tables-container {
    border-top: 2px var(--border-gold-color) dashed;
    border-bottom: 2px var(--border-gold-color) dashed;
}
.table-data {
    margin: 20px 0;
    padding: 4px;
    border: 2px solid var(--table-background);
    border-radius: 5px;
    overflow-x: scroll;
}
.table-data::-webkit-scrollbar {display: none;}/* remove scrollbar */
.table-data__info {margin: 0 !important;}
.table-thead {background-color: var(--table-background);}
.table-data__info tr {color: var(--white-color);}
.table-data__info tr th,
.table-data__info tr td {
    min-width: 100px;
    position: relative;
}
.table-data__info tr th::before,
.table-data__info tr td::before  {
    content: '';
    top: 5px;
    left: 0;
    height: 80%;
    width: 1px;
    position: absolute;
    background-color: #000;
}
.table-data__info tr td::before {background-color: #707070;}
.table-data__info tr th:first-child::before,
.table-data__info tr td:first-child::before  {height: 0;}
.table-thead th,
.table-tbody td {
    border-bottom: none;
    font-size: 12px;
}
/* End tables info section */

```

![old](https://user-images.githubusercontent.com/52893501/159471689-dcae8767-a271-4766-bdcc-1df0d812c073.png)

##### Older Invoices `HTML`

```
        <div class="container">
            <div class="old-invoices">
                <div class="row">
                    <div class="col-12">
                        <h4>Older Invoices</h4>
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-12">
                        <div class="all-state">
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                            <div class="state">
                                <span>EGT25</span>
                                <span>open</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

```

##### Older Invoices `CSS`

```
/* Start old invoices section */
.old-invoices {margin: 20px 0;}
.old-invoices h4 {
    color: var(--font-gold-color);
    margin-bottom: 20px;
}
.all-state {
    max-height: 400px;
    overflow-y: scroll;
    color: var(--white-color) !important;
}
.all-state::-webkit-scrollbar {width: 10px;}
.all-state::-webkit-scrollbar-thumb:hover {
    border-radius: 5px;
    background: var(--background-gold-color);
}
.state {
    padding: 5px;
    display: flex;
    justify-content: space-between;
}
.state:nth-child(odd) {background: #292929;}
/* End main content*/

```
