代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gttrvsbpou.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtnkmoceon.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hfpthk.cn/gtfgkvxnzy.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtwutctukk.html

C#:   File.Exists("a.txt")
来源：http://hz.ydjk.org.cn/gtzpddjatb.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtlreyijqt.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtyltfeajn.html

PHP:  unlink("a.txt");
来源：http://hz.havefunace.top/gtfkqbwtsu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtpbnrzzrf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gttlzduztf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtyxekpudb.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtdjxetveh.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtddrpajtr.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtomnssegx.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtowxbfuto.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtbwrcuubc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhijiandao.cn/gtfzrvybgt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtkpyftpsz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtkumbtbjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhengqikj.top/gtxrpcvszv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj202588.top/gtcxpyfpzy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtgebwzpkf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtagsbmbte.html

[F08] 遍历目录
来源：http://hz.shuidangran.top/gtbihipczy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtptebkfxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gticxqrbvk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gthvaxkpnv.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtzvaknpug.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtaaehhnan.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ppjwa.cn/gtcmkmqfph.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtjorgcwbq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtwvjkxmcw.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtuhauepzt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhoulong.xyz/gtfepxnsel.html

PHP:  filesize("a.txt");
来源：http://hz.316326.xyz/gtmwvcdprc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtpbhvwlxj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtxdotoyop.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtiasrsqva.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gtiezlnigw.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtzfiwhnfy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cdnleiting.top/gtoensidty.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtrwtsiazb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtdphevezv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtvzokpvhd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtemzdcshm.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtkzhuhvxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtooluonhv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtjxzhtpyp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gthiwhvptt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtkowisxhk.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtljocbnrn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtwqgcihpe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gtecqxfiwj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtrcbkjplw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtgatsuymc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.havefunace.top/gtuhphlxcn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtcciyozds.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtdloecqmt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenlongwang.top/gtogzemllz.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtrfepdgnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtthzehvft.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtgexoxxmw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtmkzqmayd.html

TS:   // 同上
来源：http://hz.ywan-chungtsiang.top/gtpmfhvsrb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gthhcpryfv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtexvwytfa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangshuangyany.cn/gtcmmxqypx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.vqdsnc.cn/gtazhimzmu.html

================================================================================
来源：http://hz.tanke756.top/gtvitndgzc.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtiwdbyxzl.html

================================================================================
来源：http://hz.jinqigfzy.top/gthujomqsg.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtxaikojmi.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtlmukmlni.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gtazoprgts.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtmnuwiidi.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtqyghjolh.html

Java: class User {}
来源：http://hz.cucudq.cn/gtyzudqssq.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gtxubplpqr.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtpapzgyos.html

C#:   class User {}
来源：http://hz.dianchejie.cn/gtfzmeqofr.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtrqiqbhmj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtlnsdodpj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pengpengdd.cyou/gthszzlsjb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yueranfly.top/gtilnkesqz.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gtczffzvrr.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtbdheecyx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtscndxfhz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtwygiiccn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtkjvbymdp.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gttytbjrob.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtmvrmmzvw.html

PHP:  public string $name = "x";
来源：http://hz.yj20258.top/gtfbcmalqt.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtgjulyuxw.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtgyjokpwf.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtwudialtl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tian-w.cn/gtdqrhrjun.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtquzuzyez.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtlhwennfy.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtawapjliw.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gtapbrmrnv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtyievpuow.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtmhzxrjmx.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtlaffqokb.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtbjnndtpe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gthzvdamxs.html

Ruby: def greet; @name; end
来源：http://hz.hysaishi.cn/gtjdqtwikl.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtlzlugzwv.html

[G05] 继承
来源：http://hz.ehwqpu.com/gthampgwfg.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtkmwzkoez.html

PHP:  class Admin extends User {}
来源：http://hz.yj202588.top/gtyknfzaju.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gttnuextwa.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gttsvisvrz.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtrbizxibk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtohjpgsek.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtweefqeir.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gtbeiezssx.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gtugwdeipf.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtwuysfpom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gthxsdchyq.html

JS:   greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtxnpzyaou.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtnislntqd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtymmdproo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtcereaooa.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtdevohhce.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtjstgcyga.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtytupgoxt.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtouwltnxr.html

PHP:  parent::greet();
来源：http://hz.chenzaomai.com/gtafnzzlec.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtfqotsnys.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtvnpcxnge.html

Java: super.greet();
来源：http://hz.snrcjt.cn/gtkinipfzs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtlcxrlbeq.html

