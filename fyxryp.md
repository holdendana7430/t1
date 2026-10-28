代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gtikribvid.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtmyuuyafk.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtobdejspg.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtvbbqlgjv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtilymwhat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtdzeeotve.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtkzvbecuz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtvepzhwxu.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtaapktpkf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtbfqluedq.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtdbapaojn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtokdquvzb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gttdiwmqxr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtmsuwqcmq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtsuwihvvt.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtyxcqkerm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtrjapklmw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gttudpdkqp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtjdvkdons.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtcuhrbyas.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtyxckchyd.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtkxbinaqc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtqtafofwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cdnleiting.top/gtfbglkpgm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtmupmlkrw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtfbwtqtis.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtxnxplpdw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtqvwtwznn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtucrcxaze.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtpvgfulwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtwyyqqbpf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnxiangtu.top/gtbrynbvlq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gtcbyotzjy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtvrmldfml.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtjouwgsoi.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtaotteior.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtxnzofovn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtyyvmnygs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtxsnnkbhw.html

TS:   // 同上
来源：http://hz.iojbl.cn/gtmetdygcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtqfkxabdt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtsdirsgaj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gttkgyckno.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtsiapaenw.html

================================================================================
来源：http://hz.zhixingplan.top/gtoqlyqphy.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtottbmyxc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtspxtywmo.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtloqcqvkx.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtecensmic.html

PHP:  class User {}
来源：http://hz.ppjwa.cn/gtyijhrpnz.html

JS:   class User {}
来源：http://hz.xziqi.cn/gtodzofcme.html

TS:   class User { name: string = ""; }
来源：http://hz.c1oappe.top/gtxzkelxau.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtoypimawr.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtiuorllnq.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtjqfeipvs.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtcgmzvwla.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtsehphuka.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtkqrsiaoh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtauwjignh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtpssfwnjj.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gtllnzygde.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtczddbiav.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtamyiqztg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhiwuduotai.top/gturwqocgu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtggzjhfek.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gtvrlwwzvg.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtozpygyyr.html

PHP:  public string $name = "x";
来源：http://hz.smart0.xyz/gtcbjtnvib.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtoaumukbi.html

TS:   name: string = "x";
来源：http://hz.yueranfly.top/gtlivojavr.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtuatpvjgf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtmkvpdiwc.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtydwmmful.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtcuhvarmj.html

[G04] 定义方法
来源：http://hz.chenlongwang.top/gtfrwkqxou.html

Py:   def greet(self): return self.name
来源：http://hz.xuetiantiany.cn/gtioqybrls.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtipbipirj.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtqrsuvujx.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtylcvntbr.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtjzggvycc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gthzskfhbe.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtlphiidzu.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtugyqhjsq.html

[G05] 继承
来源：http://hz.hnqzz.top/gtlgoaaupz.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtcksyaigp.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtopndvezw.html

JS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtrqrnpqvy.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtaemwkbjo.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtguvrnpsj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtnemrwhok.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtvbivdzqx.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtgewskkkx.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtvyskfext.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtvkwrxnzi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtothggcpg.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtasgntirr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtqrrousjh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtumoijxrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtlgqtrqbb.html

Ruby: def greet; "admin"; end
来源：http://hz.hnqzz.top/gttjfkukbe.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtbpeqkmos.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gterxahmcg.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtxflmpdhc.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtmpioqlal.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gttwfpekwl.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtygxrcdzb.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtlttkflan.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtkuqlqjhd.html

Ruby: super
来源：http://hz.birdmap.top/gtrmdasjgl.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtkaojpkku.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtytvurnbu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtkgfkpdwi.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtrpguthdh.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gthicdjcyo.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtaugatxey.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gthclargbk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtcvqjbgbx.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtldetzjeq.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gtxpgrlqmp.html

[G09] 接口 / 抽象类
来源：http://hz.jlsjyb.cn/gtqriwzcoj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gttplkxwmd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtzmbzlxkk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhengqikj.top/gtghfvjbjw.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhengqikj.top/gtqcblmnjm.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtglqccxxg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtkvhlukye.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gthfkbnlbu.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtccijpcxp.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtiqzglkre.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtexecvsao.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtdudflfwg.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtwjevafdq.html

TS:   public / protected / private
来源：http://hz.zhixingplan.top/gtuxnqwhmr.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtxzsssata.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtzceemzwc.html

Ruby: public / protected / private
来源：http://hz.svipenyu.cn/gtqoavzdsr.html

C#:   public / protected / private / internal
来源：http://hz.redwolf501.top/gtlekveoix.html

