代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtlcqlplwq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtymbmrkmq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtrhqsrtxt.html

Go:   os.Remove("a.txt")
来源：http://hz.yongpay.top/gtmyuezahc.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gtyqffykvu.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtevrbzcpx.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtrxfgsmfs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtuevnsksd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtexqgpgbs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtbbxugpae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtghyerpsi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gthlgiahmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtbywycaop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.iojbl.cn/gtnohifinf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtdidgmelm.html

[F08] 遍历目录
来源：http://hz.ehwqpu.com/gtefgaczdb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtjletenfc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtueguiwhz.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtarpozwmd.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtkipixntq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gthphyurnd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtwoekygrz.html

Ruby: Dir.children("dir")
来源：http://hz.sweek.top/gtgamclswq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtwieeigcd.html

[F09] 获取文件大小
来源：http://hz.zhengqikj.top/gtylefckrc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgfzy.top/gtarohojmh.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtgipaksft.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtdcbntiqc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtzfoypoot.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtemgvlkiv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtjkiwvicg.html

Ruby: File.size("a.txt")
来源：http://hz.chenzaomai.com/gthugfujgz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtpadsoinu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtcwvjnymp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtajiynpex.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhongyouzk.top/gtrktjtvfp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtaspwovwm.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtdthwfyzn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtoquikjzr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtplclwysx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtkpikhfzi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtmymswpuu.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gthenpdrmy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gteltpqmue.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinyuanbaomall.cn/gtuzctyvgp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtkswyjmob.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtwsrqqmln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ivvv.top/gtyznfvxzn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtohxqrvzz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtjxliznij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.svipenyu.cn/gtmhvrzjbp.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gtfhnwktor.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtjbftvdta.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtapsvkanc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pycfn.com/gtnixfqdiy.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtcpsdhaws.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtawemolmg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuetiantiany.cn/gtslhqzsro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtmcelnmkg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtmwiumbbw.html

================================================================================
来源：http://hz.meibo888.top/gtjiigljnt.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtfyxjfxua.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkeikvaaq.html

[G01] 定义类
来源：http://hz.cashguo.top/gtqxfvqdzc.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gttyepplhx.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtfbyhaflf.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtkqndkosz.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtatuncgqg.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtbbxpnjkr.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtqomyxncc.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtmzlfwsqq.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtjawmicsf.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtpficuiwn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtgcnpbdnl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gttmvmcztp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ybcxt.top/gtfjrkeykm.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtqsfisexl.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtewjciydr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gtbnqvsiyt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gteditogne.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtpzcghyvy.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtvunwtkvw.html

Py:   self.name = "x"
来源：http://hz.vqdsnc.cn/gternmatht.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtfdncasjz.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtemrawlwv.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtpfpnmggs.html

Java: private String name;
来源：http://hz.daria6918.cn/gtlaxrsahi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtqiwsxpcj.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtmfwsunvf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ehwqpu.com/gtnaawyikj.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtsimasjrf.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtrmbtvcbs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cashguo.top/gtmkhclrsl.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtlgjvuztp.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtbpdckfxd.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtdzquoxzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtilkhtyeo.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtqzetpahc.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gthumjycvf.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtxtdarhxd.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtysriwzys.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtmkqhodts.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gthriylscx.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtqnhuevjp.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtpcrfbxbs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtsimeungt.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtfkapegnr.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtzshaabkd.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtlmhelxnh.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gttanelxbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtsljpacix.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtkbyjurky.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtygjmrsix.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gthldqhebx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gttrstnagr.html

Ruby: def greet; "admin"; end
来源：http://hz.xylfe.cn/gtaambrdde.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtuhyfoqcy.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtdgilyylm.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gtutsqflgt.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtncgutwrq.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtpsmvnjmu.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtmhyuqypb.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gtwscbthvj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gtdjlzbczu.html

Ruby: super
来源：http://hz.52xcode.cn/gtkwesyrdv.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtbhgdrlxo.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtklhpnumi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtqjxzcffp.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtgjsgrzrc.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtkctrdsiy.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtwhlqqoby.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtohqkgnmj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtutzutexz.html

Ruby: def self.f; end
来源：http://hz.gzhubu.top/gtxobuvvkl.html

C#:   public static void F() {}
来源：http://hz.zycfv.cn/gtnehbfcdp.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtktmiujqy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtgxqfisqx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gteuymtbvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gogol.net.cn/gtntrqgubg.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtypffyoxd.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtctbwotws.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtmxjbflop.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtmihkuetk.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtjosbgvgb.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gticvfmeps.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtbgbgkyem.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtpfyqgceq.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gtdgkohiaj.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtckuxoavm.html

