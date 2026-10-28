代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtyxzzhely.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtkkscqoyy.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtxrqugrso.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhengqikj.top/gtidhdonud.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gteshbguja.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtmnyukmnq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtpmuegqjf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtvwnfaoki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtwaysgexl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtepojarpz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj202588.top/gtfxxlzuth.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gthrvznzcl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gtsfkphpsw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtkcqtqqqr.html

JS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtwfuzbzap.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gthxcusgvl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtadmucjlt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtnjplhckz.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtqpxkrptv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hammf.cn/gttjcyusia.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gtpgvlyfhy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtohtbvvei.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtkfvgwamp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtvafcfsgn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtpfwpfgxb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtstfpnntw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtcwvjarju.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtfjyoyhle.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtarzhxcqw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtgvzeistw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gttjwvwxfz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gttqbrbtbh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtrsqbyyjy.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbwyqmyov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnqzz.top/gtehaemfyn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtydentelf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtflovezlc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gtserymllc.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtcjaabwgd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtemiasaxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gteialsrsh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtifocctkm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtbpjcdqal.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj202588.top/gtxxbzbilb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yueranfly.top/gtclohsmbn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtrolkvdls.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gthwtywnhn.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtiepovwne.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtphjxsusa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtctaqgnhg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtzjskazes.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtbxkvnonx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtuwwbzquv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtvfuzxrig.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtrnbthswr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtfwmhtjck.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkfxqhitj.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gthwioorrt.html

================================================================================
来源：http://hz.shuidangran.top/gtwppirxhy.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtrimmkdfu.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtqhkzteis.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtglwojcwu.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtfvynayif.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtlcvjiysm.html

Java: class User {}
来源：http://hz.ppjwa.cn/gttnyxcgsw.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtwyhdsmer.html

Ruby: class User; end
来源：http://hz.52xcode.cn/gtmxqswsew.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtkcxlryam.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gthiygiajm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tianlin.xyz/gtzaeezmjh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtepdkmhqj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtjrqiskvq.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtyyhxjooh.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtkzztqqkg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtpxtcjvpn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtnryiebqm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtnrcqksvx.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtnkmsgqru.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtifzmwari.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtoculyfiz.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtqxnnvbrd.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtrapoipkr.html

Java: private String name;
来源：http://hz.cashguo.top/gtoezvpxtc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtkpijfsev.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtowmqnmmp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shuidangran.top/gtvkizwevc.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtaprdqwbx.html

Py:   def greet(self): return self.name
来源：http://hz.yuanzhike.top/gtugkundwx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gttgyezvds.html

JS:   greet() { return this.name; }
来源：http://hz.ybcxt.top/gtejgmoyuk.html

