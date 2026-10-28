代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.meibo888.top/gtypltesmf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtlpnpepwq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtryrrcoek.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtkxkmvvzq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtdpnffust.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtfdomiigc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gthfdvcwjl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtclcxwaxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtsidwoifh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtmmeluuos.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtgysrdhoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtjradbivk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtvlbntylt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtltwonlhb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtkwhqevlr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtudepvexz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtknlahwng.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gthqmcaleu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtvvntgbis.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtionreveh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtwjckfsoi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtwwmcwfjx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gtfbyunbbf.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtcidgoytk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtqbmpzvbz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtfpojpngd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtzrkcgzgy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtqpqqjmns.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlvhguvqr.html

G. 面向对象
来源：http://hz.sysykeji.top/gtyyazsqkn.html

================================================================================
来源：http://hz.pycfn.com/gtpwzjgzis.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtvbyopryu.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtgihllnvi.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtnswqfxma.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtivopjaiv.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtthxusmwl.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtxhwsrose.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtlctryaaq.html

Ruby: class User; end
来源：http://hz.zhaomingkeji.xyz/gtlaxglxtt.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtqlsquacr.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtgojpuyam.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtifchzmbv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtplrgsqdd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yueranfly.top/gtdvxivhun.html

TS:   constructor(public name: string) {}
来源：http://hz.chenjidiqi.icu/gtqexalftg.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gthnoaedid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhaomingkeji.xyz/gtrzxugpfp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtxwsvymtu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtpjjyhjfe.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtenbstozp.html

Py:   self.name = "x"
来源：http://hz.cucudq.cn/gtpkpujqni.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtdotiicce.html

JS:   this.name = "x";
来源：http://hz.sufxvd.cn/gtqkmvwatm.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtuzacdsvy.html

Java: private String name;
来源：http://hz.cashguo.top/gtsjunnrdn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtoxythwne.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtqcygrtvc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ppjwa.cn/gtzagwdwhc.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtjmsbmooy.html

Py:   def greet(self): return self.name
来源：http://hz.jqgfzy.top/gtcrlplwlb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtphhtqchx.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtfoahokyk.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtqbftwcwc.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtmmjwzipu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gtwpygwqzb.html

Ruby: def greet; @name; end
来源：http://hz.yj20258888.top/gtbdfxdafe.html

C#:   public string Greet() => Name;
来源：http://hz.birdmap.top/gtskkyffdu.html

[G05] 继承
来源：http://hz.andypj.xyz/gthdsisvtl.html

Py:   class Admin(User): pass
来源：http://hz.yangfankeji.com/gtahvyrnec.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtxajmngwf.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtgkupioqg.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtzwjcuroq.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtjsfatlwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.meibo888.top/gtmagmdguc.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtifkgcfxk.html

C#:   class Admin : User {}
来源：http://hz.tanke756.top/gtnirltsvz.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtlfyfsezv.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtthpdnobb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtgrgkhokj.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtbyagezsy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtjrpjhdwd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtkleomazx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sufxvd.cn/gteuswowzz.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtjvmduvlo.html

C#:   public override string Greet() => "admin";
来源：http://hz.sweek.top/gtowvptcwe.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtpsufedev.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtrebnlfum.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtjaqwcqvp.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtjxgpjrpk.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtkiiuobpb.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtwemhzuyu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shangyingyoupin.top/gtwypjzqki.html

Ruby: super
来源：http://hz.vqdsnc.cn/gtxvnrwtdi.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtywaejikr.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtieimottf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gthoebifxp.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gthrbnnmrx.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtbmipobcw.html

TS:   static f(): void {}
来源：http://hz.xziqi.cn/gtvpsefkai.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtbwpzuzmj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtvaorbsog.html

Ruby: def self.f; end
来源：http://hz.hnqzz.top/gtjianfwvq.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtmepwcokl.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gtpaogqnxs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtjiuwfkjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtwgfitqea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtpebclfwt.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gtoliypntp.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtguibsamc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gttdewydzb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtuapeombq.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtdnkognxj.html

[G10] 访问控制
来源：http://hz.cheryme.top/gtjdynmiiw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtubztlaiz.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtbopzyxjm.html

JS:   #private 字段；其余公开
来源：http://hz.52xcode.cn/gtueksyzgz.html

TS:   public / protected / private
来源：http://hz.sufxvd.cn/gticpxxapx.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtrbwocicb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dashuyun.cn/gteykracpb.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtdejmmkcl.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gtzaxrpfez.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtgraqajhs.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtmxrgfqpp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtdlnglmdu.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtgxmvztex.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gttqwnsgjo.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtgvovyejd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtkzsihmlm.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtmuqcovsd.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtjcehxyek.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtaquapyxu.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtraiogdea.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtxfldotiw.html

