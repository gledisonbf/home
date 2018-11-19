# home
Algoritmo de Criptografia utilizando base64       com interface

package criptografia;
import java.util.Base64;


public class Criptografia extends javax.swing.JFrame {
    String textoPlano, codificado,pronto;
    public Criptografia() {
        initComponents();
    }

    
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        btnsair = new javax.swing.JButton();
        txt_input = new javax.swing.JTextField();
        jLabel1 = new javax.swing.JLabel();
        jLabel2 = new javax.swing.JLabel();
        btn_criptografar = new javax.swing.JButton();
        btn_descriptografar = new javax.swing.JButton();
        txt_output = new javax.swing.JTextField();
        jButton1 = new javax.swing.JButton();
        btn_info = new javax.swing.JButton();
        lbl_output = new javax.swing.JLabel();
        lbl_output1 = new javax.swing.JLabel();
        lbl_output3 = new javax.swing.JLabel();
        lbl_output2 = new javax.swing.JLabel();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setResizable(false);

        btnsair.setFont(new java.awt.Font("Arial Black", 0, 10)); // NOI18N
        btnsair.setText("SAIR");
        btnsair.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btnsairActionPerformed(evt);
            }
        });

        txt_input.setText("   ");
        txt_input.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                txt_inputActionPerformed(evt);
            }
        });

        jLabel1.setFont(new java.awt.Font("Arial Black", 1, 24)); // NOI18N
        jLabel1.setText("CRIPTOGRAFIA");

        jLabel2.setFont(new java.awt.Font("Arial Black", 1, 10)); // NOI18N
        jLabel2.setText(" DIGITE AQUI:");

        btn_criptografar.setFont(new java.awt.Font("Arial Black", 0, 10)); // NOI18N
        btn_criptografar.setText("CRIPTOGRAFAR");
        btn_criptografar.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btn_criptografarActionPerformed(evt);
            }
        });

        btn_descriptografar.setFont(new java.awt.Font("Arial Black", 0, 10)); // NOI18N
        btn_descriptografar.setText("DESCRIPTOGRAFAR");
        btn_descriptografar.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btn_descriptografarActionPerformed(evt);
            }
        });

        txt_output.setText(" ");
        txt_output.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                txt_outputActionPerformed(evt);
            }
        });

        jButton1.setFont(new java.awt.Font("Arial Black", 0, 10)); // NOI18N
        jButton1.setText("LIMPAR");
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });

        btn_info.setFont(new java.awt.Font("Arial Black", 0, 10)); // NOI18N
        btn_info.setText("INFORMAÇÕES");
        btn_info.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btn_infoActionPerformed(evt);
            }
        });

        lbl_output.setText("      ");

        lbl_output1.setText(" ");

        lbl_output3.setText(" ");

        lbl_output2.setText(" ");

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addGap(193, 193, 193)
                        .addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 230, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 101, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addGroup(layout.createSequentialGroup()
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addComponent(txt_input, javax.swing.GroupLayout.Alignment.LEADING)
                            .addComponent(txt_output, javax.swing.GroupLayout.Alignment.LEADING)
                            .addComponent(lbl_output, javax.swing.GroupLayout.Alignment.LEADING, javax.swing.GroupLayout.DEFAULT_SIZE, 549, Short.MAX_VALUE)
                            .addComponent(lbl_output3, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                            .addComponent(lbl_output2, javax.swing.GroupLayout.Alignment.LEADING, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                            .addComponent(lbl_output1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
                        .addGap(64, 64, 64)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                                .addComponent(btn_descriptografar, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                                .addComponent(jButton1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                                .addComponent(btn_criptografar, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                                .addComponent(btn_info, javax.swing.GroupLayout.Alignment.TRAILING, javax.swing.GroupLayout.PREFERRED_SIZE, 143, javax.swing.GroupLayout.PREFERRED_SIZE))
                            .addComponent(btnsair, javax.swing.GroupLayout.PREFERRED_SIZE, 143, javax.swing.GroupLayout.PREFERRED_SIZE))))
                .addGap(32, 32, 32))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 34, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(4, 4, 4)
                .addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 30, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(3, 3, 3)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(btn_criptografar)
                    .addComponent(txt_input, javax.swing.GroupLayout.PREFERRED_SIZE, 90, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(11, 11, 11)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(btn_descriptografar)
                        .addGap(18, 18, 18)
                        .addComponent(jButton1)
                        .addGap(28, 28, 28)
                        .addComponent(btn_info)
                        .addGap(0, 58, Short.MAX_VALUE))
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(txt_output, javax.swing.GroupLayout.PREFERRED_SIZE, 123, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(18, 18, 18)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                            .addComponent(lbl_output1, javax.swing.GroupLayout.PREFERRED_SIZE, 23, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(btnsair))))
                .addComponent(lbl_output, javax.swing.GroupLayout.PREFERRED_SIZE, 25, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(lbl_output3, javax.swing.GroupLayout.PREFERRED_SIZE, 25, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                .addComponent(lbl_output2)
                .addGap(10, 10, 10))
        );

        pack();
        setLocationRelativeTo(null);
    }// </editor-fold>                        

    private void btnsairActionPerformed(java.awt.event.ActionEvent evt) {                                        
       System.exit(0);
    }                                       

    private void txt_inputActionPerformed(java.awt.event.ActionEvent evt) {                                          
             
                 
    }                                         

    private void btn_criptografarActionPerformed(java.awt.event.ActionEvent evt) {                                                 
        textoPlano = String.valueOf(txt_input.getText());
        codificado = Base64.getEncoder().encodeToString(textoPlano.getBytes());
        txt_output.setText("Texto criptografado: " + codificado);
        

    }                                                

    private void btn_descriptografarActionPerformed(java.awt.event.ActionEvent evt) {                                                    
          byte[] arrayBytesDecodificado = Base64.getDecoder().decode(codificado);
        String textoStringDecodificado = new String(arrayBytesDecodificado);
        txt_output.setText("Texto descriptografado: " + textoStringDecodificado);
    }                                                   

    private void txt_outputActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here:
    }                                          

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        txt_output.setText("");
    }                                        

    private void btn_infoActionPerformed(java.awt.event.ActionEvent evt) {                                         
        lbl_output1.setText(" Base64 é um método para codificação de dados para transferência na Internet.");
        lbl_output.setText("É utilizado frequentemente para transmitir dados binários por meios de transmissão,");
        lbl_output3.setText("que lidam apenas com texto, como por exemplo para enviar arquivos anexos por e-mail");
        lbl_output2.setText("É constituído por 64 caracteres ([A-Z],[a-z],[0-9], \"/\" e \"+\") que deram origem ao seu nome. ");
    }                                        

    
    public static void main(String args[]) {
       
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(Criptografia.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(Criptografia.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(Criptografia.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(Criptografia.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        

        
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Criptografia().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton btn_criptografar;
    private javax.swing.JButton btn_descriptografar;
    private javax.swing.JButton btn_info;
    private javax.swing.JButton btnsair;
    private javax.swing.JButton jButton1;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel lbl_output;
    private javax.swing.JLabel lbl_output1;
    private javax.swing.JLabel lbl_output2;
    private javax.swing.JLabel lbl_output3;
    private javax.swing.JTextField txt_input;
    private javax.swing.JTextField txt_output;
    // End of variables declaration                   
}
