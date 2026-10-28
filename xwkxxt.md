代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtvaxoijbf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtxpzmhmop.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hfpthk.cn/gtaslkyfht.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtoyeqfufv.html

C#:   File.Exists("a.txt")
来源：http://hz.hfpthk.cn/gtreyqstqp.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtfkyqwbqc.html

Py:   os.remove("a.txt")
来源：http://hz.zhixingplan.top/gtkmleamjl.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtfbkxvrrs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnzokxkoo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gthwttroid.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtbaqerrfr.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtxhuiaopp.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gtsknnlmnj.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtkqcnnsxt.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gtvcmrvhpp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtaybgymav.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtfrgvwypf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtiuedssbf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtejxhndno.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtbfitrybf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtpjbrtowx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtlttzcbis.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtzaolmfpv.html

[F08] 遍历目录
来源：http://hz.zdqjudy.top/gtgkjeyzqc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtlnphhsva.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtbljhbqda.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtcngtddcw.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtgimccdcd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtbrcifttj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtlcldylye.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtsyyutduc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtvmisftwy.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtvxavlgmr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtokamizym.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtkvnleiew.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtiqljvupk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtubttgcea.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtzsawoiiu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtfwryixnz.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtqqfrhkfv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtfwvadsvo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtiauiktdx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gthrwzcjpz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtotymxbyt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtrtdcolar.html

TS:   path.extname("a.txt")
来源：http://hz.yj202588.top/gtemlglzwn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhixingplan.top/gtvscimqca.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtcjurbiew.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtgecqurle.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtzbpcomet.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtuujwfocu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtkgxhrdwy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtlhelwmoo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtaxfhvuvm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtpxncklat.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtsuvsmdtc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hysaishi.cn/gtufdatjom.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtjsxfwzdk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnxiangtu.top/gtqifwckwu.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtmujdmbav.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtctylczzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtifqedmnj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtwktmheln.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtaoqurznp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gtyxvxficq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtrkadkoga.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtpmyrtpjx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.redwolf501.top/gtjrxfilrf.html

================================================================================
来源：http://hz.xuanzx.com/gtduthmfpg.html

G. 面向对象
来源：http://hz.xziqi.cn/gtwocrqixb.html

================================================================================
来源：http://hz.cashguo.top/gtlucpesve.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gtandbdnqg.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gtxleiyxfa.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtkvsggjpv.html

JS:   class User {}
来源：http://hz.nanxuanxn.top/gtybnbsgnx.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gteamkgbbo.html

Java: class User {}
来源：http://hz.sxryk.cn/gtosyacacs.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtryzokoka.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtkebnygel.html

C#:   class User {}
来源：http://hz.yj20258888.top/gttsiwxzyb.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gttrbqshlj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtovqrashm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtpmehxcet.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtpfbresur.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtfbgvweno.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtsplpscxd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtcgrhxxxf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtvandvxif.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtagpbmaqy.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtsnvvbaaz.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtbkhnkmtu.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtwnpycpez.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtasrcvvcq.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtrotyykgu.html

Java: private String name;
来源：http://hz.yvedp.cn/gtmduzydmo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtdtgwwpzi.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtjrhiuxhp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtnigjxnjt.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtpqqvswtp.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gtwacyxwqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtdjjbrklc.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtsbdyjlwf.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gteqshcmhy.html

Java: String greet() { return name; }
来源：http://hz.bjfxy.top/gtisydmtph.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.daria6918.cn/gtryjqadzg.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtfgzwgrdk.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtfayzbtzt.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtbbvzreqg.html

Py:   class Admin(User): pass
来源：http://hz.svipenyu.cn/gtytemtcqc.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtkpbkujlv.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtvididrpt.html

TS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtwepwhmfz.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtponrmfwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gtpvnkomxt.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gtierviyju.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtpjswymrx.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtavrapaqk.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtjxscpwow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtjtiqdchj.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtbfolashe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtlzqipgkk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtsirnnedu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fzhhl.top/gtvxmidjds.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtkfrrexsr.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtqjwjparj.html

[G07] 调用父类方法
来源：http://hz.yj20258.top/gtkhbwuwra.html

Py:   super().greet()
来源：http://hz.yj20258.top/gtnkibwxun.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtsmuxtamr.html

JS:   super.greet();
来源：http://hz.aibaodan.cn/gtruovmuxv.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtowjmkktt.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtghrimlmx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtodogsoth.html

Ruby: super
来源：http://hz.hywenlv.cn/gtwhipuslx.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtclkrmiaw.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtoxqqxmmq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtttgdwnmi.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtzbdsijmz.html

JS:   static f() {}
来源：http://hz.gaohongyu789.top/gtcytpophd.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtbwzyjuaz.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gteoaudmna.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtnsfrdqnk.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtyeydmxsq.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gteecbevgp.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtllluiwlp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ybcxt.top/gtioryonyf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtccikkjmn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ppjwa.cn/gtyktqubcu.html

