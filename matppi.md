代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtzylsxoec.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gtphdxziro.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtssbmjutg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtxhfutkgr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtbqoenuke.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtybdxstdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gteblrubnb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtaczmlwsy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtdiathyqv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gtldaceyzz.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtfvrlfamn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtxitxntqx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gtnsfsemmb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtyhereadm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtbfexytai.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gttqzohpau.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtmbimhxyy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtokokwqot.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtvfypgrrg.html

[F12] CSV 读写
来源：http://hz.chenjidiqi.icu/gtxhhcztcn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.birdmap.top/gttjrkbcsh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtjstvshru.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtazxtnbmf.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtmmdzwlsf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnqzz.top/gtkefodysi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtzycdhfgf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtmjhlyycq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtfztqazoq.html

================================================================================
来源：http://hz.hnxiangtu.top/gthgknrhza.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtsysashrs.html

================================================================================
来源：http://hz.ivvv.top/gtqclzrtan.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtsdhetqbf.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtkauayycg.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtkcganhit.html

JS:   class User {}
来源：http://hz.meibo888.top/gtkxsovztu.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtnnheguey.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtjqexppwa.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gttptkxoag.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtdibmrzhe.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtbstkhopo.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtbpcxrwej.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtaxkagwna.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtkkgfcgnn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtuginlhyk.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtdmqnrspj.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtnhpqmcnk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtaxefjjdm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gthqcelvpw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gthctqoxda.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtlcizcjyh.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gteigpdnen.html

PHP:  public string $name = "x";
来源：http://hz.smart0.xyz/gtmhvbaibj.html

JS:   this.name = "x";
来源：http://hz.nanxuanxn.top/gtqjvumcnn.html

TS:   name: string = "x";
来源：http://hz.chenzaomai.com/gtbwjqlgdx.html

Java: private String name;
来源：http://hz.gzhubu.top/gtiremuodv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtgpibtbfw.html

Ruby: @name = "x"
来源：http://hz.yongpay.top/gtoriljjgi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtotyhomfm.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gthrijcexs.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtkabamxad.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtnwrxwfhx.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtxvrgfxnr.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtihxrxysw.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtgjkykkzc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtvtgegkfz.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtehvyfpif.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtrtaqthso.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtbvlrfxzu.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtduefqobn.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtnlhvrdyk.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtgdolymwc.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtljuwxsce.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtgpazsmey.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtktlrsaml.html

Ruby: class Admin < User; end
来源：http://hz.hywenlv.cn/gtzwwpykit.html

C#:   class Admin : User {}
来源：http://hz.gaohongyu789.top/gtwtvfdjjn.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtktnvcvim.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtofuvwozu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtiafvlfky.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtzmkoynrm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtcqwoubtd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtiujicyqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtrmlursck.html

Ruby: def greet; "admin"; end
来源：http://hz.0kj1m.cn/gtdxhqrxot.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtdcjczfaw.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtovhndwxl.html

Py:   super().greet()
来源：http://hz.cashguo.top/gttgcwoccv.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtzibhxybh.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtgxeiwppf.html

TS:   super.greet();
来源：http://hz.gogol.net.cn/gtxjktoytg.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtxudynbsq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtyiejitri.html

Ruby: super
来源：http://hz.svipenyu.cn/gtxxeakzfx.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gtqiigkwwk.html

[G08] 静态方法与属性
来源：http://hz.daxiang520.top/gthnlgkfnb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtglbrleqn.html

PHP:  public static function f() {}
来源：http://hz.aibaodan.cn/gtbfooycpl.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtkqtaqelx.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtxwrlcjzi.html

Java: static void f() {}
来源：http://hz.xziqi.cn/gtlrmwjcdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtopgsrmxt.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtglasitxh.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtyjvrrjby.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtxhdriboy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtjlhkefxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtkplbrseo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gtspveflsx.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtbjkhxrjw.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gttfcbsyru.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtgjyjsupj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuanzx.com/gtixzqgvbk.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gttdhswyor.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtpajetylp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtnaukqwpy.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtwrghvazq.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gtqridmlos.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtasayzqtt.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtcqeweaax.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gtltkybkar.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gtvxzsjeww.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtiornoqsf.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gteqwuexja.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtvnjdpraf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtepuxroad.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gttrvpfdxd.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gtdmxazkgz.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gtzrufydxf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtqfqptsrp.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtfibxkeks.html

C#:   public string Name { get; set; }
来源：http://hz.jinghuilouyu.cn/gtiqqqashw.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtnplkvvkv.html

Py:   def __str__(self): return self.name
来源：http://hz.meibo888.top/gtyztwymzb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtdrpbjuww.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtoxlqugsg.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gtzzqctobe.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtutzntanf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gthzvaboyf.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtdoyxkdpa.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtupluecxp.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtdwjlamer.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtyxmisbxp.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtlhaiotmq.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtzjttfyvu.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtmddsxeon.html

