代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtyxumckth.html

================================================================================
来源：http://hz.sweek.top/gtqhmevaom.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtmqlwqdqf.html

================================================================================
来源：http://hz.mhx1999.top/gtzoqtcbep.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtewpturda.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtihreuzas.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cdnleiting.top/gtzttwlkrr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258888.top/gtavdntmeo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gttcnkntal.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtfsmimebt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangshuangyany.cn/gtisxlwrhv.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gttlvkbrhj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sweek.top/gtqiwnxgtd.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtyscgqdiz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gthkakpnkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtrerxhbev.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtfwyfyrzp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtkwzinprp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gttvavmtbp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtmftmhnpc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtdafeayey.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtjfpmmptv.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtudngipqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtrkahsrwb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gtzpdgjsyd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtpkgkelhy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtyoyhyizv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtmpivjxby.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtxghgwoxi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gtjtdjkjia.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtqrcpinxv.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gtwqhjlnuv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gttzfxefmw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtbdyxtzdb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtfsixvqxx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtjihhiiov.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtstkimgug.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtarhzncpd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtsoetamtw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtkxbhduqn.html

[F05] 判断文件或目录是否存在
来源：http://hz.guannengcc.top/gtbovgpuyv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gzhubu.top/gtqnbsoeus.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtoeojbwby.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtxtriwqro.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtgrcbbofo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtgolgjicl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtflxuvzgq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gteodznwsc.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtibuwezcs.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtajwtlosq.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigufen.top/gtcrnrurxa.html

PHP:  unlink("a.txt");
来源：http://hz.havefunace.top/gtspzlmjip.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtlafgykla.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtyglfwrom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtyexofwgj.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtwananwrw.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gteezqtdii.html

C#:   File.Delete("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtgulehdvj.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtygnhcjse.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtdolbnmda.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtgictnkqa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtbnhzlsli.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtdutikpxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigufen.top/gtyhxlkkee.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtkkartsya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtcffgkoqu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtyjynvryr.html

[F08] 遍历目录
来源：http://hz.zycfv.cn/gthxtraygc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jyoumei.cn/gtcjyxjbwp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zycfv.cn/gttbcnadfm.html

JS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtwrwayaha.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtjrxssvpn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtzuvwjxnf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.9152youxi.cn/gtluugejot.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gteupjdmpe.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hysaishi.cn/gtjvazywtu.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtzatizrrb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtxaretxbr.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtmlftjctq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtkumebbmm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtvkodcfqn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gttkmlfxfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gthntnpiyb.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gtwmkjesio.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtkonbwjla.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtoaqqfnbp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtyblopqmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gtcinhgxmv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtywjqaetz.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gtzqytxmbq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.9152youxi.cn/gtjsouxddv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gteeozszjz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtacnwvgqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtldrqucjn.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtqhfskubq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtyuddbngo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtflronqry.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtkpfnqtni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtclglxaws.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtkreaxuho.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtlyphqeyg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtiznsvxqp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtecouqcoy.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtfukzbviq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtypeapynp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtbrxnvshd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yongpay.top/gtcnbdsbgx.html

TS:   // 同上
来源：http://hz.meibo888.top/gtcjjtarvi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtxlvadtdw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gthidbipvh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xingfuxueyuan.xyz/gtfwwjowjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydjk.org.cn/gtqvhjxypr.html

================================================================================
来源：http://hz.sweek.top/gtmiypurem.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtqowfgupk.html

================================================================================
来源：http://hz.quarkkingdee.top/gtxtxbzehb.html

[G01] 定义类
来源：http://hz.cqqwz.cn/gtwqjbbmod.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gtafvrcbjq.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtncqxvjoh.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtpqvwsvat.html

TS:   class User { name: string = ""; }
来源：http://hz.hongshengwenyu.top/gtuwldekyb.html

Java: class User {}
来源：http://hz.xylfe.cn/gtojyhahyq.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtlwdsptlf.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtkoccibty.html

C#:   class User {}
来源：http://hz.iojbl.cn/gtmjqtfoqw.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtvbmkoydc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtywomsbcj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtietdsuiq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtipsrlrnd.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gttrxhehxm.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtdrvsnvtl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtwyzteccc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtqiygkknq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtdlienktq.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtwhaykhjb.html

Py:   self.name = "x"
来源：http://hz.yj202588.top/gtvkheqaft.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtchhmtpuv.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtzfqdfjgl.html

TS:   name: string = "x";
来源：http://hz.sufxvd.cn/gtgnibydgi.html

Java: private String name;
来源：http://hz.yongpay.top/gtywusglxe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtluyteugx.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtrnueswac.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtwwmubbyw.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gturvkayfi.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtoetzgfmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gteiirqfou.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtkrkjlgwn.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtsrihulgc.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtjusgbiee.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtbvnsqmfk.html

Ruby: def greet; @name; end
来源：http://hz.redwolf501.top/gtelutukmo.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtdrkkdsin.html