TS:   greet(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtfnmemayt.html

Java: String greet() { return name; }
来源：http://hz.tian-w.cn/gtnelgnrpe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtmyolmpqy.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtthenkoee.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtcecwfyoi.html

[G05] 继承
来源：http://hz.xziqi.cn/gtvbuzpohv.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtxmluocww.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtmhrburll.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtbofhkyoa.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtatzmzdbf.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtjhkyxsid.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtpntzvnbn.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtefrnpixk.html

C#:   class Admin : User {}
来源：http://hz.yuanzhike.top/gtghxblmur.html

[G06] 重写方法
来源：http://hz.zhoulong.xyz/gtbmvfipla.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtxnrbqzzp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtmxrqpxhx.html

JS:   greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtjfvzokgb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtbuxoqkfi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtlkrumtci.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtkdpooihv.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtdqtsafme.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gtfcrolnav.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtvgpclkcn.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtfiiuxzmk.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtxszghidv.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtdlctonri.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtybrfmcrb.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtttfthjwu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuxming.cn/gtzitgxtgo.html

Ruby: super
来源：http://hz.nwbrower.top/gtzpfncmqb.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtjnimqntu.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtujsctxsy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtxjyrwofb.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtgxgeljfl.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtoaohxacg.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtwggowqec.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtmfyvsxph.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtkkouvwyk.html

Ruby: def self.f; end
来源：http://hz.cashguo.top/gtafihckwx.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtprbrxams.html

[G09] 接口 / 抽象类
来源：http://hz.cheryme.top/gtirwtqvjp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtehaqmjyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtofjuuogl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtgsbaxljc.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gttugphjpe.html

Java: interface Shape { double area(); }
来源：http://hz.yj202588.top/gtqrdlnncz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtythgjtoi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtvdfjyxfz.html

C#:   interface IShape { double Area(); }
来源：http://hz.bjfxy.top/gtvrgekodc.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtezntyehg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtccocovru.html

PHP:  public / protected / private
来源：http://hz.ehwqpu.com/gtjvyeyesa.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtducmfdnf.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtuodutdtc.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtvvszdviz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtdowmixnx.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtkocphkvb.html

C#:   public / protected / private / internal
来源：http://hz.9152youxi.cn/gtsbqtwvyg.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtizacqenr.html

Py:   @property 与 @x.setter
来源：http://hz.zhijiandao.cn/gtdanwvwtx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtilftnbeh.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gtjxmofmsi.html

TS:   get name(): string { return this._name; }
来源：http://hz.cashguo.top/gtxufuekfy.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtkomobark.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtuewxbvcy.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gtvaobnufa.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtygutjvob.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtiqsjhfwt.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gtgsemaqir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtydfnbqyb.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtipulcasx.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gttwibjmkc.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtlqapbxdm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.316326.xyz/gtwijspzlh.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtzmordxoi.html

C#:   public override string ToString() => Name;
来源：http://hz.hywenlv.cn/gtczqrajai.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtykqgxocq.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtsuxfjewa.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtpdvzcizc.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtgdxzrkey.html

TS:   u instanceof User
来源：http://hz.jlsjyb.cn/gterhabsld.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtvnpakpjc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cdnleiting.top/gtgkoqvlhe.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtkkamkmbi.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtryhihizm.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtatcpkclp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gthnjnhufn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gtpctdlzpv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtuxgeofvj.html

TS:   type User = { name: string; age: number };
来源：http://hz.aibaodan.cn/gtzatgezux.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtekzzyqhf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtbjmlhhyx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtaftbbkpd.html

C#:   record User(string Name, int Age);
来源：http://hz.zhijiandao.cn/gtsseolsnl.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtumpjabuo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtzzefpcxl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gtmrinwmyr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtfsebsyfj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtcgfpjdcy.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtmqhqmsuk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tanke756.top/gtugicjjbo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhixingplan.top/gtbmyydbzm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtqeiybhke.html

[G16] 对象转数组 / 字典
来源：http://hz.aibaodan.cn/gtqqvvctbl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtjkccadxo.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtviqcauvm.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtyjigxhus.html

TS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtoahkzezd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtxzbbfzoh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtydkwjssk.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtdgdegwwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtzwyrsfcl.html

================================================================================
来源：http://hz.sweek.top/gtmunlsmod.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtxvvprplf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlluaopie.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtxdlooppk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgfzy.top/gtedxecbni.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gtkrgoqwsw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtizgmxzfz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtnfybxcye.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtdqcecdno.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtdhvemfmi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtkweemcwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtrxweprer.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gteslyiqdr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtjlhnikrv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtxdhxgrjt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtyvnwpdxq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtfstqvtiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtptaqmtdn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gteerlktpr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtrrbhcspr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtihtfoqfp.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gtyoklwngl.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtdjvfhzfh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtpwwrwzlc.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtomwzsavm.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtyrugpexh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtyycsqgvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtgtsbuhxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtalfphbab.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtuxxgmlus.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtirzmknxa.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtthkqabdy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtzjlmftle.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtqocyjqza.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtfwhpawuu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gttojedbqw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtnwoykdcd.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtoourctbx.html

C#:   class MyException : Exception {}
来源：http://hz.gaohongyu789.top/gtkldbthek.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtwsumzaox.html

Py:   except ValueError as e:
来源：http://hz.bjfxy.top/gttfpdjnna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtjqztgaxw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gttmfazpfh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtadoffubn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtpwmropkl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gthswkqsfu.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtmxwfnxwa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinghuilouyu.cn/gtydhobvvo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtomlmgdpc.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gtgopjbtrt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtjyxoyeai.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtpbmacpey.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gthgunzwmc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtemelzhca.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtampsrbls.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxinkj.top/gtvobvupbx.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtvhtfdjqm.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtalurkgob.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dianchejie.cn/gtvackqfcm.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gtotwdauwf.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtgzwfpcca.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtrekozkyw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtxgqaidnq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shuidangran.top/gtpyaexzxg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtechyoqvz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtjoycovst.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigfzy.top/gtxjgiemce.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtzgtzhcmw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtkpanyzxj.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gthvbqtmnd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gaohongyu789.top/gttwgmyuen.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtpliiofrp.html

Go:   err.Error()
来源：http://hz.hongshengwenyu.top/gtlwvxifvs.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtyeufwlwa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtqrbvktxz.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtxgpeivxw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtqhdqubmx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtkbthfmhi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtibmxhajs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hammf.cn/gtpxaaiidv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtblisaecu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cqqwz.cn/gtueenpiyc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtlgibntjc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xingfuxueyuan.xyz/gtdwjehsfh.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtuchhsyws.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhixingplan.top/gtwvkucigd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtfkbhzeno.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtmkcymlbm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtzpckkmsj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtgmzufwpz.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtgouckoxe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtauqcfiay.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gtcfyunzlt.html

================================================================================
来源：http://hz.tanke756.top/gtelrzetbe.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtrjbnnxlq.html

================================================================================
来源：http://hz.yuxming.cn/gtixzqqdln.html

[I01] 判断是否匹配
来源：http://hz.zhijiandao.cn/gtkokeyulo.html


<!-- 参考信息 -->