Java: public / protected / private / 默认包级
来源：http://hz.yueranfly.top/gtklhfehwo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtdmfntmak.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gtlvdkfxzc.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtexkpxgmn.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtqnoktzti.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gtqectqvtc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtccewcunu.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtytgmynor.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtcgkbvbcp.html

Java: public String getName() { return name; }
来源：http://hz.jyoumei.cn/gtehpunvwb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtfdfycwts.html

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtmdgvcteg.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtttiszxbl.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gthkryljiy.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtlqautgkb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtackezzih.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gthxmyifja.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtmwfovguk.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gttiufelcq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtwoaeoezu.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtkiwyoxoa.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gttzwgqevs.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtmelnpmas.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtalneapan.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtowiuvixw.html

JS:   u instanceof User
来源：http://hz.ydjk.org.cn/gteusjerrw.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtscmtbydm.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gthxrdwdxd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gteylcdjtj.html

Ruby: u.is_a?(User)
来源：http://hz.yangfankeji.com/gtibqhfiyw.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtegbqvngf.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtkynaraly.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtbmupcbop.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258.top/gtofwtqpjs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtsrhplkse.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtpjwrdmhj.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtkhguzhre.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtqypozxam.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtlxpdiwkc.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtxkidojpd.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtdacuejca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtuzcayoso.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnxiangtu.top/gtnfmnyoik.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtfojanbmr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtlnahpjsk.html

Java: enum Color { RED, GREEN }
来源：http://hz.52xcode.cn/gtuknulmnl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtrswquvun.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtgjduwjix.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtcisrbvaf.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gthucaizvh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gthpdjexzp.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtemkzmeca.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtekxyeerp.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtxcomkbol.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cheryme.top/gtjkivhsxz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtwwxwexsu.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtprnqqanj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtifxevbzn.html

================================================================================
来源：http://hz.cucudq.cn/gtkjqosnzg.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtlloarncp.html

================================================================================
来源：http://hz.yuxming.cn/gttemaffqh.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtjolvtzcl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtdyvlbfod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtsotukmuv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtyxivhuso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtepxccrtc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtrsazdrhp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtjzzhncve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.316326.xyz/gtzgsxeoug.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenlongwang.top/gtebrvsiak.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtcpemiyxw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtcxznuczg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gthfsgxelh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtkyecqday.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtqydopkmd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtdhkyshiu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtgchehabg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtdxjeojpj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtpnitygzo.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtdfaaxqwt.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtircdypmd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtfjlvvtka.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtgubgpinw.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtauzpheur.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtphpknmnh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtvzmwmqmh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtxyjcqfwf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtlpqoimmk.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gteabqgnxv.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtrmqdulap.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtkrpkmhhh.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtcehlngyk.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtordgsesi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtwfsfanlz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gteynhmoqp.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtbvlpymfe.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtalbehqnf.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtdnqsfqui.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtaqhroxhw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtninudpai.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtsmgrnndh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtbfzqpfvz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtjtyzeeuk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gtsmoorblz.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtjoncktro.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtqsbnsxgt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtinpzeeav.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtztphaicj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtrlgborqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtfdodtvis.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtzlagwjzh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gtzbjubvjf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtpjsxypvz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtxiucheeq.html

C#:   obj?.A?.B ?? default
来源：http://hz.yueranfly.top/gtjakwikwx.html

[H07] 断言
来源：http://hz.aizwys.cn/gtquayzkja.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtgouonotb.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gtnwoquefj.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtcbrzhsxi.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtbmetepfl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hongshengwenyu.top/gtrunrvsgt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhongyouzk.top/gtgadwlgfo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gtquxyqten.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtrbiiyuip.html

[H08] 获取错误信息与堆栈
来源：http://hz.mhx1999.top/gtyaxdbnjs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtxzbfluih.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guannengcc.top/gtxkegkbaa.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtmfeeyfbl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtuzuycbri.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.bjfxy.top/gthsbfitkm.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtrbeupgwc.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtaqusckml.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtwgtumyzy.html

[H09] 带错误码的异常
来源：http://hz.sweek.top/gtfmchpakp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gtywrhhchi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtogumeatp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtrxlhxrdk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtjckzzzac.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtrndhimfm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gtdzusgttw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuxming.cn/gtughgqece.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtrvdhysjv.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtuoroceuy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtbnxzpnph.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cashguo.top/gtozwdmlan.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtstyhsnvw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtnucqnnhm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtsppvokqj.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtwhxzfksq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtkenmhngx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtlxauaans.html


<!-- 参考信息 -->