代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtqkyfzarq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ywan-chungtsiang.top/gtwwjbfthg.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gttqijbvkk.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtvghyofeh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtdbsxndmp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtzzniejvh.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtbbfuaeub.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gthbrttifl.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtyskcgsku.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xinyue.icu/gttvhkwivs.html

PHP:  filesize("a.txt");
来源：http://hz.zhongyouzk.top/gtutthbpky.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtlgdkgfns.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtxvjrxopn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtuyfhtzpa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtsqsksyxo.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gtnqrlyxzk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtcvxrptpf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtqyvigbdt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtnwgkmqzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gttvlsfqyw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtucfcfvky.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtbakstqpc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtpnxqxvhn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtqlieeftv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtlwwlcrpt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gtyojluamv.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gttsvkjlhz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtbishltpf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtmpmqafwa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtkpndgbhe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtzqmwmhrm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtzzqvpgyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtslrhedrw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtxcrlttcf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.c1oappe.top/gtccqitobk.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtmhxpqugg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtvnybovut.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtktqrbkvo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtgoiouuqu.html

TS:   // 同上
来源：http://hz.ivvv.top/gtqwciwlko.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jianghu66.top/gtojkcmwjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtlauqkxhi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtqcbzrnrd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtnspmkbou.html

================================================================================
来源：http://hz.nwbrower.top/gtzkiiqlrh.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtamdujkem.html

================================================================================
来源：http://hz.fzhhl.top/gtatgpabcz.html

[G01] 定义类
来源：http://hz.meibo888.top/gtadmfdguc.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtbporkinl.html

PHP:  class User {}
来源：http://hz.c1oappe.top/gtklezkhfc.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtepzxgeot.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigfzy.top/gtclfwgekk.html

Java: class User {}
来源：http://hz.wangdashe.top/gtnrebqjbc.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtcudlhmkc.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtbtqcutpm.html

C#:   class User {}
来源：http://hz.yonumen.top/gtnnkcbhsc.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtmuuifxcu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hywenlv.cn/gtwuacmnmm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtvyivmzjd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtxdgtgtct.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtuzapnvjj.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtsbshmuvc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtltxktbwo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtmizfepin.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtluqwipkq.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtxiclulst.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gttsjxndqi.html

PHP:  public string $name = "x";
来源：http://hz.hnxiangtu.top/gtkgarbmhj.html

JS:   this.name = "x";
来源：http://hz.hnxiangtu.top/gtwbmpqewp.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gtamkggrlf.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtzthrjeyx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtszgjfvey.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtfxyejlgj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtqdrohecn.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtatrgairz.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtkdrgqsur.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtizopwuci.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtdzdlzxzt.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtdprxokso.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtputiiosk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtgfzkelwm.html

Ruby: def greet; @name; end
来源：http://hz.jianghu66.top/gtouamukkt.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtitqsmynb.html

[G05] 继承
来源：http://hz.cheryme.top/gtrmemjkwx.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtbgannhgo.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtdsatwrxx.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtkpwrjevk.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtmpszngdf.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtiovsbsyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtvfpjbxbd.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtrpaxilkd.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtbkgkeabk.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtnnaltozc.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtoitgcukf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtsgqieyfk.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtqxenoblr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtxiwhzpky.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtwbhwwqik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtnvddfvpm.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtzvfdjelh.html

C#:   public override string Greet() => "admin";
来源：http://hz.tianlin.xyz/gtnhzcirsc.html

[G07] 调用父类方法
来源：http://hz.sweek.top/gtcarbarav.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtrpjexgyr.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtgfjfupcj.html

JS:   super.greet();
来源：http://hz.ybcxt.top/gtmfevqjyc.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gtiwjnbtkq.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtohlbroce.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sufxvd.cn/gtfiekekxt.html

Ruby: super
来源：http://hz.yj20258888.top/gtubrzhlmi.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtjsonhksy.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtnbrqivps.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gttbwhfmic.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtkyapfsns.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gthyvzggih.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtliavchkt.html

Java: static void f() {}
来源：http://hz.ydjk.org.cn/gtxxmjfcdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gtidawozpp.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtokksssvm.html

C#:   public static void F() {}
来源：http://hz.xylfe.cn/gtqcalovtj.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtoepevrah.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cucudq.cn/gttxukmaws.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.iojbl.cn/gtcfhogdog.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gtfiqnybpb.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtiosvfsph.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtitceufjl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtdofbylgj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dashuyun.cn/gtxebonkyk.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtnvnybwfb.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtvlkevmuc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtpzfdotdr.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtfiztidmi.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtwhvvyuns.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtplpwitdd.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gtdrwcpewe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtrtrfdkuy.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtmbvbvoin.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtgdpvwfkw.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtxzsoicjj.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gthjyipefs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtcfmyzvnc.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtlfbtibaj.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtdisogfvi.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtakmoypuk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cdnleiting.top/gtodevtrjj.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtpzcffzqi.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtwwczuyvb.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtfbfaniao.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtxeomtjra.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtluugdcyn.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtcmzltyrv.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gthkyyfnmj.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtfouzexjk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtjqfmrogg.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtruuunspx.html

