代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtfyjspjgl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtawoqzkgh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtrqawqoro.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gtwdzbqqjs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dianchejie.cn/gtlqbwjxan.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtrqdkbhev.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtbjmybits.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtzudzjntd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtnblewjcw.html

TS:   path.extname("a.txt")
来源：http://hz.fzhhl.top/gtopmwdprh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtjbuiawzm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxinkj.top/gthrnlsjzk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gthpolsxap.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtgblshutt.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtpbyrcyzb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtlgnilmmh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.9152youxi.cn/gtidfivecn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtoxkzgjxj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gttdxmufve.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.birdmap.top/gtbpturhql.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gtjckztinz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtjyeixidf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtywybwthp.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtmseywjlz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtbjfpnyjr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gtqzltjpef.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gthujeljvy.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gtlhvtcezx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhijiandao.cn/gtquehcywq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gttgvtsipn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtfinoleaz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtjlpqbgqh.html

================================================================================
来源：http://hz.fengsongda.top/gtxxeznpmp.html

G. 面向对象
来源：http://hz.wangshuangyany.cn/gttgqperjh.html

================================================================================
来源：http://hz.cdnleiting.top/gtjizcpgyi.html

[G01] 定义类
来源：http://hz.52xcode.cn/gthgotsydx.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtphpwrmop.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtmdapwohh.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtpoivquqv.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtjxdgxlss.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtsnnajiih.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtciuhxxtk.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtekbatjyt.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtmlxzgynn.html

[G02] 构造函数
来源：http://hz.yj20258.top/gtothjsqlx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gthkrvsirm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtrlfvejch.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gtvyshtlwz.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtyvpqcrvg.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtquginveo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtvmkoqvsb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtmdrjapil.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtozavapqt.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtsjnlsomp.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtrxaednam.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gttidvcijk.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtxebphvdg.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangkeji.top/gtuodqkpvh.html

Java: private String name;
来源：http://hz.havefunace.top/gtfcvnxuxg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtxrzzncjf.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtsqzczsyw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtscsvemnx.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtwawtmric.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtyckyrvoq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cashguo.top/gthdmpgcyg.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gthimvncot.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtqubbeeyj.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtgrdzskng.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gttrjxufkq.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtvqpsvory.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gteprezfgc.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtkpxdhszl.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtucqpnjpg.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtbfyhobgp.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtnpydymid.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtusygbzga.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtzuhfnxgv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtbodjayci.html

Ruby: class Admin < User; end
来源：http://hz.smart0.xyz/gtccvhrtut.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtpwlxwjjh.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gtcgvnphos.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtuipumhvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtuyejlsbk.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtcwnzwnhr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtltdtxnej.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtvdngcqsy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtnzvbdblb.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtbrwmkyiw.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtghqxsoqp.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtuqwzsbfi.html

Py:   super().greet()
来源：http://hz.xuanzx.com/gtdrvqwnws.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtvfotnokc.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtrysvhlom.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gthsrnixdn.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtahxiksic.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtxnduiono.html

Ruby: super
来源：http://hz.yj20258888.top/gteqokmeyr.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtbmbaivov.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtftmmfhca.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtygrdgiar.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtsyhwhaoh.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtczsknamn.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtkhnmjhxb.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtzozadbif.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gtqdoxhstt.html

Ruby: def self.f; end
来源：http://hz.quarkkingdee.top/gtjkpykimf.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtryxxztmo.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtdibpkexp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtijnefzvc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gtabbnixrz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtroziiymd.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj20258.top/gtnglyhiqb.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtuqvzwnxu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hongshengwenyu.top/gtralknzqq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtidoqczki.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtycaycatg.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtvzllzlwi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ehwqpu.com/gtocjpgshe.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtdkoacofg.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtexvcmsug.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtkfkluwtk.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtbulsdipz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtkxspepdy.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtfklyvimq.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtlixbsxws.html

[G11] getter / setter
来源：http://hz.ywan-chungtsiang.top/gtpglydmox.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtbhnmqmrj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtijmudjmj.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtectekdlu.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtlgxesmic.html

Java: public String getName() { return name; }
来源：http://hz.bjfxy.top/gtapaxqjja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtzcnnpejw.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtkqirvgeg.html

C#:   public string Name { get; set; }
来源：http://hz.fzhhl.top/gtvqxspcpt.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtnrisihdo.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtxnhmchvl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtefbyqply.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigufen.top/gtrfceotpv.html

TS:   toString(): string { return this.name; }
来源：http://hz.tanke756.top/gtacgaxadw.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtyaoqtvqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtksyhqprr.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtdinoichj.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtbrdrnqem.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtjrpywzwb.html

