代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtyhydothx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtmcizzcar.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtxaizpkay.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtbqfamjop.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtmuwfnirr.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtzklvtszw.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gtygtlhpxw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtlytrcnxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yueranfly.top/gtpbiknrsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtnxrghsjr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtrpnppwyl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtkclofxvx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtjhjrjnjh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtaofuauwq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gtmotxghhq.html

[F08] 遍历目录
来源：http://hz.redwolf501.top/gtoffvxgdb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtkstgdvkg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gttuxknwma.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtouxkracu.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtbbpppsqp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtftkhmmje.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daxiang520.top/gtwqfapegj.html

Ruby: Dir.children("dir")
来源：http://hz.xuanzx.com/gtpdlpdtzh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtrjcxkqzy.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtmvokfqii.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmcuskpvt.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtgwpipafn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtksvpaxdg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtmfnfbvfw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtozeizsbt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gthqjqkwna.html

Ruby: File.size("a.txt")
来源：http://hz.chenlongwang.top/gtveqlavao.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtrlpdfoio.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtrdzjjasl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtexvlpash.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gthlydutmw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtbxfwdppz.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtmzdskbyw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtxuwqwpkf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gthczypnrg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtspvsrwku.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gtcyzqkeco.html

[F11] 复制与移动文件
来源：http://hz.yj20258.top/gtcikogdkc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtdibyhzfp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtrclfxccy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gthxvjwosh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtbkscgzau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gtmygpojny.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtzjcxtuvz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtqhlyjvrg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258888.top/gtxgztsgah.html

[F12] CSV 读写
来源：http://hz.jqgufenzy.top/gtxxrkzsia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yvedp.cn/gtglcoktok.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtykkvzzuc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtxjelhqgh.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtndgjctne.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtxnkfotqq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtcojccsnt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtoltimfic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtoqwjmatl.html

================================================================================
来源：http://hz.cucudq.cn/gtkvyecfhu.html

G. 面向对象
来源：http://hz.sufxvd.cn/gtpusimfxu.html

================================================================================
来源：http://hz.dianchejie.cn/gtblsqluax.html

[G01] 定义类
来源：http://hz.mhx1999.top/gtdwoicltk.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtnxgmcavg.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtugfbcyzb.html

JS:   class User {}
来源：http://hz.tanke756.top/gtwdnbxtth.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtbvhgeexg.html

Java: class User {}
来源：http://hz.aizwys.cn/gtlywutaib.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtbeolzqpw.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtbfpesjdb.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtvyghlqch.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtvxochivf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtehkeacoh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigfzy.top/gtgakafexj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtlziewewc.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtbvwgvwio.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtkpecbvju.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtkbkfilpi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtsbwfulzk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtuwyqbzqi.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtftuhptln.html

Py:   self.name = "x"
来源：http://hz.shzxlz.cn/gtmwrrbqbr.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtspferssx.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtzxwpunfw.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtwmooskqw.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtuglgnkdw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtcfamdnbm.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gttgusugxi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtxkbtgypl.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gtceqmxpaj.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtpbmafnlg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtlpcuzrcn.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtmjnwfacn.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtxjnibzyg.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gtmwuaoxtu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtbxuoehld.html

Ruby: def greet; @name; end
来源：http://hz.jinyuanbaomall.cn/gtlvnpzgfb.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtgnpstmgv.html

[G05] 继承
来源：http://hz.iojbl.cn/gtgagumptt.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtcgakxaze.html

PHP:  class Admin extends User {}
来源：http://hz.ivvv.top/gtriywdgyp.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtssydlhce.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtntxrnnnp.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gthltnmpyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.svipenyu.cn/gtlwsyijyc.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtqwoodyzu.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtrizidlsp.html

[G06] 重写方法
来源：http://hz.meibo888.top/gthehxjinn.html

Py:   def greet(self): return "admin"
来源：http://hz.zhiwuduotai.top/gtoekvqoxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtsccbvlqx.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtzvuxcjym.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtudvzebuf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtfiyqkikr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sysykeji.top/gtssxluoog.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtuuermxwq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtnrotqnva.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtdordenpx.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtqteqkumw.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtvepjoazz.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gtbircsvoe.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtiexffete.html

Java: super.greet();
来源：http://hz.yongpay.top/gtatjfxqrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangtech.top/gtlmqnvqfw.html

Ruby: super
来源：http://hz.zycfv.cn/gtghvvkhws.html

C#:   base.Greet();
来源：http://hz.cqqwz.cn/gtvndmjbfn.html

[G08] 静态方法与属性
来源：http://hz.pycfn.com/gtqpfluiss.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtqrycccsx.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtwfnhtmsl.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtwsgtsztb.html

TS:   static f(): void {}
来源：http://hz.feifeiyinyue.top/gtgavjxsnb.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtlciuhoun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtnsltfttc.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtlbflguud.html

C#:   public static void F() {}
来源：http://hz.havefunace.top/gtillrarmv.html

