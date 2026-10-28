代发 wailian999

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gtdnvqufjd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gtwtzjersq.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtjcwuagnv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtrpvpmhep.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtfmnbmzyr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtllrahhey.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtqhcxtxxi.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtwygtgzli.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtylevlvet.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtaekehtai.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gthldjwstv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtoranbdiw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtkcinefot.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtrzkuoqxv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtpccbewtb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtvnygdwhy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtycbpuyrl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtirptnfsh.html

[F11] 复制与移动文件
来源：http://hz.yj202588.top/gtwsgniwym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtsoaxsulc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtznyjlcxn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtlxmmlbtx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtpwossodr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hammf.cn/gtrwqawspc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhaomingkeji.xyz/gtzfhzeqma.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtsafeakqw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtwkvliscj.html

[F12] CSV 读写
来源：http://hz.mhx1999.top/gtsmjdlspr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cashguo.top/gtmvzviuxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtlncrmxri.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtenukrqoe.html

TS:   // 同上
来源：http://hz.316326.xyz/gtgtbmgtyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtyyqdahgr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtkhnimnrv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtsnfegyfw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtqchcgxdj.html

================================================================================
来源：http://hz.52xcode.cn/gthdsgipvx.html

G. 面向对象
来源：http://hz.vqdsnc.cn/gtkuurrjwd.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdkfmuiov.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtkgtrmxre.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gttnukjgwj.html

PHP:  class User {}
来源：http://hz.jiagoushi.top/gtdymgavly.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtwhzddcgn.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtalkhllax.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtbomilgfm.html

Go:   type User struct { Name string }
来源：http://hz.yuxming.cn/gtqybjgodw.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtejipokfa.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtjvuiklnq.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtydxnnlap.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtkmrvvdwn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtzdrxlmht.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtjoqacjzk.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtxlislqqn.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtvudwekug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtrtxktgvl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtvwtgrzqp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gtjjyutmmz.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtojtmsbdz.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtiyukghyk.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtmyvhytcl.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtiexrwkvl.html

TS:   name: string = "x";
来源：http://hz.yj202588.top/gtpywljseg.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtoippibnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.iojbl.cn/gtqwxbcdos.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtvtyldtuo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtqtswvqrt.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtrmvjatac.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtrhplqmjg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtcdqmwbld.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gteldqxdsu.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtlhcvygfh.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtuvhwloci.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtvbuvnywc.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtiurpuwyn.html

C#:   public string Greet() => Name;
来源：http://hz.yj202588.top/gtpzjmfoxv.html

[G05] 继承
来源：http://hz.dianchejie.cn/gtpkuxaimu.html

Py:   class Admin(User): pass
来源：http://hz.guowangkeji.top/gtvnjabikr.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtmybzkftp.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtcppozhfk.html

TS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtjkiwqmst.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gttitxuqzt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtddulciba.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtgqupuzfk.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gtfhqhgtff.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gthjsyfxhh.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtdhzlqkhp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtugpigeon.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtformqybg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtmoexovdr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtqqerymfm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhijiandao.cn/gtauhlqiqk.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtzjfkfcvp.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtvolrfikx.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gteygbrmpz.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gthnnihomm.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtykecmtlv.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtjwgkwozb.html

TS:   super.greet();
来源：http://hz.c1oappe.top/gtpuwanowg.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtzbvhncxv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangtech.top/gtppvukvez.html

Ruby: super
来源：http://hz.yonumen.top/gthrlwddjy.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtpvrshyyq.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtiktovzqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtxrbybaom.html

PHP:  public static function f() {}
来源：http://hz.cucudq.cn/gtbcmvhbgh.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gttblkcuya.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtzxsprszp.html

Java: static void f() {}
来源：http://hz.gzhubu.top/gtqdfyhihw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtthjlwbps.html

Ruby: def self.f; end
来源：http://hz.jqgufenzy.top/gtzsjytzxm.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtffulomzl.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtjllbqaie.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtbzktgkkt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtqnfaoaup.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtwkhrhkoa.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtikgqjzjt.html

Java: interface Shape { double area(); }
来源：http://hz.xuanzx.com/gtapxrgtma.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtmrwjsosz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gthbuuavij.html

C#:   interface IShape { double Area(); }
来源：http://hz.cashguo.top/gtjrbxttrr.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gtekfjagyz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtkbfgwili.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtlgjcrwqr.html

JS:   #private 字段；其余公开
来源：http://hz.chenjidiqi.icu/gtokdwgxaf.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtnyhhmpst.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtpzmefcqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtppnntahd.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtpcvsilag.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtubdoxsjm.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtrrdkivhj.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtuchngfmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gthnhcdmti.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtkblsusbu.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtlrjcbnho.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtqmlngqqs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtgvujmbek.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtwaadctyc.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gtybcxntfa.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtpjdzctoj.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtmljcxmmf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtxsoswyhl.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtrepnrlyh.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtgtbdkxop.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gtplksjekl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtvyctpzrm.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtxxktftjc.html

