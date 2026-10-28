代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.bjfxy.top/gtcsgvgacb.html

================================================================================
来源：http://hz.zhixingplan.top/gtndarggym.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtmclnftkf.html

================================================================================
来源：http://hz.sufxvd.cn/gtllpkrfal.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gtievuzthc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xingfuxueyuan.xyz/gtaukxytab.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtzhrjzvkt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gtqrvklnfx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtoryqtots.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtwkudavab.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtasgqdiss.html

Ruby: File.read("a.txt")
来源：http://hz.iojbl.cn/gtibnioauv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtkkisfzgh.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtczvhnwxy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtlxjymwqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtjcwtzirz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtlsmzsino.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtmtqrijla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtoamtlyxg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtsxukowlj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtcdnpgbgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtfibxcqqz.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gtvaychvkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gtqzmucffj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtrjwvbroy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtdcilnoux.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtlcxlvgyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtqpfyowfs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtzekudkrx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtfhoziuiw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtrvwtjnsf.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtypszmoea.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtrduuasuo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtpayjbdij.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtplhvfczk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtkkyevsqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtyzoetsax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtcmyuwvtc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtqsbwhtac.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtpqktkwdx.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtbqfzuwmr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtkpkisjcv.html

PHP:  file_exists("a.txt");
来源：http://hz.dianchejie.cn/gteuafgboa.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtorrcvejb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtmlbhbvfz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtzbsehwer.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtupnmmqqg.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtblbowuhi.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtltzkikuv.html

[F06] 删除文件
来源：http://hz.cdnleiting.top/gtztggtsni.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtexjubcyj.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtzcnmehja.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtpuqxifxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtcpoztlpw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtvegbwfuk.html

Go:   os.Remove("a.txt")
来源：http://hz.fzhhl.top/gtspakmqfz.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnwrmlgen.html

C#:   File.Delete("a.txt");
来源：http://hz.feifeiyinyue.top/gthexswyud.html

[F07] 创建目录（含多级）
来源：http://hz.iojbl.cn/gtswvzlyid.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtilfgmiui.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtghqjuvbw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtwdqnzqmt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtcmkyoaez.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtxvqzvvnr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dianchejie.cn/gtegqxnffv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnxiangtu.top/gtulsbsqeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtyvwgwbuw.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gtlivpqssd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.vqdsnc.cn/gtiiltzjbr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtpqodxjxx.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtsglwarig.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtsigsnpiu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtabrhrzup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtlierxqlj.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtcljqhfqu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtsgytxmuj.html

[F09] 获取文件大小
来源：http://hz.nanxinkj.top/gtzuvkptge.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gtnjhpddwy.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtbdeznxhm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtbcouezoq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtryybznld.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtfgpqbesr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtuvbtbdim.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtokquwcpd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.havefunace.top/gtzokzzovx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gtncvuzjxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtgpejjhyf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtzdwhqego.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtgxpvufnk.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtciuuzcmy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.c1oappe.top/gtthwgruim.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtyvpzllbb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtiwpafzyr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gthkplsndl.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtfgbnkeoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gthbfcvkvb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hysaishi.cn/gtjiririto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtuoetmpsh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtrdgchyyg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtzvcuanzv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtkglmqqqc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtzglqszup.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtqwmzxzlp.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtbcpfpljh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtzcjjiuxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtrdfxqgkm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.smart0.xyz/gtsgrlijff.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtsdiiyxrp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pycfn.com/gtakcobpno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gttxhiqerz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtifpyxvhu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gthzfkcyhx.html

================================================================================
来源：http://hz.52xcode.cn/gtjqioqvwa.html

G. 面向对象
来源：http://hz.redwolf501.top/gtjsbeqsvu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvicmtgxc.html

[G01] 定义类
来源：http://hz.cashguo.top/gtgwbunhpg.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtacagbcqx.html

PHP:  class User {}
来源：http://hz.yonumen.top/gtznokwwqp.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtqrdgjfoh.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gttbwsvoub.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtgffknsee.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtcfmoizxr.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtmljvxvjb.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtzluczozj.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtsdzqvrcv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtnbqncjld.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zycfv.cn/gtwaxfdzhp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtxevkohek.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtzgdkcsbn.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtgtzzscar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtjiuqhknn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hywenlv.cn/gtgsxwzjjx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sxryk.cn/gtirqdvure.html

[G03] 实例属性
来源：http://hz.gotoacloud.top/gtnuhrlfjm.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gtctlsojtj.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtzqwsyjpe.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtglaxlftm.html

TS:   name: string = "x";
来源：http://hz.gaohongyu789.top/gtndxocmzn.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtpipgfvvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtfduvtbqi.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtclvfzxqa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtigupnctt.html

[G04] 定义方法
来源：http://hz.cheryme.top/gtbsznyxjy.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gthclrmdhp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtlknzdqoa.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtyjhsaygs.html

