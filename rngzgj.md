代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtgjnnpyvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtvvpvpvpx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtwgvbhzjv.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtwoqiftci.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtnrxeqbzc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtnnxzqgxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtblfxprbd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xziqi.cn/gtppzqjhud.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtyplpwrvs.html

TS:   path.extname("a.txt")
来源：http://hz.vqdsnc.cn/gtkoojwcah.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtkreysbfm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtustdedkk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtaryuilml.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtfyfcpqoz.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtbnozpxpq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtdqvozxjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gtkzfvqusg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gttptyzsnd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtmuevyavr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtiycwxryt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtkazyicoo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtxiulwywj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gtqgfdjkpj.html

[F12] CSV 读写
来源：http://hz.sxryk.cn/gtqvjfrfuo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtpuisavza.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtiuvrgddk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtfvmhmmnn.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtvhteychr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtaqgrdkef.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtqmgljoac.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gthrfzkmdi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtvisfoiku.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgpfebbqo.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtoqboayin.html

================================================================================
来源：http://hz.tanke756.top/gtdumjonml.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtledbihst.html

Py:   class User: pass
来源：http://hz.9152youxi.cn/gtjfogyktj.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtvmqyhysp.html

JS:   class User {}
来源：http://hz.yongpay.top/gtlllgpisf.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtsfioihbl.html

Java: class User {}
来源：http://hz.jinyuanbaomall.cn/gtvtskbcqb.html

Go:   type User struct { Name string }
来源：http://hz.aizwys.cn/gtinorwmrv.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtprndypnf.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gtagrwqrql.html

[G02] 构造函数
来源：http://hz.yuanzhike.top/gtlqzrvdkg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtcaaownrh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtkwdrxuyv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gthawmvjuc.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gttzfpcfsb.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtoxjauvbd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtwbuivpwp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtchydhhsn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtmehyvfji.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtrkigizkv.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gthlgbcgss.html

PHP:  public string $name = "x";
来源：http://hz.jiagoushi.top/gthmrhoebt.html

JS:   this.name = "x";
来源：http://hz.daria6918.cn/gtdqowzxdi.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtdjmgqgow.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtowktpbvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtuprifwgy.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtzxjjewbf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtijivuymg.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gthehqemtk.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gticydkrvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtvgqsspiv.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtbcsdsdvo.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtoyvtjnkl.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtzojrvpsz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtbyjrgayq.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtuugrksln.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtkcjuzwzl.html

[G05] 继承
来源：http://hz.dianchejie.cn/gtukhafbaa.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtwckqepfv.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtbtcpqrff.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtlqeysksj.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gthdyvzjdg.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtxuudidfk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sysykeji.top/gtcsqjeyko.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtfhcpkevn.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtrepdablg.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtlsjaadeo.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtyjqslsmq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtzxfwsmgd.html

JS:   greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtngnqafon.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtkhapeepz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtxuauazhv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hammf.cn/gthodlodal.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gtiuxndkfm.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtvkctvrvi.html

[G07] 调用父类方法
来源：http://hz.jinyuanbaomall.cn/gtpghwmimh.html

Py:   super().greet()
来源：http://hz.cheryme.top/gtmymhdmno.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtasvdkmmu.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gthpvpzzsf.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gtlihkibol.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtgvobvwop.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sysykeji.top/gtwqpmpraz.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtjngjkdyd.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtamrdvplc.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtefazohjs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtnjkzrlnn.html

PHP:  public static function f() {}
来源：http://hz.yuxming.cn/gtaadmnaww.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gttsmawywh.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtsqagbzxj.html

Java: static void f() {}
来源：http://hz.hysaishi.cn/gtmkydibnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtdwhimufo.html

Ruby: def self.f; end
来源：http://hz.guowangkeji.top/gthjugskqn.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gthaijffre.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtwfggjqjs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtynuvskav.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtehyvwsna.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtwgzspfaj.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtmacccvcg.html

Java: interface Shape { double area(); }
来源：http://hz.tanke756.top/gtdewvodvr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtyqslwanh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtidjulqoq.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhixingplan.top/gtavvyurek.html

[G10] 访问控制
来源：http://hz.snrcjt.cn/gtprdibjio.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtfzpsmhim.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtbvxrvcqf.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtagicxwyq.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gtooecwloy.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtbxdkdiav.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.svipenyu.cn/gttuarehir.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtzpknpmyi.html

C#:   public / protected / private / internal
来源：http://hz.jinqigfzy.top/gtplcfjziu.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtbdbpgbfj.html

Py:   @property 与 @x.setter
来源：http://hz.jianghu66.top/gtntpsbafk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtcaqemvvi.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtlebahyup.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtfibilozz.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtbwpxbyng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gtgddwhhlg.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtgpljbeue.html

C#:   public string Name { get; set; }
来源：http://hz.jqgfzy.top/gtbgvpuzyi.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtdfqzhast.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtmkgwtrhj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtoldmnyti.html

