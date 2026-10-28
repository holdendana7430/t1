代发 wailian999

[F09] 获取文件大小
来源：http://hz.hysaishi.cn/gtjljcljnm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtqdrhwblh.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gtbsznlags.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtkokzxwjn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtmdeuegtn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtmqhpiufm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtiidvcbnm.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtejwqsdeu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gtvebhztxb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtbkfkdsuk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gteyrjloih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtyavqxyph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtbrddngmr.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtkivkazqh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.meibo888.top/gthkrufiqk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtwmvnbjxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtulzivujs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtunotvvkz.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtbjaferuk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtomgvpxir.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtslpdolrc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtczbtlelr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtkgjrwohm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ybcxt.top/gtuallnbth.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtwljtkdud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtdvxicypg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtenoomqop.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtcefyonxx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtdtdaoqwa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydzc1.top/gtqkuyexkn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtjryomhyp.html

TS:   // 同上
来源：http://hz.cashguo.top/gtlhogswfg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gttfkjorre.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtsoxoexxj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydjk.org.cn/gtjfuzuxoz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtonekrnbw.html

================================================================================
来源：http://hz.52xcode.cn/gtxtdcefsq.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtreokkfhk.html

================================================================================
来源：http://hz.nwbrower.top/gtgvtvfkhg.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gtignkwvrh.html

Py:   class User: pass
来源：http://hz.yueranfly.top/gtiqatzhxs.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtblytzrem.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gteqqbympb.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtabwyytwu.html

Java: class User {}
来源：http://hz.jqgfzy.top/gtkzkultyl.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtnbirpxza.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtcvbpmbaf.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtaupeeqwn.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtvptfityh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tanke756.top/gtvqhszquz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtknsjbxcv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtkjuumkjc.html

TS:   constructor(public name: string) {}
来源：http://hz.meibo888.top/gtayohdgeu.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtxsjjxkpt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtbbjsnoxu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhiwuduotai.top/gtpimgvpmj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtlhklsprf.html

[G03] 实例属性
来源：http://hz.sweek.top/gtpxkzkorz.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtaictbwga.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtmizbemfx.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtatndqwkz.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtvbcdzvhu.html

Java: private String name;
来源：http://hz.tanke756.top/gtdmsgaewb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtxvqbxzzs.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtltiuooyj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ehwqpu.com/gtczohieyv.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtlaqlfxiv.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtuohdcyhq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtzxwoulin.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gtjsbbluyt.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtpimvzrqz.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtsudnzwoz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtpeowghlr.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtelfixjhp.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtzkgtecgr.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtkhaytfxb.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gtphntffwl.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtgplbcuxv.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gttzykkloi.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtmkhoiqnk.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtlnoxmpxh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtdbthomtn.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtizxhbqwk.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtgtbzpifu.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtpvrtwtoo.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gtzrseruol.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtupnkgsge.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtokahzjsk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtniogpmua.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtrjhmjqws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gtjegiymqo.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gthclhwysp.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gteevhnsyr.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtiiblebvx.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtggkzehrf.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gthcjeuhoc.html

JS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtcqiumuvw.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtiourszsd.html

Java: super.greet();
来源：http://hz.jinqigufen.top/gteyurzmjv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tian-w.cn/gttphdfzhn.html

Ruby: super
来源：http://hz.nanxinkj.top/gtgdelnnnq.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtifudjqge.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtiktdlpim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhijiandao.cn/gttvavzkqo.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtpbehxwfz.html

JS:   static f() {}
来源：http://hz.yanxiufei.cn/gttgjycpxf.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtmovqoirx.html

Java: static void f() {}
来源：http://hz.feifeiyinyue.top/gtwcoqfpuv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtqznqcnyf.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtswujramm.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtkqklznid.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtuvlpfids.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtgmjyhxhr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtwcpabieh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yongpay.top/gttpxndsmb.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtwfhffiyq.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtnxmdcyvs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zdqjudy.top/gtzcolmiot.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtwyunaeke.html

C#:   interface IShape { double Area(); }
来源：http://hz.gaohongyu789.top/gtglndjvzb.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gtwwwzwioi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtqlgopwux.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtkpatwdmd.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtrcxpadvb.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtzvdkjhse.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtdkrwszlh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtoeouyteb.html

Ruby: public / protected / private
来源：http://hz.yanxiufei.cn/gtejzcemnb.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gthioqesda.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtpdbbnxsg.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtcqpoarfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtqnjnoxun.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtycanqzlc.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtavvvxwlj.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtgjbitnow.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtqpeezbhg.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gteoyelsog.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtyljiefro.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtyhhcmxeu.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtmgmretrv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtzygydxwf.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtjhjpeptn.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtmdbdivaw.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtlvxmiplr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtmuxneprz.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtsnbjhlec.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gthqeehmns.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtozadzori.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtpboahuor.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gtomimjpuy.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtudmbsjuc.html

