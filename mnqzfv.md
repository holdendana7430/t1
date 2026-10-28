代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtneylarms.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtadjlvdql.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtiuinbyvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtibbfnzwm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenzaomai.com/gtkrnkqhzp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtldwhmfkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtscqptqli.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtkdaskxxf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtlufhdzxn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtmlsrkjcg.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtoekvwnvh.html

TS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gttnheammx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gttssdysvd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtszcknfkl.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtfxmjpumv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtmyvqdbrr.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtnhurflrg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtbisqzbhh.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtbqykkooe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtsrprsehq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtmvurpdow.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtvoiwkpvm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtjqrflqau.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtkzwiuddl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtibfrzjrq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hammf.cn/gtshbnzejq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtqnhjymsh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtlveqzdpg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtytxcfbai.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtpnchkyyb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gtgggmoupa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gteejzkpwz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtwygnlfzc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gttbekeizg.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gttslbevii.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtqbufcupe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtvaxzurxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtzbfwdova.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gteuruacit.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtkiiqsrxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gthuoytncw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtaljagrwy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtifrsnehf.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtwytgqgkr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.smart0.xyz/gtbubowzbl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtbvceglnq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtfbyiibzz.html

TS:   // 同上
来源：http://hz.zhoulong.xyz/gtduvaiuhw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtufrlolfe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtvdsuckan.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtbiwblaqg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gterezzvpw.html

================================================================================
来源：http://hz.dianchejie.cn/gtrqqsnsfq.html

G. 面向对象
来源：http://hz.jqgufenzy.top/gtaksuiycj.html

================================================================================
来源：http://hz.mhx1999.top/gtzuhjatky.html

[G01] 定义类
来源：http://hz.quarkkingdee.top/gtugpfypii.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtvwhmsetz.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtenaqjaqp.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtrxvtcnvf.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gtbybyrxtk.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtldorgdqp.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtufbngnib.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtanjgibdi.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtoyclannz.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtdibkqdjv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gthqzwdinq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtrbtfsjys.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gthvphhxib.html

TS:   constructor(public name: string) {}
来源：http://hz.316326.xyz/gtrjmfkzfo.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtwzmuoxjx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtdhkghftz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtvqshoijr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtvhrbeaqi.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtbfqqkhms.html

Py:   self.name = "x"
来源：http://hz.tianlin.xyz/gtjnoaliwn.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtpymsllhz.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtmillumlh.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gthxosegkq.html

Java: private String name;
来源：http://hz.fzhhl.top/gtjsdjitvy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtoojujixm.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtqtvxzvey.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtmperhygt.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtdbroulqa.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtffpwlepp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtslayftal.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtqqglwxzz.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtbfhrdwcb.html

Java: String greet() { return name; }
来源：http://hz.nanxuanxn.top/gtdllylbhv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtzhivafqe.html

Ruby: def greet; @name; end
来源：http://hz.redwolf501.top/gthkfjhzuo.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtklhezhqt.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtgdwyrehg.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtfdsbccbu.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtardjflgp.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtgvwohprs.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtfccehihy.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtxallsjyx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtjeojthuo.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gtqfhgkist.html

C#:   class Admin : User {}
来源：http://hz.hammf.cn/gtchkjmqwu.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtbcacenil.html

Py:   def greet(self): return "admin"
来源：http://hz.vqdsnc.cn/gtwwxxgklb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtmdhxkswl.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtuvafdppl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtptdseyfr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtbrnzgovc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtcdhqekor.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtkdfolldq.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtzcqsvbmd.html

[G07] 调用父类方法
来源：http://hz.tianlin.xyz/gtgtervsjx.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gtprtssfqa.html

PHP:  parent::greet();
来源：http://hz.nanxuanxn.top/gtnmhctbga.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtmqljhbik.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtwfbslukz.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtqxzwwcbb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtiuztujeu.html

Ruby: super
来源：http://hz.ehwqpu.com/gtworrbzzf.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtcjmoziry.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtwmggfswh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtjqayltkh.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtuiddbpgh.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gthqhcqrep.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtugtoioji.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gtlqoelysl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtbnuacbtn.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtzitvvsne.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtaqzkrupo.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtscwchldr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtrvjotljd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gttzontfob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtzcqoseal.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtqcobodbx.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtehsppiih.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.vqdsnc.cn/gtnptptynl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtkyqryqeo.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtutktevzz.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gttpjtpsir.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtprpujzis.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtnpvfsmvh.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gthirhutfq.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtvxytkapu.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtfpibcoxs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtrponatdf.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtvaqhxbth.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gthudughbd.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtcwsekjgl.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtibzlzmhx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gthxmsechf.html

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtibrdxfga.html

