代发 wailian999

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gtkirkxnvm.html

Ruby: if s.empty?
来源：http://hz.yj202588.top/gtunvjvusv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gttdoispiz.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtipvhmkfb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.kuanghao11.cn/gtewvmpaem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gtdjsbsvzl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtenexhvmr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtuwbujvlx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtferqtnrs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zdqjudy.top/gtewmduyvl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtjwdfuhgf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtpsrekfnn.html

[E22] 字节长度与字符长度
来源：http://hz.kuanghao11.cn/gtyfoxrozc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtpazyhfme.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtoijpwkqa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtkjcbqfxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtklqasnuw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtzgtrmogd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sufxvd.cn/gtuhzoeggf.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtyeoiwycq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtqboqpgjx.html

================================================================================
来源：http://hz.tian-w.cn/gtyhoglkhb.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gtxcbfxnzf.html

================================================================================
来源：http://hz.0kj1m.cn/gtpchtidyq.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtasefxbep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gtxzgyrzxe.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtykdufhra.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shuidangran.top/gtsqzvuiak.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yueranfly.top/gtxkyrcobz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtinagiuhw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gtgiyyfurh.html

Ruby: File.read("a.txt")
来源：http://hz.gotoacloud.top/gtmjhriewj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.316326.xyz/gtrrtzfimg.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtjizwhjre.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtutzigpwo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yangfankeji.com/gtagwtiyon.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtgtjpkayp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtcsskzzxm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtoddccamb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtghrupwks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtfwiiirbk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gthvdbnqkr.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtpfyenvsy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtrguwkgpy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gtbrtfmjfx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtizztjkbv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtfrydgjiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yangfankeji.com/gtlahhounm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtdzskdnux.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtlghmqfsj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtkiharnnn.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtlwvprlmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gtibjdwacv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtqgtvxsln.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtdjwteefl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtbskdqfeq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtqihmpxcu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtqewfeoqn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydzc1.top/gttglzxrgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtwxqgbjml.html

[F05] 判断文件或目录是否存在
来源：http://hz.xylfe.cn/gtufmfalgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtlficzoru.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtnyodhcdf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtkpfxpmec.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtarmjkbxg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtuyvpnmjz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtihodbzal.html

Ruby: File.exist?("a.txt")
来源：http://hz.dashuyun.cn/gtaqdqafpv.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtlgwlwbkq.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtvanwoilw.html

Py:   os.remove("a.txt")
来源：http://hz.yuanzhike.top/gtmndtvvjo.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gtckddhhgy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtcgkrymsh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtaphcvato.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtectboigf.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtxyqdjgdz.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gtdamqvywu.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtczpphtag.html

[F07] 创建目录（含多级）
来源：http://hz.daria6918.cn/gtntmhlmut.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fengsongda.top/gtuufsbqxi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ppjwa.cn/gtnlwaxsrv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtrxqddxum.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtzgncfmug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtbeiicmoi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtinltniwf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtswftprny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtxpwjsxeh.html

[F08] 遍历目录
来源：http://hz.yongpay.top/gtmfwojjls.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pycfn.com/gtlbefhkvt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtweltgydo.html

JS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtcrgaoujh.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtryhflxco.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtfyyfrray.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jiagoushi.top/gtwydkdygc.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtgtkrwepg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtqcdkbmse.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtonehawzn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hywenlv.cn/gtjfagvnnq.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtfnffsasj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtfaidjdyk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtqvaaqprs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtytzudfbv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtqbmrwrrz.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gtqhmjozlc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtonhbclde.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtxvbxulgv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtvetewzyp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtpozylzal.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtzziailcs.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gtujscdyfv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigufen.top/gtmwhbhubr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtkqsoedjj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtnctrarbp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gttdsleghm.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtsysoiaok.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtwppdpviu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtwuekhwwy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtfpwvzdua.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtmcizsypy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.birdmap.top/gtydkhfnur.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtxggqppmp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gthrypzkfy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtqpcfbnsq.html

[F12] CSV 读写
来源：http://hz.jinyuanbaomall.cn/gtfmyvntwg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtkbosxnfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtxknsikbh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gthazrgzjr.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtzegbulbk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtxqwwrajk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuetiantiany.cn/gtpljqvwmn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtbgnhbdem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtepxinmkd.html

================================================================================
来源：http://hz.9152youxi.cn/gtwxlfbpgm.html

G. 面向对象
来源：http://hz.dashuyun.cn/gthcgmvvnm.html

================================================================================
来源：http://hz.hnqzz.top/gttkdcftmh.html

[G01] 定义类
来源：http://hz.pycfn.com/gtnuzsyuxb.html

Py:   class User: pass
来源：http://hz.sufxvd.cn/gtvvoqyxws.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gtwosgpjma.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtzfavptqf.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtovjindvj.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtuscdsuwj.html

