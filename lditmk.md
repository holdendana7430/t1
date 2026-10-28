代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtnogciaby.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtnltxwsbd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gthsvqragt.html

Ruby: File.size("a.txt")
来源：http://hz.gotoacloud.top/gtldghbzxm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtsyykubig.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xinyue.icu/gtkzdbobco.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtosavwoin.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtznbsomcw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtqjupbxms.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtxyqozzjk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gthzskctwt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtjamnwtfx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtkvlhkdin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gtjdvhabsh.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtdpemzdsj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtjiyrkhvo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtjxlmsayi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtfioordbv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtnhrpwheo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtuqesxfqq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gtqgavhyof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtrxfxzarx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtrrbfazbr.html

[F12] CSV 读写
来源：http://hz.yvedp.cn/gthiyoltfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtickvaovf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gtjglltgmz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtomettmqp.html

TS:   // 同上
来源：http://hz.ydzc1.top/gtuykpgfvo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtdpvnemud.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtdicqttck.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtpbjnrpxr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtemzlchfw.html

================================================================================
来源：http://hz.sweek.top/gtsbumqday.html

G. 面向对象
来源：http://hz.bjfxy.top/gtjgemhlof.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdwqtskfv.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtyiquudgq.html

Py:   class User: pass
来源：http://hz.nanxuanxn.top/gtkyjaiszq.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtyazblnew.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtjvaaduel.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtkbfmzgke.html

Java: class User {}
来源：http://hz.xylfe.cn/gtskwdrhnx.html

Go:   type User struct { Name string }
来源：http://hz.cqqwz.cn/gtdxflovcc.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtdqmflckt.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtvgpmvjdf.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gtnoticrgl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtbuscagdb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtathlphrg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtgjjifdse.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtlnkrsfsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gtvoopznqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtpehyrymw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtwyawoqwd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtgndykljp.html

[G03] 实例属性
来源：http://hz.yj202588.top/gtyrferzau.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtwloagcut.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtuftnaqxz.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtouuftjes.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gtbjcsvqtf.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtxrszsbyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangshuangyany.cn/gtkbvpexrt.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtyormqmiu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtyfmgjqlv.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtobiwsyqo.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtwrgmzrnh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtoycsfnzj.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gttrghpdwn.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtzhahkxiz.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtclxusoan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gthsdjrvhg.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtsyavwwfp.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtvntbvswh.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtdgpzzayf.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gttnzojqbu.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtogimtgjg.html

JS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtkimhfuev.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtbanbpoxg.html

Java: class Admin extends User {}
来源：http://hz.gotoacloud.top/gtacrmxyyr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gtrltkqfan.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtrvucpiob.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtzkuhwdys.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtvsguocbr.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtlzqqrccf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtotjangsu.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtukbwqeoe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtoulwgxpy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yongpay.top/gtyqfznkvc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtpvafycmq.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtvqfrsswj.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtnnvradrn.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtpjxiycox.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtevjyxakr.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtebjadcco.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtoygpumtl.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtmhuevpdt.html

Java: super.greet();
来源：http://hz.ivvv.top/gtatztrhfv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtfskzviri.html

Ruby: super
来源：http://hz.birdmap.top/gtxwqjlfna.html

C#:   base.Greet();
来源：http://hz.jinyuanbaomall.cn/gtowtdnyts.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtomdwuehy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gturwkhwqb.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtkdcpnkwz.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtjlqdxwwa.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtblgjonnd.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtiqnkqhdo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtbpsfcwxo.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtzwnbzvcb.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtbgxpltvh.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gttigxlimj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtukevkfvk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gthpxuguxe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtvkyhyhdn.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtdfyxyvpd.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtmekaozqn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtegfjoyfi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtkzklirvf.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtokbppoxi.html

[G10] 访问控制
来源：http://hz.chenjidiqi.icu/gtwvzaekey.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtkedhjbiu.html

PHP:  public / protected / private
来源：http://hz.jinqigufen.top/gtqwhqtxta.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtgqvpjjpf.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtpcavimvl.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtsfeintze.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtybdonphu.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtpotojvjn.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtexzcfmhb.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtligihhph.html

Py:   @property 与 @x.setter
来源：http://hz.wangshuangyany.cn/gtkzxkimfy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtxhzzzpbb.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtrstgartv.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtyvxgvqro.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtznylpgqe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtfeswkdmz.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gtswensljh.html