C#:   public override string ToString() => Name;
来源：http://hz.guowangkeji.top/gtpdrpzopl.html

[G13] 判断对象类型
来源：http://hz.jinyuanbaomall.cn/gtcewanybt.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtafxbxpye.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtilbwnznq.html

JS:   u instanceof User
来源：http://hz.yj20258888.top/gtxomhqrkr.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtmelijnmx.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtamuyohuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtqqatxuue.html

Ruby: u.is_a?(User)
来源：http://hz.hammf.cn/gtbvxeekle.html

C#:   u is User
来源：http://hz.cucudq.cn/gtlsgbmpfq.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtvqmfwvzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtbwocmdoa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtztocwvbh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gtpskxsrwv.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtbtjfarot.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtyzxcclse.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtuadtcmyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtjtyxhpqr.html

C#:   record User(string Name, int Age);
来源：http://hz.nwbrower.top/gtmgathbzq.html

[G15] 枚举
来源：http://hz.tanke756.top/gttnygxejf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtsuzskvbj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtrptoiydr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtbgxobbat.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtdevxkukz.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gteobokxne.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtzlajwqwy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtrmzfwxtj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtbtfwmfwj.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtezlotgng.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nwbrower.top/gtfiqndtgd.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtijuyfcis.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gttacdbexn.html

TS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtjhjfvpat.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtvhneitiq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtomkwtaga.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtnogohgzu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtzkqqlhug.html

================================================================================
来源：http://hz.zhoulong.xyz/gtachftfuk.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtwumfjisd.html

================================================================================
来源：http://hz.yuxming.cn/gticiqwmbi.html

[H01] try / catch 基础
来源：http://hz.pycfn.com/gtpkhzqknw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtapsqzmhx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtxhtmdqbx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtvehdilwb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtsovqhrjq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtwtrpoyru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtjedtqjos.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gtpwwrknar.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ppjwa.cn/gtrrgotrry.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtslcnjjqw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtxliazyje.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtvhygwpyv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtslareqod.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtvyungbgf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtxxolqlii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtzxnxangn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtjtkxizjc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtbgsqwmyi.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtnkusbohl.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtwtwuxlit.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtzefknxwp.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gttinxohqo.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtrheykkop.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtpebdpavl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gthhppcrtb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtqheymnok.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtdozcbmvk.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtpvdfgpwz.html

Py:   class MyError(Exception): pass
来源：http://hz.redwolf501.top/gtajaybeku.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtmlbosqtv.html

JS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtqmvvyfqm.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtargxxpcr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtnfgaogdj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fzhhl.top/gtofcyrqll.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtllejbpfb.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtdanuattm.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gthcdfoact.html

Py:   except ValueError as e:
来源：http://hz.gzhubu.top/gtbytosjhm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gttzomzwao.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtpbhvpgcv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtkgisxlib.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtwxiaqdhy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gtajfvwpvi.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtjxgjtocx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtjinqwklj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtzlgbjrhb.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gtrqgcrhxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gtmdqnkmzj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtcmaksxxf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gttzmeeqqc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtblrqxvbb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtukskqxnu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtmcijadci.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtenfuogru.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtbflvzidj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gteknvozzx.html

PHP:  assert($x > 0);
来源：http://hz.zhiwuduotai.top/gttdgiihua.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtjmrwrswe.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtsiffcjsd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gternzxlsu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhixingplan.top/gtkwbopxwy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yangfankeji.com/gtilwdczsj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtkczivlqn.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtjzqbrxop.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtciodcyhk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guannengcc.top/gtkqpmtsqm.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gthheenydn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtoakibdto.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cucudq.cn/gtqrlrawwh.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtcfxoqzcj.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtnyyjabsv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtsmwjncld.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gttiiqldfx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gtdmktqfub.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtzsvksqrb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtnrpsenre.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtlpelhsrf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtvgdjpqwq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtqbdbajgu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtfrcqvqjp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gtnkaglgbu.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gtkikovckp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtylzbhabm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pycfn.com/gtykxbtcub.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtcrsptlnl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtunxkrpmm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtkvrougdb.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gttfyikqmn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgufenzy.top/gtvunrocpg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtuytxtkvq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtommgcodk.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtmwngictw.html

================================================================================
来源：http://hz.cashguo.top/gtveudbcxu.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtnmwqhapi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtiglifsau.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtgnevfurr.html

JS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtkaswixze.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtguxuohzm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtfbjrdcmx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gthcktliuj.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gttsyzbhbx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtspqdfhjd.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtyoudkmte.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pycfn.com/gtokiaquez.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gotoacloud.top/gtkfxjfaun.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtovdktkao.html


<!-- 参考信息 -->