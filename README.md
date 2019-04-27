# Windows-forms
Pequeña introduccion a windows forms
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que pueda hacer cualquier tipo de operación aritmetica.
        }

        private void button1_Click(object sender, EventArgs e)
        {
            try
            {
                int numero1, numero2, respuesta;
                numero1 = int.Parse(textBox1.Text);
                numero2 = int.Parse(textBox2.Text);

                respuesta = numero1 + numero2;
                Resultado.Text = respuesta.ToString();

            }
            catch
            {
                MessageBox.Show("Error!!!!");
                textBox1.Clear();
                textBox2.Clear();

            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            try
            {
                int numero1, numero2, respuesta;
                numero1 = int.Parse(textBox4.Text);
                numero2 = int.Parse(textBox5.Text);

                respuesta = numero1 - numero2;
                Resultado2.Text = respuesta.ToString();

            }
            catch
            {
                MessageBox.Show("Error!!!!");
                textBox4.Clear();
                textBox5.Clear();

            }

        }

        private void button3_Click(object sender, EventArgs e)
        {
            try
            {
                int numero1, numero2, respuesta;
                numero1 = int.Parse(textBox7.Text);
                numero2 = int.Parse(textBox8.Text);

                respuesta = numero1 * numero2;
                Resultado3.Text = respuesta.ToString();

            }
            catch
            {
                MessageBox.Show("Error!!!!");
                textBox7.Clear();
                textBox8.Clear();

            }
        }

        private void button4_Click(object sender, EventArgs e)
        {
            try
            {
                int numero1, numero2, respuesta;
                numero1 = int.Parse(textBox10.Text);
                numero2 = int.Parse(textBox11.Text);

                respuesta = numero1 / numero2;
                Resultado4.Text = respuesta.ToString();

            }
            catch
            {
                MessageBox.Show("Error!!!!");
                textBox10.Clear();
                textBox11.Clear();

            }
        }

        private void button5_Click(object sender, EventArgs e)
        {
            try
            {
                int numero1, numero2, respuesta;
                numero1 = int.Parse(textBox13.Text);
                numero2 = int.Parse(textBox14.Text);

                respuesta = numero1 % numero2;
                Resultado5.Text = respuesta.ToString();

            }
            catch
            {
                MessageBox.Show("Error!!!!");
                textBox13.Clear();
                textBox14.Clear();

            }
        }

        private void button6_Click(object sender, EventArgs e)
        {
            textBox1.Clear();
            textBox2.Clear();
            Resultado.Clear();

            textBox4.Clear();
            textBox5.Clear();
            Resultado2.Clear();

            textBox7.Clear();
            textBox8.Clear();
            Resultado3.Clear();

            textBox10.Clear();
            textBox11.Clear();
            Resultado4.Clear();

            textBox13.Clear();
            textBox14.Clear();
            Resultado5.Clear();
        }
    }
}
____________________________________________________________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio2
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que el usuario ingrese en una caja de texto  y lo muestre en un mensaje.
        }

        private void button1_Click(object sender, EventArgs e)
        {
            MessageBox.Show(textmensaje.Text);
        }

        private void button2_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }
    }
}
____________________________________________________________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio3
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que concatene varias cajas de texto y las muestre en un mensaje.
        }

        private void button1_Click(object sender, EventArgs e)
        {
            MessageBox.Show(textBox2.Text);
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {
            string limite;
            limite = Console.ReadLine();
        }
    }
}
__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio4
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que por medio de una lista muestre los paises de centro america y muestre las banderas de cada pais.
        }

        private void comboBox1_SelectedIndexChanged(object sender, EventArgs e)
        {
            if (comboBox1.SelectedItem.Equals("Guatemala"))
            {
                pictureBox1.Visible = true;
                pictureBox2.Visible = false;
                pictureBox3.Visible = false;
                pictureBox4.Visible = false;
                pictureBox5.Visible = false;
                pictureBox6.Visible = false;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("Belice"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = true;
                pictureBox3.Visible = false;
                pictureBox4.Visible = false;
                pictureBox5.Visible = false;
                pictureBox6.Visible = false;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("Honduras"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = false;
                pictureBox3.Visible = true;
                pictureBox4.Visible = false;
                pictureBox5.Visible = false;
                pictureBox6.Visible = false;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("El Salvador"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = false;
                pictureBox3.Visible = false;
                pictureBox4.Visible = true;
                pictureBox5.Visible = false;
                pictureBox6.Visible = false;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("Nicaragua"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = false;
                pictureBox3.Visible = false;
                pictureBox4.Visible = false;
                pictureBox5.Visible = true;
                pictureBox6.Visible = false;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("Costa Rica"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = false;
                pictureBox3.Visible = false;
                pictureBox4.Visible = false;
                pictureBox5.Visible = false;
                pictureBox6.Visible = true;
                pictureBox7.Visible = false;
            }

            if (comboBox1.SelectedItem.Equals("Panamá"))
            {
                pictureBox1.Visible = false;
                pictureBox2.Visible = false;
                pictureBox3.Visible = false;
                pictureBox4.Visible = false;
                pictureBox5.Visible = false;
                pictureBox6.Visible = false;
                pictureBox7.Visible = true;
            }
        }

        private void button1_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }
    }
}

__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio5
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que por medio de un radioButton pueda cambiar de color un panel o contenedor en un formulario.
        }
        private void radioButton1_CheckedChanged(object sender, EventArgs e)
        {
            label1.BackColor = Color.Red;
        }
        private void radioButton2_CheckedChanged(object sender, EventArgs e)
        {
            label1.BackColor = Color.Green;
        }
        private void radioButton3_CheckedChanged(object sender, EventArgs e)
        {
            label1.BackColor = Color.Blue;
        }

        private void radioButton4_CheckedChanged(object sender, EventArgs e)
        {
            label1.BackColor = Color.Yellow;            
        }

        private void button1_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }
    }
}
__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio7
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa cuando el usuario precione un boton este pueda seleccionar una imagen y la muestre en un contenedor o panel para visualizarlo.
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            pictureBox1.Visible = false;
        }

        private void button1_Click(object sender, EventArgs e)
        {
            pictureBox1.Visible = true;
            
        }

        private void button2_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }


        private void button3_Click(object sender, EventArgs e)
        {
            pictureBox1.Visible = false;
        }
    }
}
__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio8
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa donde el usuario pueda mostrar varios formularios.
        }

        private void datosToolStripMenuItem_Click(object sender, EventArgs e)
        {
            Form2 f2 = new Form2();
            f2.ShowDialog();

        }
    }
}

