package com.testinium.page;

import com.testinium.methods.Methods;
import org.openqa.selenium.By;

public class LoginPage {

    Methods methods;
    public LoginPage(){
        methods = new Methods();
    }

    public void login(){

        //nereden - nereye seçilir.
        methods.click(By.id("OriginInput"));
        methods.click(By.xpath("//li[@id='react-autowhatever-OriginInput-section-1-item-1']"));
        methods.waitBySeconds(3);
        methods.click(By.id("DestinationInput"));
        methods.click(By.xpath("//li[@id='react-autowhatever-DestinationInput-section-1-item-3']"));

        //tek yon checkbox tıkı kaldırılır
        methods.click(By.xpath("//label[@class='oneWayCheckbox']"));
        methods.waitBySeconds(10);


        //gidiş - dönüş tarihi seçilir.
        methods.click(By.xpath("//div[@class='D_FSF__col returnDate__col D_FSF__focused_input']//label[normalize-space(text())='Dönüş Tarihi']"));
        methods.click(By.xpath("(//div[@class='CalendarDay__content' and normalize-space(text())='31'])[2]"));
        methods.waitBySeconds(10);



        //aktarmasız tikine tıklanır.
        methods.click(By.xpath("//input[@id='transitFilter']"));
        methods.waitBySeconds(15);

        //yolcu seçilir.
        methods.click(By.xpath("//button[@class='default-btn block passenger-select-button']"));
        methods.click(By.xpath("//button[@class='base-button active']"));
        methods.click(By.xpath("//button[@class='primary-link-btn']"));
        methods.waitBySeconds(15);

        //ucuz bılet bul butonuna basılır
        methods.click(By.xpath("//button[@class='primary-btn block']//span[normalize-space(text())='Ucuz bilet bul']"));
        methods.waitBySeconds(30);
    }
}
