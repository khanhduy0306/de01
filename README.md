```csharp
using System;
using System.Collections;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Data.SqlClient;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace lab1
{
    public partial class Form1 : Form
    {
         "QuanLySVConnection": "Server=DESKTOP-327D948\MSSQLSEVER;Database=QuanlySV;User Id=your_username;"
        public Form1()
        {
            InitializeComponent();
        }
        private void button5_Click(object sender, EventArgs e)
        {
            SqlCommand command = new SqlCommand(query, connection);

            command.Parameters.AddWithValue("@MaSV", txtmaSV.Text);

            command.ExecuteNonQuery();
        }
        LoadSinhvienToDataGridView();
    }
    private void btnThoat_Click(object sender, EventArgs e)
    {
        this.Close();
    }
    private void btnTim_Click(object sender, EventArgs e)
    {

    }
}
}
        }
    }
}
