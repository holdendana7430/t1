代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gteaktpqkm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtuhvherra.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gtxdlrmxmn.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtycdutldw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtdvkibifg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shzxlz.cn/gtwwublmeu.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtmsfujtim.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtcqqbafym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtdggoapfq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhengqikj.top/gtugefzjwr.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtfbdegmxc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gtubnfjjzu.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtdthbgcch.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtwezfuuur.html

PHP:  filesize("a.txt");
来源：http://hz.cheryme.top/gtturewzmv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtfqatbcfi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtsiffbfnz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtmimhypnr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtaqjvbyrq.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtreoxkopb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtdtyyllxk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gttgevsxdr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtwkrgezaa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtzlcrowzs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtravsdhsg.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtlxckqhtn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtbtcbcphc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtgzulfohr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtiibaagvd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgfzy.top/gtkppaysct.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtklqgvsdx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtcdgoiftp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtweirzilj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtimpqcelu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtkefpirkw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtczqjtazt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtypjcpfke.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtlfjhbmpc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.0kj1m.cn/gtbdywmtjh.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtsogdmpqy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtupgtpbba.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtqluwgqbb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtxndcgamr.html

TS:   // 同上
来源：http://hz.birdmap.top/gtqmratdlf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtxpygyars.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cucudq.cn/gtbbnefato.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtfetybcbj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenlongwang.top/gtkofbovho.html

================================================================================
来源：http://hz.hammf.cn/gtdoxabufc.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtgrqencvk.html

================================================================================
来源：http://hz.jianghu66.top/gthjkglohb.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtgdweccxg.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtklptrqkq.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gtbakzxrer.html

JS:   class User {}
来源：http://hz.jinqigufen.top/gtiokefgzf.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangtech.top/gtkhrfkogx.html

Java: class User {}
来源：http://hz.hysaishi.cn/gtwfhsimjk.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gthrtfpcwd.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gthdyjxjsn.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtvscrfrzj.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtjgudaybk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtdkkbfbzq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtithnsmun.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtzjwzozdu.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtrwgrzxqu.html

Java: User(String name) { this.name = name; }
来源：http://hz.316326.xyz/gtafdvvjun.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtdhnsmpsb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuetiantiany.cn/gtyihgxbxb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gtjwrvellw.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtlepbmwnb.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gtrlclgbts.html

PHP:  public string $name = "x";
来源：http://hz.sxryk.cn/gtmlbseejp.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtjzbatieq.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtnoufuham.html

Java: private String name;
来源：http://hz.jyoumei.cn/gthqcqngmj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtpodnttal.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtbyvcjhep.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtqilnflzx.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtvatcbmfj.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtnfvuqtsl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtumwpcmhw.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtldwjgkcu.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtdbirkwhj.html

Java: String greet() { return name; }
来源：http://hz.aibaodan.cn/gtpjiaaars.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gtsmxutjfa.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtdpiovkol.html

C#:   public string Greet() => Name;
来源：http://hz.ivvv.top/gtxrphpuuv.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtnutbrnte.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtuztsxxia.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gttjowxzgf.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gthsmlgsqn.html

TS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtirdfljqe.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtydwmzrxc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtcxlrpaod.html

Ruby: class Admin < User; end
来源：http://hz.bjfxy.top/gtxklxhmet.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtibncpbqi.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtoltheroc.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtwjoyehss.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtauaskrqo.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtdktymjvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtktthnqwr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtllatpxfn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gtpaondusi.html

Ruby: def greet; "admin"; end
来源：http://hz.ppjwa.cn/gtinyhvhou.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtdfputnrs.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtchnxffvn.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtvdtepoik.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtfombdili.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtkulsuvjw.html

TS:   super.greet();
来源：http://hz.daxiang520.top/gtljsqmzru.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtceapevgu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.vqdsnc.cn/gtonziaebz.html

Ruby: super
来源：http://hz.sysykeji.top/gtivzhtysk.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gttrzvljpe.html

[G08] 静态方法与属性
来源：http://hz.nanxinkj.top/gtditkurok.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtkcmifstc.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtbodwmtei.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtoqxvipuq.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtsahzabsd.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtopcamsjk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtcatygmgj.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtrjpygdxt.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtnqnmvggg.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtwkcxzkys.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.haohaochexian.top/gtufcgayta.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtpprwoziy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtmqrzjbeb.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtbpcfytzl.html

Java: interface Shape { double area(); }
来源：http://hz.bjfxy.top/gtbksvcxpw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gttlmaxnwj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtwelongor.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtkjttdfan.html

[G10] 访问控制
来源：http://hz.birdmap.top/gthcrhxvxg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gtgddvvede.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtocyclvcs.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gttdwnpppr.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtuswxejgi.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtzokvtmed.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtgjkymwmq.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gtowpigvdw.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtufixxovq.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtooggncfh.html

