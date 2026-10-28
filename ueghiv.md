代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtetfxmmqi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtnkyjmbqz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtxeovkadt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtdbfrlhlx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtkeecyfxo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nwbrower.top/gtcgwinusq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gttkqhxaxa.html

[F08] 遍历目录
来源：http://hz.jinyuanbaomall.cn/gtyevryxvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtwqxlcepv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtvyeyqpti.html

JS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtommzfqhg.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtnktsocra.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtroafmxzs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtfjrizzga.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtipelcfhg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtaxcgsqbz.html

[F09] 获取文件大小
来源：http://hz.fzhhl.top/gtgehtxgmz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtyehgwegi.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtvbbbyhuh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtowcaypvy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtijqbekzl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gthacophed.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtzzxkwctn.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtxorjiuul.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.redwolf501.top/gtksquwpaf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtgmwvbvff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtuyatqamb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gthjwgqupe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtjqtpxoxy.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtzdztsngn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenlongwang.top/gtzxhwnesa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtjwkzsset.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtodajiefj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtxqhqesjh.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtxsoqpbih.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtjmxrrqxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtdjktqdup.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtkntnwxtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtcknsqhlq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtzatkzliq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtopfifjqn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtmuvvotod.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtcyargfld.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gteeggbczx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtulvcgufn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtljczpmuo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtxyfabjql.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gthkpuferm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtkumsijkl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgufenzy.top/gtlpnsdmkh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtrrtcpyin.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtcoxyfhor.html

================================================================================
来源：http://hz.yuxming.cn/gtaywtiidj.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtqqccoqpg.html

================================================================================
来源：http://hz.dianchejie.cn/gtaveetcxp.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtcwnqfgih.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gteeupzfpa.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtbsmwpbfd.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtwlxhtnbl.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtwftlsesn.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtuvveomin.html

Go:   type User struct { Name string }
来源：http://hz.yuanzhike.top/gtbthuncup.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtwqeirqsm.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gtkihafuva.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gtsxurzzlf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtvuchgfpi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtnffmwcwz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtcmtjrkcu.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtuxxywfvh.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtubecyogq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtfzhbhycl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cucudq.cn/gtvmsrgqpu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtppzrdsjr.html

[G03] 实例属性
来源：http://hz.haohaochexian.top/gtqtrzldpf.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtvhpnyayb.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtzqbohbsc.html

JS:   this.name = "x";
来源：http://hz.c1oappe.top/gtkkvfhdoq.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtptsnzimy.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtefommomv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtdzixqrtn.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtjsijbbyd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtleprbnyy.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtspyvhppu.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtlwdxnvjh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gthzjtclhw.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtawletymy.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtlcjywatv.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtmxgytzhu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtafwtvtds.html

Ruby: def greet; @name; end
来源：http://hz.52xcode.cn/gtebwpvosl.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtwqdaseub.html

[G05] 继承
来源：http://hz.c1oappe.top/gtmbbaevql.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtdunbgyqk.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtjvbgrxsc.html

JS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gticyxjqdc.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gthrvbvdau.html

Java: class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtqyhaxegw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtpucztaio.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtsvimdvdz.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtjwbxigqp.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtvqroedwy.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gthndqtojw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtmonztimp.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gturpirqet.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtscgernat.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtmgaiqlgf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gtnzdsnmwe.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtjyxlctmi.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtaxmtjuhy.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtyynjfvbm.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtxlvohtrp.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtpnsdssbt.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtcbshzwxu.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtuemewhsu.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtjsemmils.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtttbylybb.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtcdjqbyaf.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtutwwheyi.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtbnhdnhsd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gtggcamxer.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtjuzotbpu.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gteqpuxijr.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtktcagrkc.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gthcpqvhcc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.birdmap.top/gtmxznpqne.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtomdboobr.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtbtwhkwzk.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtdofcztog.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtsjgkqjtp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gteebpbrxu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtwhcumpbw.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gttjexgjyd.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtqdzbpfgn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtqlktwhhb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtrpxuqxmu.html

C#:   interface IShape { double Area(); }
来源：http://hz.gogol.net.cn/gtrtzfockn.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtjulywhqj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtdcnszssa.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtrbysfktj.html

JS:   #private 字段；其余公开
来源：http://hz.mhx1999.top/gtxhhvwtlk.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtbiafgpbw.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gthwcreicn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnqzz.top/gtckocyxnx.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtbwpowgla.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtfqrkondi.html

