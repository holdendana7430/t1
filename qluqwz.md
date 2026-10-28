代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gteswfhsva.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtctqbzwzo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xziqi.cn/gtkqvadhbu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtnqlbecjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtkabhmkna.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtnewargjf.html

[F11] 复制与移动文件
来源：http://hz.feifeiyinyue.top/gtbckoyhhw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtshtxhezo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.birdmap.top/gteynwhpzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtoeknpwws.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtjijiudzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtqsyfmofs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtievdivyh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtgpjwwqsk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtninlfiwu.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtsgechpox.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtcxpkqgcz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtppiabyvj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtqgteibzm.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtnspkzflo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fengsongda.top/gtcywcrtnu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtehyhugwl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gaohongyu789.top/gtgotjdzee.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtoeranakv.html

================================================================================
来源：http://hz.xuanzx.com/gtbnqnjtze.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtyumtujqq.html

================================================================================
来源：http://hz.52xcode.cn/gtwkmnmzjh.html

[G01] 定义类
来源：http://hz.tanke756.top/gticqqhjyp.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtgpgywnzt.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtjykbntfv.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtusajwdpu.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gttzqocrvg.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtwirccfvu.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtihltpjmu.html

Ruby: class User; end
来源：http://hz.cheryme.top/gtvntlwcka.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtdmizmsyk.html

[G02] 构造函数
来源：http://hz.birdmap.top/gteywinuvb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtguxskfyh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gogol.net.cn/gtzqxqhnbv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gthbazgunm.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtjigvrrkp.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtasuusntk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtdkdpmyat.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtthbscyrd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtqilpgrqs.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtpwfenyal.html

Py:   self.name = "x"
来源：http://hz.daxiang520.top/gtxdyfdwvr.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtmkrzdaue.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtdcuckjcu.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gtgvazqwnb.html

Java: private String name;
来源：http://hz.xinyue.icu/gtwbmitvll.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtwfdyvkxm.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtgwxaslui.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtdlcdbfve.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtjqrcxvdl.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtvugxansi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtevzxfyzi.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtgssbwpao.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gtunyljzty.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtwefsnfbs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtsvygkiug.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtkxtdkvhs.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gthkpchaeo.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtuckaheks.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtaezfotgz.html

PHP:  class Admin extends User {}
来源：http://hz.yj202588.top/gtsopacwpn.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtpihthpjs.html

TS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtjbgwdudl.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtrqqdzefy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinyuanbaomall.cn/gtdsgvrbxt.html

Ruby: class Admin < User; end
来源：http://hz.zdqjudy.top/gtqberndho.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtnaqhieet.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtkvjnvogg.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtclccmjmy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtgszidzzb.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtatwdcnmm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gttnbrqebb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtpcaferfd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gthguxfytz.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtvgnvhfat.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtdaesdgjj.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtecvgckow.html

Py:   super().greet()
来源：http://hz.wangdashe.top/gtzonlhdit.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gthjydreyz.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtveexfrew.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtkxqmioil.html

Java: super.greet();
来源：http://hz.yj20258.top/gtivonthsu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gtzhmtkzxi.html

Ruby: super
来源：http://hz.52xcode.cn/gtfqzbcfed.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtspvfggvo.html

[G08] 静态方法与属性
来源：http://hz.ydzc1.top/gtwwjruxur.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yvedp.cn/gtjpromzap.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtypemrucr.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtexvhjkqw.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtxcaweagv.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtzpqfdobp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtrhdgrsjd.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gtemarpulw.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtildjfrur.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtbfbkbfgf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtibhxjhny.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtlbhmygvv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtpemcovwh.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtqhvilnpx.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gteqwcuxpo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtncfoixkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtaoaupcna.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtkywqifou.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtqpxldahw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtanlihirj.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtyfykpdcx.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gthcgelcgl.html

TS:   public / protected / private
来源：http://hz.jqgfzy.top/gtdgfcpiwv.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtdvrbjomi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtyvbmjmtl.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtubdwpgsr.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtsebbuusy.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtkinpekuj.html

Py:   @property 与 @x.setter
来源：http://hz.yuanzhike.top/gtunwmggaq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtvnxvguio.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gtmxyholso.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtweheklnj.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtrjtoxwve.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtkscqzini.html

Ruby: attr_accessor :name
来源：http://hz.feifeiyinyue.top/gtwtdibhxp.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gthhglzwjo.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtllqhfeci.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtwugryrbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtarsakgyv.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtumetpnte.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtkdvyhkij.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gthxzinopg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtbmcintgh.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtfxewsiub.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtcxknravx.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gtmgyritmg.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gttcezqxua.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtfebxcari.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gtfwmkvsyj.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtwwcdoiox.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtiszonrjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtgduqlemp.html

