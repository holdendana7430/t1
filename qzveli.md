代发 wailian999

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtwavbtuwt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtpinlerkj.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtyhaedsir.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtypjdvkfa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtocpkdsdd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gttguugbyn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtsxmcwscp.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtolbtgzib.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hywenlv.cn/gtdcynqszl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xziqi.cn/gtfssyuhtz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtzoflpbbg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtciqjgipp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtgjuamkzj.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtzjhsecya.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtflgfwyje.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtoowwbitk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtasscfxem.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtljyokkmq.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtonkxcjtl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtemlqpwts.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtjyewjqde.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtuufzuolh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtqrnerpsw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtbpotgevg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gtkeicopta.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtsfpvsrmc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtbwvsxxep.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtbelbxvic.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtlrdytnhp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtyvotjbfp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtwlgtwffa.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtazbgzwup.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtcdhyzqwe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yvedp.cn/gtewybfxzy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gthslcmhnb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtonngxqhy.html

================================================================================
来源：http://hz.yonumen.top/gtmpwlupnz.html

G. 面向对象
来源：http://hz.zycfv.cn/gtyqhlfioo.html

================================================================================
来源：http://hz.haohaochexian.top/gtyvsxzxgj.html

[G01] 定义类
来源：http://hz.snrcjt.cn/gtpvpdumkv.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gthriolbxs.html

PHP:  class User {}
来源：http://hz.tian-w.cn/gtbmlzglmx.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtmctgkkhn.html

TS:   class User { name: string = ""; }
来源：http://hz.ppjwa.cn/gtfgtdxxkf.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtixfssjkx.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gthhlhnrpm.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtxhqjtkcz.html

C#:   class User {}
来源：http://hz.havefunace.top/gtdjgiemsv.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtuftukqyu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtpeoiewzd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtyrsztger.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtkjmhkmkm.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtrnxikidf.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtcdkpoawt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gtlcqisich.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.andypj.xyz/gtorzgpakw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtkxckwhqz.html

[G03] 实例属性
来源：http://hz.yuxming.cn/gtwrvqawkw.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtxzkhdphy.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtjfpkeohg.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gticndjtek.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtvnwxorru.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtydkpdymv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gtfwedgvxa.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gthevshplv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtldsdptan.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtdiuzjbmi.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtnrmaudbz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtoyrlmgkk.html

JS:   greet() { return this.name; }
来源：http://hz.cdnleiting.top/gtdvnazylx.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtoqvhwhve.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gttmonxafc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtdcyopxov.html

Ruby: def greet; @name; end
来源：http://hz.gotoacloud.top/gtpabcuiop.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtkfbthdhj.html

[G05] 继承
来源：http://hz.c1oappe.top/gtipwxecen.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtycavsalj.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtmtvhmdtk.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtvitgemhe.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtbzbuwsum.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtirvkxvil.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtmmlmeebu.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtzevorkvc.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtyhigusrb.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtnqnmsyat.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtlfuvwgso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtsvlxcbwe.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtihihbdqw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtsqcmople.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtioowcqhu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtvmpuladf.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtfxbmsxwl.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhaomingkeji.xyz/gthoomrwzj.html

[G07] 调用父类方法
来源：http://hz.jyoumei.cn/gtdegpzwxe.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtarjezkvi.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gtbbogfnnq.html

JS:   super.greet();
来源：http://hz.ivvv.top/gtyoiawwow.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtrennjirr.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtgphftpfd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtkjseouwp.html

Ruby: super
来源：http://hz.yuxming.cn/gtvvsfhqcm.html

C#:   base.Greet();
来源：http://hz.shuidangran.top/gtaxzqpryd.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtbyfuwmyz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtnezsumcw.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtbbvpzkmt.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtogsaihtw.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtzdwmitkg.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtgjhnkool.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtfbwutxxx.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtzxqurrcm.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtfxpghvkp.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtffnukgeg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtkbwhuvbb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gtfssztuuf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtdebuabnn.html

TS:   interface Shape { area(): number; }
来源：http://hz.jianghu66.top/gtmnadgmje.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtkkctwcqn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtiwtzaska.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtltllpnhs.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtozuaykqk.html

[G10] 访问控制
来源：http://hz.chenjidiqi.icu/gtpjzoxgqc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtschtnanl.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtmfmbmniu.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gtumdggand.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtzxcklrto.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtvumaqtoy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtdtpztxyf.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtdhnozcxs.html

C#:   public / protected / private / internal
来源：http://hz.chenzaomai.com/gtmovxkmhr.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtbrjjtviq.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtvsdvleex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtipjmcsnf.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtaexscgwv.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtjcdhffmp.html

Java: public String getName() { return name; }
来源：http://hz.jyoumei.cn/gtolthkvpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtlhqjmrhz.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gteikunfyj.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtabguhwpw.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtdijtcxru.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtpuhdkxox.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtgwspngmq.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtiluiesqn.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtgnucuyzc.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhoulong.xyz/gtcnkucias.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtgdracggj.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtbcjvysbv.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtyobnkmnz.html