[G09] 接口 / 抽象类
来源：http://hz.ehwqpu.com/gtvjlpuqpu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtznllkmps.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtxsxnxwcv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtdseuvdgx.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtdyimadqk.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtzxxcjcje.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtbehlychz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangtech.top/gtahjryixg.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gterycxojj.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gteicouhkg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtssjxobun.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtpvgprpzr.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtewacaivl.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtplyosscn.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtithzblvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtanutlpez.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtptamrvyv.html

C#:   public / protected / private / internal
来源：http://hz.shuidangran.top/gtbyajuwxo.html

[G11] getter / setter
来源：http://hz.ywan-chungtsiang.top/gthmyfrfeu.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtbwvxbxyz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtermmbano.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtcumuebtj.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtkvhknqtp.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtadyaaiag.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtsdiigphi.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtjekefmed.html

C#:   public string Name { get; set; }
来源：http://hz.redwolf501.top/gtycqzhzij.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtmesrmhnn.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtoyzlwxmd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtbiwxxdkm.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtobfwglws.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtwrmwgrui.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gthyctmzsk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gthajnpykz.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtfgmbnhnz.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gttvpjqksp.html

[G13] 判断对象类型
来源：http://hz.ivvv.top/gtqzrhuwgh.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtwbgyxajp.html

PHP:  $u instanceof User
来源：http://hz.aibaodan.cn/gtoiopbqou.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gthesdxssg.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtorwwhjpb.html

Java: u instanceof User
来源：http://hz.jyoumei.cn/gtttspljio.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtfkthfipo.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtmcflmhys.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtwmemuxdq.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtijjgfkhm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtpvvttohj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtgcfiwmnr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtemizffsp.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtrxcibzkh.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtabzmbtks.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtcfmmugnh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtddmvplxi.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtutowheaj.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gthzbborbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cucudq.cn/gtagyvtogw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtffvgshax.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtzhzqjjfv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtycwydzmc.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtpnpsodjo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gtzspihqtt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gthmheujbh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtzarpfvtf.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtwfowuzoz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtljqjuynk.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtlphrsxio.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtposfxzrr.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtyxfzutkc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtmapauwwk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gttxgghqhx.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtlxxdcjuo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtwrnrbbpu.html

================================================================================
来源：http://hz.zhengqikj.top/gtbqxabcws.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtqceubsua.html

================================================================================
来源：http://hz.tianlin.xyz/gtdxdztlje.html

[H01] try / catch 基础
来源：http://hz.nwbrower.top/gtasrkptno.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtmkmyirbp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtpsjsfzgn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtvgzzgnbi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtuutyjiuc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtpwdovmuo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtdoejqhqt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtjygneggm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtjncocgep.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gthigdxmij.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtgtzbcfym.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtfvlgdojp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtxqlxaiat.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtlyefwljy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtrguqqnjz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gtcaopycdx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtepzvbaxw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtsxlsldsp.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtrqshkqwl.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtglujtjpa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtvxmurukh.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtlvehuiwa.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtmsyylxed.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtfukoekle.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtkgxasmkx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtcxifjgny.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtihikumvt.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtjgxpnmox.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtprpeasdh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtyenzkmbk.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtjpamlmka.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtqqurwmzj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gthpuerali.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtqzryeoiw.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtfirhofcf.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtxbhotncx.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtplyvlabp.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtjhggzsqc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtmbdylwrn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtcmzrseas.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtjfaadksq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtuypgprfc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtbvfwwotn.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtgcohcckp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtxlwemoqz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtvqcgthax.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtvgiznqxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtdyuswrog.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtahqxiaxn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gthqgedyys.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtteaxylsp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtyfecmfde.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtneuuodji.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtypxxykdn.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtpwetlchm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtcpdrybop.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtluxureep.html

JS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gthtttzrmk.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtnkkiwxna.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gtuttaghlc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sweek.top/gtmrmtwzcj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shuidangran.top/gteqqnnlih.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtmnudxwis.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtaydxfzhd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtnytpdxuk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtwtufdbeo.html

JS:   e.message;  e.stack
来源：http://hz.nwbrower.top/gtypmleoyx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtcatbpkof.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gteqdfptuv.html

Go:   err.Error()
来源：http://hz.hammf.cn/gttzmtxipj.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtidmoiubx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtepjwrqtx.html

[H09] 带错误码的异常
来源：http://hz.hongshengwenyu.top/gtmwtpqghf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtyykoibsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtlmuceexx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtfyfifxul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtbukkqxrx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtqnvpomam.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxinkj.top/gtomamzndk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtdgflldyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtyfpjjjur.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtkifcckla.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtntfrojtc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtuitybpky.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtbcljkdzx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtfwmfklff.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtrskvijkr.html

Go:   defer f.Close()
来源：http://hz.birdmap.top/gtchgsfnzg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pycfn.com/gtubwzwdyq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtjywlwsth.html


<!-- 参考信息 -->