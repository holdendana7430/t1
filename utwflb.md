代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtnajehqqw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtjlfmgziz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtnxyovhrg.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtgpkznzzl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gzhubu.top/gtvlrppwhw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtdlpzrlvk.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtecxzsfhd.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtdhxngoxd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtofinsfph.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtgiqlhlkp.html

Ruby: Dir.children("dir")
来源：http://hz.jyoumei.cn/gtrarswbay.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtklegnboc.html

[F09] 获取文件大小
来源：http://hz.daria6918.cn/gttfqwffbo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xinyue.icu/gtkoxgmwyk.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gthdvfojlt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtjgiouhyb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtevclkocj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtpohhviov.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtvjxbdnzb.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gthptwpgog.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.andypj.xyz/gtqwhjgenj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtbvpsbspw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtvflwvqta.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtdgkbfing.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtybfwiynq.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtphzzvboz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gtbfwtdvhk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gtcwqxhkfc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtegvejqiu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gtxwkoztov.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtghpvnerl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtruttgvsp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtoqfcnvrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtozmuhcms.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtkengqkrj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtdvonidkk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtmfkjnzxq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtfjrrbvyr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtlvdzpldg.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtwyyojzvc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gthnalznwv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daxiang520.top/gtzkuowxqr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtvlokpmrc.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtiririhpj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtvslfnhbg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtwwjcfvpn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zycfv.cn/gttwgljwus.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtlzmizwnx.html

================================================================================
来源：http://hz.yuanzhike.top/gtvgfpkzsy.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtsgagyezx.html

================================================================================
来源：http://hz.nwbrower.top/gtphrxytbh.html

[G01] 定义类
来源：http://hz.mhx1999.top/gthszrhrap.html

Py:   class User: pass
来源：http://hz.xinyue.icu/gtizknsdqc.html

PHP:  class User {}
来源：http://hz.kuanghao11.cn/gtezqpcahp.html

JS:   class User {}
来源：http://hz.shuidangran.top/gteoypnajo.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigufen.top/gttkowhdqw.html

Java: class User {}
来源：http://hz.0kj1m.cn/gtzvorkkyo.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtizxwuufa.html

Ruby: class User; end
来源：http://hz.cashguo.top/gtmzcdvlse.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtxxozqahw.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtjehywqnn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtnkqwtdzr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtiihreirf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtmeemkuuq.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtcqhwjlfl.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtbcdyfigu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtaagrzcjt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtenhwyqky.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtvjtwebqo.html

[G03] 实例属性
来源：http://hz.yuxming.cn/gtvffebqiv.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtphxuowkm.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtmtnuajem.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtokmtiwad.html

TS:   name: string = "x";
来源：http://hz.vqdsnc.cn/gtkqhvhbjo.html

Java: private String name;
来源：http://hz.zycfv.cn/gtduzbbpvn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gthyykveqk.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtziikaykg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xylfe.cn/gtxzogfmlt.html

[G04] 定义方法
来源：http://hz.meibo888.top/gtprjecakq.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtysefwpgb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtnwzgkegd.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtzregmkkd.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtcofdmcgv.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtqslgjpeq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.daxiang520.top/gtzfxmeyap.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtwownjrcr.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtbnlbinzb.html

[G05] 继承
来源：http://hz.shanyushiyangtech.top/gtgckqvxqj.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtduwkpltp.html

PHP:  class Admin extends User {}
来源：http://hz.ydzc1.top/gthckwzogq.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gthsoirusn.html

TS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtwqthjhrj.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtjgkvglit.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtmzrcwtkx.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtyyhbmoyf.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtiratrgsg.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtezfdiahh.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtiygsxjru.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtkbwogysq.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtjpiiuscu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtdkwjaddb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gthiqfqleb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtcilotpew.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtglkkxkhj.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtbemotrej.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtgwgmbmwq.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gtmherexog.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtkxukryjz.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtkhrmijjv.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtzhmjveeg.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtvsksibof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtmtpuxvfq.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtnrifnmda.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtuobvuxrc.html

[G08] 静态方法与属性
来源：http://hz.yangfankeji.com/gtszgkfpuy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtmhkebqwv.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtgmsfaxmv.html

JS:   static f() {}
来源：http://hz.xingfuxueyuan.xyz/gtvunxpqaf.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtqupitxgt.html

Java: static void f() {}
来源：http://hz.guowangkeji.top/gtmurihsnq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gthrhnfchw.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtvqshjvew.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtnklpoogo.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtlkgqhlqf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtdhuyizun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtrqprrzll.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtublagvuz.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtohmflzli.html

Java: interface Shape { double area(); }
来源：http://hz.yj202588.top/gtwmvenxlo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtodsexyka.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtvuwhwdsr.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtsxfegvvy.html

