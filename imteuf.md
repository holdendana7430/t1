代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guannengcc.top/gthrvbvihh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtxtqyrkob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtbsqqhjzx.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtogkycixt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtgmdjomne.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtpjzgxxan.html

JS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtpngumvou.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtrhkvmaje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtkbugzraq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shuidangran.top/gthaevfhbn.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtyeqqrhvl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtgwuymtvh.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtssihzugy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtgpepcbmy.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gthtghhtff.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtqnuorhrr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtusowlcwj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtsotjcaxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtzjosrnkk.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gttxidgrru.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangshuangyany.cn/gteuzxushy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gtkrxkmucy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gturqpkdbs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gtnswamrrl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtqrkeosgt.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtqqfcshft.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtvlmxppcf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtubjyvqmu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtnmvhbyug.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtjeebtaco.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtcxcbwhpo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtahqckblr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtucxcvkrx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtufovxiiv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtyfbgrads.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gteayisogj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtlfxzzngz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtljpsjkvo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtnftdreed.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtmzjwurrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtjqohdisv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ppjwa.cn/gtbgrgfder.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtmumiqhad.html

TS:   // 同上
来源：http://hz.yongpay.top/gtkidptnwp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gtfcsvjkqm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtrxskshvx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtffeguydg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtzyukezrq.html

================================================================================
来源：http://hz.xinyue.icu/gtztvcnnls.html

G. 面向对象
来源：http://hz.yonumen.top/gtzcamohrq.html

================================================================================
来源：http://hz.sxryk.cn/gtboyyypmi.html

[G01] 定义类
来源：http://hz.xingfuxueyuan.xyz/gtkjgvecys.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtscsocrzw.html

PHP:  class User {}
来源：http://hz.jiagoushi.top/gthsrldcuf.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtfwwsdwkh.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtewgnxoqu.html

Java: class User {}
来源：http://hz.cucudq.cn/gthtpcmhrl.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtqgcbpobj.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtlldoifat.html

C#:   class User {}
来源：http://hz.quarkkingdee.top/gtkktjbpxh.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtxpxjusje.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtkfchakdu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtcyuhktuz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtqwbkfmkb.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtkgamkjkr.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtgcgodlnc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtfnarcbbi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtazzraius.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtodrdhrgs.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtjkmfvbou.html

Py:   self.name = "x"
来源：http://hz.tianlin.xyz/gtqwlujjsf.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtaguzwazr.html

JS:   this.name = "x";
来源：http://hz.daria6918.cn/gtwvxzazao.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtxwlcifkl.html

Java: private String name;
来源：http://hz.cucudq.cn/gthnseqddb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtmlbinbml.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtrvjscxfh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tian-w.cn/gtcbdbqpfu.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtlspzmstc.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtnsufezxv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtnivbxewq.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gtnhplzpbh.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtqlleczgg.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtbdbyfjmn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtqllkghwn.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gtsvuhtnmi.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtgabisbhf.html

[G05] 继承
来源：http://hz.xuanzx.com/gtbvjuzkup.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtasqtoinp.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtuhxunruf.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtwqruvbet.html

TS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtstaidbyn.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtkcelflwz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtwfagetmb.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtiuoijbzw.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtybgdafqp.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtnafhkizf.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtfwpfikhb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtaamegnnf.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtqaralcmg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtafbyichu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gthiuwwixj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gtgnfvjdxt.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtogvdwtjm.html

C#:   public override string Greet() => "admin";
来源：http://hz.feifeiyinyue.top/gtfkpidhqc.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtsphyltly.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtugyjlujt.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtqbqmmngz.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtfqamltld.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtpqrzmzmf.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtxgwoqfbb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gteroiadnj.html

Ruby: super
来源：http://hz.sxryk.cn/gtpvrkbcnq.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gthxsiitrr.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtibzvjrwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtrtcakizw.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtsztswnvh.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtrwptyntp.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtdjtymsvn.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtsbigwemt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtpsqdcppd.html

Ruby: def self.f; end
来源：http://hz.yueranfly.top/gtbpvqeojl.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtaokeabph.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtojyqlupx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtisrodzyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtydkdnxzt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtrszyzbyc.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtxtztozuc.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtjqhlzxjv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxinkj.top/gtobcbwnvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gttohlrfez.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtvnxccyqu.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtflvxebid.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgufenzy.top/gtsfiiuswa.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtaxzkqpld.html

JS:   #private 字段；其余公开
来源：http://hz.yongpay.top/gticjrhvbk.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtmhjzumsw.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtuelplqyu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtwmszlksp.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gteolfisbn.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtrqsbtceu.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtzmwmivss.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtcpjkcdyx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtslzvkszw.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtpjvjapbc.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtqzudmseu.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtxvvpblke.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtlimblxqt.html

