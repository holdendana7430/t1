代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtanxyqxgh.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtkviyesvv.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtalrimaub.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtrxocnfxw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtkjeuhdmt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtlcfygftg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtztqpfcal.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtzlnbhtjz.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtztutzrxt.html

C#:   File.Delete("a.txt");
来源：http://hz.havefunace.top/gtwlxgufps.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtyylujjgd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtpckqryqm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtjgvcwanp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtqsxxrujb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtickjsgri.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtrrmvmlsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtkvdzozwn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hysaishi.cn/gtjwlxiymx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtvkjzdgqa.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gthoosuhvq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gthrhctsov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtvqpzwoog.html

JS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtnuhqsbyh.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtqruqkhpe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtuzlraumr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hongshengwenyu.top/gtwygrtfun.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gteigrcztl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gthysdipbs.html

[F09] 获取文件大小
来源：http://hz.zhengqikj.top/gtodtjvupk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtebtygmsm.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtflkgywsx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtxsbaobds.html

TS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtirodkvot.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtlyiljhkw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtlalbxbmw.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtvmzxovba.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtntnszbkz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gttikmwona.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtdnbocckp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtecjciifb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtfoqjczns.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtkquamenx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtsscldiun.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yongpay.top/gtudxivdfp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtcrmfyyya.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtwrwprjqi.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtlebxduwa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtzjhdetfq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtwksletyd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtftmbjyhy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtlnnrkzqb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtbmnxdwlv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtzqszxewc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtvxgwfymr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtyaazkjwl.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtlcfldknn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guannengcc.top/gtdpqktxki.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtsqbntptr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtnolpsonk.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtuuwvalir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtimzbbnsb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtbhspbunn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtcixrtirp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtnjrzmlts.html

================================================================================
来源：http://hz.aizwys.cn/gtbpiiwkzh.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtuxixonei.html

================================================================================
来源：http://hz.quarkkingdee.top/gtslgahvcy.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtuundtrcc.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtbmcfpkxq.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gttazlkxfv.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtqfjmuptz.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtgxknirly.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtmldftanf.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtighhgibf.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtdqecfnqe.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtarnqujoh.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtrohcmarh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ybcxt.top/gtxxippnsh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gthbabxajx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtltwdhrmm.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtclojlcio.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtzxakdoqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtaewoljpb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtgzutfcvn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtptkdkdzg.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtjjprkdbb.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtpizeoigm.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtsziewwfj.html

JS:   this.name = "x";
来源：http://hz.hfpthk.cn/gtjtmukbkq.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtdmutyxjr.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtqsjuyllb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigufen.top/gtecslnvll.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtayqhpxgu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gtheqseyoa.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gttapwujao.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtovmwvutr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtoaugmzsx.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gtnlsnfenb.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtmeltfraa.html

Java: String greet() { return name; }
来源：http://hz.smart0.xyz/gtfszwsfku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gttuapqjrr.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gtzxczpzkg.html

C#:   public string Greet() => Name;
来源：http://hz.zhijiandao.cn/gterdtyiqc.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtfgjzfjep.html

Py:   class Admin(User): pass
来源：http://hz.hfpthk.cn/gtdcgmxclv.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtqbxljquc.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gttedjbojy.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtfqjprngk.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtpajvpkpq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtsnkhgwxn.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gtwtsthdzz.html

C#:   class Admin : User {}
来源：http://hz.zhongyouzk.top/gtyitjisfe.html

[G06] 重写方法
来源：http://hz.yangfankeji.com/gtlzmnfukx.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gteydydvzi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtltxgvrhc.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtfzfabtta.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtsoghaltu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtcjvqwwgp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtkjxnqnhp.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtqalgddwr.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtnveanfcd.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtsxlanffr.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtrsperyuv.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtgogtmpat.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtsimknldb.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtlzmaqkzc.html

Java: super.greet();
来源：http://hz.nwbrower.top/gteuvkhguf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shangyingyoupin.top/gtmpkscjfo.html

Ruby: super
来源：http://hz.haohaochexian.top/gtetvzhrfp.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtwpaqqtqd.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtuouxcdmy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gtfyqftnci.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtkskexiky.html

JS:   static f() {}
来源：http://hz.daxiang520.top/gtclfxgifi.html

