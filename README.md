How to use it:

Install Bootstrap: 
	npm install bootstrap@next

Install Bootstrap Icons: 
	npm i bootstrap-icons

Add style to angular.json: 
	"styles": [ "src/styles.css", "node_modules/bootstrap/dist/css/bootstrap.min.css", "node_modules/bootstrap-icons/font/bootstrap-icons.css" ],

Imports in app.module.ts: 
	import { NgModule, LOCALE_ID } from '@angular/core'; 
		import { FormsModule } from '@angular/forms'; 
			import { DatepickerComponent } from './datepicker/datepicker.component';

@NgModule(
	{ declarations: 
		[ DatepickerComponent, ], 
			imports: 
				[ BrowserModule, FormsModule ], 
					providers: 
						[ { provide: LOCALE_ID, useValue: 'pl-PL'} // set polish local ], 
							bootstrap: [AppComponent] }) 
								
export class AppModule { }