[G13] 判断对象类型
来源：http://hz.ppjwa.cn/gtjmealuvt.html

Py:   isinstance(u, User)
来源：http://hz.daria6918.cn/gtkolmapvx.html

PHP:  $u instanceof User
来源：http://hz.cqqwz.cn/gtrwwubbtk.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtgcrcvkkw.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtgiqjqvsc.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gttyfphcud.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtbprbwqav.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtkgntwrrq.html

C#:   u is User
来源：http://hz.daria6918.cn/gtmwfvwdbu.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtjjxveccz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtdifuffzo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hammf.cn/gtbbgnqjxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gteletqkle.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtpsxvtpfe.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtoaokqrps.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sufxvd.cn/gtevwovtvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtraedycvx.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtegrwnewn.html

[G15] 枚举
来源：http://hz.jinqigfzy.top/gtizeksnft.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtovcvgnuv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtkhkxyvzb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtwitwrzhu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtswpppsks.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtohjnqtsr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtvorcqlxt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtjknwjyzq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtftgiscce.html

[G16] 对象转数组 / 字典
来源：http://hz.hnqzz.top/gtsahocqjt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aizwys.cn/gtnenlpriq.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gttjspaddl.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gttkmujbpa.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtbezmries.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gthoejiwel.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtacnzggpp.html

Ruby: obj.instance_variables
来源：http://hz.ydjk.org.cn/gtowgfjdnl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj202588.top/gtoitwjhsh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtakkjzfjx.html

H. 异常与错误处理
来源：http://hz.sysykeji.top/gteefqdkxo.html

================================================================================
来源：http://hz.yuanzhike.top/gtbxzajcmb.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtzrpspvkh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtojuzoknd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtarjfxfjv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtlmpwhsou.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtrvznrmks.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gthtxhzvzj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gtjsdiqmuu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtmfrlvcti.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtwzwyjrfj.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gtzmqtkqsp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuetiantiany.cn/gtsxtwlsrq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtxcfwwawo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtcjjteqmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtklagpmer.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gthogboewr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtccnodkly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtcdyrjzpj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtzvsccedo.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtsruhrppa.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydjk.org.cn/gtulwqlmzz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtmvcomkzq.html

JS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gttgsdheqh.html

TS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtknusxowu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtniovqwfq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtishswlev.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hfpthk.cn/gtcwpedhiu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtptbpbcfq.html

[H04] 自定义异常类型
来源：http://hz.jyoumei.cn/gteldtbkhp.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtocwrhxuf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.iojbl.cn/gtauwuhxho.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtsfdpbnyc.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtoaldmdxo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtulgsoihv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gttftmpqju.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtoejffrcd.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtwtptudvp.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gtrocslmkc.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtounoixyp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtzowarqoq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtlaggimfb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtrgbdahox.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fzhhl.top/gtgigledtp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtsedgboea.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtwuzekjmw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtlkxeqmyh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtvgjpezhx.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtuvqksyoc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gtttofoezz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtjqurkzfv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtfwxkwisx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gtsrpsstpu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtmldryink.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtjphmznkf.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gteilxxlpj.html

[H07] 断言
来源：http://hz.guannengcc.top/gtnfrnamvq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtyqmfmplm.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtbtzuwacq.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtkccnnoiy.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtvbkpferl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtxgnstdhn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtdunsxycm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtzwjurodr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtlzcmnubr.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtghfgkuyp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gtmuucrtwr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gteehluzxv.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtfuzfytlk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtfypjqgkp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtqsrwpuqu.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtzaxmqdhe.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtwmbgqzvl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtvxcvexyw.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtunljeezq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtgblaxvgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtxqsaboha.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtkbvfbojh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtrwatizbk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtngaxqxtm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtyqihajyc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtgjutnmpd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtdmnmszym.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtfbgbyqzg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xingfuxueyuan.xyz/gtgdbsldqi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shuidangran.top/gtjqoajmmj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtwndgzrmm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtvegtitdm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.9152youxi.cn/gttslmbajr.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtabcwwbcz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtbheslocc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hysaishi.cn/gtjaalcltk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtftbescgn.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtidrkhrti.html

================================================================================
来源：http://hz.yuanzhike.top/gterbocdls.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtghufuutz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtbcxzevhr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtefmlaojh.html

JS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtxchkszju.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtorwaddly.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuxming.cn/gtoztdktyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtmxqejffk.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gteymktdjk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhijiandao.cn/gtipqswwfv.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtneirxghr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtzliavwpr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xingfuxueyuan.xyz/gtbuuzmukk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtqefbopfm.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtrbbmdpbk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtsjuwhyek.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtzspchkle.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtsohomlum.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtstzaxcor.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtfelrctmn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtqxippkrd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtleqrqhkr.html


<!-- 参考信息 -->