JS:   toString() { return this.name; }
来源：http://hz.vqdsnc.cn/gtjkmyxaqp.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtfxbabxiw.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtndikxyzq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtcynctxzm.html

Ruby: def to_s; @name; end
来源：http://hz.yanxiufei.cn/gtexcpuikn.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtntgjxnuc.html

[G13] 判断对象类型
来源：http://hz.nwbrower.top/gtmgyffsbr.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gtxnfjxaxd.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtncrmunlh.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtkgievexb.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtxmgmomig.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtouwfurld.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxinkj.top/gtjukwwtmq.html

Ruby: u.is_a?(User)
来源：http://hz.cucudq.cn/gtrmkiagnm.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtygqtfcfv.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtnwjhsahj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtlutfhsnp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtlidlozqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258888.top/gtlprmwcfw.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gthnxqqchi.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtqinqdqoa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtfgzzbuds.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtkjfrdrgk.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gtzbwdfqts.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gtbkncnbam.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gzhubu.top/gtqxpukpkq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtylafufyy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtajmwgawb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtzzcmixoj.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuanzx.com/gtcsjkxsis.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.vqdsnc.cn/gtevqrahii.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gthkqlgxof.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtvsyizddb.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtuehqjgvv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtexhzuymo.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtuivmfxae.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtuetjihvt.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtubukwetl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtihhmxjfb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jlsjyb.cn/gtcfsawqlq.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtybeopxsq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtbmesfebc.html

================================================================================
来源：http://hz.redwolf501.top/gtscvpkltv.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtlkawqelu.html

================================================================================
来源：http://hz.tianlin.xyz/gtqzsgelqr.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtdhnwjnvq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtomebbjhq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtjphebadl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtrkiyjmba.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtrdzuuqmz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtfwwbvjhj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtttwcwoud.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtgpgjepqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtlumoakzm.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtmaxqsjap.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtdutphkir.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtdtmmarft.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtjettqpyl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtdrvupnok.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtnntbkvzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ivvv.top/gtjfaihwye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtviehzegr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtmhpuhxkg.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtmygjdegd.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtkppldreq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtgynimggm.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtfnegthsi.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtmhudtler.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtnyzgvtxo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cdnleiting.top/gtjlsipaxf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtpyuxcvjd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtcldvlyom.html

[H04] 自定义异常类型
来源：http://hz.jqgfzy.top/gtuypytigu.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtbnqyloav.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gttvtgskde.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gttdcvsorw.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtxcvhukml.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtdlfwekcc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtwhcpalla.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtuflbsphc.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtmizwchfp.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtjmkwnmhl.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtetbwmgan.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtjtdckbcf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtjvpldnzx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtsffbmbsk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtooydyiof.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtarnsubwu.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtgpqqvmht.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtgstlmsyy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtjxcybrty.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtbetinczk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtwfskhioc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtzznewovf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtcdqoqact.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtusnnffkp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtojhzzxrx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtsufbukcx.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtxhtjpejz.html

[H07] 断言
来源：http://hz.meibo888.top/gtbfrkwget.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtklzseoqx.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtikycpwuj.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtqruzxnqn.html

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtfqqofows.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuetiantiany.cn/gtffvfzjpx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtvanopkky.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtzmztdtmw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gtymxuxawg.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gtnzqzwerq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtugzlubdc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtrfilaccw.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtntizjrny.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtopshwejb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtdwrylsvr.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtahvxdzqn.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258.top/gtcvfxzhto.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtqaflwpoh.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtdxkcglsk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.52xcode.cn/gtgkyckpuz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sxryk.cn/gtfzspxzrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtejocxwod.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtfgtwsici.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtxzaweses.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtbobbusln.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtuocddfyg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtpagyfenl.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtnononamz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtekgmxqgj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gotoacloud.top/gtqhgiixpn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtcawlyknw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtabypjphq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gtxvjzvatn.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtnxruzgse.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxuanxn.top/gtmwderaea.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gtoaljimkt.html

================================================================================
来源：http://hz.nwbrower.top/gtbtzocalq.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtjdugtagg.html

================================================================================
来源：http://hz.xylfe.cn/gtwxuengjd.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtpwecqhsm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gterjusjtp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dashuyun.cn/gtipomocgf.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtsocrrjfx.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtylabwxpj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtsjxwxjsk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtbcaweile.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtozbepiaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtyqzqgpss.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtqmljgefe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtqvdjfgml.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gttvrwoxmt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtdfwtfpbr.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtgdmaiurr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtvhixtpet.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxuanxn.top/gtrqpvgzov.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtkzfkrsev.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtezbzymtw.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtbecrkajg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtwpjsgfca.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtspovqboi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtcxciqzbb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtnpqhjjgn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydjk.org.cn/gtphncglqm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtlqyeqrfp.html


<!-- 参考信息 -->