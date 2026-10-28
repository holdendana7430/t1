代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gthlwxinut.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtqvjvjeby.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gtqxbxdasv.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtkbbhajnu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shangyingyoupin.top/gtunpfghdw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sxryk.cn/gtqxtpabzo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtpelpgeod.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gteckhbqdy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtkucvnyyn.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtnrrumrow.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yanxiufei.cn/gtguhawqyr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtfxsajepp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtwjqljyid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gtdpksdlzc.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtqkiffpww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtxgjlruxv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtxgqmlqbv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtgoafdfwi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtecjgzvgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtpwatwtar.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtfknohmgi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtonvxsjyw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtpgzulfpc.html

[F12] CSV 读写
来源：http://hz.pengpengdd.cyou/gtglxlpcka.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jiagoushi.top/gtpjpklfwf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtamhsgqgv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtjxbbjxtb.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtywwvwbdq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtjvhtrcwv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cucudq.cn/gthqtldikj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gtwpplffhf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtlvmfwogv.html

================================================================================
来源：http://hz.zhixingplan.top/gtogxvfuwt.html

G. 面向对象
来源：http://hz.mhx1999.top/gtgkwlskjt.html

================================================================================
来源：http://hz.ehwqpu.com/gtopzkkgvc.html

[G01] 定义类
来源：http://hz.shangyingyoupin.top/gtcgtrvqxn.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtaqshwlie.html

PHP:  class User {}
来源：http://hz.yj202588.top/gtympxzgyw.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtszcokvah.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtyldovdys.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtcowealqk.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtjjaopyfv.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtwmegwcfp.html

C#:   class User {}
来源：http://hz.chenjidiqi.icu/gtlxclzwmo.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtzqkmauhi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtrdrmfvsr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gthhkeoqzt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hammf.cn/gtvthohmgu.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gthpiazacc.html

Java: User(String name) { this.name = name; }
来源：http://hz.bjfxy.top/gteotmldvi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtsuhbqmba.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gtfrjpgoea.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtvmxigzsd.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtnvhkuddl.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtusihgvwo.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gthcxezkci.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtvttsunpx.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtwwlbzhrn.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtioxbxeqd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtxfzfqqzr.html

Ruby: @name = "x"
来源：http://hz.sysykeji.top/gtsotmxxxe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtfhdogaaj.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtwdqbuwzv.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtwcxgmqbf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtxgzhltzs.html

JS:   greet() { return this.name; }
来源：http://hz.yuxming.cn/gtishevpxo.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtbnffbogr.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtsienilfc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtznkrzvam.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtuiotemdo.html

C#:   public string Greet() => Name;
来源：http://hz.chenjidiqi.icu/gtxovatrqg.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtpdrjnlir.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtwtcpstpq.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gtbaaehomy.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gttksccelr.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtpkpkbnem.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtsnqcubgo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtlsayifuy.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gthzshxjxm.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtyepeytnd.html

[G06] 重写方法
来源：http://hz.nanxuanxn.top/gtdldyghmb.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtzkpnvlzq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtwnmknxkc.html

JS:   greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtfxsbmjwx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtmmrpegsa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtnrvsniut.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydjk.org.cn/gtzxbthjtf.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtlntmzixh.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtiwfiviyr.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gtblxjxpml.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtcrrvymam.html

PHP:  parent::greet();
来源：http://hz.shzxlz.cn/gtoqsshefb.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gttefaxtjn.html

TS:   super.greet();
来源：http://hz.yongpay.top/gtkwdqozfo.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gttkjwwdmb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtohlbkycf.html

Ruby: super
来源：http://hz.gotoacloud.top/gtyhbcaczy.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtykyltcgx.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtnffcpgwz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258.top/gtteajhahr.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtldxgtbmd.html

JS:   static f() {}
来源：http://hz.mhx1999.top/gtmavtnimv.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtckvxogjp.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtxgqpgdll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guannengcc.top/gttxqmjzea.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtmcctmzqe.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gtlxdeomud.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtgkpiyehp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtxrwgfrxl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.smart0.xyz/gteqwlxoys.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hfpthk.cn/gtxqnqtomm.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gtnnejcjye.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtavmcqpxl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtdjzmpfqn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtzdjqpnfe.html

C#:   interface IShape { double Area(); }
来源：http://hz.shzxlz.cn/gtiixrkkoe.html

[G10] 访问控制
来源：http://hz.cqqwz.cn/gtcvyeoncr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtbxeuxgyz.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtyimdewmf.html

JS:   #private 字段；其余公开
来源：http://hz.yongpay.top/gtyesevzvm.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtndkgpuxo.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtvgbwzwoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtadmtnaqb.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtitvtjovk.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtafhbjtjq.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtaheqyxvd.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtsjubiznf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtatjcusfm.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gthdtkzopl.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtcklmctlp.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtozxhuiou.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtpjiucpbe.html

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtgjenvhpw.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtapmooufl.html

