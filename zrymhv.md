代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhixingplan.top/gtskhrxgyj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtacrcbrcv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtvypiyzev.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtumbjdjfd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtiwbutkyk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtskybombg.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtlwzlmodx.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtyfjbfzvw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtwqgvswap.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtsxjqhteh.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtbdkgstio.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gaohongyu789.top/gtzgeidmsf.html

[F09] 获取文件大小
来源：http://hz.feifeiyinyue.top/gtrhqiexdt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gtuqxobgpy.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtwrnxzztm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtquprosmn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtxkseklmb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtcolshxsn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtjmpsalpx.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtsgpmbtal.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtghsaroaj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtrwnvwbor.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtjwwaradv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtmnxwqnma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtcbuovokt.html

TS:   path.extname("a.txt")
来源：http://hz.9152youxi.cn/gtpicirojg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtexcxyndn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtpqlmbeey.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtusccvzvf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zdqjudy.top/gtgbmxohbu.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtrafgbnem.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtpujgeefo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtuwvgawyp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtvuidqlta.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmiupgxif.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtcwzyfqum.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtjyaewdtp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtcwqpywyj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtkiodblcy.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtdzhnsysa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtbsowjjfl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tanke756.top/gtiulrqxiq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtycqvlosm.html

TS:   // 同上
来源：http://hz.zycfv.cn/gtjksjntam.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtadqufxaf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shzxlz.cn/gtenawsefi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtpskuczbk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cheryme.top/gtbuhgqvgb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtobayglla.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtsessxzqr.html

================================================================================
来源：http://hz.tanke756.top/gtqkhidrjz.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtpezwqnaj.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtheuxzlll.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtdcybasqi.html

JS:   class User {}
来源：http://hz.wangdashe.top/gtgyykcioe.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtftjkmiqx.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtwhdefhnw.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gtgjjyuntn.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtcpoentsl.html

C#:   class User {}
来源：http://hz.sweek.top/gtceudocac.html

[G02] 构造函数
来源：http://hz.jianghu66.top/gtfglvugmk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtzjhxitbt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ehwqpu.com/gtougqcesz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtkldfjqej.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gthmlxlrep.html

Java: User(String name) { this.name = name; }
来源：http://hz.hywenlv.cn/gteuilnbmm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtrmxhermy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtwtdwexux.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtpqrasmqt.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtaigmrpdh.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtkpwcsqtk.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gttzlhjsag.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtqbxssapk.html

TS:   name: string = "x";
来源：http://hz.shuidangran.top/gthqvgvuqv.html

Java: private String name;
来源：http://hz.hongshengwenyu.top/gtwyharean.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtwhboabub.html

Ruby: @name = "x"
来源：http://hz.ydjk.org.cn/gtllwppmrm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtwryrvlkh.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtrqcqpmho.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtlqtwxcap.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtblhwveju.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtiglonfpy.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtpjoigwkb.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gttcncspgz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtcvluxmcy.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtcpoxvgqc.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gthjrnfqlu.html

[G05] 继承
来源：http://hz.nwbrower.top/gtgyjesvae.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtyyecvset.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gtkrptxljq.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtyopirjeg.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtenftwybf.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtbxlprwyf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gtfwlyabmn.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtlvgdmjhb.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtabnkekvd.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gttiwneamm.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gthbnpfyds.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtiredtfcu.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtssygzypg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtiobnlsit.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtvniglyia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtftypasmk.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtgdbfdhvv.html

C#:   public override string Greet() => "admin";
来源：http://hz.tianlin.xyz/gtbrllmogg.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtaozovvcx.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gttpwblwln.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtsvnjzohz.html

JS:   super.greet();
来源：http://hz.shangyingyoupin.top/gthwpalqpl.html

TS:   super.greet();
来源：http://hz.snrcjt.cn/gtlrepldoq.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtvppebpap.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yvedp.cn/gtxntunqim.html

Ruby: super
来源：http://hz.yonumen.top/gtxeflltit.html

C#:   base.Greet();
来源：http://hz.quarkkingdee.top/gtscewnnip.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gthjniopil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtjbeyqsrj.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtjlzcpojq.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtpevonrhi.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtwwwyhtqp.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtvrunenjh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtyqpygdfv.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gtnzcicqrp.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtocvpxqmw.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtyzrqyvta.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gthsgwnvgw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gttcdygfpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jlsjyb.cn/gtjgcyffkn.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgfzy.top/gttmwxuwpb.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtmoypkahg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtfvmonbjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ehwqpu.com/gtzhjmszgd.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtkegzpdkx.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gtrrkzdfkz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtwenzbvqg.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtxtynlknl.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtirridvzj.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtnuqowudl.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtmswjrtjf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtqymhwibb.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtkdakeuda.html

