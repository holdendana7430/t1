代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtzempqgbv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtgkdvpwis.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.c1oappe.top/gtvwtvtrov.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtdvqhciry.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtuaobecwe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtzfpsmbgq.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtyrpafxhh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtniqnycvm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtstdqfiyj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtitsmyvkk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtbxkiekme.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gthzvrzpte.html

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtdfnsdngy.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtjjdwasro.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtdpqfcccx.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtmdoxbybr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtefedgetw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtkmleqexm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtnaodjxyv.html

Go:   os.Remove("a.txt")
来源：http://hz.tanke756.top/gtkfjqiohl.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtxpnycqhi.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtjtvifxtg.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtgjubbsaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtxqrlyqlf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gtnvcjikoz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtcrcuycco.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtgxlufidy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtwroszauk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuanzx.com/gtrowslmdp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gtzggqdbet.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtatwimvsk.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtzbrsftrn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.quarkkingdee.top/gtlljeqcxh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gthoedqsbh.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtnofkdfik.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtredassst.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtezrtlgnt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtfbmasgzv.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gtsfxpgcup.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtaczdwgun.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtmbrtiqgy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtxxhjbdzu.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtfsubqcqf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtonolrhoh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtnjswncud.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtkdkcaeez.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtfvrhyhej.html

Ruby: File.size("a.txt")
来源：http://hz.cashguo.top/gtijksjqvr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtixwztges.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtohflgbld.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtigzuzoce.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gtingfrycp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtptcvbokl.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtqspmhdvi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gthlclxhst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtpvsnlunp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtnsevvzye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtshgnmyjr.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtgqingjis.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtoiuqqlqd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtgtnvlzkq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtapbjdzsp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtuvjsqkfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gtbiadflys.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtkojccepk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtovdgices.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aizwys.cn/gtpoayoffe.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtmygdugqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtnzyqxfyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gthhicrlqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gteasncuvz.html

TS:   // 同上
来源：http://hz.birdmap.top/gtsbefsswc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtpzkhsmbm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtfedoqoee.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daxiang520.top/gtayvgtrtn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtylfakosp.html

================================================================================
来源：http://hz.wangdashe.top/gtproeivzm.html

G. 面向对象
来源：http://hz.chenzaomai.com/gterjceroz.html

================================================================================
来源：http://hz.ydzc1.top/gtaseyxeni.html

[G01] 定义类
来源：http://hz.gogol.net.cn/gtjxduqcuk.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtfgltqrjj.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gtjeddkqsd.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtqjngnwnh.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gtkiqbolbq.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtwqxrcgix.html

Go:   type User struct { Name string }
来源：http://hz.xziqi.cn/gtmogtzqgd.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtzansggny.html

C#:   class User {}
来源：http://hz.wangdashe.top/gtuxatnqzl.html

[G02] 构造函数
来源：http://hz.quarkkingdee.top/gtxihubruk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gttfchbgxj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtmhravhin.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtxtagztot.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gtstbcuihj.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuanzx.com/gtfnenrivc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtrqfutnie.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtyelzoyry.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenzaomai.com/gtahxcyuqd.html

[G03] 实例属性
来源：http://hz.ehwqpu.com/gtfbyppgcq.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtnrjlwikc.html

PHP:  public string $name = "x";
来源：http://hz.cqqwz.cn/gtidhbfbxx.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtlknvckzt.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtcwvakshl.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtiqvanwoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtxqbwirsa.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtzforfqcz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gttssvxacq.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtktpilqjv.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtyxspbtxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtamqxzsqm.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtbbtmjsmt.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtdkyzruqu.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gthgtekjan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gtaauiyesm.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtsmmyhpzs.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtvjrvvhiz.html

[G05] 继承
来源：http://hz.havefunace.top/gttrxbxial.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gtehjpjnsl.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtiyzhugop.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtsvaqxlsh.html

TS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtgefvxnfb.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtsnasgquv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guannengcc.top/gtbblzvzdf.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtrooeuqrw.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtnpkstcyw.html

[G06] 重写方法
来源：http://hz.yuanzhike.top/gtwnflfuzn.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtwfknaabw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtgvynwnyt.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtheoftjgm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtjacbosvf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtaptsombx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sysykeji.top/gtvvcorkto.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtttcgordk.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtqltrimer.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtuoxrnewt.html

Py:   super().greet()
来源：http://hz.jianghu66.top/gtlrqdilaw.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtbhzodxdt.html

JS:   super.greet();
来源：http://hz.sweek.top/gtowwskuna.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtfbxayzhl.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtfhrmqhwv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtdnsikzlv.html

Ruby: super
来源：http://hz.jiagoushi.top/gthahwjzph.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gtllujyldh.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtayrbvtgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtrgefhpzx.html

PHP:  public static function f() {}
来源：http://hz.yangfankeji.com/gtmiayyjot.html

