代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtswqxgird.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtsupimisv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gteukbqtkj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtczdviatc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtnddejjuy.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gtojdytffk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtdrguidlr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtjvimdwxe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtwztfinyi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtapmlesfy.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtuifjomqo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtdnextume.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtvvambokq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtsqxslnau.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtxqmslylt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtkzwskfyr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ivvv.top/gtrazstmfs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtcrgmqcea.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtkxpgzmhm.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtowvkiygj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtyaewvlwn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gttzhcvtyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtrdusoevi.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtitfjkorq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtmbnhuihw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenjidiqi.icu/gtallzuvcl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtkrttcmle.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtanjzhulp.html

================================================================================
来源：http://hz.vqdsnc.cn/gttvanrhda.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtjsxfwwal.html

================================================================================
来源：http://hz.zycfv.cn/gteeqjdqdb.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtitamiymv.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtnhjuljlo.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtukfczgnu.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtokggnhba.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtigskfauz.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtvxjdrwgu.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gttnwgqtfd.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtfmcqblix.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gtaidbahsk.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtnausnupe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtjlhmzfno.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gtqlcpupaz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtgyemzdnu.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtkrdxydaf.html

Java: User(String name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtpdibvtlg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtsejvxkdf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtiwhbxcwy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtmpgxaykq.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtcdungcio.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtjxhxxfdx.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtrzqiqzzi.html

JS:   this.name = "x";
来源：http://hz.sufxvd.cn/gtyzvclris.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtlohncoja.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtovdwfsac.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtbadqvhbl.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gthtqqjgul.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ehwqpu.com/gtmonyjruv.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtuvxtgzsh.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gthgknvkbe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.havefunace.top/gtqsvktots.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtnwmddotd.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtcrleedjs.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtkwhzykos.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtxzalhhoz.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtvgmaynsz.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtszberatp.html

[G05] 继承
来源：http://hz.fengsongda.top/gtrogkyona.html

Py:   class Admin(User): pass
来源：http://hz.ybcxt.top/gttfzwaegj.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtespkyinf.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtzhzttfhl.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtqfzrvvlc.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtfjwgnqws.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gtvnszjjvb.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtuauojapz.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtsznepfwp.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtmefumzjf.html

Py:   def greet(self): return "admin"
来源：http://hz.xuetiantiany.cn/gtwplouzcq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtxnqfdscn.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gthasxxrtj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtphwgrkxs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtpamftlhj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gttmsagbmi.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gthnwhuvgt.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigfzy.top/gtnhhselvw.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gttbepmsvn.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gtmctbtquf.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtlulcbrlj.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtzaqfpovb.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtjppexlyn.html

Java: super.greet();
来源：http://hz.ydzc1.top/gthjelezhz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtanmveoof.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtyedkojvi.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gtgnrmaixz.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtykljepfi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtgcuceteu.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtwycivbrs.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtguhatlqq.html

TS:   static f(): void {}
来源：http://hz.xziqi.cn/gtquarlqbf.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtndvxtghy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtentfpwhj.html

Ruby: def self.f; end
来源：http://hz.9152youxi.cn/gtleodvfdw.html

C#:   public static void F() {}
来源：http://hz.316326.xyz/gtekcjsbye.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtscpxvyee.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gteqxqnksi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gthszriesl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtlvxiusra.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtdmnbasga.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtzhszkxjw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gthzrkfmmr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dashuyun.cn/gtngkasmkv.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtdkksofny.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtalkolznx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtqxwwnfjs.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtiiuqusbd.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gtnbsthuts.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtrcmwjcmq.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtlbwrdgzs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtmvttisxj.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtnxigjkpx.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtuhwuiekz.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtoggxohtv.html

Py:   @property 与 @x.setter
来源：http://hz.yvedp.cn/gtkfkqdubi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gthwrtbrte.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtlsvpzpvn.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtkaytkkhr.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtyjzfaset.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtzbpiwxdj.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtevovvrwe.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtkegjpvmv.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gthptsulqr.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtrmeghkfd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtqszolfig.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtxottyhll.html

TS:   toString(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtmbrbclfs.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtqhhsbkax.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtbmeauglz.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtbukiiozw.html

C#:   public override string ToString() => Name;
来源：http://hz.tanke756.top/gtqptrqaux.html

[G13] 判断对象类型
来源：http://hz.bjfxy.top/gtzaukuxrs.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtbgfqswpr.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtbhuzmpoa.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtdntyfruu.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtayucxnpr.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtyhtafwum.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtjailwaao.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtlxpcysbj.html

C#:   u is User
来源：http://hz.yuxming.cn/gtqbwfxgjb.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtxnriikgv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtupkzkfcu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtswzprrqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtpuyeltyb.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtgqcnkebs.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtmdwlwhto.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtbfwgzsbb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtinmuyvkp.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtgomqwlni.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtzrmitxla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtexttkcyo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtcpjfsptm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtnlhovrkh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtwxrutypv.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhongyouzk.top/gttnxdyctk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtodcrpcna.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtonmovzry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtqcxjltdp.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtfnaompsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtuedlucdx.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtptiptjcu.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtyfmqiqeu.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtjjowdvtm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yvedp.cn/gtzmbypvgt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtxfkzpfoc.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtlstuftab.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gtnlnfmntf.html

================================================================================
来源：http://hz.gotoacloud.top/gtyssockeg.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtduitdjlc.html

================================================================================
来源：http://hz.jiagoushi.top/gtdmlooleo.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtjijanvsk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtlphqqyva.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gttagrxcux.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtrcmjjsfw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fengsongda.top/gtxblwczel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtwpimnrqm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gthjnidclg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtemrwdfqi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtkbarhpfb.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtofsiiksm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtscstjfat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtxcyytngy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtrxyykfgn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtyhjpqgow.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtpeftoovo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtbdjvdvex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtdlsytdpb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtyjkymazj.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtbjfusgyq.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gtvzjqwoqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtluoxwtwf.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtbtzqvvlc.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gteekyxcaq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtsglzzapa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtjhtwlxhh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gthwqfeani.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtjjcqyapv.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtqbkngscs.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtaghbomrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtvkmvbsob.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gthhzmdqpz.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtwsvodhsl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtltojuapx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtwgjvblva.html

Ruby: class MyError < StandardError; end
来源：http://hz.hammf.cn/gtmfijmaso.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtpvqbumgk.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtcfkpuptm.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtrhlxrpzg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtmtaxdfsx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtnbvicjpx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtgvjronkv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gtmammtgwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtdujxsuab.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinghuilouyu.cn/gtvxoljrfz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtykjnxvzc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gtweviphfj.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtkaeurctu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtkfkhnjin.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtnexmfktz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gttbtmcklz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtasfcezdd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtfxlzmdzd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtayjgmviq.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gtlgxrrrqh.html

[H07] 断言
来源：http://hz.daria6918.cn/gtfvtlhyux.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtjomouxsx.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtnbpprqjp.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtkvkzlzew.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtbjzcvozp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gtuwqqqbls.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhixingplan.top/gttjpddwln.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtwaxuimht.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtftakedll.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydzc1.top/gtgtgvizku.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gtgqxvdfza.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtuciidifk.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtbhqwvfqm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtfgcwuqyl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtnjrhfxnw.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtrcqbllpm.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtgfmqbzob.html

C#:   e.Message;  e.StackTrace
来源：http://hz.iojbl.cn/gtyiszaqox.html

[H09] 带错误码的异常
来源：http://hz.cucudq.cn/gtfrrnrcep.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtjrknuskk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtpwbqxyxu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtzsfnkfmz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gtwtnlbpmi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shuidangran.top/gtzayrzyyh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtsnxuwnjg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtmbcmexws.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.feifeiyinyue.top/gtlcfqkrgz.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtocdurbad.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtbfibnpah.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtiveqttuw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtyreullit.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtkovndiby.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yueranfly.top/gtpxhsfvad.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtfefuwceg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.andypj.xyz/gtgjywlvle.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtojddnktk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtntqxmcsa.html

I. 正则表达式
来源：http://hz.zhiwuduotai.top/gttskizfzg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjmdzawnd.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtpckobsaq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtrcyqrtis.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangdashe.top/gtffwjhdfu.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gthsboslme.html

TS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtozwexxfd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtikeyprdc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gtmxjgmwbm.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtulxkedjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtejebyeui.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtbmzfreqm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtcujnzsds.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtzurarxhe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigufen.top/gtuzyrpyhm.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtrtviicho.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtelorslfk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtwurymdcw.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtyrfvmcli.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtrsqtvqjs.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtvetjlxux.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtjlqqdezr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xziqi.cn/gttlearnxt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gtxxpzermo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtokeacebj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtuxltjvbo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aibaodan.cn/gtkxzhsljl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gtmvxvylgt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tian-w.cn/gteritcrmu.html

[I04] 正则替换
来源：http://hz.wangdashe.top/gtllgsraox.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtrmuztxpw.html


<!-- 参考信息 -->