C#:   public string Name { get; set; }
来源：http://hz.bjfxy.top/gtpwheccnp.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtgtjgvscy.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtsfexbcfe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtlolklpdj.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtmnlmrupm.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtqfozvwog.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtwdcsitth.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtvkfltwzo.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtlrgntbob.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gtgydmetap.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtmgcmzqdk.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtmbczfsln.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtnpbulktr.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtlbhzyqdo.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtrsqshfuq.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gttrsoardx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnxiangtu.top/gtrdvimjgk.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtaaylnkla.html

C#:   u is User
来源：http://hz.jinqigufen.top/gtxmxvmiyb.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtswiudnkb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gtnbkdfhdj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258.top/gtbcxpnhuh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtlvnoqayj.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gthrsmdkqn.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gtbpetkykj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtahighlit.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtsjycljvl.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gtoiherkvw.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtyfydxksp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtdoruygpl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangdashe.top/gtleijxhdg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sweek.top/gthwmgazup.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtfbkmafue.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gtsvyunfqa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.316326.xyz/gtgmynefjy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtmlnhkxev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtscgansec.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtelkewgea.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cashguo.top/gtnsmwrymf.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gthwztdebn.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtefpakrrr.html

TS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtrllndvxl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.9152youxi.cn/gtkckqxvwo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtzpevlpld.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gtmqhlrimd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtcdmkojvv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtlwnruwqf.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtakotxlbo.html

================================================================================
来源：http://hz.hnqzz.top/gtkundvabu.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtinjwejhy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gttraaewdr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtlhklunlj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtdnrggqws.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtaridnydy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtdxrfilsu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gteqxmlzpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gthbhscrzr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtnlvofvhu.html

[H02] finally / ensure 收尾
来源：http://hz.sysykeji.top/gtqehbcqfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenlongwang.top/gtnatdyifu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtzutkfdcr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtbufehvvd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtiscnqzgk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtrfumcsmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pycfn.com/gtbyzhjhjm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtwxsqgxua.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtwdvyajho.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtvogeweet.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtowbafqrp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtkcsggpjj.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gteppxdlyz.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtovehqbap.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtylbytdyb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtdrumupbs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtkwdqctkb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtxpsbsrxz.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtmutlzvue.html

Py:   class MyError(Exception): pass
来源：http://hz.gaohongyu789.top/gtmtndczhq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtejmarock.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtonqlbmxx.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtmyxgvmnb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtffjavqia.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtvdszcrsp.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtzkrfeutc.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtrhlpigya.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtzjhelbab.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gteljvuxyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtvnqgbpag.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtbxtvgytg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtbjjtdywr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtlvdzshlj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtcxoaxnka.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtujzczylm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtbsrshgwd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtykomgaix.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtjylwjwal.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtftkwvweb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtqdlkvqdd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtewxsuxct.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtqljxgadw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtmhovbuim.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gtlfymuzkp.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gtiwulzyhi.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtgkpxumdl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtsadonfgq.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtravmnvjs.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtpfxfzifb.html

TS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtytdvdugg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtnizoqhlz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jianghu66.top/gtafiqzdsk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtaqahtusq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtbezifnct.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gtpunweyfd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtaffhvikq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtkpejgorj.html

JS:   e.message;  e.stack
来源：http://hz.yvedp.cn/gtgaxppzyk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtwgfcarsv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtlwwuexgf.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtroonsqyr.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtffrtzfng.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtsnahysww.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtzofmkmel.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtbgdkkyca.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtpqgmuchk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gthqbyutoh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtjadybmsk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtgxgfbkpe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtvpambfbt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtbwcelkxy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtcinljywd.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtexcmfwyl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gtlvqzeotq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtsccqzdcr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtxtlrhjnn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtabdwmfyt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtknccdphx.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtlsiskkel.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtwxlryiso.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtppaycdbu.html

================================================================================
来源：http://hz.guowangkeji.top/gtvkgzlygn.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtypdnvhkg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtskqnvwqq.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtahbpsakt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtqwktmwoz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtrkpurvvj.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtkawxjvlq.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtyykqsoar.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigufen.top/gtuwcrgfsk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gtzgvbxwsc.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtghxzbqil.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.smart0.xyz/gtvfnfqqmp.html

[I02] 提取所有匹配
来源：http://hz.andypj.xyz/gtavwbxdhn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtfvsvdhvd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtxrxnhyms.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangkeji.top/gtbpnofmnz.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtpbwukjng.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtrzrytahl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtkllhrzem.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtwawaetbv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gttjgjmzvy.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtitiwzhhi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtfoslmeox.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gttrkelbet.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtuovdxnyn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gteuflpugy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtivqmnuod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtrvyvcphm.html


<!-- 参考信息 -->