JS:   static f() {}
来源：http://hz.cheryme.top/gthvbbramc.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtbqjmytaz.html

Java: static void f() {}
来源：http://hz.feifeiyinyue.top/gtkeyrwbkt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtfwlcnbki.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gthtlxtdcl.html

C#:   public static void F() {}
来源：http://hz.xuetiantiany.cn/gtjcrkxnme.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtlvfbqbny.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtwixfkiwp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtuzrkeluv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtjfrwiryk.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtbwlsjxzw.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtvtrbgqqt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zdqjudy.top/gtfkhnzylq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtjsfjgdqz.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtkunxsbmk.html

[G10] 访问控制
来源：http://hz.fengsongda.top/gtwudxnjhn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtqwghaeip.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtabzvfatj.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtbvurjtnx.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtyexnznda.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtswenbszz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtkmbagdrq.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gthxmfhbyt.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtkkweppgv.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtknmafbcx.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gtiqxqkjpk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtdohswidg.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtqkzefflu.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtjvmrtlnx.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gthfhfowsb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtqlxohzbm.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtdgmnjpjb.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gttfblxeum.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtuwdzsoby.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gtzlmetpcl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtgdkczjbg.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtgfgdfpjf.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtaxqibton.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gtqxczagag.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtdcjsbglv.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gthgkavcdt.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtychmlhij.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtcpxgeklj.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtmlkvpycp.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gtkkecajun.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gttwkcktlm.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtyycebsqh.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gtbsyzwhiz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gthcopkzhd.html

Ruby: u.is_a?(User)
来源：http://hz.quarkkingdee.top/gtzyofjbnv.html

C#:   u is User
来源：http://hz.tianlin.xyz/gtlzyyvxdv.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtqsspuuux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtqroetnvr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtprvybvxi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtuyhzrbpy.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtqitqwwxb.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtmnedhdxj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtzexmddin.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtlervfgfb.html

C#:   record User(string Name, int Age);
来源：http://hz.daria6918.cn/gtygkeixyf.html

[G15] 枚举
来源：http://hz.nanxinkj.top/gtliwcfllp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yanxiufei.cn/gtalcqzksb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtujcyiuka.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtbywvvbmy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtynpffeen.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gtkypuqszy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtmomjaazk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtunkuchnd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtqlkrxrzn.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gteklhshfv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtybiixwfk.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtqwxywpnk.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtgkapxsbe.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtbhmjyqdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtqhraotze.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtxujxtpkd.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtzgxuptlr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yvedp.cn/gtamsxjmno.html

================================================================================
来源：http://hz.ybcxt.top/gtutlladdq.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gteofmsdkt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttjkgghqq.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtwovlowze.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtqebkkxpa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxuanxn.top/gtvuoburlu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtdwawsexa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtkwghvfti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj20258888.top/gtjbzuqlvt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tian-w.cn/gtwkkuhzqy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtfxcljypy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtkkxffztj.html

[H02] finally / ensure 收尾
来源：http://hz.wangshuangyany.cn/gtepdyelha.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtxlahrdod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtzizfyrtz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtykntjmbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtpiefozmq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gthjaxkoea.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtesjoimvl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtgvbswnwy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtjhngephv.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtlkgnicod.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtvjqnkzho.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gttkfdewaf.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtfzunwajr.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtvzwiavfm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtxkiygvzf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtkoqtsuvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pycfn.com/gtxazblrwr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtderdjkyf.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtfmgmyfii.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtqkktndqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtcarlyock.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtoqrnohqe.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtiqrwdikt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gthroqcfri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtpyrgqwbu.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtszrrugul.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtotqxbrmm.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtrbcymdqw.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtzdcknkkl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.316326.xyz/gtdkiqagcf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gthvxhjpbl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gttywabsex.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gtpzmagjwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtbcpkcbad.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gtybryzghs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtlmroijio.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtnseaudpa.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtfbhazykg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtlwqvvtwn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtmojipmap.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtyhakxxdf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtlfliacmo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtmtsrtfjo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jianghu66.top/gtzzrwpjry.html

C#:   obj?.A?.B ?? default
来源：http://hz.xziqi.cn/gticxfygbh.html

[H07] 断言
来源：http://hz.andypj.xyz/gtcnnkmcsy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtzramhjyo.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtdxkqiuno.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtdrumjvks.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtdthsnned.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtuicrtlgi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtvxvxvsff.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtyozuodty.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtvepgmrnv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtwsazmlvg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtdgvlpdwq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtkjglehvz.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtywgidhrd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtikvrgmhg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtsszhzxln.html

Go:   err.Error()
来源：http://hz.xziqi.cn/gtshmycchu.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtspmzdzuw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtevjxujou.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtdscbbnjw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtagwmkfmn.html


<!-- 参考信息 -->