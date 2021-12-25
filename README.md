<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:background="@color/blue"
    tools:context=".MainActivity">

    <FrameLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="@drawable/bg_home_wave">
        <RelativeLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_centerInParent="true"
                android:text="Program penjualan"
                android:textColor="@android:color/white"
                android:textSize="24sp"
                android:textStyle="bold" />
        </RelativeLayout>

    </FrameLayout>

    <ImageView
        android:layout_width="match_parent"
        android:layout_height="37dp"
        android:background="@drawable/header"
        android:backgroundTint="@color/darkblue2" />
    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <LinearLayout
            android:layout_marginLeft="10dp"
            android:layout_marginRight="10dp"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical">
            <com.google.android.material.card.MaterialCardView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_margin="5dp"
                app:cardCornerRadius="10dp"
                app:cardElevation="3dp"
                app:strokeColor="@color/darkblue"
                app:strokeWidth="2dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_marginBottom="10dp"
                    android:background="@drawable/form"
                    android:elevation="10dp"
                    android:gravity="center"
                    android:orientation="vertical"
                    android:outlineAmbientShadowColor="@color/black"
                    android:outlineSpotShadowColor="@color/black"
                    android:padding="10dp">

                    <TextView
                        android:gravity="center"
                        android:layout_marginBottom="10dp"
                        android:textColor="@color/darkblue"
                        android:textStyle="bold"
                        android:textSize="20dp"
                        android:text="Ringkasan"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"/>
                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="10dp"
                        android:gravity="center"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="125dp"
                            android:layout_height="wrap_content"
                            android:paddingLeft="20dp"
                            android:text="Jenis produk"
                            android:textColor="@color/black" />
                        <Spinner
                            android:backgroundTint="@color/darkblue"
                            android:paddingLeft="5dp"
                            android:id="@+id/jenis"
                            android:layout_width="match_parent"
                            android:layout_height="40dp"/>

                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="10dp"
                        android:layout_marginBottom="10dp"
                        android:gravity="center"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="125dp"
                            android:layout_height="wrap_content"
                            android:paddingLeft="20dp"
                            android:text="Nama produk"
                            android:textColor="@color/black" />

                        <EditText
                            android:id="@+id/namabrg"
                            android:layout_width="match_parent"
                            android:layout_height="40dp"
                            android:layout_gravity="end"
                            android:layout_marginRight="20dp"
                            android:layout_weight="1"
                            android:hint="Enter product name"
                            android:inputType="text"
                            android:textAlignment="textEnd"
                            android:textColor="@color/black"
                            android:textColorHint="@color/abu"
                            android:textSize="15dp"
                            android:textStyle="bold" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginBottom="10dp"
                        android:gravity="center"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="115dp"
                            android:layout_height="wrap_content"
                            android:paddingLeft="20dp"
                            android:text="Harga"
                            android:textColor="@color/black" />

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:text="Rp."
                            android:textColor="@color/black"
                            android:textStyle="bold" />

                        <EditText
                            android:id="@+id/hargabrg"
                            android:layout_width="match_parent"
                            android:layout_height="40dp"
                            android:layout_gravity="end"
                            android:layout_marginRight="20dp"
                            android:layout_weight="1"
                            android:hint="Enter product price"
                            android:inputType="numberDecimal"
                            android:textAlignment="textEnd"
                            android:textColor="@color/black"
                            android:textColorHint="@color/abu"
                            android:textSize="15dp"
                            android:textStyle="bold" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginBottom="10dp"
                        android:gravity="center"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="125dp"
                            android:layout_height="wrap_content"
                            android:paddingLeft="20dp"
                            android:text="Jumlah"
                            android:textColor="@color/black" />

                        <EditText
                            android:id="@+id/jumlahbrg"
                            android:layout_width="match_parent"
                            android:layout_height="40dp"
                            android:layout_gravity="end"
                            android:layout_marginRight="20dp"
                            android:layout_weight="1"
                            android:hint="Enter quantity"
                            android:inputType="number"
                            android:textAlignment="textEnd"
                            android:textColor="@color/black"
                            android:textColorHint="@color/abu"
                            android:textSize="15dp"
                            android:textStyle="bold" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginBottom="10dp"
                        android:gravity="center"
                        android:orientation="horizontal"
                        android:padding="2dp">

                        <TextView
                            android:layout_width="115dp"
                            android:layout_height="wrap_content"
                            android:paddingLeft="20dp"
                            android:text="Total"
                            android:textColor="@color/black" />

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:text="Rp."
                            android:textColor="@color/black"
                            android:textStyle="bold" />

                        <TextView
                            android:id="@+id/totalbrg"
                            android:layout_width="wrap_content"
                            android:layout_height="30dp"
                            android:layout_gravity="end"
                            android:layout_weight="1"
                            android:inputType="numberDecimal"
                            android:paddingRight="20dp"
                            android:text=" "
                            android:textAlignment="textEnd"
                            android:textColor="@color/black"
                            android:textStyle="bold" />
                    </LinearLayout>
                </LinearLayout>
            </com.google.android.material.card.MaterialCardView>

            <Button
                android:id="@+id/Total"
                android:layout_marginRight="5dp"
                android:layout_marginBottom="20dp"
                android:textStyle="bold"
                android:textColor="@color/white"
                android:text="Total"
                android:layout_gravity="right"
                android:layout_width="180dp"
                android:layout_height="wrap_content"/>

            <TextView
                android:layout_marginLeft="5dp"
                android:layout_marginBottom="10dp"
                android:textColor="@color/black"
                android:textStyle="bold"
                android:textSize="16dp"
                android:text="Metode Pembayaran"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"/>

            <com.google.android.material.card.MaterialCardView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_margin="5dp"
                app:cardCornerRadius="10dp"
                app:cardElevation="3dp"
                app:strokeColor="@color/darkblue"
                app:strokeWidth="2dp">
            <LinearLayout
                android:layout_marginBottom="10dp"
                android:elevation="10dp"
                android:outlineAmbientShadowColor="@color/black"
                android:outlineSpotShadowColor="@color/black"
                android:orientation="vertical"
                android:gravity="center"
                android:background="@drawable/form"
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <LinearLayout
                    android:gravity="center"
                    android:layout_marginTop="10dp"
                    android:layout_marginBottom="10dp"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="horizontal">
                    <ImageView
                        android:backgroundTint="@color/darkblue"
                        android:layout_marginLeft="10dp"
                        android:background="@drawable/wallet_24"
                        android:layout_width="30dp"
                        android:layout_height="30dp"/>

                    <Spinner
                        android:id="@+id/pembayaran"
                        android:backgroundTint="@color/darkblue"
                        android:layout_width="130dp"
                        android:layout_height="40dp"
                        android:paddingLeft="5dp" />

                    <TextView
                        android:textStyle="bold"
                        android:textColor="@color/black"
                        android:text="Rp."
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"/>
                    <EditText
                        android:inputType="numberDecimal"
                        android:textSize="15dp"
                        android:textColorHint="@color/abu"
                        android:id="@+id/tunai"
                        android:layout_width="match_parent"
                        android:layout_height="40dp"
                        android:layout_gravity="end"
                        android:layout_weight="1"
                        android:hint="Enter the amount of money"
                        android:layout_marginRight="20dp"
                        android:textAlignment="textEnd"
                        android:textColor="@color/black"
                        android:textStyle="bold" />
                </LinearLayout>

            </LinearLayout>
            </com.google.android.material.card.MaterialCardView>

            <Button
                android:textAllCaps="false"
                android:id="@+id/payment"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginBottom="20dp"
                android:layout_marginRight="5dp"
                android:layout_marginLeft="5dp"
                android:text="Selesaikan pembayaran"
                android:textColor="@color/white"
                android:textStyle="bold" />

            <com.google.android.material.card.MaterialCardView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_margin="5dp"
                app:cardCornerRadius="10dp"
                app:cardElevation="3dp"
                app:strokeColor="@color/darkblue"
                app:strokeWidth="2dp">
            <LinearLayout
                android:elevation="10dp"
                android:outlineAmbientShadowColor="@color/black"
                android:outlineSpotShadowColor="@color/black"
                android:layout_marginBottom="10dp"
                android:orientation="vertical"
                android:gravity="center"
                android:padding="10dp"
                android:background="@drawable/form"
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <TextView
                    android:gravity="center"
                    android:layout_marginBottom="10dp"
                    android:textColor="@color/darkblue"
                    android:textStyle="bold"
                    android:textSize="20dp"
                    android:text="Rincian Pembayaran"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"/>
                <LinearLayout
                    android:gravity="center"
                    android:padding="2dp"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="horizontal">
                    <TextView
                        android:paddingLeft="20dp"
                        android:textColor="@color/black"
                        android:text="Total pembayaran"
                        android:layout_width="120dp"
                        android:layout_height="wrap_content"/>
                    <TextView
                        android:textStyle="bold"
                        android:textColor="@color/black"
                        android:text="Rp."
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"/>
                    <TextView
                        android:inputType="numberDecimal"
                        android:id="@+id/totalbayar"
                        android:paddingRight="20dp"
                        android:text=" "
                        android:textStyle="bold"
                        android:textColor="@color/black"
                        android:textAlignment="textEnd"
                        android:layout_gravity="end"
                        android:layout_weight="1"
                        android:layout_width="wrap_content"
                        android:layout_height="30dp"/>
                </LinearLayout>
                <LinearLayout
                    android:padding="2dp"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="horizontal">
                    <TextView
                        android:textSize="11dp"
                        android:textStyle="bold"
                        android:paddingLeft="20dp"
                        android:textColor="@color/black"
                        android:text="PPN 10 %"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"/>
                </LinearLayout>
                <LinearLayout
                    android:gravity="center"
                    android:layout_marginBottom="10dp"
                    android:padding="2dp"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:orientation="horizontal">
                    <TextView
                        android:paddingLeft="20dp"
                        android:textColor="@color/black"
                        android:text="Kembalian"
                        android:layout_width="120dp"
                        android:layout_height="wrap_content"/>
                    <TextView
                        android:textStyle="bold"
                        android:textColor="@color/black"
                        android:text="Rp."
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"/>
                    <TextView
                        android:inputType="numberDecimal"
                        android:id="@+id/kembalian"
                        android:paddingRight="20dp"
                        android:text=" "
                        android:textStyle="bold"
                        android:textColor="@color/black"
                        android:textAlignment="textEnd"
                        android:layout_gravity="end"
                        android:layout_weight="1"
                        android:layout_width="wrap_content"
                        android:layout_height="30dp"/>
                </LinearLayout>

            </LinearLayout>
            </com.google.android.material.card.MaterialCardView>

            <Button
                android:id="@+id/clear"
                android:textAllCaps="false"
                android:textStyle="bold"
                android:textColor="@color/white"
                android:text="Print"
                android:layout_margin="5dp"
                android:gravity="center"
                android:layout_gravity="center"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"/>
            <LinearLayout
                android:layout_marginBottom="50dp"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"/>

        </LinearLayout>
    </ScrollView>

</LinearLayout>