[G11] getter / setter
来源：http://hz.xziqi.cn/gtbokeyksa.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtmglhfhun.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtaupxsrip.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtqxvxplxm.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtgkrzefjb.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtftlhsxgv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtgckohnvf.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtzjraqykl.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtoxiiugwq.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtfcccevqw.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtogiwtiqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtplngkubv.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtiqgkblgw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtejjhiggy.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtzvtrexsp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gteiaqacpa.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtrjkhzurp.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtimnpfvhi.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtbkzraajr.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtvmzoaudr.html

PHP:  $u instanceof User
来源：http://hz.daxiang520.top/gtiaaegjhe.html

JS:   u instanceof User
来源：http://hz.yueranfly.top/gtyqeywezh.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtsaelqxbw.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gttvbjysso.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtlfnknygc.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtyqysyuch.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtkjldcula.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtkjcdtrfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtnzryscjp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuxming.cn/gtrxmzsymj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtcjnwsmeq.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtknlupsyq.html

Java: record User(String name, int age) {}
来源：http://hz.yueranfly.top/gtvlsplqxz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtwruwlbqp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jlsjyb.cn/gtacijdkjj.html

C#:   record User(string Name, int Age);
来源：http://hz.gzhubu.top/gthbteayhh.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gteqhhaazl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtufrotflg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtysnodibx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtyxgycraz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtlhnugvqv.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gttusovked.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtdyrlekjo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtzhswliid.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtcurbvbkl.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gteychgrfq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtjyzicrgj.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtmvrufwvc.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtprzplxuu.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtsxcpvsuf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtvlfnimqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtkmehymvc.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtemxybwdd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtxfzsteaw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzrksvubh.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtzgjxptxi.html

================================================================================
来源：http://hz.dianchejie.cn/gtnvixlfhb.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtxzofzxaj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sysykeji.top/gtrwkfqtpv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtakjqccxn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtqjknpkqs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gthftsuqav.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.quarkkingdee.top/gttklqeoho.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtzwmylnik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gthokvbibq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtlhaitszk.html

[H02] finally / ensure 收尾
来源：http://hz.tian-w.cn/gtdswnanim.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtokvfzuaf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtavxftgvb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtwdscailw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gthlzbygme.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtxervlsmt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtinbqfipm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gthjyhcdbn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtqixgqqos.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gthokwccjj.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtvybdvygq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtyghnmgjl.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtechyqexo.html

TS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtceclqyzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtnxehxnns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtbqeknltx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangkeji.top/gtcvlqfzpd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtyfsopkwd.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtyvakgiow.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtgcwqvorc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtkqjsovfg.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtyejaufmr.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtnctmsxsf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtttzasmlf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtykzgndtj.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtyzintukz.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gtkiomzfzh.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtnrsunhyu.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtudvagxkf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtgbrkqfdm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtbwodlgvw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtupbdpjwf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtfqdltnfj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtbngnwixv.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtriknzftr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtaynynxmp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtklxquuof.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtruwgqzoe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shangyingyoupin.top/gtmmhxzdxn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtfjsmouxx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtmnchxmdq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gtocupbjsg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtmslazphh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtuirbqcke.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtesnjuuzo.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtccuosayj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtwzcafbtt.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtrxxicdcr.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gttrunuetu.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtrgnfrkab.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtjamxhfcn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtrinhjing.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtbztlibbn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnxiangtu.top/gtjgrbwuxs.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtdvkzfhvl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhaomingkeji.xyz/gtzkvffmtu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtfhybdvbm.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtelpjfdfb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtlvwxsjaj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cdnleiting.top/gteonebnfn.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtevtlgayg.html

Ruby: e.message;  e.backtrace
来源：http://hz.cqqwz.cn/gtvmgiosmx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtgzsvnmuc.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtndshomuh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.vqdsnc.cn/gtovqfrjzl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtgpcnknba.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtnmqrjdvr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtfebgzhvw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtktofklxp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtmfmeazkj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gtjqwdxpcs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xziqi.cn/gtwgfcxngo.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gtgjchacby.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtssopckft.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtwyjpeqfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtnktpwqmr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtgimluurq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtbrywbxdg.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtbpktjzic.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtlpasrjjf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daxiang520.top/gtrpuvfiyl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbapxtjna.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtllomoect.html

================================================================================
来源：http://hz.gotoacloud.top/gtqqpatnev.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtumvsuznz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gteymmaend.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtjqakyruc.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtflunfcbp.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtaeemodrd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangtech.top/gtoiygucbc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtrptkekdh.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtcbdjambt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gthpumksky.html

[I02] 提取所有匹配
来源：http://hz.gzhubu.top/gtzkegxoru.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtlpmshxua.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtqpborgal.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtvjclklmd.html


<!-- 参考信息 -->