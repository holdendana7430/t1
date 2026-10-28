代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.aibaodan.cn/gtgwjkivuq.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gttluhwhbn.html

Py:   os.remove("a.txt")
来源：http://hz.fengsongda.top/gtdnfbmxof.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtoatbqzly.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtbzsglmqz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtpsbjffxi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtapdqopcm.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtjesjerns.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgufenzy.top/gtrdmevmek.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtxwjevkff.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtofwzxoxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.haohaochexian.top/gtzfxivqpb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangtech.top/gtlrthqqao.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gttipknbap.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtxjphbohn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtikyoakbc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtlkcejtag.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtipbjetzw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtfvzkmenu.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtuibpheii.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtamelxxam.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtvxrdwolc.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtgdkfunzn.html

TS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtyiczmbli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtgdlqjavw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gtekyhimmr.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gthlazoqdz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtlhxzvbaf.html

[F09] 获取文件大小
来源：http://hz.havefunace.top/gtnehxmuwy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gtkjcslhjf.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtjqkjimkz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtvhkqdwvt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtjjciozny.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtlvyvdjjc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pengpengdd.cyou/gtpasncavi.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtmjwgfpvv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtytmzebrk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtuirfixvi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtyzojioyt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtyuvudfwq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtorgqewkv.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtjzsmwzkf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gttysvpnxv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yongpay.top/gtkeynxvqj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtmeiwfmsi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gthilztcuj.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtnccniyqn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtqxuvhxit.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtcenrobza.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtssgrlddy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtlmfiqshv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gthktbsxmi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gtwshnjzhq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtzcxzimkq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtmixhtgmb.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtyhzfbujy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtmxltghad.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gtohrvidht.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigfzy.top/gtyxzjpmva.html

TS:   // 同上
来源：http://hz.tanke756.top/gtrjszpbat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhiwuduotai.top/gtlebzleel.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtqxqoaemv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtlbtvusie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhiwuduotai.top/gtksrtohzy.html

================================================================================
来源：http://hz.ppjwa.cn/gtidqkjkfd.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtofyatqme.html

================================================================================
来源：http://hz.9152youxi.cn/gtepdqpfsn.html

[G01] 定义类
来源：http://hz.xuanzx.com/gtrqgdgnzi.html

Py:   class User: pass
来源：http://hz.yj20258.top/gthzrtcfqz.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtixuszyxh.html

JS:   class User {}
来源：http://hz.gotoacloud.top/gthclsdlet.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtkspauvuh.html

Java: class User {}
来源：http://hz.yj20258888.top/gtpwacxgfk.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtzomorxqq.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtdzuaaerr.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtunfqsknb.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtbcdclzgt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtvodjirkq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtlxycusqc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtolvpysiv.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtxxbuzxnc.html

