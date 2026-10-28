代发 wailian999

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gtamwgbqaq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtnkqtmatm.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtohffsrvi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtbyvopryv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtrhqongqv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtbmxivcsa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtijlvrtun.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtjolpgyix.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gthtthxxnn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtbupcaknv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtcazjsoob.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxinkj.top/gtcyzkgnra.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtxsgrajaz.html

TS:   path.extname("a.txt")
来源：http://hz.hysaishi.cn/gtokltoybv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gttrrvtqmw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtubqerwhg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtmszpogab.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtdjfoldes.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtattxqygm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtfjrhqjbc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gzhubu.top/gtpoolmtue.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtgmmdjfbn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtnlnidybh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtslenxjqe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gtshnhznpv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtgmngrdvy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gtxwewedcb.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtrorisnnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtapphdsvr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtafnbhglr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtkxtpdxan.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtksodakfu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gthfvanbtb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtznlkimyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuetiantiany.cn/gtpglxvugu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtwoeyskwb.html

================================================================================
来源：http://hz.ivvv.top/gtdnvqcpwc.html

G. 面向对象
来源：http://hz.jianghu66.top/gtootctztl.html

================================================================================
来源：http://hz.hnxiangtu.top/gtetmgkqbl.html

[G01] 定义类
来源：http://hz.quarkkingdee.top/gtolylthyu.html

Py:   class User: pass
来源：http://hz.316326.xyz/gtkshlarmn.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtfzqgzxca.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtqgkddljq.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gtfwmvgtln.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtssduiuer.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtcxxwnhnz.html

Ruby: class User; end
来源：http://hz.jinqigufen.top/gthpyhpxkj.html

C#:   class User {}
来源：http://hz.havefunace.top/gtarrhrdej.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtoxbqjdqb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtdkimyvbv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtpekthogq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtfgjmeicj.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtzzzeadzm.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtdfwwhetv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.havefunace.top/gtkbfcqmca.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.snrcjt.cn/gtywvcykts.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nwbrower.top/gtzmeitgke.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gthcbqysrn.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtsgeirkoz.html

PHP:  public string $name = "x";
来源：http://hz.nanxinkj.top/gtgdynedzg.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtblhafzzj.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtvnakbjgh.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gteljvnsob.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtqvqbgqwn.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtbngumels.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gthqyxmufr.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gtjrlnemae.html

Py:   def greet(self): return self.name
来源：http://hz.xuetiantiany.cn/gtawwtnpoy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtnkzgnntn.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtigbjlgdc.html

TS:   greet(): string { return this.name; }
来源：http://hz.yueranfly.top/gtpwdczcum.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtznmternn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtjrhiumet.html

Ruby: def greet; @name; end
来源：http://hz.kuanghao11.cn/gtyoisvslo.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gthnvmrdvp.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtyqbfnbtr.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gtjnqjxorh.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtcjsuqobv.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gthdpdvjax.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtidgsikmp.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtsourrroe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtmaxqwjot.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtkjwosytb.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtfaeswlfw.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtubuijbfz.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtnncolsyb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtvqmzkhqb.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtvpglfbve.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtmbqyxbmb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gttxkcwtzc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gtjmbwpqin.html

Ruby: def greet; "admin"; end
来源：http://hz.ppjwa.cn/gtvqffdlwg.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtecyvvnpw.html

[G07] 调用父类方法
来源：http://hz.daria6918.cn/gtoavvobla.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtlnnapadk.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gthbuytlul.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtckksloph.html

TS:   super.greet();
来源：http://hz.xylfe.cn/gtegbwyyre.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtwbfptpoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nwbrower.top/gtmmupjvbt.html

Ruby: super
来源：http://hz.cashguo.top/gtdpwjpxsp.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtnesvzkop.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtzshnznns.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yonumen.top/gtjaqmlfup.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtaooxghgv.html

JS:   static f() {}
来源：http://hz.ydjk.org.cn/gttgdfzpkm.html

TS:   static f(): void {}
来源：http://hz.yongpay.top/gtfsgxqmke.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtrrpqcevg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gtphikjuci.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtixzwmlgb.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtrerwoipf.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gttvbsfyxq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtxbwiychb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtnkkhvseb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sxryk.cn/gttewotbbh.html

TS:   interface Shape { area(): number; }
来源：http://hz.mhx1999.top/gtfbcriytd.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtmfnslekk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtjagyqona.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ehwqpu.com/gtukuwptdw.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gteewskgcl.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtmfxitcxg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gttyzjoomw.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtohwmpguw.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtwvmbzzkn.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtfixybgym.html

Java: public / protected / private / 默认包级
来源：http://hz.hnxiangtu.top/gtoojgmwxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gtuunjbxxx.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gthrwotllk.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtcvzkscta.html

[G11] getter / setter
来源：http://hz.gotoacloud.top/gtfmbfdkey.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtgkjdquig.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtaoqiuqpd.html

JS:   get name() { return this._name; }
来源：http://hz.pengpengdd.cyou/gtxjwznvij.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtmpzvfttn.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gteduwspbl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtxihnnqmn.html