[G12] 对象转字符串
来源：http://hz.haohaochexian.top/gtcpektmtl.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtqmvtezjr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gttwgfkstd.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtxtmuwikd.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtcvyatsoc.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtknvydpgt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtclvmhvmj.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gtefpyasgi.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtquimrquv.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtiniefqpp.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtcbhntkgn.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtpaycrvyc.html

JS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtpervgfdj.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtwzxgmpbd.html

Java: u instanceof User
来源：http://hz.c1oappe.top/gtdefbvxvk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtzosnghap.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gtmlmwcqaw.html

C#:   u is User
来源：http://hz.xuanzx.com/gtsydxbcbh.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtjyfsjpsk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtmurqeppz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtloteaohy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtapqharqi.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtxlaodban.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtildnsbne.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gthnququry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ywan-chungtsiang.top/gtiaukiatl.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gttkrgdelw.html

[G15] 枚举
来源：http://hz.yonumen.top/gtdykxccez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xziqi.cn/gtzganqgvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtgccfnvrn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gtguhxljaz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtdjpsopze.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtszkxipxc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtlvnokqgj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangtech.top/gtkudnrrhk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtunlluxpa.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtikxqvmkn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtkxtpmlmp.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtnvzeobqi.html

JS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtirjwjjbj.html

TS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtaemdcqhr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtywdzcmom.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtgqlvgipf.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtfrbbsaym.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtdmnjxrva.html

================================================================================
来源：http://hz.yanxiufei.cn/gtamoopryd.html

H. 异常与错误处理
来源：http://hz.chenlongwang.top/gtbiljzhzp.html

================================================================================
来源：http://hz.chenzaomai.com/gtiusyewwr.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtebdjsfrh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtijmbkdaj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtmwhplrst.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gttmtynemp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtsqmdmxtl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtbgntvbku.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtlnuughbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtgqkdnusj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtgaztfhcu.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtnnxfxmeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gteilntpnc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtzjtwgwck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtejtxyema.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtkypdvkbs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtirgvrdsv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtqqvqyyjj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtquktegil.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gthnheeefw.html

[H03] 主动抛出异常
来源：http://hz.316326.xyz/gtufggxnpu.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gthwyrxhhg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtohclcfbj.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtryoxfsby.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtjvlzflwg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtehosgahp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtbrdwkcsk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtpiunziea.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gttzvqpvve.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtarfihsyd.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtdccbxhyl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtzrueplly.html

JS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtulcfoolp.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtnbgggxdz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtdjdikwka.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtiheklegh.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gthvjfybcj.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtlyiomeyy.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gtxudxxqrs.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtwwlalhzx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hnqzz.top/gtmzfvgvah.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtzwhwagyq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtflnjdetq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtbjlfwbfw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtwxtavdhw.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtbxfmllzn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtupkfwiot.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtflknhkee.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtfgyofrut.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtqnoyqiti.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtuxvlooki.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtblqedmbh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtlipkicgb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtwdjirgbl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtzahmpgop.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gttyfdadcm.html

[H07] 断言
来源：http://hz.hnqzz.top/gtembxpxcb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtwnhagoxo.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtardkfurp.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtvbewjthc.html

TS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtqgehvlmr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gttbvbtkkd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhongyouzk.top/gtclovzbmm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj202588.top/gtrxuyoajh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtytfuuzod.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtgtnmsbek.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtplbnyyyj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guannengcc.top/gtxqlhvlzv.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtrrhirqch.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtmzxfbdid.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtxbgrhxea.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtoubmnxfv.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtkmsdtewf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtttnqhwus.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtxevekgkp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtwfsipnji.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yanxiufei.cn/gtyblzrajj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtbyxgjvfy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fengsongda.top/gtesaxxmbj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtwotrspoa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtazvhmoyy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinghuilouyu.cn/gtufnpsoao.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtrvqnzwvv.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtkxemewot.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtcfoecnjf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtdzbuytzs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtovkrgagc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gttrakxlpl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtrnjgctxb.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtdhceaapg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtwajylexk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtylaaipeo.html

================================================================================
来源：http://hz.tian-w.cn/gtcllzkazp.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtaxbpbuvm.html

================================================================================
来源：http://hz.yongpay.top/gtkvckhyud.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtovvbzeab.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtewarupfz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.vqdsnc.cn/gtuukdiokn.html

JS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtxnydbwqj.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtrdvhslio.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtflnbzofr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtzbmmzzev.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtvhfsseqf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtatqwnsgf.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtwmzxtoum.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtsbginqmd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenlongwang.top/gtpenoknah.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtnytinkqf.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtdrwtapeu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtuhsowmov.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shangyingyoupin.top/gthjitzfhl.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtvczqwsia.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtfzbxdhik.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtffvxiwro.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtsnshvcfm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gtpudtyzmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtkpgxbdkk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jlsjyb.cn/gtkicuzeib.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtrxcyvlpr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtmtmhirvr.html


<!-- 参考信息 -->