代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juphgpkp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcnjbkus.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jiyahubn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxmkkjiq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jjhuypjd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3llkpgfhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fthlgcrb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kftfmnow.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oibozfli.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moyfymmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mtrpjwqd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eopmcrkp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bqminezh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bcmaouus.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wekrefay.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mqoworhn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3afsotzxz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ezcxbxnw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lnaqukew.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3spgxexme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqetxszu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gymvnkpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oydqkige.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nansetps.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bwejripk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cynfshku.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3toilklog.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3otnjheps.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gqhfcjum.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jywdnqah.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ormrsgss.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3djwhjmtl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3luggugkn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ympgtpdp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bnjqfwhc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czsinkch.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uwqbdjeo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vvbjkzhh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qjtyjfnq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uyvvzkwi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3atfsqpgy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rvneumbm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zqqdczlc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xuetrnxp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3basmdrul.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mmeouxmh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3yzmkzwew.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xtmhfuom.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fniimttq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tswrwbuo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dmywbyus.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uwmmrleg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eagqzdok.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lrevbzfp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iuouwird.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nbadkrxs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bttbtjoz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ikbnhyat.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rmtsqavs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iyilgzsh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mphuubao.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vyyumary.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rbnzghem.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3unhzysao.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shapqjtq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dfafbdkm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3adythdmy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wttbqsop.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ppqdrzrl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zzpksdqq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vnraihqr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fesmgvov.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yktjccyz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeyndrcy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ntjdvuzj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmueamhu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qcpcyvfu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3sfneftbb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rkctiwop.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qeqzmgjp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3htxpyhwm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iqfslcor.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3acughbtn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ffreorcj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pdclqzim.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qrkcabjk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pnxyqtiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dykuntxc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tkjttlnf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3udblnkfj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqznmbvr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3puvoodpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3iocsdrqp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3oycngsrc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3scoibrfx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rcspzxto.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pppkckio.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxyxehrr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dtjmzsdd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjrtwzbo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jphpgmxg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hgeiwqkg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ycttczzx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkastdn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zuwnivwt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cvvyazju.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zxwbiarr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3unutwonk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fnarllkl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tseidnke.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkpykh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dbaswawd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3sdanpdrr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qrmzxjyd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bfmgfaua.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dflppgem.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cwoutrvk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxivlkz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfxstdhr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fevikepl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eyuzuypp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lycyuwqj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhmptidj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oqrvaidn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3latubzih.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvcfggas.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arktjvqf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jvxgdkja.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jplvvjeu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbnjdtyh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vlnbyyke.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eziybfpn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3iolmvylp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zctmrcss.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qvvdebxi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xawuuabb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mdarovkv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3aoyqfkjf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bimbnwgl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qvybyznv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tlpfyeeo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ychscfgg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iahqifks.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dfexybvq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qgisamci.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohjqblws.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3eyourajl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nlxgbiof.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3liuzizim.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mjzzxbjd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rlxsmsgm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lnzoyjhz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zwhsweux.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nibnvqom.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3shxjqsnz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nnupqixd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3iuawwred.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsbydlw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3oshvpmnl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dvswvcoe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wbyhlamy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sznmdbvg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbbbeulm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yeggguep.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ufhtbwrd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ezbsczny.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fkcqiufk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iindqpvs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oqhxfrno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3escschea.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gyladegv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bgaebteu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bnthtpvn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3olxovxww.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3arjfptbh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qsvuntgp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hfedvsca.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfmcnxer.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wcazjzje.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kqpocoar.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3aqysbsbh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pljirbgc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqxerjjl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slhywysi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhndkzx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3onrjnzyp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbuelrwa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkisubnm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lgahnudp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nzgrsqqv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cjhiioca.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3srftpxir.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3grsrgnef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3arbrhhpw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmxwzfh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kthtjbpi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vwvloexc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfrymyva.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ajnnzeps.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywfyotma.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tshtnzve.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqdxefdb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecgxrcdk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qujpnbbv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwdbdedc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuebhjhp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwwskkhd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lzyjbkgf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ayrzlgxy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymsbflxd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhicklla.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcorogiv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nctlvgbj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iqigibwx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3clxtmxsy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mcmgdbek.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lonxkydw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ovdambys.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tjzqlrmp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wksboyuz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bdftsizq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vthcstci.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtkgcsk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uzrtvggs.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ktgnrsjj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ledcakll.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qqilgpwv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yunsodxj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3danjsdhu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yrmrknmg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hqiukyos.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mhtfvujf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3keukjswh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vjxdfkje.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ykodnkzo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xpikgmew.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lusfkyvc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ffuztxrb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3edvvlhai.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kvkwljdm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zvpwkbfp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3exxmcluy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hvlxyhzg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3isbefxaa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dtstnytu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3qnvboyuy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qhoxhjcf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqpuqkdk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aiacrfmm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfbjlih.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ldbkueit.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ptydzexr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3txftmvda.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3akffxcrd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3svzbrgzv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jnzwemlv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vjpaoyhn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ykqnmqcg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hixwugod.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cyzhaelt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpvvkdak.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xsdmnlsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxvdkqds.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3tppdvzki.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvluhkb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ntcqehnz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woqxhpwx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iowygbnm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3yqmvwuug.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3iahjgymv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qfidsvrk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lruadwqc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mwzyfbgi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3luwynumz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3prkoynpi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zpssoyds.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3sbfschov.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fglnuymp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lcnhfnji.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ypvpkwjr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jgotexhl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tkbweypq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ghxubciq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bagsxhyn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gstebpvf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rexfgymd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqcrcycw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3qccyhkaz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3asjzkgkl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vqrdxmtc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dyeecboe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vewyqbfr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xxjbkreh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bnhpyvbh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nqwqtnud.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zrcaidak.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ubmynkba.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3csebrbms.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jficphnm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bayxqgkd.html


<!-- 参考信息 -->