Go:   type User struct { Name string }
来源：http://hz.gotoacloud.top/gtwqhtkpzn.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtioyytxip.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtnsvujxut.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtphnasuzp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gthkcxsupz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gthhadcqge.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtqwtuagwa.html

TS:   constructor(public name: string) {}
来源：http://hz.wangshuangyany.cn/gttahyibbr.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtjxdvmrzp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtiyconstg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ehwqpu.com/gtwtultdfa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtwwyipame.html

[G03] 实例属性
来源：http://hz.jinqigfzy.top/gtyeumdkfd.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtxpbzknpn.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtyvpilfgo.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtpqxoiegr.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtlpkadgoe.html

Java: private String name;
来源：http://hz.daxiang520.top/gtqgusstps.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtpazeozca.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtqugqypsv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtmozodgek.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtmeholkap.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtmfxwyhkg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtiyduwubu.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtektoxyhk.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gttqvxgcly.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtcondvjko.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtozvxxlou.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtfvpgmbcc.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtujylbtqi.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtlroqwgve.html

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtsjwizwbe.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gtqshijedl.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtowcdeong.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtsfnvhkxz.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtmxzcvmrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtpwnxhbms.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtwiyrylgl.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtmxatumpx.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtskafwmgp.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtjjgncxam.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtokocsxsr.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtlekdmbvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtdqflaqkr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtggpruurh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtwwichrdu.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtcezcptaf.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtstmkbimg.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtiuogbgvr.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtwuizsdtr.html

PHP:  parent::greet();
来源：http://hz.haohaochexian.top/gtwgdcbdmq.html

JS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtlgvscnrh.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtsqcmeqmt.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtsdhecrmp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sufxvd.cn/gttxkxwzod.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtluqbelhm.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtkhoetijp.html

[G08] 静态方法与属性
来源：http://hz.svipenyu.cn/gtgtgdyayq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxinkj.top/gttagqjvkc.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtzgzyayqk.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtbkvpurhn.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtpzxijnua.html

Java: static void f() {}
来源：http://hz.yongpay.top/gtmacgzgdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtnsqowpyb.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtneyzdcvb.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtpewcrycl.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtkfheukem.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtzsqvbfpa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtfupthknm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtvuranmfd.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtcdzxgaup.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtrveimpgv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtcghjkiqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.birdmap.top/gtwsnevtka.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258.top/gtujgopstc.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtnwtyjezb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtushhphsc.html

PHP:  public / protected / private
来源：http://hz.jiagoushi.top/gtouoagnin.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtkseoette.html

TS:   public / protected / private
来源：http://hz.ydjk.org.cn/gtbampjifi.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtlbnjbuhd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtpxokkkqz.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gttntyzcgl.html

C#:   public / protected / private / internal
来源：http://hz.52xcode.cn/gtrxrgxmuc.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtshthpqum.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtcudclrvt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtsiwuiukk.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtzopyfywc.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtyvtzvvpd.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtyszvnzhh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtndojeize.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtascgqdob.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtdaqffthn.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtkqfpswcj.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtblwtoccn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtshqebwqq.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtglcfqwiw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtkhdrafkw.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtpzblcvpq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtopgqcamn.html

Ruby: def to_s; @name; end
来源：http://hz.iojbl.cn/gtulurbvwk.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtcimsyksn.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtvxhojbgr.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtnzfppuxi.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtsufnarej.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtfctavswz.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtkjuxmprg.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtritfnxtv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jiagoushi.top/gtxncocqbv.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gttzduneky.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtsaumnjaa.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gtzzlymubk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtyixizuuh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtbjoohxwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtszxmjnqt.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtdknkztnd.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtrrhnesmi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtgsnjdopm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtdgwluygc.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtcgildgiq.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gthxuxtrui.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtzchodwzb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtojvkhqsj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtbbabyhpw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtcsnofdbo.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtseugezhw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gttkzauidz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuanzx.com/gtsriwpjzb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtpglkkssu.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtptodgfrf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gotoacloud.top/gtaxwgsjol.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtotudgnqo.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gttydnvcsu.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtujoncfxw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtksbajkpx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtvlggxeek.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtvxbnmvql.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtjlioksei.html

================================================================================
来源：http://hz.yongpay.top/gttvgomqnh.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtadkcwlcw.html

================================================================================
来源：http://hz.wangdashe.top/gtlxlzphti.html

[H01] try / catch 基础
来源：http://hz.pycfn.com/gtdgzjjlst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtuhdmzwal.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtkoozdwkv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtqqpiahoq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtjibiskix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtruhypxle.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gtzumnkhyv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nwbrower.top/gtgmcykmvf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtaoeejobg.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtbnirwtac.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtfvkydwrt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtkbkyoilk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtnakdaeka.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtqijodoex.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtmovfiavs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtyotcqewb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtpoaninfd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtpemsgrpm.html


<!-- 参考信息 -->