Java: u instanceof User
来源：http://hz.iojbl.cn/gtngslpecc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtaojkaxdp.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtxlngcwvd.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtuducqhvk.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gttwawrqsr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtplgitclx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xingfuxueyuan.xyz/gtptigaaii.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtxydhphpf.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtcalekkyx.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtjbrroovs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtlkbadniw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtdybqjpjh.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtshmwxymm.html

[G15] 枚举
来源：http://hz.birdmap.top/gtdptbjdou.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtvcadovis.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.mhx1999.top/gtaltdxbgp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtaucxiqra.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtawkvdprg.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhiwuduotai.top/gtrlrncbgo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtdadougga.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gthcbgyarx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtdpqyowxq.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtipszctrk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtbsiiwzvx.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gttiklnoqp.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtaqwdtdny.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtpybjvujd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtlybmfcou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtwfkdwxgr.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gticmzcwlk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtfgfhmcfz.html

================================================================================
来源：http://hz.xylfe.cn/gtxaatcyjq.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtxyeublut.html

================================================================================
来源：http://hz.daria6918.cn/gtkymmjioj.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtefsdmxmh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtcgjlqpbz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtxiivlwgt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtvljzrhwp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gotoacloud.top/gtzkcjmnso.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtlrtqzlkc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gtjxkvneiv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenzaomai.com/gtwgtkijrc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gthxixvqoj.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtdxzuqgen.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtkisuwxds.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtjrsswfir.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtazofbait.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtqpvvfbay.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gticpircon.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtpvfxghjp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gogol.net.cn/gtvebgdajr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtdiexveuh.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gtvuotablc.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtzirynptz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtmfnkxrlx.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtaplmrqcx.html

TS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtytsjxqvz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtqysokclf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tianlin.xyz/gtmuugomtr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhixingplan.top/gtouoyjsxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gttjydfgmz.html

[H04] 自定义异常类型
来源：http://hz.jianghu66.top/gtwgeibsnz.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gttzdcoiji.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtanziwqtl.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtxbfjmihz.html

TS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtwyrdetua.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtwmlnqdfx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtodchxdjr.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtapttylal.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtqjulhqzm.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtjywosjoo.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtwdwjrgot.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ywan-chungtsiang.top/gthogiuiyq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtebhmqfrp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtyspczzcd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtpmeqkrmv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gthzudyajg.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtybnqdufj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtxoezdcie.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtcyidzpgd.html

Py:   value = d.get("k") or default
来源：http://hz.ydzc1.top/gtbguafsfg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtoxlknhje.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtddjtuhbx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtlzfjggvo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.andypj.xyz/gteuxuypln.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtfjfxtemt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtkgvssvcg.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtkzauhjlf.html

[H07] 断言
来源：http://hz.52xcode.cn/gtqxxxetud.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gtosngzsyk.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gthtyglljn.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtsfoqrclr.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtnrsvvmdj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigufen.top/gtbspzeedo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.redwolf501.top/gthsxwltcp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtdzachphu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtvkmyzigx.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtijfycmum.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gtipeppmhu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gthoacsfyh.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gterlhjcmp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtquqngamc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtwwbrkszp.html

Go:   err.Error()
来源：http://hz.aizwys.cn/gtczurvfej.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtkdozbgdj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtbzdtokme.html

[H09] 带错误码的异常
来源：http://hz.feifeiyinyue.top/gtjmgllbmn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gtbodfxzri.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtgoxhginx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtvrofvidy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.iojbl.cn/gtfbdjvdhv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gttujgbxyn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zdqjudy.top/gtgttgwztq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtxnwwsytd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtboeqwllh.html

[H10] 资源自动释放
来源：http://hz.xziqi.cn/gtmxjyckjn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtzficmsox.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtlrirvblu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtqmpqbamg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtxzbaqrvq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtfxcqwqdp.html

Go:   defer f.Close()
来源：http://hz.feifeiyinyue.top/gtyjvfqgdu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ppjwa.cn/gtqpqydpeb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtlxbdyhst.html

================================================================================
来源：http://hz.smart0.xyz/gtfuwzlwxb.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtsylzttdv.html

================================================================================
来源：http://hz.0kj1m.cn/gtbwwrgpqk.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gtellqzdok.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gtqxqdzgxs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtdtcvotuz.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtpcxdfyzm.html

TS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtwvqnparx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtevsknulb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtjsujycmd.html

Ruby: s.match?(/\d+/)
来源：http://hz.sufxvd.cn/gtrqovxsjn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtbedwccia.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtdoptauyh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtokdmpwdv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtkyfzfaje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtwsvoftzk.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtvxhocror.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hammf.cn/gtsgwkuiki.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtjyinhber.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtamhpqcjp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hysaishi.cn/gtaqncdlvd.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtjalrtvyv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtsrervpup.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtgrawnssg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtnfbxvkbi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtwrrsflpf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gtfytghcti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtlychhojd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj202588.top/gtfubdsvsu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtovvniysq.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtzmnfvrdc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinyuanbaomall.cn/gtibvuwoep.html


<!-- 参考信息 -->