Java: User(String name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtzsuamofc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtdfdselql.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtjtrfaxgq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtzlpbtrfx.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtxbrlgzxg.html

Py:   self.name = "x"
来源：http://hz.yueranfly.top/gtafzvkwjk.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtshegipbo.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtgqzcvslh.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gtrzzejnrf.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtbjfvpnuw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtdtytrydz.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtatzuvprn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhixingplan.top/gtzyayhhmt.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtejsvrccc.html

Py:   def greet(self): return self.name
来源：http://hz.cqqwz.cn/gtixvbwxbu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtxdscevfq.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gthhzloptg.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtkwwnokmj.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtwptmxrfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtdkffkheu.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtekspjkuy.html

C#:   public string Greet() => Name;
来源：http://hz.shzxlz.cn/gtnhfvnska.html

[G05] 继承
来源：http://hz.sysykeji.top/gtrjpznkps.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtnxuodzmi.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gtiiczwrct.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtrqqymxcu.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtaedcttui.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gtzirpnguk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtiozsflyq.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtmxxepuff.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtjdesvisz.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtczsyqfvk.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtrdszlfcj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtoozraslw.html

JS:   greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtkvvzhmff.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtfbfapimm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtcbejieku.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sufxvd.cn/gthakhynoo.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtpnpojhqc.html

C#:   public override string Greet() => "admin";
来源：http://hz.daria6918.cn/gtktdjxuul.html

[G07] 调用父类方法
来源：http://hz.shzxlz.cn/gtwcbouphr.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtesxlvnnb.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtsxntbqnq.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtbmfpjuum.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtrvfyvhof.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtareplahf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtwlrkzobw.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtdqnqlmaa.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtbfzqsqap.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtelhrbqha.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gthqjxfyco.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtwlwldrri.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtbruselra.html

TS:   static f(): void {}
来源：http://hz.shangyingyoupin.top/gtxddhaapo.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtnoyjizkh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtqgyewsfl.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtaawlcxoc.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtgbggbbyc.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtsbdjtobp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtgtzzvxtp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xziqi.cn/gtcdevsnpn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtbombjdxc.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gtqakikdcn.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtwqnixpwo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtpexxssdw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cqqwz.cn/gtudwdzkpc.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtsugzyudv.html

[G10] 访问控制
来源：http://hz.ehwqpu.com/gtqbeekxye.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gtukdkcedz.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtctmcnfix.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtxcrnhpki.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtwhfhkwrw.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtyraotwvj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtzqbuhxpk.html

Ruby: public / protected / private
来源：http://hz.vqdsnc.cn/gtfbmgcvcs.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtmfadwmzr.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtecqumnch.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtzuwozicc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtruezkazn.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtpuorxczl.html

TS:   get name(): string { return this._name; }
来源：http://hz.hfpthk.cn/gtnoedblbp.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtenrehjib.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtwexcukzf.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtukbddrwl.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtbrhxtuln.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtkbmwotcr.html

Py:   def __str__(self): return self.name
来源：http://hz.daria6918.cn/gtbtlzwzeb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtsrmpkkny.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtyheyvier.html

TS:   toString(): string { return this.name; }
来源：http://hz.tanke756.top/gtvskeuler.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtdeafzkyc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtwhivlkod.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtledjrliz.html

C#:   public override string ToString() => Name;
来源：http://hz.hywenlv.cn/gtvviokblr.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtmsmcrsfh.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtegxjzxim.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtxtgioeqt.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtnwrdmhfn.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtsiwuvzne.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtueunpnjr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtrxynfyyv.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtlsknnoca.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtsqknuavh.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtxzjdinor.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtpyleahmo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtwijkbviq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tanke756.top/gthzzuypqw.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtajnezzro.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtzgrgjqxe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtqgrphtms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtrzxsaypn.html

C#:   record User(string Name, int Age);
来源：http://hz.gzhubu.top/gtsmiobqag.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtkqsifcrz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtstrgwjql.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gthrelnapr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtfjoeteqw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtgfjkvcmu.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gtwyoqchnc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtlcopfdqr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtwudnsyji.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtsgownrgp.html

[G16] 对象转数组 / 字典
来源：http://hz.daria6918.cn/gteiyzapey.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gttgqlvkff.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtaubuyvht.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtkskmpecg.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtdbkephzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtuwqesshq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gtrepfctzo.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtzbilyhbr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gtlbonjqix.html

================================================================================
来源：http://hz.gotoacloud.top/gtyuqwmzrw.html

H. 异常与错误处理
来源：http://hz.jinqigfzy.top/gtrbyzcyyp.html

================================================================================
来源：http://hz.dashuyun.cn/gtzkaktvhv.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtohwxuahy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtphkykdpl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtdknntsor.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gteyujmaes.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtneivqkzj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gtxocyzjjz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtzmilutiy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtwjldsulv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtcqnioshq.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtxbgsomae.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtriyeomdf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtprdkkxbb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtlocsmmdv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtuxzikcea.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtgtvgngdj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtaebovezl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtqposvxwn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtfjuiqnni.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gtddkznbxl.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtpdmiwzvl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtslmmchvt.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtryclygkq.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gttafziogp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtmngzfjss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtuxgnihaz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtenvpwhcl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtruuwdmux.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtgfrikncf.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtcrzhlkbo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtotcdlayn.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtckslmlhx.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtcmtmkquk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtzertbznv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtektqlkdt.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gtzkzgwini.html

C#:   class MyException : Exception {}
来源：http://hz.hnqzz.top/gtoudupmhv.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtzezuwwfe.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtnhzhaqgp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtcmpqgbrj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtinbrunvg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtvyvtxbab.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtpumwqvxg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gthcjndaep.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtvsuyyppd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gttbhcwsqi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gogol.net.cn/gtuisiecia.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtudtoakku.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtruwzuofm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtelsnsria.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtateqkiwi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtzkofnjkc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtomirrasp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtalsijkhx.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtsgkudxns.html

[H07] 断言
来源：http://hz.guannengcc.top/gtllqjuecg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtuzzliqiy.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gtbbiaqbef.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtghomkmce.html

TS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtaxhguhlg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtijyuiirc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtwkcqnxvc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigufen.top/gtacvaqfxw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtjtcqwaqv.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtzctkqsub.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtmoiasgif.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtowseywqq.html

JS:   e.message;  e.stack
来源：http://hz.c1oappe.top/gttqsuxzbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtvofaqtxk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtgkcvzgqv.html

Go:   err.Error()
来源：http://hz.pengpengdd.cyou/gtngryrpxb.html

Ruby: e.message;  e.backtrace
来源：http://hz.cashguo.top/gtxnqtcxec.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtwnxnidat.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtknvysuqn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtrowydlso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtaypsiinh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtlhgofwjj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gttisvpzpz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtuuzxmmrj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtkdhzxdvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtdhivillh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtpkouighw.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtabjsctux.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gthebmdlnp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtthnyspfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtfhcyzyli.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtucxahbpp.html


<!-- 参考信息 -->