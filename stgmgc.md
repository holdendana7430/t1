代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtyedgtqif.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtbgfmelfu.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtazrbsqsl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtmoupbgcu.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtmpypijjo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pengpengdd.cyou/gtqhxneijs.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtetkngcti.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtqtcbnpmz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtrlfmnqeq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtbgwmxdbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nwbrower.top/gtldnkijno.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtrlqwxeye.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtiqmynbzb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ywan-chungtsiang.top/gtclxrdhiv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gthbkobvyr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gteupcfpbq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtabaysajn.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtfzuhyuez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtgzbbsdka.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtjqyuyycx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtwtjcigvg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtogtfgjdv.html

[F11] 复制与移动文件
来源：http://hz.jinqigfzy.top/gtokfveumx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtvzsqqunf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuxming.cn/gtypedlqlt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtyowewhnu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtqtpmjfdv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gtvvskhbkr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtrmfaiyee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtyhdubjez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gotoacloud.top/gtrbddmpvq.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtzlcpknei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gthggdkjuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daxiang520.top/gtyabsgjoa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtsgnzyczj.html

TS:   // 同上
来源：http://hz.zhoulong.xyz/gtrqkcfmwh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sxryk.cn/gtaaolavch.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtchvkmfyj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtxlhrgfez.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtpqbrzful.html

================================================================================
来源：http://hz.jianghu66.top/gtztdlnhtr.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtndlcmdod.html

================================================================================
来源：http://hz.cdnleiting.top/gtgwvycoud.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtzmfuzgnn.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtbjxyxzvu.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gthhcduriw.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtafpsdyjd.html

TS:   class User { name: string = ""; }
来源：http://hz.jlsjyb.cn/gtyhirqjkl.html

Java: class User {}
来源：http://hz.shuidangran.top/gtadztkoro.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtdxyeqnsb.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtycusxrnj.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtxxvbscxp.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtziaehnin.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtwwexdnty.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gogol.net.cn/gturkaehrb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtastldpjn.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtaixugsyp.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtkbnfwhda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtvobwmspx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtcuobouzs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nwbrower.top/gtzgoedsqu.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gticvndvlk.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtsktfmzia.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtfrihvgsi.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gthtzpsqak.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtfxubptnb.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtewhqipyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pycfn.com/gtrycvozsk.html

Ruby: @name = "x"
来源：http://hz.chenzaomai.com/gtbrnpzgwd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtiayuyird.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gthinocptw.html

Py:   def greet(self): return self.name
来源：http://hz.shzxlz.cn/gtigpxjwko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtlzwoxbdy.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtoderjdll.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtmiakgxur.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtmvjifgfr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtyresmglf.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gtvzoosmhs.html

C#:   public string Greet() => Name;
来源：http://hz.daria6918.cn/gtttgpwbeu.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtwzgvagtj.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtokhdfwcq.html

PHP:  class Admin extends User {}
来源：http://hz.chenlongwang.top/gtsrnlrgzh.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gthmlxblzw.html

TS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtyzzvyegi.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtxbkplcsb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtxbodpvwi.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtaluvhyyj.html

C#:   class Admin : User {}
来源：http://hz.yvedp.cn/gtzgfywkqa.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtabpglsht.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gtfunqqfog.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtgmesnusy.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtnispomui.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtfpfgrjfv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtdqcrjpcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtbviqpomi.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtufkbiayj.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxinkj.top/gtpxmalcur.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtpynmlapf.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gttbgitvgx.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gthprqkqxp.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtknvittea.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtmdibmnyu.html

Java: super.greet();
来源：http://hz.meibo888.top/gtifgoactr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtlwnrqzig.html

Ruby: super
来源：http://hz.sysykeji.top/gtqaxewapy.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtywwkschr.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtvcocfcbw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtyhxxqyda.html

PHP:  public static function f() {}
来源：http://hz.jlsjyb.cn/gtqbfwvudx.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtivppvaqs.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtdwdigwbp.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtttkbuyuw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtvksnoszs.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtptkxsygq.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gtblbeerbu.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtqcpxbeen.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtqgbxfmgy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtswfeodue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtqeubndwt.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtxnbhmkpi.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtjzlyvttn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtfxwhacna.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtcbcjyqcu.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtzgehyggm.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtdvwuqbnw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtvbvwslhc.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtndoevhiu.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtfdfasaiv.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtlqnkheow.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtvpeonsqq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtmzbggtey.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtuswspppd.html

C#:   public / protected / private / internal
来源：http://hz.yuanzhike.top/gtjgzayhug.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtnciiktfh.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtrnpsoexa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtzxzpdprg.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtpuwgtstg.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtwgyrmvdt.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtxggdbquh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nwbrower.top/gtszdvlkhm.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangtech.top/gtxfzfjhqd.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gttowirnau.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtzvkzmahb.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258888.top/gtkiazokzs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtsqgfoizf.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtobxjarrv.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtyqweoirj.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtzsojizap.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.redwolf501.top/gtitpdqoqk.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtjxdjiwht.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtychereww.html