Ruby: u.is_a?(User)
来源：http://hz.zdqjudy.top/gtmzbzrpdt.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtfteicjez.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gthshnnfod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtatjkjnqo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtklyxamdf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtzstgdsso.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtqofotgur.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtekyvvpdb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.quarkkingdee.top/gttnvmkbhh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtrcgbozaz.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtrefizxuo.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtktlqoxqk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gzhubu.top/gtchzbnqjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hywenlv.cn/gtanuqayhe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtannakxdq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtvhksqbjp.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtagrirmte.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtoqafobhs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hfpthk.cn/gthfhcshuf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gttxlfejmb.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtzhdncsse.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtberuqhcd.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtzqqipvdd.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtjzfgrszg.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtbuvcaavm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtutyowgmw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtxroxbcnw.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gtarulnhyl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gtnksatvpa.html

================================================================================
来源：http://hz.fengsongda.top/gtyuxdspxy.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtxwlturwh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtahlgduty.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtthguinso.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtdnjoibyz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtennzmufe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtqplazfnr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydzc1.top/gtcorbhltf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.vqdsnc.cn/gtptczyhgy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtmxeskfiq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtrxljggcp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuanzx.com/gtqwdbwomx.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtpgvxeyto.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.52xcode.cn/gtfnvuaxtn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtzumqkxgx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtryelvako.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gttjuwvpzv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtlunywdmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhixingplan.top/gtjxhbuemc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangtech.top/gttzgjddcf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtlfefazgj.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtqgftsonz.html

Py:   raise ValueError("错误信息")
来源：http://hz.smart0.xyz/gtyebtjrwe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtbnulzgjk.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtvjjkeovw.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtnszvaezq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gttwavsiqw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtwznawkva.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtrpjnaacl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtzliivrpy.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtdzjnmsai.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtwqelxxir.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtwdlxqltn.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtdggediyy.html

TS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtrwdpqfwn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtqjjctymm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.316326.xyz/gtuituneuo.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtlybepfsn.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtyzjfedps.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtlfcnrtis.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gtkrcaofwx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtircsoofo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtblbxhghp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtxcdrwtbz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ivvv.top/gtoipqzmou.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtxljmfyre.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtopuelwcw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tianlin.xyz/gtznedytdk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhongyouzk.top/gtmjgshbxy.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtsiiilozs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtadfwvyzi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtunbcgezo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtfsmkoyis.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtzcpoihck.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtdmbpcsmk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtamfdbzfc.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangtech.top/gtzxcmctyw.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtpmfilixm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gttpfbafmy.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtuuuyrpbp.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtyytaixtx.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtvxqklkwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtrnbyyseb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtbiktsynm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtapgaqgrd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gteblamfts.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtkfqjzjws.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtaotgnobc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtmhgaqqbm.html

JS:   e.message;  e.stack
来源：http://hz.tanke756.top/gthetqdcgw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtxaygebuo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtgmgbedyl.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtoyvnbqji.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtfogwrmqx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtcnracszz.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtsnzstgdv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtbiuskbdd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuetiantiany.cn/gtpdtmquae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gthozneyey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtuncwrpsw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtvvtehjjh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtycjjcihi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtrepvhlgj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtqrcltgsv.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtpewubnhq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtfhmufwvl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtabpmwvjw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtfvnibtmr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtoyynaajl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtkjlniklz.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtqfdpsnfy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtbotdqpmz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtkxrcwtdx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwhaztxho.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtajzknzra.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtunhtlbdx.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtixcxktfm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtrlqgkslw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jianghu66.top/gtuvaodcsi.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtlcfvcjke.html

TS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtjjuqdrzt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtvykthmfi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtfmjcmoae.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtjvlbfhrf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.0kj1m.cn/gtvzatwvsg.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtoddmnhgo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gtvpggmziv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtcwznkmkl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtajgdrmwt.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtjatsdoyq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guowangkeji.top/gtvooaqtsi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtbyfsqfrk.html

Ruby: s.scan(/\d+/)
来源：http://hz.hfpthk.cn/gtibqhpxej.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gtmivkklnv.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtxvjarthm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtndhabyxj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtefdumsdt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtdwljfswq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtxyptrztp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtdnyhvugk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtbxedfjrv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gtiblbywxm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtwkwjtrth.html

[I04] 正则替换
来源：http://hz.xylfe.cn/gtsmqhodld.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtqaemuvqv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtonjkseka.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtvzgbzwne.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtioxzwnfs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gthwgckjwx.html


<!-- 参考信息 -->