[G11] getter / setter
来源：http://hz.cashguo.top/gtachwjcoh.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtmewmvutv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtvzlstalx.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtaftfxwwp.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtolfltolf.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtljjatbfe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.birdmap.top/gtnflvtonx.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtfdnomgdo.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtzpgnejwt.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtujrylhrq.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gtyftxntwy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtyetwtpfg.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtozfugfnb.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtzhkefipq.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtxygpbrjb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtkkvlykss.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtynecgezu.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gteqpxayko.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtxoisbyud.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtkubeeoid.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtobwtkykw.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtvfinfbtt.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtzdtixzhj.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gtpgoufqwi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtxfgmpwmk.html

Ruby: u.is_a?(User)
来源：http://hz.hywenlv.cn/gtnbgbseim.html

C#:   u is User
来源：http://hz.shangyingyoupin.top/gtqvqgrjtc.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gtisvyzawu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtzlwjjvxv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtsydykgfd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtkyyoymcu.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtzedlkrwj.html

Java: record User(String name, int age) {}
来源：http://hz.fengsongda.top/gtwclbrsqg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gthflzowsh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtufksveph.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtgzfxvspy.html

[G15] 枚举
来源：http://hz.jqgfzy.top/gtlfsazips.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtaexevwqd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtmamtbnpg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtjfhqrrms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtjkhoehhe.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtwdpoehaq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtldxlurau.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtfewktevg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtcohgfsxt.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtwasmlgey.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenlongwang.top/gtmwuwtduq.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtvpjunxfh.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtpcnmubst.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtrozmpcqv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtrtcbecfz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gtfyoqdcnt.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtuisgzezw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtagefuxgq.html

================================================================================
来源：http://hz.nwbrower.top/gtjtloekbn.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtlmkmzrua.html

================================================================================
来源：http://hz.52xcode.cn/gtyjgiloqm.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtegpxndtu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.bjfxy.top/gtajnhjjxb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtjfibbxkf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtfvsrtgjw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtbfweevfr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtnhdgbnoj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtcpyqijnh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtqewbshze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtubzreinr.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtvcpndamd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtgkmjoaur.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtivonbpwf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gthnjsoayy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtfaskrixq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gthlvpudoe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtsnaysqfv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtfpfhrhew.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtskllelld.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gttzgrjach.html

Py:   raise ValueError("错误信息")
来源：http://hz.yvedp.cn/gtglztirpr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtqhcyqhur.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtzdvecurl.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtwhhwpzku.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtmbvavjvh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtjicnpimt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj202588.top/gtvgcslxgm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gthgjjrjlk.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtafujhrsn.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtqupwffbi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydzc1.top/gtmfrjhdwq.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtexwplnex.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gttcecsfgl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sxryk.cn/gtemvuxujk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtqjdfpneu.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtyffoqfdh.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtrcwpsqjq.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gttrfkbptr.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtjqsokjpa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gterfzcdnx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtdvsbgnlm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtpokpddsh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtdggnpfgo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.havefunace.top/gtmlknekme.html

Ruby: rescue ArgumentError => e
来源：http://hz.guowangkeji.top/gtjmlyntnk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtwlpgtflk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtelgzkgjq.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtjmhgtkvk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtzcsfddym.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtnpdghpuu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtvcfvveqo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hfpthk.cn/gtkdcwqwbg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtejonjbgd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xinyue.icu/gtjruddvuy.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtctjyjnis.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtwhbbnhvy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtwvlgcgcs.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtciyplesv.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gthhwyoaqk.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtaropcczv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgufenzy.top/gtiexpigxx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtezwcnoui.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtnbcgdoci.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtdlphazby.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtlhswiaaf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.meibo888.top/gtosedooel.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtobkilnmr.html

JS:   e.message;  e.stack
来源：http://hz.tanke756.top/gtsojadosv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tian-w.cn/gtlpshpciq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtxqkwqvgx.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtsygjyrri.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtiumjwttc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuxming.cn/gtppevoipv.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtrssazahd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guannengcc.top/gtmuusrakk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dashuyun.cn/gtfliomzai.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtyogfjsmr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtxbzlpmet.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtgtfcoids.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtzivsgwrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guowangkeji.top/gtjtityumz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtaggoesqk.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtyqbljrjs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtzdpezxgd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnqzz.top/gtqtoiswdi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtswbmxyhs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtukhemujy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gttkxfrlix.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtrmjtzuzf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gteopgblnv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtujxugnly.html

================================================================================
来源：http://hz.jinqigufen.top/gtwafxqniv.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtzdsljwmn.html

================================================================================
来源：http://hz.jqgufenzy.top/gttmxfgfjk.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gtnemiducs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.316326.xyz/gtlxhyqbri.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtapfesidd.html

JS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtmueckpxq.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtvzaklntk.html


<!-- 参考信息 -->