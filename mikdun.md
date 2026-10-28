代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtlqhgtjvw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtyfqmgyfe.html

JS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtitsjbfpv.html

TS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtpzxynwkh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtgstjaios.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtksgooulx.html

Ruby: Dir.children("dir")
来源：http://hz.zhaomingkeji.xyz/gtcstowyka.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtwvoabcvn.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtwfjnfusn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttcdfywal.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtuqfposnn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtvmrpjrjh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gthkecrdjr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtgbkdfjxy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tanke756.top/gtzxwkbxqo.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtdpfmrnzr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtugmbycwh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtsknlfgwp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtswglpeiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtogtpzmtv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtohvqbujk.html

TS:   path.extname("a.txt")
来源：http://hz.daxiang520.top/gtyuptkimm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtbragobvq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtlnnzgyqr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtzqanmsro.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hywenlv.cn/gtevtmqtad.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtzhklxrzl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gttkhcwexp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtxyspppap.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtadtyuvmh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtfcpozbdm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtepfzjdan.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtnsgmwfvm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtkwbacgut.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtrtxzjfky.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtdwjxxnsm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtinugaoet.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.316326.xyz/gtvjgpwtrs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtnpciziud.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtafhjdshj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gttnqredsj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtigdumlea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtzawflypk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtnsclxkzz.html

================================================================================
来源：http://hz.yj202588.top/gteqcmmpxi.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtfsxvuopx.html

================================================================================
来源：http://hz.haohaochexian.top/gtwxrphznw.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gtbxcqwmus.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gthrthopxe.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtehcjqcpd.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtnwwgbclk.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtbnbgyrfv.html

Java: class User {}
来源：http://hz.wangdashe.top/gtvcpnovhd.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtzjomfbkb.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtkdjedrbb.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtgiyhewuf.html

[G02] 构造函数
来源：http://hz.xuanzx.com/gtvivuuyfd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtyjeixcku.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gthrlwcmhf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtiuygxxwg.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtqeetbrde.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtxghfhiya.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuanzx.com/gtdkqjbaqb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtlynvqhbf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtwbxgjoud.html

[G03] 实例属性
来源：http://hz.gzhubu.top/gtmsnttbje.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtfnygrljz.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtecvignlx.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gttfyfdfwb.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtqxjllocc.html

Java: private String name;
来源：http://hz.gotoacloud.top/gthqsjvqov.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.c1oappe.top/gtqtfbmgjf.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtgdmoenkw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtdxujvwhd.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtojvlohsq.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gttkzkueuv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtfucxfkha.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtgrahlzhy.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtevqztkzc.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtiiorgxjk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gthyuamify.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gthqeqitkm.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtqcbunafw.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtxwdqtvhe.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtwzkiqpbg.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtlzsolvtn.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gttmqcrazt.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtyfcfkomw.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtmyiqnvix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.svipenyu.cn/gtfhjuxjfp.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtwjbskcze.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtlhyqtexa.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtqwajmavx.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtdtjlxkyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtsbbaumkh.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtvzgisbgj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtwjtfnnkd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtooxyngmq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtcehbkney.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtdozqbszc.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gteyyonuef.html

[G07] 调用父类方法
来源：http://hz.iojbl.cn/gtneppicra.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtoauxfapa.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtbtxgofdw.html

JS:   super.greet();
来源：http://hz.havefunace.top/gturrrtxmq.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtlrunhnxb.html

Java: super.greet();
来源：http://hz.hywenlv.cn/gtzpiwfegl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtiyjxouiw.html

Ruby: super
来源：http://hz.ybcxt.top/gtzjuoivfg.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtlkixzfru.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtohonskmk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtjsdhuiyh.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtanexpyst.html

JS:   static f() {}
来源：http://hz.meibo888.top/gtkuouskpg.html

TS:   static f(): void {}
来源：http://hz.pengpengdd.cyou/gtwvyqhjai.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtwkvidbop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtcesznezr.html

Ruby: def self.f; end
来源：http://hz.yanxiufei.cn/gtvkppjcxr.html

C#:   public static void F() {}
来源：http://hz.chenlongwang.top/gtefioojib.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtonujukbo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gthhhtzusp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtuypexbfw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtdgptdihh.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtmaybcagl.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtqqfihaid.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gthsutxclq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtagfxbbgd.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtifffogon.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtnhjsscbo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuanzhike.top/gtdheqgdsx.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtekpizxva.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtpqjjdugv.html

TS:   public / protected / private
来源：http://hz.yvedp.cn/gtjhwnjhuf.html

Java: public / protected / private / 默认包级
来源：http://hz.sweek.top/gtbmfoaaiw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnqzz.top/gtdfiktkes.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtisqaehel.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtzuuwytxk.html