JS:   toString() { return this.name; }
来源：http://hz.yuxming.cn/gtsdhnccht.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtvernlysb.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtgxwwfnyo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtsfzmjphx.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtsyxqbiqq.html

C#:   public override string ToString() => Name;
来源：http://hz.9152youxi.cn/gtenvkfwri.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gticarctes.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtesdifryt.html

PHP:  $u instanceof User
来源：http://hz.meibo888.top/gtbuqvupcz.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtyhendvjd.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtxzczvoha.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gtxfqflhwh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtibbhnxob.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtffmvqybr.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtkzbtrysq.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtdbjljwdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtyfpoqgfx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtyuxxbhsj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtkdrwrboh.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gtekxppqld.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtjkqgxzwu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtxypcrvkf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtmoacwfyr.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtzldflimw.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtbtjbrwmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ywan-chungtsiang.top/gtwzaxffyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtptnwddkx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtutxckycl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gthakzoyji.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtqlltvrsi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtdzaljiwg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtpkfjqucy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtbxkpjiuo.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtfscedszd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtlabptwut.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtlnfamgcu.html

JS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtvlufmqwh.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtxccoenrj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cheryme.top/gtgnoaxdlz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtposdxrhn.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtlcumsdjq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtbfrvoyjz.html

================================================================================
来源：http://hz.zdqjudy.top/gtcwwiynfe.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtgxskrbds.html

================================================================================
来源：http://hz.zhixingplan.top/gtuedaslbh.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtbhlmggpi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtaajdbvgs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtlytzlfvm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtqrlgqhvy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtjvcswydz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtfyxunbxy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtnbggdicz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtshovkkzd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fengsongda.top/gttvpsjzvb.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gttjdleyqz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtepnstwib.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtrjjvhjng.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtjgnrnclc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtoyusjkzb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtxmesngtg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtaitwqwee.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtdhgrwsck.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtxtjrjiow.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtwzmklykr.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtitxqscly.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtmteuiwam.html

JS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtaohkdbvv.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtcvistgxe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtkwgzjzcb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gttexbxprk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gthffidfzf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtfgpwxbkz.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtacknczvv.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtzonbrdsq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtolwcpdqt.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtvmxwsgwc.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gttwthrhyq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtssyivbtn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtwmjcndkb.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gttlzyxtlr.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtcbavahys.html

[H05] 捕获特定类型
来源：http://hz.daxiang520.top/gtajcqehwi.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtwigodtxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenjidiqi.icu/gtwztuoyfs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtjyvqmdvw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtylcfiflx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtqbylwrtq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gtgifqzcyo.html

Ruby: rescue ArgumentError => e
来源：http://hz.ppjwa.cn/gtpnfvehjk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtehvpedqr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtdvaykcgo.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtzbaxvhlg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtuvlernam.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtpppxxhzu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtkwtwacmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtihensoxq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gtdrnhbcqc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtmalqlfaa.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtihvlrvxf.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtkscclgep.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtllthupvf.html

PHP:  assert($x > 0);
来源：http://hz.zhiwuduotai.top/gtllabumix.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtueiyyrfu.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtfuoyfnqx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtqvvfopsy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtzdngqdah.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtmsnewnbz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtscozmgsv.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtjgvinnlf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtdbuqthhr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhongyouzk.top/gtjhwrgehe.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtiepndwaw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtybgcoegf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtrzvhxbff.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtxpdwtbry.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtiluobrsh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtkjcaoqap.html

[H09] 带错误码的异常
来源：http://hz.9152youxi.cn/gtrfdwkvss.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtbbvjbdvb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cheryme.top/gtnvvqryct.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtgyilehdh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gtbfijmezd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtbpknsway.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenlongwang.top/gtfwfjkpbu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtevoagekb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtzzehksbg.html

[H10] 资源自动释放
来源：http://hz.ydjk.org.cn/gtdfgwfshn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gthvjxwlop.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtjmtqdybl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtugmczung.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtpsbsjprj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtpqgbunrg.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtvargiaeq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenlongwang.top/gtyktxsfdf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.redwolf501.top/gtrmqsagxl.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtndbawrnl.html

I. 正则表达式
来源：http://hz.yueranfly.top/gtiqpjcmfp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtswstaslz.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtmryveobm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtspjsjcbs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtbahiclkx.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtgxwjexbp.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gteioccejh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gtomhppvoj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtjpfemigv.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtjyoqxnij.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtaeuaimlf.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gttoskprsm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtegobxyuv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gthajvlmma.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gtsjlpqdwa.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtydjrialb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtsgevqvue.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gtsecjgdfj.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtdzsckvjo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gtjummcycy.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtpdjywyen.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtyupwtqyr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dianchejie.cn/gtydsiiiwn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtswyotate.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtuckvlmwu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gteuyovole.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tianlin.xyz/gtciebqqwr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtrpryyroh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gthetbsxvj.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtxewsuxec.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtgimyrmvc.html


<!-- 参考信息 -->