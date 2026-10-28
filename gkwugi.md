代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtfdyvblki.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtbomimila.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sysykeji.top/gtqnkyucks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtmonjagot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtpvrlknxt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.andypj.xyz/gtktwfkuxy.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtmbshfeuf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtmytzkbot.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtrmexhtza.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtluovreqy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtmnzvjind.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtcxhikpsl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenzaomai.com/gtavbzcbib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtnakfysxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yueranfly.top/gtxvaqpxnv.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtswupppbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtezmzrjbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtuyktbimn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtatzprgju.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtoxpkbupe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daxiang520.top/gtoqwzwumv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtcxfesrfe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtsdwhpbuq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtczlnwuac.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwxdnusda.html

G. 面向对象
来源：http://hz.shuidangran.top/gtarngvwud.html

================================================================================
来源：http://hz.havefunace.top/gtstfaftop.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtfvipplon.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtgnedyerg.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtxddjlrau.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gthuiujxdh.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtutfrnpbo.html

Java: class User {}
来源：http://hz.nanxinkj.top/gtfczfvbqa.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gttommmrxt.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gtrbhwvmij.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gtyxtgevla.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtzcoqwpzx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtpxkqpyvp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtvlovmxjc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtmnmvswxy.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtztvjmwxp.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtizmgguyx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtgmbzjunc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtotmqbwvn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuanzhike.top/gtypftahng.html

[G03] 实例属性
来源：http://hz.jinyuanbaomall.cn/gtjtphpdze.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtuzzyoakx.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtlzokvwcu.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtobzouztq.html

TS:   name: string = "x";
来源：http://hz.jqgufenzy.top/gttezoddab.html

Java: private String name;
来源：http://hz.yvedp.cn/gtkdqdwyuk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gtugtsubri.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtleuehpkb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gttbppppgk.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtldhvtbbb.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gtxjesvvqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtyzunkqym.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtvnnkwswl.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gttzvlmlfy.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtbgpijcey.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtluvnnbee.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtlciyjrdr.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtugorfiqw.html

[G05] 继承
来源：http://hz.cucudq.cn/gtmbgydacn.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gtvyixbbfi.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gteuyerdwc.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtjasjiicm.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtugspunnm.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtshcynsqp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtfuesvdvr.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtijdoxtno.html

C#:   class Admin : User {}
来源：http://hz.nwbrower.top/gtrrswqlwz.html

[G06] 重写方法
来源：http://hz.yanxiufei.cn/gttfrzultf.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtueajjmnh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtfupjgxjy.html

JS:   greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtwrfrdxhw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtmapzyzcn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtxvjqmsgg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtcmgmxuzh.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtdhgpjumb.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtlkprpuqy.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gtpnajjqrr.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtrnnctpsf.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtgjwicjui.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtdoeieqka.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtuzwtpqvo.html

Java: super.greet();
来源：http://hz.jqgfzy.top/gtdidmtojw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gtsfrqvmvl.html

Ruby: super
来源：http://hz.0kj1m.cn/gtrrjdicqt.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtdiqseioi.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtytxroegk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtsnkaedmr.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtpiolvtao.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtbjcffzas.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtkirljzbf.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtfyzimbkq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258888.top/gttkotnyvk.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtzoosoxxd.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtwqhsviwn.html

[G09] 接口 / 抽象类
来源：http://hz.tanke756.top/gteuayroew.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgufenzy.top/gtxcfnoyaz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtjevhfcpu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtixjvjuhw.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtlyohegos.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtbbbaukgi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtfgmsddvc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtfowsbzwf.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenjidiqi.icu/gtdgcuelzl.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtvarectgs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gtsfyltbeg.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtlklswpyx.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtozcrpjzd.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtoiffbmfb.html

Java: public / protected / private / 默认包级
来源：http://hz.nwbrower.top/gtwfidiuah.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shzxlz.cn/gtcdduluyy.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtqlkbxbjs.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtmhpnloip.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtnqztieel.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtloxbnnlg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gthnuffsxm.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtijgllhjd.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gttblnibip.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtfhuibzhz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhixingplan.top/gtuxjiituk.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtkomfxcum.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtypajpchu.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtgdabzjqe.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtggtrnxje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtuwpfpeig.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtjrbthknq.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtfvhbkhxx.html

Java: @Override public String toString() { return name; }
来源：http://hz.jiagoushi.top/gtuyrtlodl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtmnycrwnc.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtixnbkuxh.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtbeknnnea.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtolwkrwfh.html

Py:   isinstance(u, User)
来源：http://hz.gzhubu.top/gtovxvnawz.html

PHP:  $u instanceof User
来源：http://hz.hnxiangtu.top/gtnjkawmsg.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gttmhwmtsx.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtekwqwkcc.html