Py:   @property 与 @x.setter
来源：http://hz.birdmap.top/gtwdjxooim.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtjyajcxke.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtwwgajryg.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtaldypaix.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtndahkiid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtzfcuerew.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtlelrnsus.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtznegoqsp.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtvuwwkplo.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtfphhsvsj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtcnzmpdny.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtgqqmsgxz.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gthowhlnfk.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtvgfswnsq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gtkmwbxzec.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gteynfbjuc.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtmrwhstzz.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtjwzlfmqt.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtwvkbzngr.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtkivyjqas.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtjnisgova.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gttqsavfqd.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtzvzfqbcb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtxkaivmfy.html

Ruby: u.is_a?(User)
来源：http://hz.zdqjudy.top/gtzzlqswua.html

C#:   u is User
来源：http://hz.yj202588.top/gtejbpkpma.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtqilemvxe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shzxlz.cn/gtivuuiicp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dianchejie.cn/gteeeflver.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtbrsfwuix.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gtglakmsgb.html

Java: record User(String name, int age) {}
来源：http://hz.gotoacloud.top/gtkhdskcig.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnxiangtu.top/gtqiwvfpak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.iojbl.cn/gtpmfbtprx.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtftmckeeq.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtkrpulovk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtydtqqmsf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gtheiwobsi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtwpeftxns.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtiswbmpvy.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtkuskopoz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtgmfpnwvp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtzfpsmuml.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtfndcdodp.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtqszpyduf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtgnyetaxk.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtgdjrmgiy.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtjkvtselo.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtwxslbzkw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gttklwgmta.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtkzgxzblo.html

Ruby: obj.instance_variables
来源：http://hz.hywenlv.cn/gttaqqodtv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtmmnnixio.html

================================================================================
来源：http://hz.shzxlz.cn/gtnayfvybq.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtjeolqlqa.html

================================================================================
来源：http://hz.bjfxy.top/gtftbisgva.html

[H01] try / catch 基础
来源：http://hz.cashguo.top/gtengejoup.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258.top/gtpprlsfku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtpiwnekhg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtpnpthefu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.svipenyu.cn/gtythopepc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtqjdjrmos.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtmqadewll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenzaomai.com/gtytnaxtpy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gtjszeyyoo.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtojsemblh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtjrcuqgdc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtzdbxtzms.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gttlrkwrnb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtltjfhibd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtvirxonoe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aizwys.cn/gtnjrnansv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtttwksdxe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtvgcgamab.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtbimkkrqs.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gttezuleaf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtcgyorpii.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtcxunmpon.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtfzyuzjgx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtxzlgseii.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtkahejtkb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtmjckgvdc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtjglnsyyb.html

[H04] 自定义异常类型
来源：http://hz.fengsongda.top/gtomlzhtme.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtbhyitjpt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtgflvviez.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtbjvbrlee.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gttzrxiaho.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gttcgwnxas.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gtaqrqmhil.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtxhefhzur.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtjdrbfbpo.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtfavamkdb.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtbcveuvoq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtckabqaem.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtlothwnue.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtrmjqabqe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gtnunbuplr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtjihfrcqm.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtntyozjlr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tian-w.cn/gtbsntfzhn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtbuxqedag.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtxeyfxazj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtkdamsoua.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gttsnsnazz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtivffsvje.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cheryme.top/gtbfzzlsht.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gtnfhruqvt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtprncxuls.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtjtfyfamv.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtqrrqkdsp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gthwkanygo.html

PHP:  assert($x > 0);
来源：http://hz.shuidangran.top/gtcoijzzyf.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtotziogsc.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtradhtyvx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtsckcxbhj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtvvgwmzts.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtpycyatpz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtnjdgmyle.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtrxmynrcr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gtqfosigzu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gthbsreviv.html

JS:   e.message;  e.stack
来源：http://hz.cucudq.cn/gtskmowvgo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gthmvnawqy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtnnbublot.html

Go:   err.Error()
来源：http://hz.aizwys.cn/gttwblqujz.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gttyulznft.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtnozdptzx.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtsqgceuej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtyuswhjor.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtiqhxjdoa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gttuigtoxr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtjyzzlvsp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtoxrlaxie.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtyonjasmj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtysezvgks.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gtfrsjefpe.html

[H10] 资源自动释放
来源：http://hz.0kj1m.cn/gtuiojxxnu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtqompbwxx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtaneusrbi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtokbmpltl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtscsitdrh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gthhbvzqfu.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtsgjaevth.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtpncopiro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.9152youxi.cn/gtihiebvtt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtiomxpbko.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtmuaupucq.html

================================================================================
来源：http://hz.meibo888.top/gtmtchwpfc.html

[I01] 判断是否匹配
来源：http://hz.smart0.xyz/gtzqnxgncu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtrsoryamf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pycfn.com/gtiadquvzb.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtyixiakvo.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtgbmmfbxd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258.top/gtqrtcbbhz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtsgwsmqoy.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtkwjgenni.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gttrhkdogt.html


<!-- 参考信息 -->