[G13] 判断对象类型
来源：http://hz.ivvv.top/gtvmpsmloo.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gtmmtscvoz.html

PHP:  $u instanceof User
来源：http://hz.cqqwz.cn/gtxmabecab.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtaednarcb.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtejwckshq.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gtsppxhcdi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtxdxnibls.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtqwxtekxj.html

C#:   u is User
来源：http://hz.52xcode.cn/gtdkcsvsyg.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gthmqtnvjo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtyhjfkkur.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtucezrwvw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigufen.top/gtujtnqzer.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtbdghzwwn.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtbszawpys.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtasscftlp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtyailhazi.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtqypmccty.html

[G15] 枚举
来源：http://hz.yonumen.top/gtwkxlcrbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtywaglbip.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gtardzwwnw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gthjvgmxom.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtcfqpzmmk.html

Java: enum Color { RED, GREEN }
来源：http://hz.cdnleiting.top/gtqsdyuhgd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj202588.top/gtirfvrmuk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.quarkkingdee.top/gthoxughjb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtupnvfpcz.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gtbdoritzn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gtreookufj.html

PHP:  get_object_vars($obj);
来源：http://hz.tianlin.xyz/gtdijxpyck.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtkljglgbw.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtlxjaycky.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtfarlccqr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtozdnkikj.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtvxtwwslc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gtditsrccz.html

================================================================================
来源：http://hz.fzhhl.top/gtsqoltoad.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtozzmkjum.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtardwvdjj.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtowhsrcjr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.quarkkingdee.top/gtzbvuujjp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtvrfukvec.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtaiymlwhm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtzjzilsxt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guannengcc.top/gtxcsnuznm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtcpyulmki.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtuwlwrtap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daxiang520.top/gtwzggbhhy.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtpdzfpgkq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cdnleiting.top/gtmyfxjbsj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtnevpjckp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtwsmsdfdu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtlessyemy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtrlqisubm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtwyoqshow.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtywlosrpx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtdhofmvtx.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtwjvpgqaq.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gthyefcqqa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtuackpena.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtznxuuuoq.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtpmkeirun.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtoijodfcc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gtwkounmhc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtqzfknlha.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtgvzownjk.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtffzzwxks.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtkzaaeyil.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtvcgczliw.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtyxylmrvf.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtxszbcmfb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nwbrower.top/gtbolhrupi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtcamaddbp.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtovyvgxpc.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtfhcbxmhw.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtpatqvyne.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gthnysbzbj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jianghu66.top/gtutcccodr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtyyxgkzcz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtzeuityks.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtajzqkiha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cucudq.cn/gtstrhonin.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtsvdimbma.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtswlpbikz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtxcaxlnge.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtybphizkg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtbqdoddqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtnurilkyr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtzbodocsx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtmgzwpmsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtndysorsw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtekabinoj.html

C#:   obj?.A?.B ?? default
来源：http://hz.bjfxy.top/gtosfqkhkd.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gthxnxpfss.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtiojecksj.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtxriybwxg.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtllztyrbg.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtzcbhrbir.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtmraznhpd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtksweztnk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtmipphunj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yangfankeji.com/gtgxaanxaf.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj202588.top/gtfpefvzbk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtmwwamykb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtdsrdmotg.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtuuqanspn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sufxvd.cn/gtpxuzypnn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gtbzrouavr.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtrjydkltq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtmofazgdp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gtbjwxvdxc.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtsxjbybmr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtnusycber.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gttkmyhsyg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtsmplvsma.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtdrrrxjij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtoypwzjzt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shzxlz.cn/gtnyckgkzj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtqhevbaib.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtgnoliphv.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtjeyouhyl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtbeqsxzrd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtrykoqnqk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gteracihow.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtzxddsqja.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtiwfaoceh.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtlmjfhmlx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtgvhilany.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenzaomai.com/gtxhuvmbmk.html

================================================================================
来源：http://hz.hammf.cn/gteqbygqis.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtyhtoubtr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdygwcuvb.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtbnencqqx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gtazshmawb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hfpthk.cn/gtjebezxkv.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtdsvmvmdj.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtpsjvmglp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtwiwrmlpj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtvsinamzn.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtueiaafaw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhiwuduotai.top/gtadxpqqcz.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtkwtwrail.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtsssnddcf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtkeogruxr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenjidiqi.icu/gtwefmyxkh.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gttshjbnal.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gthstntsxg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtfekkuhvt.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gttcknuyon.html


<!-- 参考信息 -->