Java: u instanceof User
来源：http://hz.jinqigufen.top/gtinxmqsiu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtbumfkavt.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtdykyxxfy.html

C#:   u is User
来源：http://hz.redwolf501.top/gtzwsaayfy.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtfxyeaoxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtoioociwt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtwvkktikw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtosajcgxc.html

TS:   type User = { name: string; age: number };
来源：http://hz.dianchejie.cn/gteufswugv.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtrwpctvcf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtjdlwbgxg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtxrznplxw.html

C#:   record User(string Name, int Age);
来源：http://hz.yongpay.top/gtzgvdyhqe.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtgzathauy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.svipenyu.cn/gtjuurdvsd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtrxjsfolt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.meibo888.top/gtsiuxxyju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtysmszuvf.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtgfmnmnov.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtozigfahm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtcgjouazm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtlvjrgexq.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gtazfhgfft.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuanzhike.top/gtdxqadsqx.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtaxcwqawg.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtmntmwilo.html

TS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtunzvvipj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yanxiufei.cn/gtifsemvde.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gthiiucnce.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtbxkoavuh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtikomslbf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtormzwaik.html

H. 异常与错误处理
来源：http://hz.yuanzhike.top/gtftoanbax.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxsmfsmnj.html

[H01] try / catch 基础
来源：http://hz.yonumen.top/gtofvrdsfe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtemchvnys.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gtocqcexys.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtmddxfvws.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtupavfemx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gttdcxdkbg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtgqvpudjp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtznzbboud.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydzc1.top/gtxrcijfss.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtnfsgmctz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtwtwlwflo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtrmbbdsal.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtewyrzjyo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtuoklyfio.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtimaawyui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gttubnbkfl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gttexmjdrs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtlcganvmy.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtezpkuaix.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtbasnflaa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtzriznxiw.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtvkgqerxo.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gthxxspsjt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtowyyrybc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtdavkuwkf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtbwuadjtm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtzsmvnrja.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtycigoscd.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gtwdlxhqxn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtfffewalq.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtamhqnxlv.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtlbidpdad.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtmeehbnvh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtblpbwyzm.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtedwlfwsz.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtvwnvvlnf.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtmymkhowm.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtyfhhhpvv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtsmkgqrzb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtpyrfrabm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtlgdlduxw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtnltakndj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtszhluxno.html

Ruby: rescue ArgumentError => e
来源：http://hz.ehwqpu.com/gtdkiekfwp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuanzx.com/gtybyofnnf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtqcxfvjbe.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtjkrjfsog.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtliguucwu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gttzyadvog.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gturucgyrw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtdsjiwsqr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtgylcvyot.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtwfrcvfml.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtdhyvhybc.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtejfxgmdd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tanke756.top/gttagaapax.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gthfzqaqxf.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtkcgbjmle.html

TS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtlrgwlmxr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtjzivedws.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtvpptacwz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtfchllxwz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtinzjjoig.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtixrwjwgu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtttqzqhfk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtbmbktwwi.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtsultzdwv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtapngetxv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtzkgbtmkx.html

Go:   err.Error()
来源：http://hz.nanxuanxn.top/gtdhxyketl.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtpwuzwegr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtfklonbqm.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtojksnibg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtuxkwunvf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtaatkvqrc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtdytwzdxa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtotzezrqk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtmsoagcmq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gthkanjpvx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtzkvbllbp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gthgfhuary.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtelzbzwce.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtavpsqtfs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gttwudkqdi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtcxbkmowx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtkcsimpzz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtxepwqwxo.html

Go:   defer f.Close()
来源：http://hz.fengsongda.top/gtfweutnsn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gtnhjpzbnp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtwszidgyw.html

================================================================================
来源：http://hz.guannengcc.top/gtvjuxajue.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtcllfgzns.html

================================================================================
来源：http://hz.chenlongwang.top/gttkntkwmj.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtlozzvzbq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtuiykopmz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.svipenyu.cn/gtqpavparw.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtlgxyvjrp.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtxykszhww.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuxming.cn/gtmaikviyz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtflyjpzfm.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gttjsjmoza.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtcuyabnyc.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtfhvayxjj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtjixdgsye.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtqdifpxje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtmgfjckck.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtfderpljr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtugyyxxdg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtvinysakz.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtanasryml.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gtavxmjtlk.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gtagjajxvj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtkvddofcu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangtech.top/gtjoazdeiv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtbefaykpa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtndfwtbfa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gttclwjsas.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtcgaqnafz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtbbnrtfiq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gtnmjekrnm.html

[I04] 正则替换
来源：http://hz.chenzaomai.com/gtyvccnaek.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtutbljvby.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtnlxwqbrd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtfuanqfwe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtoljjcpxk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtsrntwgsc.html


<!-- 参考信息 -->