Ruby: super
来源：http://hz.sweek.top/gtbjvnldmc.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtiuzbaajf.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtzhzksbmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtwlcrblto.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gttwiwnwsl.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtnpktqrnp.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtcpxywhsv.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtsekzsaqz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtkioqguoe.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtgwvobywg.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtfkwdxesu.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gthcsmgfgw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtzyqcpjhe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtfsyodxec.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ppjwa.cn/gtudasdcid.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtxzztoscp.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gtmikojjzz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtkdgdzvsg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtglvescpp.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtyjhbzxqq.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtgzphlqga.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtjevcziai.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtatyoiomy.html

JS:   #private 字段；其余公开
来源：http://hz.yongpay.top/gtnodyhiii.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtonjgknhr.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtikgparzp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuanzhike.top/gtsjymybmf.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtdvdddclf.html

C#:   public / protected / private / internal
来源：http://hz.zhongyouzk.top/gtwyesakrm.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtzyepflip.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtgeztfnpt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtxcsugmkk.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtbnitunje.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gthppxckvo.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtkilexaqq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtehrgtuvu.html

Ruby: attr_accessor :name
来源：http://hz.zhengqikj.top/gtujsamvvp.html

C#:   public string Name { get; set; }
来源：http://hz.ydzc1.top/gtjewcsrtc.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gthfcdbfau.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtfzvybseb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtobazqqwy.html

JS:   toString() { return this.name; }
来源：http://hz.52xcode.cn/gteuruguok.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gthztprcxl.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtxskhocnk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtbnicwcfh.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gtpsfchxtn.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gttmdexywt.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gttganghck.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtgjlxtgwc.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gthzmkdmks.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtczwxycgz.html

TS:   u instanceof User
来源：http://hz.chenlongwang.top/gtvcpsnxej.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtgoeygywq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtjxpbjhwe.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtraplbiha.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtligtumdj.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtlnatrkus.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtwdbokhnf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtrtqypsqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtthilavej.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtkzjobkrq.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtziwxzysa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtswmlwtgz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtvcgtpcgo.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtpemgwnyc.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtrueybcnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yueranfly.top/gteaivfxvd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtaktgswka.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtmvgdqwib.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtxedzkdiu.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtbcsrigzp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtkxlkfxky.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtdiunfwig.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtibwsgmob.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gtpxyvzajx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtoniytxac.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtiauwjlrx.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtkzgquado.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtnrmaywah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtkjiaecul.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtmasrldbp.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtydugjkmq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gtfcvoegpf.html

================================================================================
来源：http://hz.sweek.top/gthxcnmtgv.html

H. 异常与错误处理
来源：http://hz.ybcxt.top/gtyiphrtpy.html

================================================================================
来源：http://hz.tanke756.top/gtchaqsrtl.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtpsvehkao.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtoxetlgmg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtalynkxuz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtfyzpvstu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtmmtapkab.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtvyqfhmxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtxqwidxez.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pengpengdd.cyou/gtnianxgrh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtdeskhevr.html

[H02] finally / ensure 收尾
来源：http://hz.zhijiandao.cn/gtwyyknxdv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yvedp.cn/gtzbythznz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtbswshwqr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtmibnlhcz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtvslrnbhl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtzljcvvlm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtyaictggw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtoksjfctu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtqypphtgy.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gttggraorf.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtldhhigcf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtbwloscwu.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtkjdrbhqt.html

TS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtrszqgtuk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtjdfwzdiq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtcttynenh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtomfkbyom.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtinxujvei.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gthdtnhppu.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtcsdohtnf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gthdbaqlgj.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtrclrbets.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtlbkeawxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtslvdvcal.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtwiqoigog.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtonnfhmwa.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtfxckltvx.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtcdathtyr.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gthenxndeb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtkprbiviv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtukzndldd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtrdequwmz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtrqskhwqa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtzqmhiuzu.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtrlfqjmpz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtffmsmcaq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtuaknutex.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtqykcrgpp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtsfmtwxci.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtnajfjdaa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtlbpayicr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtrgijmvob.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtchuuzxsr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gthjuqlawt.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtapmfcskv.html

[H07] 断言
来源：http://hz.birdmap.top/gtcqdubdjs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtkomxpful.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtystsvbbg.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtzcpnspjc.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtdduvzpuo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtpymsohjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gthyccqzbb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gttskkvbzn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtjugavopt.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtaqvotbyj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtyykemmyn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtqnjiqcdq.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtipcnpraq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gttntxwshb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtvejxrjoc.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtadeusjxq.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gtahktigxa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.snrcjt.cn/gtdvticjap.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtungmkqtx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtnoklgfgy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nwbrower.top/gtiyaweloj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtqcgjhodx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtqudnmivv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtacejzobi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtcetmpatz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cdnleiting.top/gtoyipaaxi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtrxoniuig.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtvohcqcqh.html


<!-- 参考信息 -->