TS:   interface Shape { area(): number; }
来源：http://hz.hysaishi.cn/gtxvomiiwf.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtgaqakpin.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtcgkupwjs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gterzhavyp.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gthcqqdjha.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gtoixnobde.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtibyinkff.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtpbfrycas.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtultwuvsd.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtmecyuwui.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtryquzhvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtsynrxnvj.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtexptpjul.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtrprcdxkb.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtbjwtaczr.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gthhwgolpe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtxnlmaglj.html

JS:   get name() { return this._name; }
来源：http://hz.hnxiangtu.top/gtvynqvcng.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtogtwntve.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtfylpuagb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtqpgzlrzt.html

Ruby: attr_accessor :name
来源：http://hz.zhijiandao.cn/gtbpcpwosl.html

C#:   public string Name { get; set; }
来源：http://hz.mhx1999.top/gtaoozrpmg.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtbsfzmeue.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gthjkpxfph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtsqurcmvk.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtofhtmcct.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gttyucwdvj.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtnqgyqbqw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtispyvakt.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtsjzopirj.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtudpojgri.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gtbxovugbi.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtbwvmakfd.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gteppemxtz.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtktpfnork.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtigjjblgg.html

Java: u instanceof User
来源：http://hz.birdmap.top/gtqonedyzs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtghnynrai.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gttmoiowzx.html

C#:   u is User
来源：http://hz.yj202588.top/gtewhjhdek.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtgpwdnxeh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtvungpvgt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gtpwhagysw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtnnkranhv.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtqymusjku.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtwqvmlqrm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtijezygxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tianlin.xyz/gtitspaaru.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtbmqwseck.html

[G15] 枚举
来源：http://hz.ivvv.top/gtfhwundsm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtscqarwfo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtxejlqyln.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtpkuiybbp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtnqhhevqt.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtmpgwrpxe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtcmehaqje.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtfxwwygni.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtklqqidgt.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gttigaxsqp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.9152youxi.cn/gttcycrblk.html

PHP:  get_object_vars($obj);
来源：http://hz.iojbl.cn/gtjvjxjtvb.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtdttcdtpc.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtdcekakwu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtdgpmhkzn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtepruvtpz.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtorskofmq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtqlyxiuyb.html

================================================================================
来源：http://hz.zdqjudy.top/gtogoldcom.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtaqmiivyk.html

================================================================================
来源：http://hz.hywenlv.cn/gtpelyxfhc.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtsfmvrszb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtiihpdqlf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jlsjyb.cn/gtonkfkuef.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtudpnadws.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtqvduvyvd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gthuyroxva.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtxvbycylq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtvbpqmznk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fengsongda.top/gtmevobydo.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gttehhnnvy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jlsjyb.cn/gtdoqnjyau.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtjaitpzsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtzxizxoow.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtyyoxwbmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtszqziiuu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtanzoayzn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aibaodan.cn/gtoovunkey.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtispshemu.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtvycsvmlw.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtzfhmrtru.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtygbthwrz.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtsmqeytph.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtdhwgevsx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtctuvlakd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtrvefzkkp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhiwuduotai.top/gtdvypvvze.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtdwyeufle.html

[H04] 自定义异常类型
来源：http://hz.chenzaomai.com/gtcrgfpozk.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtedxoqsie.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtdbzbtzok.html

JS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gttlxmzvpn.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtcvaaerml.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtzokirokx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtajlphaty.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtzjcpnysb.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtvlqtcjyu.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtmxlkqyan.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtlovobjce.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gtogcufexk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtclhfwzvx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gttjnguemf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtmnmhtdhu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtojaipgar.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtxysmggzi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtgnrczpjg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtkykkagwk.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtejihjaqr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtleipkjrj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtusimtavf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtrzdgtttb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtcfzdrdfd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gtulmglcli.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtvaunzrkd.html

C#:   obj?.A?.B ?? default
来源：http://hz.yanxiufei.cn/gtgbdyayri.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtltchiqze.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtkdpppvao.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtqigdzdeo.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gttuofozxa.html

TS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtcbrylkpy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zdqjudy.top/gticmwvykl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtenneupzb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.kuanghao11.cn/gtvkklsxzw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtoqimylqv.html

[H08] 获取错误信息与堆栈
来源：http://hz.mhx1999.top/gtgdmmtvle.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtkzbrwkbb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.quarkkingdee.top/gtbgwwpgto.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtttjkekae.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jlsjyb.cn/gtvxffaaat.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ydjk.org.cn/gtpqzbzkgl.html

Go:   err.Error()
来源：http://hz.xingfuxueyuan.xyz/gtonqqdfpn.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gteupnworb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtzcxriuec.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtguvqtiyh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtxgdjhhye.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtcvxybhdt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtikcjjefm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtojvzlyzp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtftuzbykv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gtwlzfyzdn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtwvjputmd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtnjmlodwz.html

[H10] 资源自动释放
来源：http://hz.fengsongda.top/gtqjbiblgw.html


<!-- 参考信息 -->