TS:   greet(): string { return this.name; }
来源：http://hz.xylfe.cn/gtjyurpaxu.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtxwfonkhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtekggqqzc.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtgfulzvbz.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtzgydcfam.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gthgdstlkw.html

Py:   class Admin(User): pass
来源：http://hz.ybcxt.top/gtcouyignu.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtxpqnyhkd.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtqhschmpp.html

TS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtzpnvddsi.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtsftkkxzl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gthtxdvyna.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtzyktslan.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangkeji.top/gtklhdfurc.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gteoytikzx.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtwnujlmgp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtokidkpfe.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtzmzfgctt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtunfvtdym.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtyndfdxay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtaxsbcupg.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtbrotbwfv.html

C#:   public override string Greet() => "admin";
来源：http://hz.sweek.top/gtqtmqljjq.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtbavynwvc.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtjskuamwo.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtqivaccan.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gttumjktdt.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtrbkjpxou.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gtmfwjmupe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtfobphich.html

Ruby: super
来源：http://hz.guannengcc.top/gtuijusxnl.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtmtbwnvur.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtsjkiajcr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtntztbawj.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtjvfhqldw.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gthxkobcpi.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtbugdsurb.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtnbtijtib.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gttfrqgkls.html

Ruby: def self.f; end
来源：http://hz.jinqigfzy.top/gtgmkxpmxl.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtkxcoiqyl.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtuuyvgxvm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtvwroggex.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtybpfinqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtfxsqklou.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtfcwytilq.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtnzllfqzh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtltwspafy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtwnqqhqki.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtwssbwzwn.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtlajvxwur.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtiybdstfb.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtpqkkjteb.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gteufyaeom.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtcqidnzlg.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtnoyxgdsq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtpbfavwiy.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtswehszqd.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtarhwpznj.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtixuklfiy.html

Py:   @property 与 @x.setter
来源：http://hz.aizwys.cn/gtjwdipkzg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtqosfqinx.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtkzwcqetv.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtmgbfivaa.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtzcjregbz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtjlzdxcxr.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtzwyeacqe.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gttpkrfepx.html

[G12] 对象转字符串
来源：http://hz.ivvv.top/gtcxcngqfs.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gtgitmprbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtpxszmnqt.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtxwuxrraz.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtatjyemtt.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtjdfwvziu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtgdnbcylc.html

Ruby: def to_s; @name; end
来源：http://hz.aizwys.cn/gtbdbkjybx.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtjouhqscc.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtemaefgaf.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gtxvrymeuj.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtdrbhhgad.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtphianirl.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtgbujvten.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtgyrnlsms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtffevzuqc.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtqahbmcop.html

C#:   u is User
来源：http://hz.sysykeji.top/gtupkvvprf.html

[G14] 数据类 / record
来源：http://hz.iojbl.cn/gthvwieevp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtogdayycb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtgrrotqxc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtnnpiffqj.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtkmffrksw.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gteezpstoy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gthejbljdc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gtkwvpjjdx.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gtcqwnfxbe.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtaazbcemp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtiksvnoom.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtsijtaicb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtcfoqhsmb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtuflonxbx.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhengqikj.top/gtfbksouza.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtvlmggvhs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtkzkylnkp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtosacqano.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gtqgldrmna.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtjockhchz.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gttnnyqvky.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtfkxyqwdp.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtsekokqfi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtqhajjzmc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jianghu66.top/gtfetlpyvu.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtoavhxlrg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtgaqrbhsm.html

================================================================================
来源：http://hz.tianlin.xyz/gtkhhbgqdl.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtsnwxpnvz.html

================================================================================
来源：http://hz.xinyue.icu/gttueklmpj.html

[H01] try / catch 基础
来源：http://hz.pycfn.com/gtdneljgxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuxming.cn/gtxhpaeiag.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuanzhike.top/gtmaxghrdh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtzharykku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtiexymldw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtkiqanxco.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cashguo.top/gtifetmuey.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtcpdwslke.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtzivnoqrw.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtkvaozmuk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cdnleiting.top/gtvoecgrxn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtcdwmdoba.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtprcpcabm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtvudzchsr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtvvexbdna.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ybcxt.top/gtuaotqvom.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj202588.top/gtcxpcljwz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtrvtxcuwm.html

[H03] 主动抛出异常
来源：http://hz.mhx1999.top/gtzhltjeeb.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtqyvivfsx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gthrotlcvh.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtnvipgstf.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtgepijvlp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtfwkkehuq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtuuhrlzno.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhixingplan.top/gtnfboitxx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtzcococuc.html

[H04] 自定义异常类型
来源：http://hz.chenlongwang.top/gtpbpuocth.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtpyophjlt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtiayfqjby.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtahqxlkhf.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gttzfypggq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtowwyenqk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.snrcjt.cn/gtusgyebsi.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gthvznznhi.html

C#:   class MyException : Exception {}
来源：http://hz.jinyuanbaomall.cn/gtnxlgzcej.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtoiykcjdq.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtiaowwrji.html


<!-- 参考信息 -->