__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio9
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que cuando el mouse pase por cualquier control que cambie de color.
        }

        private void button1_MouseEnter(object sender, EventArgs e)
        {
            button1.BackColor = Color.Red;
        }

        private void button1_MouseLeave(object sender, EventArgs e)
        {
            button1.BackColor = Color.Silver;
        }


        private void button2_MouseEnter(object sender, EventArgs e)
        {
            button2.BackColor = Color.Blue;
        }

        private void button2_MouseLeave(object sender, EventArgs e)
        {
            button2.BackColor = Color.Silver;
        }


        private void textBox1_MouseEnter(object sender, EventArgs e)
        {
            textBox1.BackColor = Color.Green;
        }

        private void textBox1_MouseLeave(object sender, EventArgs e)
        {
            textBox1.BackColor = Color.Silver;
        }
    }
}

__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio10
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//)Hacer un programa que simule un login y muestre si el usuario y contraseña son correctas.
        }

        private void button1_Click(object sender, EventArgs e)
        {
            string nombre = "Carlos1";
            string Contraseña = "Pasword";

            if (textBox1.Text == nombre)
            {
                
            }
            else
            {
                MessageBox.Show("Nombre de usuario incorrecto");
                textBox1.Clear();
            }

            if (textBox2.Text == Contraseña)
            {

            }
            else
            {
                MessageBox.Show("Contraseña incorrecta");
                textBox2.Clear();
            }

            if((textBox1.Text == nombre) && (textBox2.Text == Contraseña))
            {
                MessageBox.Show("Bienvenido :)");
                Application.Exit();
            }
            else
            {
                MessageBox.Show("Por favor revise sus datos!!!");
            }
        }
    }
}

__________________________________________________
__________________________________________________

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Ejercicio11
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
	//Hacer un programa que agregue un texto a una lista.
        }

        private void button1_Click(object sender, EventArgs e)
        {
            listBox1.Items.Add(textBox1.Text);
            textBox1.Clear();
        }
    }
}