[G05] 继承
来源：http://hz.shangyingyoupin.top/gtxsknztbb.html

Py:   class Admin(User): pass
来源：http://hz.pycfn.com/gturbhzxyt.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtobdbqxov.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtjtxaagsa.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtdxxkkonr.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtkemhsvsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gteovjmbac.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtpcytxdko.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtqzljwzbd.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gtxjdcxona.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtmnwaqtoc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtvlnqehcx.html

JS:   greet() { return "admin"; }
来源：http://hz.pycfn.com/gtcjhrxkkk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtwkhstdcz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtpxmmnirx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtzbqjxfkc.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtjjrwkaiw.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtxflxtjdb.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtvyabfhmi.html

Py:   super().greet()
来源：http://hz.yuanzhike.top/gtgzpqfjhg.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtdeqbuwpf.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtqdtmcylo.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtaolwdxqo.html

Java: super.greet();
来源：http://hz.hammf.cn/gtaikcwztu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nwbrower.top/gtpjojfjmh.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtgsfnmynl.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtrhbxjjdj.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtsnhpacig.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtaomrerte.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtiassgnhv.html

JS:   static f() {}
来源：http://hz.yj202588.top/gtoccfaybb.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtzotimyaq.html

Java: static void f() {}
来源：http://hz.cdnleiting.top/gtaqduzxsg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gttexsvufq.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtscefjngr.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtcegmvofo.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtaodwygew.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtrgbfalcv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gthmcvfxyf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtupyumrft.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtnhapdrnk.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gtqigypprv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtetpnnokp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtqonfbufy.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtftdfskys.html

[G10] 访问控制
来源：http://hz.316326.xyz/gttitgisyn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtecrkwwlk.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtyudnwpiw.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtptupbonm.html

TS:   public / protected / private
来源：http://hz.zhiwuduotai.top/gteweuvzyt.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtozbakstb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.bjfxy.top/gtxfqdxehq.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtqsfpuqjs.html

C#:   public / protected / private / internal
来源：http://hz.9152youxi.cn/gtdavqqikn.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtriwubzzo.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtfcxrafpv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtrwpmxdpq.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtqqxqfzsp.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtfjfuafpm.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtzlojfgcu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tanke756.top/gtwjuqglfy.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtebwdnwyu.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtwvmulwfg.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtgmyandpe.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtvpnslvci.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtxinaesnz.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtqqloywag.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtbbiwhcji.html

Java: @Override public String toString() { return name; }
来源：http://hz.xinyue.icu/gtbuvgnxwn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gthfagwjuk.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtwemvbome.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtrinfrkup.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtnqlwymcw.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtyiayrnzb.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtbvbsldoq.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtezynkpqn.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtihbcuzvs.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtzruquixy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtfkduvwxc.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtwegiyica.html

C#:   u is User
来源：http://hz.bjfxy.top/gtvxhrblnw.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtjosoizgx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtjkrlzdqp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtguybfrcc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtdfbmggvk.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtvyijdpmm.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtnxsqopmh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtpukrhvaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.vqdsnc.cn/gtpidqgapx.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gttapbgoju.html

[G15] 枚举
来源：http://hz.iojbl.cn/gtdofvofkp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtgasqbppe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtsmwvvpmi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtzeoischy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtmlexcjoi.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtphulobap.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtwwioktrl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtlrkwhpxm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtattdahrw.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtkhnqrikk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtaweatopt.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtgjwefjox.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtfwsfcgjd.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtbkkwkqkf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gtbshvfkhq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtwrbapheg.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtiopeismd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtwirsoenb.html

================================================================================
来源：http://hz.meibo888.top/gttejbibgm.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtpfidzabg.html

================================================================================
来源：http://hz.andypj.xyz/gtrsyawhff.html

[H01] try / catch 基础
来源：http://hz.jlsjyb.cn/gtpzkslkat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtivaywpct.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangtech.top/gtvdwxrhta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtycsvzmom.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtympehkld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtccujvdlc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydjk.org.cn/gtnlzgszjc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtmzgwfmvw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtlerqhkfj.html

[H02] finally / ensure 收尾
来源：http://hz.ybcxt.top/gtkuejvshx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guannengcc.top/gtpsvydgzx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtawqgfbsk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtooddsroy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gthsxrmyei.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtzotljgiv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guowangkeji.top/gtsrhjrwjg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtvtoyhnqy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtsbirmpui.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtuzkyyzrr.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gtrnxadfqv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtccloqogl.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtapvjxpkr.html

TS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtebqonyct.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtjkvlgkul.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtwgabmdmy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtpzrmqkjq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtuolmyyit.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gtsilemtia.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtpixdkcqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtiatvowqt.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gttpvzztfj.html

TS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtiwalxfzt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtutxtfruf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtnenctsst.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtsaenndsw.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtvowfxlms.html

[H05] 捕获特定类型
来源：http://hz.jinyuanbaomall.cn/gtqlwfcbsn.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtwnoluvys.html


<!-- 参考信息 -->