TS:   get name(): string { return this._name; }
来源：http://hz.guannengcc.top/gtnsdhcgmt.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtclgykqnf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtygllliee.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtmpahcqqs.html

C#:   public string Name { get; set; }
来源：http://hz.jinghuilouyu.cn/gtpmjamvjo.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtwiltfwja.html

Py:   def __str__(self): return self.name
来源：http://hz.daria6918.cn/gtsxyikvnl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtkuehflqj.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gthcmwyhnk.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtjhppljkz.html

Java: @Override public String toString() { return name; }
来源：http://hz.9152youxi.cn/gtsflorkfa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gtijcvwcrx.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtrddexaze.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtmpxsldul.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtclspdebx.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gttwwzfvhv.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtyivwrhlv.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtbnsvfgtw.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtrpvbstle.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtpviyxhrr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.52xcode.cn/gtdgvmbnym.html

Ruby: u.is_a?(User)
来源：http://hz.yangfankeji.com/gtgysotord.html

C#:   u is User
来源：http://hz.vqdsnc.cn/gtsuozwbaw.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtaqngpcwq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtlrigtdwu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yueranfly.top/gtvpxaouwk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtslnwsivc.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtgvpzpxnl.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtajnbrhgw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtqwsycvew.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtnxzksjte.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtidogepss.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtyxkxboga.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.mhx1999.top/gtadxicxty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gtsuipyqxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtlyypnmcv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtydweeezn.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gtwbwqcccj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtsmxoiqzz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtvgyeretm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtxvyvenjs.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtddwpwsvb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtzmmrpfir.html

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtdfdzxqkf.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtdyrwzzll.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtaolyovuy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtuktnvjgd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtesoutlov.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtiqoukxmt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gthmpbxttp.html

================================================================================
来源：http://hz.zhixingplan.top/gtfgqvmuzw.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gthpsnclkz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtoxwaeaou.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtqiwnmknb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gteezhlkxq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtdscweheu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gteczcyvmb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtklxlqfad.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gtrxldacuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtggtrfhcy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtjkvzqlxu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtowuehsan.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtpoqdludh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtntoktbjy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtxfsxyvym.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtderbrekt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtkqpecqjt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gttdlqjrmj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtwnfmmebl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtaqhibady.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenzaomai.com/gtzaoeyxwf.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtxljcggqx.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtgzucvqvu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hammf.cn/gtnnpanlva.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtvrfhrlxe.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtzhzvgljf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gttywwskex.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtqjqvldlk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtkzvimnpk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtidbqwage.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtbaxioycg.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtnoofwanl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gzhubu.top/gtwvoivmqd.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtfcvwnxjb.html

TS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtumxwwzhb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtazmjaovw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shuidangran.top/gtiwlunnxl.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtxvaoboau.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtlzigtaer.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtjijpvxdp.html

Py:   except ValueError as e:
来源：http://hz.jiagoushi.top/gtvxijhbea.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtejgejjho.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtqzhimdrq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtxfzhqgiu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtiecptjll.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtqvlfmqsr.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtxsmaqxtf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gthgghqhos.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtapzluvro.html

Py:   value = d.get("k") or default
来源：http://hz.ivvv.top/gtqridpwbg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydjk.org.cn/gtbhfaxrny.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtqsddtgaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtbvpcenul.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtwrtwvflx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtjqswkbbs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtalriksga.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtulaclqcd.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtivyluibl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtylxmabjo.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtthuvjwen.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gthxuhqzvd.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtchusoacq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuetiantiany.cn/gtwjmlctyf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gtyxkbjtht.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtolzvktqo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtguxrkmbq.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtcohnmkyn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtcrmgvdkf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtikvthbvc.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtmvpazoho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtuaqswmgp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtstnomeej.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtvicvxwel.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtaospqthq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gtvhpfcnuy.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtmfffgddz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtvrgkdfni.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtlsjypwls.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtcwmgvelv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtguqtnlve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtresqkpdc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtuzyqyjlo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangkeji.top/gtnxtgryzv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtuyvjxavs.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtkllrtpjj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtwrjegvid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtsqkfmrcz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtoxhnwkli.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtdnyzdjuv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtotkfepuu.html

Go:   defer f.Close()
来源：http://hz.feifeiyinyue.top/gteijgmgar.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtnbfjdpzu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtpjcodhud.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgwdkcgrn.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtxuzuxqct.html

================================================================================
来源：http://hz.zdqjudy.top/gtvrvkdtfo.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gtoxgafxva.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtgjczedww.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtxcudqzfn.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtmahlrunv.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtvrviykoh.html


<!-- 参考信息 -->