Py:   isinstance(u, User)
来源：http://hz.gogol.net.cn/gtjbogxder.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gthadxqllx.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtoqkgrtoz.html

TS:   u instanceof User
来源：http://hz.nanxinkj.top/gtyjqxkkkw.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtqzksofjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtjoevrnit.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtqksdokip.html

C#:   u is User
来源：http://hz.yonumen.top/gttsxvwbxw.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gttbmqelqu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtuxtpglff.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gttlbmgase.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtqfeodqjf.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gtimtwhwgd.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtewtbcjri.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtjswlhjpj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtfwzicqkb.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtprfozrbu.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtkweoczkc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtnhfwyhai.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtgzwflccf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtaiphwjlg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtrsgxeihe.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtqfbnxqnk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtmieredgz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtrerpskiw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtualwlhwt.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gturkflmqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtuwrpyxde.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtfnkfbaab.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtwtmpjsqg.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtxbsrltmp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtqktgaftu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtgsqloxyf.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtixboddad.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtaiizkuew.html

================================================================================
来源：http://hz.havefunace.top/gtistcblny.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtvxdjvvpq.html

================================================================================
来源：http://hz.cdnleiting.top/gtggunxsic.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtjaxadkic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxinkj.top/gtnwixtpcl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtzzzeylle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtuicfsnxd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtofnktkgy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gtagvkkspx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtdxzwcvkl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtvuejiuom.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.feifeiyinyue.top/gtrnfdjcpb.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtlgcmotyz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gthaprqtbg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtetlicbtk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtdasokkgt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtatpkumps.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtbndiuszr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtkkppwhgy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtoeyuvtlx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yonumen.top/gtrdmdrrgv.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtizvuqgyz.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtlgkvogzc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtawiljpcz.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtcvfoylat.html

TS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gthqdbupje.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtrwaloovd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgfzy.top/gtnpwmtapc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gthkebfutz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtstwilvnf.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtpsqtxbaq.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtpznymqkr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtnwfhspjz.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtogmmnsno.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtjnteaaxn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtdqyaruio.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtehzjjssh.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtkjpbmkwj.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gthnhbyrbo.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtbqtgetxk.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gtexdsdkxb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtflgtpwzv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtqfdypifo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtvthvpdge.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtrchkajwm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtdtacunhh.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtmczewsth.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtljphoqwa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgufenzy.top/gtvdyotwwn.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gthntbnhzd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtduxzkymm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gttokpehjs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtqasgjchu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gthepxfima.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xingfuxueyuan.xyz/gthnigeboy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtbrvgkalp.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtsgriweiu.html

[H07] 断言
来源：http://hz.xziqi.cn/gttcdierwx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtxnzliggg.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtmitbscrk.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gthzfumcil.html

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtpqyhdpya.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gttlgzcfyb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtuduwpdhl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gtvbaoftsi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtebjdxlle.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtvcxmrkhx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtxmuildjr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gtnfqiaikh.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtoloumdgh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtejxdkkjs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtmawnpwrr.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtolkulqsh.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtqbtftkih.html

C#:   e.Message;  e.StackTrace
来源：http://hz.redwolf501.top/gtukbisnyv.html

[H09] 带错误码的异常
来源：http://hz.hywenlv.cn/gtaftopdxi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtqmdvvyhj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gteyhlpibn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinghuilouyu.cn/gtrrrrcgsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.quarkkingdee.top/gtomcsmeqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtscyvumap.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aizwys.cn/gtptivnkyw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gtulnkaabz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gthuxyzgao.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtmoaijjhi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtdvaukbkh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtlsuhpjkc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtygsvdajz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtobcwnkmy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtexrocusk.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtwspxafdy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtcgtmouhw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtwfosrkcf.html

================================================================================
来源：http://hz.ehwqpu.com/gtvjnmbmoy.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtpkepwokz.html

================================================================================
来源：http://hz.ydzc1.top/gtbcgxruex.html

[I01] 判断是否匹配
来源：http://hz.chenjidiqi.icu/gtsrnhsevy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtsnvfzqxc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtoffydbkm.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtgwmhtvld.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtzactbphp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtzscoirfx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtmwsoatdn.html

Ruby: s.match?(/\d+/)
来源：http://hz.cheryme.top/gtcfwsxmki.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxinkj.top/gtggjzzqdu.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtobpafmqc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gtvpyfifew.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydjk.org.cn/gtxfolrsrj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtrsctfbuh.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtmafemdom.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gtbwkkmvwl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtqlcfucsp.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtdrxiqmqn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhengqikj.top/gtszskgshy.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtjoufjhee.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.meibo888.top/gtnkmssuzs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gtrxavdznm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtopuwsxcf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtmiygbejr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtulvhdfyq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnqzz.top/gtrweqmwpg.html


<!-- 参考信息 -->