Ruby: attr_accessor :name
来源：http://hz.dianchejie.cn/gtutjwvscu.html

C#:   public string Name { get; set; }
来源：http://hz.kuanghao11.cn/gtvqcahvkb.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtcrbltvhz.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gthiupxqbs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtdjeoiear.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtanoyjily.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtysqjazsx.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtdtmzxbpq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtsoaldbdg.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtbibclhkr.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtewwnfmgt.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtjmxkiacm.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtcceuuieu.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtcdjqjcdq.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtxebqscij.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtwstiaxko.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtctehgqjh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtjzlnyuhe.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtjvwzwnme.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtlxnclgap.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtucctfizz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gtsontbsbu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtfreievuh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtfjfthznc.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gtmjaxhbcb.html

Java: record User(String name, int age) {}
来源：http://hz.tanke756.top/gtxelrjqyg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtzbtentwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtyzhuwhdf.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtczywylfo.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtrsdrseqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtujqcuald.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtgdlqrrts.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtikzynaur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtbkuvjwrr.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gtmxyqmuvv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gthcekthuv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhoulong.xyz/gtfdxfomcn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtrskmhzka.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtnylzxunt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtcifizyjy.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtwjiyhmds.html

JS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtplfnowkc.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtgcskppzu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtjmoiqcyw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtkygsheza.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtsqcuvfay.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtiltigjch.html

================================================================================
来源：http://hz.hnqzz.top/gtobfvfdjj.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtyhduugth.html

================================================================================
来源：http://hz.sysykeji.top/gtpvguqdkf.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtfetmquia.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtfcccowyi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtyesclefu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtzmsgbwqb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtycpvghwh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtuusyblco.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtmtuciiro.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtnmxigqmk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtjfihqlzo.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtxwhqmrpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gtnagkeinq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtlfbtrdfw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtkjbimsgh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtuyxveonh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtgcpnjmmr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gtvwmwlcgz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shuidangran.top/gtkhdmjrbp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtmpeluwhb.html

[H03] 主动抛出异常
来源：http://hz.yj20258888.top/gtldbjudhr.html

Py:   raise ValueError("错误信息")
来源：http://hz.cashguo.top/gtzryqwsjz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtvazqshcp.html

JS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtsgejdido.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gteninlwyz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtsngyxdvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtoswxqrac.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydjk.org.cn/gtiwqosyam.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtixwtyetp.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtabethanx.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtrezaquox.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtqwvziyct.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtawulanuv.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtaopfpcxb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtjalglzwe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xinyue.icu/gtlqsagufp.html

Ruby: class MyError < StandardError; end
来源：http://hz.cdnleiting.top/gtypfczogn.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtogawmswe.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtqdrfmkxm.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtyajpnexc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtnzflfimj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gteclqarnt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gttninyydq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtikowxhxh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.52xcode.cn/gtgymqzeks.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gttdwurysz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gtfkxauxhx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hfpthk.cn/gtgwidsrqs.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtewtdglay.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtjkpicpqd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtntqlokck.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtvdazfxhe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtqfgfqpju.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtfejdxwnl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gtpwwktunf.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtxxexnowt.html

[H07] 断言
来源：http://hz.yj20258.top/gtnjgncsab.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gtwqrsafpb.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtokwotear.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gttuobpzaq.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtquaowrdi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gttsqxuebn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gtypgsovkb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtnvnvfetk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtljqsfyxd.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gttqkaqcnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sufxvd.cn/gtdbhtuoyv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gteyeqdorc.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gtkpgzqycq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangdashe.top/gtazvwvryy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtvnbdmbtm.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtsnszagrw.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtxswahzbt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtaawhqbsp.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtmunbdiqh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtkkixjsld.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtbtzcalum.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtioowhpna.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gthkfblcwb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cheryme.top/gtbzbusayz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtkywkziuq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtkpegerkn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtjlulwqfp.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtqlhxczfy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtczijbmsx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtdqpagypf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtvsoaboyn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtxtnvqgwv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtphtlxxao.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtyxyuzxah.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtmpzklqra.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtrtcwdkgl.html

================================================================================
来源：http://hz.dianchejie.cn/gtpbmcqvvp.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtikoaxjpx.html

================================================================================
来源：http://hz.cheryme.top/gtdwbrslkn.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtdamiiclq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gtpjcemscl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtujomzotz.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtcxbvbkat.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtnjagllmz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtpypvypov.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtbsxcjrer.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtemetlcfn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtvxhyleyy.html


<!-- 参考信息 -->