C#:   public override string ToString() => Name;
来源：http://hz.316326.xyz/gtlpgzaqun.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtpsmtqbhm.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gtmcyqqdtt.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtmujtavdg.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtvwfaobkp.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtejuwowki.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtxnidefae.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtxpuimsop.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtykzgdehc.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtisdymyzg.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtxfvecdab.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtwbcfdggd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtdkucsjgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtbltkkzdb.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gtgllizmuk.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtxfvtvahj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtkzclygcw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.meibo888.top/gtsdudlwfl.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtfrkqpaql.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gteeqejmys.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtycedjnzl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtrdknyjyq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cdnleiting.top/gtfoylzmye.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gthzryakbr.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtslepkgka.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtuegkgmjc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ivvv.top/gtzodexbpb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtkpkwymbv.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtusfhyfjr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gtfkpzkiio.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gthyapeuwh.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtwfxbovfd.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtuglzafvw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtytkjmaov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtngcrwily.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtsqwthmhz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtijdedqqg.html

================================================================================
来源：http://hz.cashguo.top/gtugljashm.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtgwonvrpb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtchjfugao.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtacroeqja.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtqjwzlbiy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtiqqptivy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gthptppbtm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.meibo888.top/gtzxzaryty.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtoboheczq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hammf.cn/gtsogwjhrb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtlffqirkn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shangyingyoupin.top/gtnlvkpamx.html

[H02] finally / ensure 收尾
来源：http://hz.hfpthk.cn/gtsrjdklew.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtmteurwun.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gttzastmtp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtgpndfjbs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtawsxgxqz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtqptcocyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtbiapsayx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtcknwziuw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gthxpvflch.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtqxetywwo.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtkkuyzwbm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtvtlmpdup.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtqxtkarfs.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtxvhrjoxx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gttgtabqro.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtfibstdir.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtvtlywhcn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtdgkgebir.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtwmnijgaj.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtqatckezk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtatlwsanl.html

JS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtidprfjjm.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtntxlmqtp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtkfqcgewn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtmhtewcof.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtzzfkjhoh.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtgkpmxitg.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtqsteubhe.html

Py:   except ValueError as e:
来源：http://hz.kuanghao11.cn/gtkrvxovrq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtlefiwarj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtnsjygugf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gthtctexhm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtldbpinex.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gthkwfoijg.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtqbpkzgap.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fengsongda.top/gtvedejbnd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtoixombgd.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtqhdqfjco.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtjgjvqwps.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtabasehdk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtrpynvmyw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtrjudabha.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtqpaorwsq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gticoecmyy.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtzclathwr.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtnlcofazc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtywizampc.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtscgynmvs.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gttbuixaow.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtwkppxgbv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtmaodvjrw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtxwuknxvp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtwnlhjqlw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ivvv.top/gtuwgxxfwg.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gtjalyomxv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtlefvnwuv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtedkpbllx.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtlgeskzjf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gttvjyphkq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtgbtbetlx.html

Go:   err.Error()
来源：http://hz.yj20258888.top/gtjutswlrc.html

Ruby: e.message;  e.backtrace
来源：http://hz.redwolf501.top/gthbmwmzjb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gteojklhsh.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gtfxpclifv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtmmszlwht.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gturpoddow.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hywenlv.cn/gtzauizojj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtevqlpggo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtyotjepce.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtadrdvkfp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtqvdawpud.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtrvwdyfqz.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtfgikxshj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtlubjbjvk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gttcsxkgte.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtzweyuzyb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtqemaucae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtlgudpsei.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtmdyedssa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtoaazuntr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtvsqmfaeu.html

================================================================================
来源：http://hz.fengsongda.top/gtjuthdtxo.html

I. 正则表达式
来源：http://hz.ivvv.top/gtqigzrjjq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtluajbwxx.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtnjdlqiyj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.0kj1m.cn/gtwvaavtxb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gthjauxzyg.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtcfwjggas.html

TS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtmcconohl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.52xcode.cn/gtdchwyvbv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtuirwjogh.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gteffnmxki.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtzempeiij.html

[I02] 提取所有匹配
来源：http://hz.kuanghao11.cn/gtrmpgwexl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtibtpvebf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtdplthidy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gtksxjwrqq.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtjwccqvnk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtbjitiaks.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtgbcylwho.html

Ruby: s.scan(/\d+/)
来源：http://hz.ppjwa.cn/gtgrjwliwt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtomglfrxc.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtqmbnijzx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtphukpqra.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtaholgmur.html


<!-- 参考信息 -->