C#:   public / protected / private / internal
来源：http://hz.fzhhl.top/gtainadrbo.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtfcsjlvba.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gthjeihhxk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtfnzotzqe.html

JS:   get name() { return this._name; }
来源：http://hz.guannengcc.top/gtcqbltzsw.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtghvcpeib.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtyevoyxuq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtzanzoyxy.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtkwteynby.html

C#:   public string Name { get; set; }
来源：http://hz.haohaochexian.top/gttcwapscg.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gthsvxdpfl.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtmqpnoyzz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtaryfemgd.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gtnpolojqg.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtswnvbmeb.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gttiifvgwm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtizkmybcs.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtzhdqqorb.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtbifyncyw.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtqwkniybv.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtbrvhjldj.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtqqiqcncb.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtctfjivhc.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtngjsupqq.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtsumvsdja.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtntpiqyyg.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtillizizc.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtffplypuz.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gthfegkoqu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtoijmspul.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtqnzjpwif.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtygjeozrz.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtoodzgkvl.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtaoeiipqd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gotoacloud.top/gtcslpdjgv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtcxnevqip.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtikaykqno.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtgdsnodiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtouwdherh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gtxdarbgza.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtxznggddu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gteenmetuq.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtmryflhwh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtkhkujrdz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtnkngtyrl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtopsdvxnf.html

[G16] 对象转数组 / 字典
来源：http://hz.tanke756.top/gtcmbithvp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtpiqfrsun.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtgaxvhttk.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtaheumbaz.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtsoaayijz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gthxsbpjyt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtwnigahyp.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtkgviqjgl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtirxhkmkc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmsconkvv.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gtebopajzr.html

================================================================================
来源：http://hz.bjfxy.top/gtgngkuhuf.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtzyhilsqk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtgprpfbpb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtbrztloph.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtouetskvu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtgiddvtka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gtgezlxjkk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtqqelthib.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtcutelwsf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtskysjsta.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gthlrdyucv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhaomingkeji.xyz/gtuhhwprda.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtuneedpkr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtpdphfftc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtphqpcmot.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtxexntjxn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtjjjlakcd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtcyfpmqbx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtdgcucqht.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gthgdsvcjs.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtzkpqfknk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtgkphhyoc.html

JS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtvdvuflkd.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gttoptkzrh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtzwjatqkt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtjyuazuas.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtbevhrikq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtxghjzfdu.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtslyfapto.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtwwingmtl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydzc1.top/gtpwlhdbqe.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gttqherxyu.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtkgdkmgpa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtwmtddwdl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guannengcc.top/gtwoloqfzm.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gthewhkiwg.html

C#:   class MyException : Exception {}
来源：http://hz.tianlin.xyz/gtulnngycz.html

[H05] 捕获特定类型
来源：http://hz.smart0.xyz/gtlkijnwjk.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtonizpwze.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gteszqigrb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtihxwutbv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtpuhdbbeu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtaibomyvg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gthxrfxnac.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtpkuqxrvn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtnuhajnxo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gttoopwhmr.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtbdazawet.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xylfe.cn/gtcqugzmvm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtidpfgobs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtqksemnmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gtyfgovinb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtfficlivv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtfucihqzp.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtpfeupejt.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gtfezwkejn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtpprhsimq.html

PHP:  assert($x > 0);
来源：http://hz.sysykeji.top/gtvarqurpi.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtqksmyftp.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtpjnqliyr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtkumricwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.9152youxi.cn/gtnjudvczu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtmeqduhxf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtwaqughmr.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtdjpzwqwu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yonumen.top/gtlrrwkbnw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtwspqlhjh.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtpgnrtieb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtyybgjnjs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtwbranyjf.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtfrdsewoj.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtcinurjvs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtcfcolttj.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtcbdjlwtd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtskcrmypb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtrtsztzdz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigfzy.top/gtjxgredfn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtoyhxergk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtugoopbrc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtydssjhhd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtghylbzse.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtztrllmhn.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtdnneaavt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cucudq.cn/gtojmlljng.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.havefunace.top/gtiqjflcro.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtrfzqxrnw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtfbtvwiqy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtlmojopmx.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtwprxyyeg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gtnxtnazxf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtqdtwslea.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtylriibtm.html

I. 正则表达式
来源：http://hz.316326.xyz/gtbpxwukaj.html

================================================================================
来源：http://hz.andypj.xyz/gtwrdefzkh.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtfaykgfjr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtudpsjemq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtfjfzrxus.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtsskotmle.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtcrxngutl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shangyingyoupin.top/gtrypefwsi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtmukajoli.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtzsrgnqdx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtymzuiyyj.html


<!-- 参考信息 -->