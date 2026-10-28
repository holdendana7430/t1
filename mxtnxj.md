代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtzgvweuwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtuonnnbss.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtywmhtrwf.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtxaxionzh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gthkzatkyh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hywenlv.cn/gtqmypxvoy.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtafpsvsud.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtlwaokill.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gthocwrqfz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.quarkkingdee.top/gtwnsgbxtf.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtxbbcoqvn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtczhkogqu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtarjqxnxm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtdrjlglub.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtebeelauz.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtyujhlvbh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtldvjkwiq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sweek.top/gtbncwktpu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtggeeghzi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtxpdksyxl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtxckwkskn.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtwysfthwp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtxmwuvske.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gthafxqthm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtvetixhxe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gttyimglgn.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtlgcwhmti.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtvmgeghbj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gthehrhhqt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtrriruxzc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtkfruhbuy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtgaqwfiuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gthglesxwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtvnommuxj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtdjokkrmb.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtcndujxmx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtxpacdqwb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtpqrmtmkj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jiagoushi.top/gteugxebwi.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtufujbbof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhiwuduotai.top/gtxvafsbek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtvibhuabp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtwkkxzfan.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gteprseajd.html

================================================================================
来源：http://hz.jinqigufen.top/gtwibubygl.html

G. 面向对象
来源：http://hz.zycfv.cn/gtxdazblji.html

================================================================================
来源：http://hz.fzhhl.top/gthnzhyccd.html

[G01] 定义类
来源：http://hz.yj202588.top/gtyjvzfkkp.html

Py:   class User: pass
来源：http://hz.smart0.xyz/gtaiqetzwx.html

PHP:  class User {}
来源：http://hz.cashguo.top/gttjlseghc.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtuzzhsiot.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gtidtsbwbn.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtmtrvuolm.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtpckgxqvb.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtzjrvvapj.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtidjyeuwz.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtckudylyu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gtlfcytixs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtopejstrd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtyyompzgr.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gtptwcmfmd.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtkzefxvcv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtvgetmidn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtqfgargia.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gthvdlwwzx.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gtxdeemzxe.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtnsqydnct.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtuxciamxj.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtjiorxrzg.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtyprwryxd.html

Java: private String name;
来源：http://hz.xuanzx.com/gtuwwkygjp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.c1oappe.top/gtwtducuei.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtsgdkwwzm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtplmsiiem.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtbqfkjohp.html

Py:   def greet(self): return self.name
来源：http://hz.jyoumei.cn/gtoyapfuaj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cheryme.top/gtlgxaoaqc.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigufen.top/gtdljvqehd.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtikjkoawa.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gtwnxucacd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtbvsdmmhs.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtuorhgnfy.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtpcnftzox.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtqskrwyqj.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gteddiorxc.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtsdmmsbsv.html

JS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtnaoebxwj.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gthzntranw.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gttbswowwe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gttzclfzjo.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtxdneorlt.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtrdfdjwwf.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtjejxsxeb.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtidwbbqxc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtetfvifjp.html

JS:   greet() { return "admin"; }
来源：http://hz.tanke756.top/gtltvdonif.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gttvdtmrrg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtiyyygxmj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtgjcntifw.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtmttxqfwe.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtwygvkkxc.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtotsoyder.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtqkzfozih.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtnsfrcibp.html

JS:   super.greet();
来源：http://hz.ybcxt.top/gtojtaypad.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtuxffcyuw.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtgvufghgx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtshfehsfl.html

Ruby: super
来源：http://hz.yuanzhike.top/gtidmnvwad.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtuaceqgga.html

[G08] 静态方法与属性
来源：http://hz.cucudq.cn/gtcnfnfron.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtnilrenei.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtlfvyjptf.html

JS:   static f() {}
来源：http://hz.bjfxy.top/gtqwoxghiz.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtfuvuctij.html

Java: static void f() {}
来源：http://hz.cheryme.top/gtzbiydcwn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtcaddkgbf.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtxdlbdrmc.html

C#:   public static void F() {}
来源：http://hz.shzxlz.cn/gtqkzgatxe.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtofgztzcx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtmoazvftq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtnpnnysrk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtkfaatxhg.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gtgmykdvlp.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtxgakkkpa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gtkjdmrlwf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtodfxdcrr.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtitmsrzzo.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtemzuzdft.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtuoplioye.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtalciivoa.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtgaayckdg.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtsyotsmfx.html

Java: public / protected / private / 默认包级
来源：http://hz.0kj1m.cn/gtbrhufpkx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtvdvzqwoa.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gteeoeetzj.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtcgbdgcuc.html

[G11] getter / setter
来源：http://hz.jinqigfzy.top/gtcifmmjqe.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtjqkufjsw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xinyue.icu/gttoksixnq.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtprdcgoaz.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtfrlvwhvl.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtglfmxybt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtcdsdqmqn.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtxwfgwwck.html