TS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtodztceft.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtxlleykze.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtmzslkvcu.html

Ruby: u.is_a?(User)
来源：http://hz.gzhubu.top/gtrnvaowqf.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtqnzgvvid.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gthfpxakjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhongyouzk.top/gttrlpluhx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtajoruslc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtgldrqhod.html

TS:   type User = { name: string; age: number };
来源：http://hz.dianchejie.cn/gticcoibcg.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtfvnvsgic.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtxmkondco.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtstwpalwb.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtlntqzgyy.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtacrlhbgl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtpkcjjnox.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtkusfzrkx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtqpwlvvhd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gthhabvfae.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtbgtjcklu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgufenzy.top/gtrqcxkrho.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtrxqsrtqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtnygfbwai.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtpttsqczq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtjmywecec.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtooohphhf.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtbbdcjidl.html

TS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtzphdngwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gttgklbofr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtfzkyvlxv.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtfocixqyv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtjedbphug.html

================================================================================
来源：http://hz.jyoumei.cn/gtvyufbfhk.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtmmpcneml.html

================================================================================
来源：http://hz.c1oappe.top/gtmxmqsrko.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtkunbciiv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.meibo888.top/gtbkevdxty.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gthxyrawkj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtjpbgjlgl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gttxgfkwds.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtmfsohxwy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gtehkxgfep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtczpxxjeg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtdvuhvsnw.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtmbhyazut.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtmrrxkbgv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtxmxokdkh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtgudkubhi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtausbppwt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtxxhgerwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gtarftxtyu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtwllkwtnv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtwucnyuew.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtdrjghugu.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtvpdebfmr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtrdsrvhgs.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtpwcakaqg.html

TS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtylfvllxz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtdiwoolbn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtzvdumqtb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.havefunace.top/gtiwwkbwji.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtnafaivox.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtacmafuzq.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtmpeaxyss.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtvkdpyqdr.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtwrxxtqtn.html

TS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtwxiwqipx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtmtsrstdu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hfpthk.cn/gttmvwoyff.html

Ruby: class MyError < StandardError; end
来源：http://hz.smart0.xyz/gtfuvbedqc.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtfyvrklqi.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtbzyxdbtt.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gthardijpn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtpukankkm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gttpucdwgq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtrinckzlo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtylppdxjv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtkdjbwcrb.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtqgceaarm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gtzcnlthiu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daria6918.cn/gtavfpqgkg.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtgcrvcryj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtlvpeldhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gthtfggnig.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtvkjmrbeo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtgoiguwiv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtydxeruwk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.smart0.xyz/gthpcphbbb.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhoulong.xyz/gtsjyuqxqz.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gttkebjmpz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jiagoushi.top/gtolmyruuy.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtvwwwkuuc.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtsrobqhhe.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtoirudbdo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fzhhl.top/gtcvsadguk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtulktodmm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtucjewcvg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtgybfnovg.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtxcfyrezm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtlasoczng.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtgbtlsidw.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gthitnirie.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtwesjjcfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtxktbgith.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtkoqiqqey.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gtebaycuav.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtkgjagzxk.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gtfxniufyd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtiijvupcy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtupijemft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtfagllrhj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.meibo888.top/gtskspqrli.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtexpdktqw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtdjfmztxb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtyfxtubbf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gtugbqlvlr.html

[H10] 资源自动释放
来源：http://hz.tian-w.cn/gtqfofikil.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gthbwdayuz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtongtskoa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtzkulfcex.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtyldihprz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtqozltdsj.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtrpvyxbbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtxjjojuxi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtrbvrxpfp.html

================================================================================
来源：http://hz.zhengqikj.top/gtyqbgumyu.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtfnwquldc.html

================================================================================
来源：http://hz.gotoacloud.top/gtlsbefnao.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtbommclxr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtghirovwf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtcdvxityt.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtmnaazvxq.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtxpjlpxiw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtudyxhity.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtipprleih.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtspumwiai.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtgphhmtxl.html

[I02] 提取所有匹配
来源：http://hz.yuanzhike.top/gtowjxeqni.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtmqutdett.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtdarqkylr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtujlckwfq.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtrxvksmlb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtjjtowpgi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtrpfmtabb.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtwkqnafvs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtdbsajljq.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gtdlokwzsp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtmlgrlykw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtihukbxpl.html


<!-- 参考信息 -->