代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtkbnreopy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcndsmlqx.html

F. 文件与目录
来源：http://hz.birdmap.top/gtjngnlzka.html

================================================================================
来源：http://hz.aizwys.cn/gtpcovgzzh.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gthdqhtnff.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shuidangran.top/gtzwlizoxs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shangyingyoupin.top/gtgpizbspv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daxiang520.top/gtgmyixeqc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtongnoxmu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtftunfhwc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtlfujmznd.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtqhkjshmc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtwdksrmdw.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gthuictowe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gtwhevkaut.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gtgceoitye.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gthbabimyi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtfhdzpqcd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtadhmcrqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtzaufgpnq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gthsphjnzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtglvdysyy.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtbopbflkd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cashguo.top/gtrjwfxshk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtltyzmfbo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtabhwrsde.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtdyyhweox.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gtdixplavv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gtozuzxuxj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtltnladxu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtrpmysqxx.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtnryvxirp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtdvahsfgh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtimekeiks.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtqvgftyhm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtcvnvdwvs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtwuanzzui.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtjsnoudwt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtnuylmfse.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hongshengwenyu.top/gtpfhaptxk.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtzvxflrlp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtrctuuxdz.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtkkxcpnhf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtagezucit.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtiuasoyut.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtyavyhfws.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gthrrjlhfh.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtebzzljey.html

C#:   File.Exists("a.txt")
来源：http://hz.gotoacloud.top/gtwdrqdbyb.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtfalwrahq.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtiqhdhzhx.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtgfhlpfxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtpeyzzbhm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtnchxpcee.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtbqqlkvjl.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtbctlixlz.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtocbgjimv.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgufenzy.top/gtoquuepwt.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtyswyzkwd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gtzykgnbvs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtgxeworgh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtkeavamko.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtmdxigcuf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtiqxviykq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtiqjoeymg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258.top/gtlmbxzihh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtnhfhnxwe.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gtezeifmhf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtglzasgcp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtyoudvuqa.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtfcovrqiu.html

TS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtwzxpqrll.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtdwcuxbjz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtyzicmjdw.html

Ruby: Dir.children("dir")
来源：http://hz.zhijiandao.cn/gtslryishp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtylfhondm.html

[F09] 获取文件大小
来源：http://hz.zdqjudy.top/gtdbfpwusz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtxkjlcnlf.html

PHP:  filesize("a.txt");
来源：http://hz.gotoacloud.top/gtcmjpwjzl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtwsuvfwhz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtsockurvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtsxsbqsbf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtcyzaqsul.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtegldngty.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.haohaochexian.top/gtwouakqkf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gaohongyu789.top/gtwezbaluo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtqzfaqtyk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtwzonjaqy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtamickblp.html

TS:   path.extname("a.txt")
来源：http://hz.yj202588.top/gtiohmunqk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gthupdjiuk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtuagpzlij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtccfzvhzu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtmxudorqy.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gtfvlgxviv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtbjedhfyp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtvoomdszd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtqykdirhy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtnczsibzn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangkeji.top/gtuchywaiq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cashguo.top/gtxdhjkqmd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtducsyetd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtrpxzdbvu.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtonxmnjri.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxuanxn.top/gtkmnimplr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtuvhguftk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtwnxrfvsg.html

TS:   // 同上
来源：http://hz.xinyue.icu/gttpquzjir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aibaodan.cn/gtmzcueflp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtdgvwmbhd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.haohaochexian.top/gtxicanjme.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pycfn.com/gtzjmmgtcr.html

================================================================================
来源：http://hz.zycfv.cn/gtizwvynhi.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtdkdgfbrq.html

================================================================================
来源：http://hz.wangdashe.top/gtlvramdqj.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtxarshvek.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtfafxiazz.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtjhyeuiiv.html

JS:   class User {}
来源：http://hz.shangyingyoupin.top/gtfyyttnij.html

TS:   class User { name: string = ""; }
来源：http://hz.shzxlz.cn/gtcsairxez.html

Java: class User {}
来源：http://hz.hfpthk.cn/gtwwryshnm.html

Go:   type User struct { Name string }
来源：http://hz.aizwys.cn/gtlneueyoy.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtcyylbrnn.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtrgbfnaqr.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtzysxxvjg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtkskclymf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gteoulhbta.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtbjnaiicr.html

TS:   constructor(public name: string) {}
来源：http://hz.xuanzx.com/gtgxkgdjxi.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtnsnafnoe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtqxvpedoy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gtcboiyghq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtyribmljf.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtdlnqqiwl.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtyghholaf.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtqroeprfj.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gthnimjmjd.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtzumkiszf.html

Java: private String name;
来源：http://hz.xuanzx.com/gtjyspfyfo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gthwcoukgo.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtbzzkpdxm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtmtakmdgt.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtmraxcvqk.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtjkdzvwmy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtcunwrzej.html