C#:   public string Name { get; set; }
来源：http://hz.birdmap.top/gtgtbmikcn.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtoowlgwfh.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtyolxuuoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtnxfvserj.html

JS:   toString() { return this.name; }
来源：http://hz.yongpay.top/gtfionofue.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtctaqokxv.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258.top/gtmsieuvdi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtswwmoyjr.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtjmpndqav.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtjoidixar.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtaqdteeue.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtgsjquoos.html

PHP:  $u instanceof User
来源：http://hz.daxiang520.top/gtcxteddhl.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtuqrwrnca.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtbrkiurav.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gtvcpfyjmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhongyouzk.top/gtbglzeplt.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtkslxnyba.html

C#:   u is User
来源：http://hz.meibo888.top/gtvgmcqktv.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtmnsofsxo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenlongwang.top/gtzocnuetl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtpiflrlfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtcnpshabm.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gtbazutjcw.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtgdrvmhue.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtmzgobdcg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtaovoiiqq.html

C#:   record User(string Name, int Age);
来源：http://hz.sweek.top/gtpfxmovfk.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtlijslnhb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtwsrbrxxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtgohrnpzd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtwctvxish.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gttnvocevl.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtodhbkdle.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gtwzrjxnuw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtlhxdyilm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtwmsxixoy.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtqwjhljrm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gotoacloud.top/gtzlpzvsco.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtasvnbxuk.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvmfdvdka.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtiurycioo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtepclpbjp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtmksuapgr.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gtahpseqxz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtinqszjww.html

================================================================================
来源：http://hz.yj20258888.top/gtglwlmboz.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtcaopydyl.html

================================================================================
来源：http://hz.tianlin.xyz/gtqwhoapag.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtydxuemlj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtvlfbpdoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtiqskazbk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtnpcpcjtn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xziqi.cn/gttxhbqino.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hfpthk.cn/gtxlapdkbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.mhx1999.top/gtnnoxnfuq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtwnddbdsj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtecnggvwa.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtevedlsgx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtuertlufu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtlkxazuom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtpcpsbueo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtvsqcxhya.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtzzgxvyup.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtjqbmkzgy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtntyaspzu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gttfudapyh.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtqvlnkilv.html

Py:   raise ValueError("错误信息")
来源：http://hz.9152youxi.cn/gtdpamnrvb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtswzogwbp.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtednyxgqq.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtxzuktgjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtjzaujalx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yongpay.top/gtzqdgxnuv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gteqvirkxs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtwcdwkiii.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtpxlkwcgp.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gthjjphjjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtecgkbecz.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gttctwgokf.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtygfadtkc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtgngfrurt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtnlyljkqv.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtdgcczwhh.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtnixpdhxm.html

[H05] 捕获特定类型
来源：http://hz.gogol.net.cn/gtxweblopy.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtdxcmvlrn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gtqdkimmhv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtktavebez.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtdfudqizt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtgbcsviqm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtozyhlosb.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtoaimwudc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtzfdzgscj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtvcchiuye.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtsrmxmhhq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtjpwqqcqt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtdpldebes.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtcnipyaua.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtayhfbyic.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtzftpsmru.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtlktcyzlw.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtvwxvwrud.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtrbjazems.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gttsyngmyx.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtuxhdtvwb.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtnnkyaqhg.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtcvvwajzm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.9152youxi.cn/gtsjoacpgf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gthuwbhgzt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gaohongyu789.top/gtbaccsssr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gthbeqmktq.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtvcreffcl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtjbvofgof.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hywenlv.cn/gtncyigwxw.html

JS:   e.message;  e.stack
来源：http://hz.ydjk.org.cn/gtckzpwibo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtcnwkisvc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtvdapojae.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtlvavunou.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtisbndtyz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtcgnkobsi.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtmhvcsmav.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtundsyfnp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gttrftqyut.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtpjomvovm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtdhxhazpk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yvedp.cn/gtlxmtjbor.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtaldjmqbp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtyqtvqubg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtbmnrcxsl.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtvssizmuw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtbshuvixb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtfbcekmti.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtgmxobtkn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtadrpqfqj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtuybfgcuk.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtzpfgouma.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtbfohjcbf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtsuhvoukn.html

================================================================================
来源：http://hz.birdmap.top/gtbvoupqcr.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtrbvtmvvb.html

================================================================================
来源：http://hz.daxiang520.top/gtwgbzbapr.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtcaaegzkz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtplmxhazs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gtlzzpjsax.html

JS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtrroswfzq.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtgwadtozz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gtddeeypjh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtxypfaiqe.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtgclzqwop.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtblcbyjys.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtyacwywrr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtoxzfemkm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtfcfbwgly.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangkeji.top/gtnbaxiwxr.html


<!-- 参考信息 -->