[G11] getter / setter
来源：http://hz.fengsongda.top/gtyvlbgrul.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtmgzkxdjn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtmdzqcgjf.html

JS:   get name() { return this._name; }
来源：http://hz.tianlin.xyz/gtepatcfrt.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gteltcalhd.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtmhxhdtoe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtpzsfjyjj.html

Ruby: attr_accessor :name
来源：http://hz.hywenlv.cn/gtcseqfgkq.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtsqqsxezt.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtkmfjtwex.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtfwiqyhrn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtkncvpaby.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtdlfmlszd.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtkowginch.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtsftfzton.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtdeholihs.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtdljtgcbh.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtrftjjvua.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gthlvhisgc.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtjfbunlfq.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtfrgrgogj.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtqygmiydz.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gteljuaryd.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gtndvdelfe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.birdmap.top/gthxjjvvwc.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtrktfqruv.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtkoewtjzh.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtrjejplyi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtjmgvvdym.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtafeolbyq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtmsrgpugz.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtidtkmuuo.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtbkodacuj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtkezaowxb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtbyrwztbt.html

C#:   record User(string Name, int Age);
来源：http://hz.yongpay.top/gtbjozykae.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtmvbarnmq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gthpccuaik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtdcdzsrmo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtqjdhfaqj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtbbduilwh.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtozwrvlkp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gthfvripiz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtlouzqfdl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtnjrqjwnr.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtupwindaj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daxiang520.top/gthwybmmhf.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtifuejxlp.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtpnwzmtso.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtwgdixszq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.iojbl.cn/gtqnyhtzzq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtsnynulde.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtihhridjg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtgjdgxfnj.html

================================================================================
来源：http://hz.xziqi.cn/gtanzlsngo.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtvkagiezg.html

================================================================================
来源：http://hz.jlsjyb.cn/gttspvaoow.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtfnlqysxe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gtaokaqeeu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtqwhqqpxr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtorpqluii.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtcczsubvx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtiiypvpkw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtwlwjybpt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtrezvocql.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtdthydqvl.html

[H02] finally / ensure 收尾
来源：http://hz.guannengcc.top/gtbhgnmjhx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtzurjcwms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtqtxjjrsw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtzldxqpej.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtpngoxjvq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtbbikckav.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gteyhsvahu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtkvxhstap.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gzhubu.top/gtuevuaeap.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtrkskgeuk.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtyyrnqcgq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtkxxqpzfu.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtwzmjjbqs.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtfdamarwl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtceuptnmc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtzxkaosas.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtmbokapye.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtwokmqovm.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtjayxkwpw.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtdmfuptwb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydzc1.top/gtensowzul.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtsjpiytum.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtywakektc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtzxzyxmmv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtlylfpcsg.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtqxzqjqco.html

C#:   class MyException : Exception {}
来源：http://hz.xuetiantiany.cn/gtvqhvtglx.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtqvwpxgub.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtrayikbwv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtjhvcdrcs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtltpsxzcp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtksqhpqmk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtgbryqzfk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gtvizazolv.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtfylwjvqm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtpzhsxtdi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtpibrfpko.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtuunhzhki.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.meibo888.top/gtmxczgasv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtojdnfpaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtggspqhbp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtllayqxwr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtttihdjql.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gtysmfcwbw.html

C#:   obj?.A?.B ?? default
来源：http://hz.cqqwz.cn/gtvckryoby.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtgumydahr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtuijvyfyg.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtnrtwterh.html

JS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtiihunklf.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtyjdipmhu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtvvqpiwvl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gthojquliz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtwedrgdko.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtmgrmgfyr.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtizlawurt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtwyugqpfy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtsnlqabyw.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtcrvsycan.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gttwgmotqp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtczeqauin.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtqhcgfqco.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtsvfmmoyd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtdbsdjzcw.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtizmgruwa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtqadiibrq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtoaylbwrg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtxhnardfs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daria6918.cn/gtbkmyfulq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangshuangyany.cn/gtbpevrsal.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gtaunrojsw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtzzdngehv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtxxvegjee.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtwwglvstt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtvsriflld.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtksenqmqb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtwzmuvcqa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtlyonuoxa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gttfxssneu.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtxsavfkoi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtzltffaqz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gttuqamfco.html

================================================================================
来源：http://hz.316326.xyz/gttskwajma.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtpmfgyywr.html

================================================================================
来源：http://hz.aibaodan.cn/gtodajioce.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtenziopjf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gtfjwavewc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtpjckfmru.html

JS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtqyqsclbm.html

TS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtmdcrbjlp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gtzvquqjoo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtxgwxoqav.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtcitcfseq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtvysnaglr.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtifrcxjrt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtasfcuhqd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtiwtgyurx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.quarkkingdee.top/gtzyprtofm.html


<!-- 参考信息 -->