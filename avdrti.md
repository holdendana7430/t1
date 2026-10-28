代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtgpbmdzjs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gthixopggt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtjggoasas.html

[F08] 遍历目录
来源：http://hz.jinyuanbaomall.cn/gtqqrnsdqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gttsnjwnhy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aibaodan.cn/gtzwrgzuis.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtgnqqnsry.html

TS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gthcxejcbx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtgadggcfr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtooeljwsj.html

Ruby: Dir.children("dir")
来源：http://hz.svipenyu.cn/gtmviwvhda.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtdrggkmut.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtgfknttai.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtpnlctdde.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtpbafxuaq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtpdpqiiec.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtxynqvfbi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtogucmdig.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gtrwrgyaqd.html

Ruby: File.size("a.txt")
来源：http://hz.aizwys.cn/gtewatlnqf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtveshtkka.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gtbmjwjevj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtdsnbkcxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtlsutyoib.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtvkkvjnqu.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtuplmnide.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtbzvbzgsn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtvgcbkhny.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gttzxpgyvq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gthpkqjzfr.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtafyfxmjk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtntioisff.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtookqrfsx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtltekfbtj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gteurfmjxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnxiangtu.top/gtjruqmcbk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gthxstebit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtqlfddyka.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtzcahqkag.html

[F12] CSV 读写
来源：http://hz.jlsjyb.cn/gtdfwqmvoj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtxmnxvqta.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydzc1.top/gtxkjblhio.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtkbsdfzmt.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtkzhvkfvw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtzjjquyxq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtmlvfmsdb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtnkpyukvt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daria6918.cn/gtygkkcxxy.html

================================================================================
来源：http://hz.svipenyu.cn/gtybarnjip.html

G. 面向对象
来源：http://hz.xylfe.cn/gtrqgfdfkw.html

================================================================================
来源：http://hz.52xcode.cn/gtoeqqjwzy.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gtfmojbbqz.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtumcloscm.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gtkhfsbivp.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gthxsvsttg.html

TS:   class User { name: string = ""; }
来源：http://hz.fzhhl.top/gtxequaxui.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtijwpfmnx.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtfbalcqtn.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtdwvgyuux.html

C#:   class User {}
来源：http://hz.316326.xyz/gtunefmggw.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtmoxzbxla.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtqguxsbgh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtznqxfqyn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtrlssnjnd.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtcoahwipm.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtfuzyjogz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtopwtgqfl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ppjwa.cn/gtpbyvqxrk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yongpay.top/gthiogxwom.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtvxhsaczx.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtowztutor.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtqxjccygu.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtvowrkyjc.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtgudmnnis.html

Java: private String name;
来源：http://hz.gaohongyu789.top/gthpinliud.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtbfycxqcw.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtznaacfag.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtiqlbaezh.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtnfbdpyfh.html

Py:   def greet(self): return self.name
来源：http://hz.jqgfzy.top/gtyqeskjmi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtpoetllvi.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtgqjriugv.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtqfsesupn.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gteowtmbcm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtiaxeybcj.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtcirzcold.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gtllqjzeug.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtaxbvqyff.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtagmloexx.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtnswtqbyl.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtzreqrrsj.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtmtgknole.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtrijhhckj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtqdrlbzhg.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtmmnfthuh.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtfmqzvtjl.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtfjmqbebe.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtyvdhvhye.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtdckxtjtg.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtrpihgikd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtpxqvfpta.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtfkzweclm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtvxwfgrfs.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtiyhndrln.html

C#:   public override string Greet() => "admin";
来源：http://hz.zycfv.cn/gtccvudcvh.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtmwcrythn.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtefapwvgs.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtvhgluxgj.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtndrsywgt.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtwlhsbjzs.html

Java: super.greet();
来源：http://hz.fengsongda.top/gthiaoknis.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtgkhdpbms.html

Ruby: super
来源：http://hz.316326.xyz/gtblkatwlu.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtgujdxdsy.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtoqtoyamh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtcvodkqlw.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtqlaqxcyp.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtmdkjwukf.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtckngegua.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtyqfkuiwr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtpmqagffe.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtaoyualnu.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtrmgfrruz.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtqmjwgdqu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtsmvkzzpz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtjkbswbks.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtcqugpvoh.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtshixvgut.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gttzxwjgrr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xinyue.icu/gtizimszky.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgfzy.top/gtwmtuykdn.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtzrftvady.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtnymqustk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gtsaqogehj.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtomywtjay.html

JS:   #private 字段；其余公开
来源：http://hz.quarkkingdee.top/gtwewzzjgr.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gtrjlnzjqx.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtqavihwrr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtwvutqfea.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtlcbkdgza.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtdomfypdm.html

[G11] getter / setter
来源：http://hz.ywan-chungtsiang.top/gteskbsqum.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtycipljvn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtzyzgphqu.html