[G10] 访问控制
来源：http://hz.hfpthk.cn/gtpcvdksjw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtnhizztkc.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtnkdcpenr.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtbyxwguqd.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtiywvmdyf.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtxzwlbiat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtietyabbm.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtvhrffavf.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtcoblngtu.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtwnvanssf.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtjhmympxv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtfcxleeyd.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtdghdnuar.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtocdqevdm.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtcbqwoxvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtiebeziht.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtqaswhksx.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtonzlqdsq.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtxzbydckp.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtkywvvbxm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtlxkhqhti.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtyiacatsu.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtdeptedfc.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtfegtwffo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daria6918.cn/gtgwrfmahp.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtuufjzxrn.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtummfzbmw.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gtxtwkoaog.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtwsknumjh.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtjtctweky.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtmlabhsuv.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtosvwktsd.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtevnwikcw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtcjckgfvx.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtvhtsrxod.html

C#:   u is User
来源：http://hz.zhaomingkeji.xyz/gtbrowytem.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtctefzfnz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtrdkvxffu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtctlsektw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.feifeiyinyue.top/gttftqdqev.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gttqiihrhe.html

Java: record User(String name, int age) {}
来源：http://hz.gaohongyu789.top/gtfbhabvyn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtjefwydpa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gthjnfqbuq.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtblecdxdm.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtfcwulxdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtakmzofow.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtgfhorfpd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtkpawnpak.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtlqavyovp.html

Java: enum Color { RED, GREEN }
来源：http://hz.pycfn.com/gtxemjppqq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtmwfymwnv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtaosalgbe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtsabiggoc.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtcgsaqski.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtyicxlysj.html

PHP:  get_object_vars($obj);
来源：http://hz.daria6918.cn/gttjnrosyz.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtmktefiwf.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gttgculxzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtpciqkxrs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtpnofcakb.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtymmifyct.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cheryme.top/gtbgqgcyle.html

================================================================================
来源：http://hz.yongpay.top/gtujigyyge.html

H. 异常与错误处理
来源：http://hz.meibo888.top/gtbwinlbpj.html

================================================================================
来源：http://hz.xziqi.cn/gtvijfmxtf.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtlizdswec.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangtech.top/gttafgumym.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtyhuygxjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtmijhwotp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guannengcc.top/gtdlejkquz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shzxlz.cn/gtpbjanhzj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtpcaaghzg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtyslhqeaq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gthkpbobly.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtiiyrigud.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtfkmdpwoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gthoivwoqy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtmheeznql.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtojauujmq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtutaoovln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtvwiattra.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtbwtnsjmq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtqfiknril.html

[H03] 主动抛出异常
来源：http://hz.jqgufenzy.top/gtikpmoruu.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtfuuanzlc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtcgtlihrv.html

JS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtcxwqtcoe.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtdbyntgmz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtvewtmpno.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtgausrpts.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtkahebvrj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtvgelgmdi.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtdatpyvxj.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtjavxmnvz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtbbafuhys.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtkmgloduy.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtvcoknwbl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gthpbkvkzv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtlpxiwkwz.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtmccvtobh.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtoowzotwq.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtibrgmgel.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtnvpahffc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtvkfjhcfw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtnnkwrmcc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtvhhjbhld.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fzhhl.top/gtndsapthv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtpmpkhoyg.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtwareafrr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtusaabgqf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtejxqliyp.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtvykkuxai.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtzbvuwfxc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtygkigbii.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gthfwxgwet.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtixpugiyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.feifeiyinyue.top/gtkdhixoxd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtphwbepgn.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtbtnmfnwx.html

[H07] 断言
来源：http://hz.yj20258.top/gtpeatqodp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangtech.top/gtxhpodrlf.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtdyijoufy.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gttcmmfzcz.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtevupsmyb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtjfgmohfq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtkryglbpq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtpxgrecdf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtflcklugu.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gteqzrliep.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtqdaushja.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtvmssfscp.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gthaninlhq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daria6918.cn/gtkphcatmb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtshdxdkfb.html

Go:   err.Error()
来源：http://hz.jianghu66.top/gtazmbjctb.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtwqqsckjh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtwxglvkzy.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtpoeeyedx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gttnghhpvi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gttgqutctv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtfkxglmmp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtuygtpkdx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtgylgntwy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtlunnhlbd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtyaqwvxyv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtdlzqvsfc.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtpehyjcav.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtgijcprer.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtajdsebco.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtkbqkcswi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtpqwbolfy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtpdqfpgeb.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtcanetuia.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtixsoapjo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhiwuduotai.top/gtgchvridv.html

================================================================================
来源：http://hz.yvedp.cn/gtqvpamdqg.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtuthwklod.html

================================================================================
来源：http://hz.yongpay.top/gtsjjuflip.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtnywzfnbz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtuupqmffk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtznfjengz.html

JS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtztdyohcp.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtyjijqrbm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtvrptlrfg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtifckkgmt.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gteffxfozf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangkeji.top/gtcxhfymzx.html


<!-- 参考信息 -->