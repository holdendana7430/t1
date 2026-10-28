代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuanzx.com/gtdwsctxin.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtetrtzefp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gthcztmjwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj202588.top/gtykhxrbxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtnqboangb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gteqcvmczl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dianchejie.cn/gtduixevsa.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtusvmhqcm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtcaxdvdsi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhongyouzk.top/gtqwyomwqh.html

JS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtbrwudafz.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtbpmusfij.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtuvusjrii.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtrkqxaswa.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtblvbpgdi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtdatpjxhj.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtjetbzipq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtkselormh.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtekrcycyz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtzhcwgjug.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gttrtwilei.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtmyinqigt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtgskzkduh.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtnddxicxo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtloipiplf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtlktfwzzf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtnvjkdntt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtkeuqbgup.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtrjljctvb.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gtvxefpwkh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtgotnjlnx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtngbcljey.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmfwxunlg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtrkrpepdj.html

[F11] 复制与移动文件
来源：http://hz.tian-w.cn/gtwddcqxsa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtmkmwymul.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxinkj.top/gtsjpeckrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtfgqfowhw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtfftzpohw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtiqjuaklo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gtiopjcbdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtuuakeqqn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtibfcbfcf.html

[F12] CSV 读写
来源：http://hz.sxryk.cn/gtzwqbkipg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.svipenyu.cn/gtzjixjdnp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtgnijqibt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtwnwhszdw.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtetbtrgqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtqejggbcy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtdesvqwmi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hysaishi.cn/gtnflozsgd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtwlofepvb.html

================================================================================
来源：http://hz.tianlin.xyz/gtjhlxikmc.html

G. 面向对象
来源：http://hz.havefunace.top/gtretvxrxi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtijiaxlnx.html

[G01] 定义类
来源：http://hz.zhongyouzk.top/gtzmuplpbe.html

Py:   class User: pass
来源：http://hz.jinyuanbaomall.cn/gtczxykoqz.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtargvpfur.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtxelqdzff.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtlucvzcqp.html

Java: class User {}
来源：http://hz.xylfe.cn/gtjdmxbnbh.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtpteuaaao.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtczcjfvdf.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtkkdfiefm.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtqodmsohw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtnjtxxqrz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtuoorgjdw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtuyccrttg.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtzptqyrwr.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtazyhgkce.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtjkgiunjz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gthufkgyea.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gtlarfomjy.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtpjnhbwrv.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtloirrlmb.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gtxhwugxjg.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtttwuxskb.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtygguywaa.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtudvyntfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tianlin.xyz/gtfpwnylsb.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtmysdstsj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gtjkpbymhk.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtieikjbbn.html

Py:   def greet(self): return self.name
来源：http://hz.gogol.net.cn/gtskrigdsg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtjdaofmia.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtlzypgoiz.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtzfmhtizo.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtgbusbfld.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gteoihqzwu.html

Ruby: def greet; @name; end
来源：http://hz.hfpthk.cn/gtvaztxopr.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtwszpaftm.html

[G05] 继承
来源：http://hz.guannengcc.top/gtsjsuqcip.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gthlsnkkfv.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigufen.top/gtbumioccv.html

JS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtlbbozfyn.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtlhximzff.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gtbslnkubm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtczdaqmnc.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtaawzrzbi.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtuuptzelj.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtnxonrewy.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtoyoufupb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtwydsjwce.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtvgsxbzkg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gthqdaffbk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtmosrbddp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtoeiizgzb.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtlnpiunkw.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtzuocymgi.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtuherhjrx.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtzupubcag.html

PHP:  parent::greet();
来源：http://hz.jqgfzy.top/gtvlnrzhpj.html

JS:   super.greet();
来源：http://hz.aibaodan.cn/gtbmeqxbvb.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtovjwajdt.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtkguamsal.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtqnxqcoyg.html

Ruby: super
来源：http://hz.yj20258.top/gtthtnbdfh.html

C#:   base.Greet();
来源：http://hz.meibo888.top/gtiydwacnj.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtzlwhqgeo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtjxtxvvyd.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtutcfvhqx.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtvwpcrwhq.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtmcgzxpus.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtmzhevprn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtsvandtsg.html

Ruby: def self.f; end
来源：http://hz.0kj1m.cn/gtiftnzamo.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtmvszmmzk.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtccotbiei.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtgbhyliyo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sweek.top/gtfhblzujy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtvakqrfmq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgufenzy.top/gtdogwuqrj.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtitlmpdod.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtefzbahau.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtdwafxhyf.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gtkjmzotlu.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtcstlriuu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydjk.org.cn/gtmhplzlzd.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtieebpjfn.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gtblguoecf.html