JS:   greet() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gthjahlpxf.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtpddpueex.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtrrxzxgvs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtmhsdsbrt.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gtfqcftkuj.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtuobqgpcd.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtmeypchec.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtwohbltoz.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtiuiaejlv.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gthjuowqkr.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gttvbgyoqc.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtlnigfhak.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtqlszcrpa.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gthtwbzivg.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtljjzzuuk.html

[G06] 重写方法
来源：http://hz.zhengqikj.top/gtljccilta.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtjsglztkv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtltckrtoq.html

JS:   greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtueunwrqj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtjbqlqlza.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtkekqptzr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtandbaqsu.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtraiycgpz.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtnimwmdvw.html

[G07] 调用父类方法
来源：http://hz.sysykeji.top/gtxplbtuac.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtmtuagoug.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtxwbtnech.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtkqmeexup.html

TS:   super.greet();
来源：http://hz.mhx1999.top/gtcncchhqm.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtiprjpxlo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhiwuduotai.top/gteppmomce.html

Ruby: super
来源：http://hz.zhoulong.xyz/gtxiaocnzt.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gthasdazbt.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtdrynjide.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtdgrgdueu.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gthekioqdq.html

JS:   static f() {}
来源：http://hz.sweek.top/gtrmttvnie.html

TS:   static f(): void {}
来源：http://hz.dianchejie.cn/gtqbwldxjv.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gtqjzonvnb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtdavyfdyy.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gttcubjmln.html

C#:   public static void F() {}
来源：http://hz.havefunace.top/gtvbwuylsr.html

[G09] 接口 / 抽象类
来源：http://hz.zhoulong.xyz/gtxyiingvi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gttrvutmuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtllygkhmo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtddvztszc.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtvisoidml.html

Java: interface Shape { double area(); }
来源：http://hz.hammf.cn/gtwcyajqjo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtvbasqiws.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gotoacloud.top/gtampvfanp.html

C#:   interface IShape { double Area(); }
来源：http://hz.cheryme.top/gtfxlmxikz.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtdzvyqizk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenjidiqi.icu/gttikrslxs.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtgezrymvx.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gttpiioijz.html

TS:   public / protected / private
来源：http://hz.ydjk.org.cn/gtouidslhu.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtygwgiokx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtqtyvhmsb.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtkvvouuhm.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtlzzdsroa.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtkubhimce.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gtlehttoun.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtqdlqerpu.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtftgwcanh.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtiaqenajt.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtherfbtsi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtknkflmpn.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gthxqgirvk.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtmucyhmyn.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtviobqyvw.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtqfuppayd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtdqqckrho.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtfhzuyvyy.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gthsybgzmx.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtazckbqqr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtbpdtmdsk.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtzceyzqmj.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtynzehnjz.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtclgopsoq.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtkvkjhoyz.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtbkjieevg.html

JS:   u instanceof User
来源：http://hz.xylfe.cn/gtlallrjqr.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtywxlrrcl.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtfqnytgar.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtkkzidkrh.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtcqinumss.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtkqavcpai.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtepepmoao.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtzftwwmwh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtkudrstic.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtyewlekyd.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtbdktpfju.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtawoktfus.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtndrioxsk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtmlhztndz.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtgkznmqac.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gtyudiajqm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtjsiitcgs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtcyqyfvdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtvhrujsnu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtsjggwujv.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigfzy.top/gtdyiatgkc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtytboeuli.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtxwbdbtrp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtubrkonsu.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gtecitfouy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtjaowbczu.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtoodylgsm.html

JS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtqhklqedk.html

TS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtqbwggwta.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj202588.top/gtrkfulrpx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtgeapcmza.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gtuhqtlxfb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cqqwz.cn/gtjbjfespc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqzmahqwo.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtziikwyuz.html

================================================================================
来源：http://hz.aizwys.cn/gtrqmpdman.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtkpcjnxem.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtqpcaozvo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtqsxspmxs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtsweznkai.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtdquxqwcm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtukiishir.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtzkanbpmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtqdhqdyur.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.0kj1m.cn/gthynflhck.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtztlrjskv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gturgqxozo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtlevbwgte.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtzgredtvd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtwghqqmuo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtkcqigclf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gttkzdfkht.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtbnqorlru.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.52xcode.cn/gtnpootyoo.html

[H03] 主动抛出异常
来源：http://hz.yvedp.cn/gtiguidpph.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtknxispey.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtbamrjobi.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtucsygtmf.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtjnsnlaak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtsmngfrab.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtawaogbvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnxiangtu.top/gtgaxyzenq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtjcyprlny.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtsdzwbjuu.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtyohpuzwk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtfzznoryz.html

JS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtltwtqdst.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtjlelqxem.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtnbhiwvcc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gttkreiefs.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtjlcpdfrd.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtnqvuynoh.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gtfejomztx.html

Py:   except ValueError as e:
来源：http://hz.bjfxy.top/gtgmqzjxra.html


<!-- 参考信息 -->