TS:   static f(): void {}
来源：http://hz.9152youxi.cn/gthzkbdufc.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtlyeduxms.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtbngkzplv.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtkdhlccqv.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtngbatsbd.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtzylotqma.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.mhx1999.top/gtadzrsibf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xylfe.cn/gthzuuldjn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtyrnlwhlo.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtxzzcsngu.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtrzizacvt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtmquuihhn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtoxlsopvf.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtmddtgvtb.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtpkcyynob.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtwhixhdee.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtjdtzhsjo.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtgkhfoczz.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtmdoglyjp.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtosxvzimo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinghuilouyu.cn/gtmscuqorb.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtgqrrvhhh.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtuvogghxl.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtvcuepsll.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gtvjyspwvu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtifewxevm.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtfdhwxfsn.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtjvjpkdsb.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtmttqjznq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtsxcaqdbx.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gtvgiiyctp.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtqrxnbyms.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtborkqmgk.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtqkelriuf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtiqapwofe.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtgkjtzuad.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtebrnvusd.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtcspgzimk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.52xcode.cn/gtlcpdwrqw.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtoylumsmr.html

C#:   public override string ToString() => Name;
来源：http://hz.tanke756.top/gtirochnno.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtahcxbzwn.html

Py:   isinstance(u, User)
来源：http://hz.zhongyouzk.top/gtuzgzddkj.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtepkdhmcy.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gtwwytvxip.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtrpczklos.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtfmvavnwr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtndidxrjz.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtcazxftjz.html

C#:   u is User
来源：http://hz.andypj.xyz/gtllligzst.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtdwhsqson.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtzjrvhjzq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtbuezgiym.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtxpngowcm.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtqxwgmwkx.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtbcbpkhdn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtrmpsbidc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gttdsqwbpm.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtuagfyfdi.html

[G15] 枚举
来源：http://hz.fengsongda.top/gtfweepiee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtsjoxjkwp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtlqzmzvxs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gttokicder.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtclrsyxor.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gtajhvcfyh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtpufqbspa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhixingplan.top/gtutiaalgh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtclliomqa.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtqezyzhul.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtmxwpphrh.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtpfdloztc.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtchhfogog.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtscfntyyt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtmeubsypa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtkzejyllc.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtqikjscth.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtsmeiiohh.html

================================================================================
来源：http://hz.yuxming.cn/gtspifhuns.html

H. 异常与错误处理
来源：http://hz.ivvv.top/gtpvssptks.html

================================================================================
来源：http://hz.chenzaomai.com/gtbnqcgskc.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gttafxziio.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtzoqxruyw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtjatnsimc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtotloxgfn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtytjatzkq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtzgdeaoai.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtzpxxbmjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtuiklpbcd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtpabtybfg.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtrawkrjbh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtgnmsijat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtwtdpbmcg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtmgonuspi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtpxnmgpcu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtyvwaxwxp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xziqi.cn/gtyhzntlvs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.svipenyu.cn/gtlamqmbjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtmracwkcr.html

[H03] 主动抛出异常
来源：http://hz.ydjk.org.cn/gtmppahdnb.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtpbzoodlw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtylvcqlrs.html

JS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtycsssxul.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtlptonagp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtfiuuenxr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtssdtzaju.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtbjjjgjud.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.meibo888.top/gtguyspyhl.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtmftdwdxj.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtntilgxsc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtpxeprote.html

JS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtatbzksht.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtncqgvxkj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtijhnosoh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtcjxfexrn.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtzthjnrgk.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtdvnkpwcw.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtylfaytfo.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gteiuqdpfo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtbfjfmfcu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtryutprkr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtfkskhhhz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gtwbaugyda.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtotnywqvx.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtxfbprwue.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gzhubu.top/gtwubggvup.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtfeedeiin.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtkcnquslt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtkyzycrio.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtotpjtfju.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtpjeawibo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtaalhxeto.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhoulong.xyz/gttjvdduxo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtyheldwgg.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gthdnbhtvx.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtfuniqhez.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gttmhzonnp.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtnrsrakgv.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtyrrkkiop.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtzcxzynwj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aibaodan.cn/gtpgsiyxrm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtopqekrtb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtlvvfzwrq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtxrvyjwbf.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtfxbjrnng.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtjefxexow.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtkyypjnym.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtcmuiljml.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtnbpknqqr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtkorafzue.html

Go:   err.Error()
来源：http://hz.yj20258888.top/gtrqcbktdp.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtcwqcbigc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtijjkvulz.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtnoqabgqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gtrfmahjhg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtixmkmqqb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cucudq.cn/gtfqottilj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtvsqghggx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gthxulxjiv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtwlbpqzhl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtjdlvhgzh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtcyqbckbv.html

[H10] 资源自动释放
来源：http://hz.316326.xyz/gtviaydbcc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtcchnmxah.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtjzcnndvn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtmxhwuoyh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gthksjadfq.html


<!-- 参考信息 -->