JS:   get name() { return this._name; }
来源：http://hz.tianlin.xyz/gtckdahumk.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtfropplks.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtymodxicf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sxryk.cn/gtldxqihyg.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtkfyjoovr.html

C#:   public string Name { get; set; }
来源：http://hz.redwolf501.top/gtdpajjoue.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtprdqkjey.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gthynbkjaj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtzaisjzxl.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtjdkaljhd.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtedgfxfwk.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtgnpisjrw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtyqtpkgzz.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gthtcyobno.html

C#:   public override string ToString() => Name;
来源：http://hz.yangfankeji.com/gtpilaqrcv.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gttozenxtt.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtkqcwzvqp.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gtpcnspwau.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtuwjaguel.html

TS:   u instanceof User
来源：http://hz.chenlongwang.top/gtkrejwwuk.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtxxqaqbqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtldbfaitm.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtqdssovqf.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtkaaphuch.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtzxrqdasw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtgogcirxw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gtpcfxwokb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.bjfxy.top/gtrcckxchq.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtjwewsaeu.html

Java: record User(String name, int age) {}
来源：http://hz.nanxuanxn.top/gtheifzyez.html

Go:   type User struct { Name string; Age int }
来源：http://hz.andypj.xyz/gtgftzyvwx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtltbluciq.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtfvpchgck.html

[G15] 枚举
来源：http://hz.wangdashe.top/gtfrvkqcmq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtcrtkjjdi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtfupxmecj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhaomingkeji.xyz/gtxjqqqrxt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtxwellfmt.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtzrkqhbcx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.redwolf501.top/gthgychohw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtfahyttqu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtbylivrkh.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gtjrpmnkpm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtmnvqqbcp.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gteuezgbca.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtxkicoytr.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtfvqxwrzf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sxryk.cn/gtnxhtpeqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xziqi.cn/gtasoahxby.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtggmjnber.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtifympmeh.html

================================================================================
来源：http://hz.birdmap.top/gthhwuhdfc.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtagemqohi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtorcahvyy.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtdkbdsjoy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtdgtugesn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtidmpqshl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtkvnqupil.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yangfankeji.com/gtghdvyuhy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtugustskm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtdluuwbpo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtsyqthzdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtvwaruvfd.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gttjlfudoz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtoosnrmve.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtmmdkocdf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtyxlfhfal.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtcdvkqxrs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtlzcbcoxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jiagoushi.top/gtzeixtxgf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gtrlnynlxw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtaljohfta.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtltsxwrud.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtcmomdknr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtulxqtgmq.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtrnwrrvuc.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtntstcjda.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtngronype.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtoistqxhz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtjkjsjpbx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtenozswij.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtoudwgmlj.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtisbmaoqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtmyulhhbg.html

JS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtaaeyuqce.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtzcbjyaza.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gttmjbnubz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gtniwqhtrk.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtudeearsx.html

C#:   class MyException : Exception {}
来源：http://hz.yuanzhike.top/gtmrcufrrc.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtkzuncfwh.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtmltffrne.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtnsosudui.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtcdulskpn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gteitwaprg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtaeoohxvj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtyabijwol.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtjdiqytkn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gtbmlhvfuw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aizwys.cn/gtzevefxuo.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gteqyekvnk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gtqdybyqvz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtrlbhvxgu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtwlgozrum.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtpnywnfse.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtumakdarz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydjk.org.cn/gtwffvjrhg.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gtrlozddaw.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtgzbiyrrk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinyuanbaomall.cn/gtgkykyvbc.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtwreesmpu.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtrdxkyleq.html

TS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtcaynstzt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtztuebgca.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gtckrtktcu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xingfuxueyuan.xyz/gtevwbyyvt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtxbvltdgf.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtegrttqcr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.quarkkingdee.top/gtmktlucwt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtvxssmmwe.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gttuxflkip.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtkxczqhah.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtrxosuori.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtdnhcqfpc.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtftrfgozy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtyjpmcdml.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtpkifplxf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhijiandao.cn/gtsxxwchqa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtwmasaobx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhijiandao.cn/gtvbwtwdbh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtxygmsroe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gteghvxozx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtkefytjer.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtfcepgroq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtrmzybcjw.html

[H10] 资源自动释放
来源：http://hz.316326.xyz/gtvsiiosdr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtnsaijgbx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtqtjsaihf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtubycnvst.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtnfmdttfe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtjklydujc.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtbjnscqsy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtmjocuhdo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.c1oappe.top/gtgvhzawmr.html

================================================================================
来源：http://hz.jinqigufen.top/gtqwkyldjr.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtrvldvhgn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtehjnyuoj.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtjioqsijh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtogyjlzgh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtysazysph.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtwiahnjsz.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtaewntlgu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtbtmwbuth.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gttjyzvyzj.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtbtnvwqim.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gtxccxwyvm.html


<!-- 参考信息 -->