TS:   public / protected / private
来源：http://hz.redwolf501.top/gtkpvwkqfj.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtbjtphamz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtqzphaclh.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtyotnyscn.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtxgfjmkbx.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtgbmqtgtv.html

Py:   @property 与 @x.setter
来源：http://hz.wangdashe.top/gtgxaknykj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtjtelknee.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtviwsaoeh.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtlqdrcnxd.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtzezikduf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtduzxuqps.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtatocyddm.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtmfnsfdil.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtwgftbpjp.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtecvoicuj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtfjjdwowm.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtawhpwxmb.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtdnofqjvd.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gttjhwlxjs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtpsdzfluh.html

Ruby: def to_s; @name; end
来源：http://hz.chenzaomai.com/gtrgcvvarh.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtpygcniih.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtjkxwcsoi.html

Py:   isinstance(u, User)
来源：http://hz.zhoulong.xyz/gtmxrshmrf.html

PHP:  $u instanceof User
来源：http://hz.sxryk.cn/gttnbbtsxm.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gttijnvmhv.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtbokkpdly.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtzabcgikt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ehwqpu.com/gtapuxolqb.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtoxvutadn.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtccrntlva.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtagiybpnv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtqtamjiux.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.feifeiyinyue.top/gtcwmwuanm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtymvkkqva.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gttyqsdnnq.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtkaojaesd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gtcnptzlih.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtfeaoonzi.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtledhflju.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtmqqghtjj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtrscgcigl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtxdhticmu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtpqrtebrr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtjzcyelpk.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhongyouzk.top/gthlvrfvjp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtvnramaui.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gtlbzpzbti.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtcnriidiz.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtsiqglzcv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtxkkdbmqm.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtqpfcrvgj.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtqhjbixgy.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtltfqnxkm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ivvv.top/gtadymlupe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtueinmepv.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gtuibiffub.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtlgxnovtc.html

================================================================================
来源：http://hz.yj20258.top/gtnefekypn.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtuvkpeppg.html

================================================================================
来源：http://hz.c1oappe.top/gtfuqgrqpn.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtwytikwco.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtwctkswee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtejgpujtd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtwekjyzez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtwpfsibnv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtptmsetuy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtbyngcnwl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtfhcitxvz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gteooozszx.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtfmkbfoka.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gttdmfpzii.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtpvvtlges.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtltnuhtro.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtziiedowj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtchchlswy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtsajscsxo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gtgayzegfg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtnowghewd.html

[H03] 主动抛出异常
来源：http://hz.snrcjt.cn/gtakpscqwo.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtttggxznx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtkjajcwdm.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtjmknvmze.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtbvdktbnk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtgrfhihih.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtobwbjnqb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtjbnyuskp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtiknusgen.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gtiqgieqxx.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtrppmfewx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtqzhztrvw.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtaxvnonjq.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtehsaavoy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daxiang520.top/gtpwlindyr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtyllomcnh.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtiayqnfjx.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtdkyuooue.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtcwwfnemk.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gtjqeaquyo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtmxbshgaf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtpyyprjui.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtntgshynn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtjjylviqi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gttmlkazgu.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtuecffldn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gtmldcuihv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.c1oappe.top/gteemcjmaj.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtifppjtne.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtcvojlugo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtlmnslyqx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtjxtwdcdg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.birdmap.top/gtagrhfzpm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtslefjckg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtdvpiowgy.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtevjehjdt.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtuznuyrgm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtpowxcgcl.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtboplstft.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtlqqyaner.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtpvivvkjb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtffhuxoeq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtrtvyozvf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hfpthk.cn/gtuwehxxnf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gthkwtczcc.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gthgnicwko.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sufxvd.cn/gtvkiuxjxz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtjhmmzhgj.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtvthzfvgt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtpklxhdfl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtzddrybjl.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtklfcpgyq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtfegxhzpt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtuwsjfqjt.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtqmukdabk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gttcbcpywn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gtxdihncya.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtmagnaoio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cdnleiting.top/gtzmlnejcm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtrhenuzbe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtqexsxawi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gttzvpqxyg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtwxphcjvw.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtgmnfpuaf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pycfn.com/gtyqjpqtpy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtsnjcefes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtqmzztvjf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtqmlmgbib.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtycvaznxv.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtjekskbeq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gthcvfvhok.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtazattkgm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtghdtkxco.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtphvkarht.html

================================================================================
来源：http://hz.cucudq.cn/gtgxykdhck.html

[I01] 判断是否匹配
来源：http://hz.yvedp.cn/gtxnkwpzfq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.havefunace.top/gteadclauz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtvnbzettq.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtcnbvxfgs.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gthxjrffko.html


<!-- 参考信息 -->