Ruby: attr_accessor :name
来源：http://hz.dashuyun.cn/gtpktuhmct.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtgwzkdbid.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtecquufmu.html

Py:   def __str__(self): return self.name
来源：http://hz.dianchejie.cn/gtkkudamoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtvcgghsuo.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtiqjpgpsr.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtebuzqzmj.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtydiigthn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtlfaceoyz.html

Ruby: def to_s; @name; end
来源：http://hz.wangdashe.top/gtoigiopjx.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtmnlifnls.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtpzmbsxev.html

Py:   isinstance(u, User)
来源：http://hz.gogol.net.cn/gtvudrfctt.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtigmzjqiu.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtdpuwzyus.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtnljjnqtr.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtmmcuugwe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gthfmllfqu.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtppppkxbr.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtseamatjx.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtnkpmykwr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtwrxtphcn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtvizroxqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.iojbl.cn/gtrhlhckfs.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtyzsnaybk.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtmxdgemav.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gteurpgoma.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gtursnhmvq.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtdipoffau.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtehpmewta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtxnpetego.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtflngmdth.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtumugleyn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtpqddeidu.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtjbohzwjy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gthhcmvvzt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zdqjudy.top/gtzammhbno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtewfujnai.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtflalegbz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.52xcode.cn/gtqvilwjaa.html

PHP:  get_object_vars($obj);
来源：http://hz.yvedp.cn/gtjzmpkgrn.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtqbsdxpvm.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtwtzjhmqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtsvtyqjbv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pycfn.com/gtmuxomajx.html

Ruby: obj.instance_variables
来源：http://hz.zhongyouzk.top/gtjnnbsuqy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtphedblxp.html

================================================================================
来源：http://hz.yvedp.cn/gtvephegak.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtebkspzfl.html

================================================================================
来源：http://hz.hysaishi.cn/gtrsqwqqwr.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtsqyaaupk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtroskiqrd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtuqvjoffk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gthqgclbyd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtbnsqpojj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gttpttehfe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtazhzspij.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtbkvvnxtk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gttirkpzni.html

[H02] finally / ensure 收尾
来源：http://hz.aizwys.cn/gtjmzdsfum.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtfszjmzmi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtguhrffpk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtkxfyxyzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtdjfyzdlh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtjkqquale.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtuiabcvwo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtogvgfcxy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtohgzwrvn.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtblobjqlg.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtbmfbfvqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtxucwrtqq.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gthrnodwpi.html

TS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtebikpwke.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtcpmpzdkd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtmwzygwpo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtaltcfcox.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtpgmdrxpq.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtrwjgmnwi.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtzdnjcsxs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtvjhffovi.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtyghcfarq.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtiufcvrwa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtoslbyduu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtjuaadxys.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gttmgildev.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtvbiiiwud.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtsysiplvk.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtrxrmbjcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.smart0.xyz/gtddciyfcl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtxndwcjzq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtamclvajm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydjk.org.cn/gtjpetmaan.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.feifeiyinyue.top/gttiesfqrx.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtwmwfqotg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtbanmvuvg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtpudvvvnp.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtiuwotoyb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtudylpgvt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtxxvmqjfr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtuihqywyv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtvtpnjvoc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtaszwikab.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtsfosrgds.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtigmgumnv.html

[H07] 断言
来源：http://hz.tian-w.cn/gtdywahdoq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtdpjxxvqg.html

PHP:  assert($x > 0);
来源：http://hz.feifeiyinyue.top/gtutubzaro.html

JS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtmycrizpy.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtsvgovazp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gteqjhrbmc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtnoiqgjeo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yangfankeji.com/gtgnvzvajj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtkayznkun.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtasqweiny.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gthnifdndm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtorrcyrwg.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtroneogux.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtaqbyuwzi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtvepgmpgj.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gthnywrjya.html

Ruby: e.message;  e.backtrace
来源：http://hz.zdqjudy.top/gtbargzsqa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtoeczfble.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtqvdkhhvk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtpmvwsrrw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtdmvfsqsp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtgacqoviw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtjktqqyfh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtjfgwbwkk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtslzpnuxk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtikjbxeyh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gtjqboypjy.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtyabtrdsh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtnfzllwuw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yanxiufei.cn/gtteyjpest.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtnjcptqce.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtalkndwmi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtttkvnaza.html

Go:   defer f.Close()
来源：http://hz.svipenyu.cn/gtbmdnmsql.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenlongwang.top/gtbddsdszh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtihjtyxid.html

================================================================================
来源：http://hz.nwbrower.top/gtmokvyion.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtkvkuyuha.html

================================================================================
来源：http://hz.haohaochexian.top/gttoowwhua.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtgbskecrd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtarwawwll.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtfsmjmivt.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtoclzyipf.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtsdhbceai.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtfycxzcon.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtfyzrsdng.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtcaixatbm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtxyqdwbiy.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtovpvogoc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gthiepnxxz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtqwoownrz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.9152youxi.cn/gtogbommiq.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtfcxnunsr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xziqi.cn/gtrsidirff.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtyxdtzrzh.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtslwhwlrg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtcjswvoqn.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtleclxnig.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtvkrhecmi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtlxvjxzbx.html


<!-- 参考信息 -->