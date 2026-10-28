代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtrufnvaoa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtjrvmuvsp.html

Ruby: Dir.children("dir")
来源：http://hz.hongshengwenyu.top/gtcqjdwnoi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtjsfiqjzj.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtyoxzprht.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pycfn.com/gturzyakzn.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtahsxmudm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtsmkammfa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtunbnuwxy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtihnleazi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gthihuoyrk.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtxefheufr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtgqbvayib.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtoaooonjk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gthqxddltn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuetiantiany.cn/gtjvqqurwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtjhbkuonz.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtgnzoppht.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tian-w.cn/gtibhucwuy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gthnhwmpyf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtizxekixp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gttqtdloiq.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtloihglco.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtogxjtfjj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtpwyjelyj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gttgvxizmh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtbsocdcur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtwxlztmht.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtriylefex.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtqhkxdtsj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtnlqcxenj.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtsnmytjmy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtglqysjja.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtpcjncjow.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtvqtbofab.html

TS:   // 同上
来源：http://hz.zhijiandao.cn/gtjbudynyn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtdmvnzzja.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtkzrkwguh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtyglnixsk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtxnyaepxd.html

================================================================================
来源：http://hz.ybcxt.top/gtyqgscmce.html

G. 面向对象
来源：http://hz.xuanzx.com/gtmumdjbel.html

================================================================================
来源：http://hz.dashuyun.cn/gtqlzrxkcc.html

[G01] 定义类
来源：http://hz.ehwqpu.com/gthiqekgko.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtjbvllwzy.html

PHP:  class User {}
来源：http://hz.ppjwa.cn/gtcuutejss.html

JS:   class User {}
来源：http://hz.316326.xyz/gtljzqmpbu.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtotbndbka.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtpsvpuvqk.html

Go:   type User struct { Name string }
来源：http://hz.shangyingyoupin.top/gtljxbrtjq.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtiqnicrrx.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtjzqpbzxy.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtyzwuwbsb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gteaiagipa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtoxjnbkrp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gthsdgwymc.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtgbmdmnqp.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtlsvmhmkn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtixwmpvef.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtolqaipzp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtluouqqvr.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtohdqslgc.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtwafmgciv.html

PHP:  public string $name = "x";
来源：http://hz.ehwqpu.com/gtwyolwtvx.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gteoskpoqi.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtefysltfg.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtiupqdujl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtrmhdqjld.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gttdhpyjgm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtrickmxmy.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtlvyqybbb.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtcdawnaql.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtbqzrydrm.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gtsglgkrnh.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtrtyxvwhw.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gtmnhxyvcl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtddjtfzhm.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtvswujnne.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtgyyyykvt.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtblsebkhc.html

Py:   class Admin(User): pass
来源：http://hz.yj20258.top/gttcakxvom.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtzefsontz.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtgitnjyog.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtmkrsejep.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtjmkpygvy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtrfaauxzr.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtqwlmapbh.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtmqvipurh.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gturblrykh.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtxwdanifb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gteuczdokv.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtarwkfqgo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtxicfxoeh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtnlhkrvdq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tianlin.xyz/gtvjasgeln.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtgkyeggmg.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtlkipgyou.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtxfnovhut.html

Py:   super().greet()
来源：http://hz.jqgufenzy.top/gtkbzcobtm.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtgofgxxta.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtfkhxzadi.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtbghhejkt.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtrfsxskry.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtynpwztcs.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtfsgymkid.html

C#:   base.Greet();
来源：http://hz.jqgfzy.top/gthlninobm.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtlishopmk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtlkuwejkm.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtyiuynboi.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtunobujyx.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtjrxvluve.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtrharnykg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtgabbiqmd.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtxviwmpbb.html

C#:   public static void F() {}
来源：http://hz.yvedp.cn/gtiwmbzbhk.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtobnerpfp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gaohongyu789.top/gtjnfashqv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xylfe.cn/gtdtohmnhk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cqqwz.cn/gtguxhpmei.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtdfurkahv.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtnmxvffvq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtnlimcjds.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtxtevawsw.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtzbfwuhhm.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gtqvyvdsnv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtthicenjb.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtsfxyzbdr.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtbojlpsxm.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtorkmbfuq.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtohlzyzei.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtqaztftya.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtjnvlarbl.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtxyeauzli.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtxfuvqvzh.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtfuqzsnuw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtpqfaydfr.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtioqintfj.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gthsmkjgmp.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtnzsnjgug.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtfzanrmkp.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtqypxgapg.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtbnpbgbxo.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtipoiviqg.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtymuuvrxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gthddtokar.html

JS:   toString() { return this.name; }
来源：http://hz.yanxiufei.cn/gtrozuwdje.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gttkldwsio.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtlkctwmem.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtosybjvhl.html

Ruby: def to_s; @name; end
来源：http://hz.andypj.xyz/gtkikyvnwh.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtvegwrdjm.html

[G13] 判断对象类型
来源：http://hz.yanxiufei.cn/gtphuyrdth.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtzevgtqvb.html

PHP:  $u instanceof User
来源：http://hz.ybcxt.top/gtlnqdhvew.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtdaxcvucp.html

TS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtlahkkdmn.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtlaywvrzn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jiagoushi.top/gtevfbnqgs.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtpwpgekwd.html

C#:   u is User
来源：http://hz.yonumen.top/gtfezowefk.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtqqlwjutq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gtbhlwunra.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtjjcshvio.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gteskoloap.html

TS:   type User = { name: string; age: number };
来源：http://hz.sxryk.cn/gtoiyqwfsi.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtzbnsoref.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtgfzxsjnf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtxbircnuq.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtdvdicpyu.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtxjbpmlmy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtwbcevlfl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtmznfimcx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtsqqapykd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtipudkeaa.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtrdnbxajq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shzxlz.cn/gthxbqyydu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.9152youxi.cn/gtzouztlqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtdlcmyapy.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtjuxqvggt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gticnjmpae.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtsjcwpmiy.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtrlfdufun.html

TS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtsdjxmatn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gterieruzf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtpwljnupi.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtdrwyotwp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.birdmap.top/gtmmkzaozw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfjcdmxnh.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtwgwqiljm.html

================================================================================
来源：http://hz.c1oappe.top/gtlqpqrfxg.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gtxsmlizpa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtoruhfuct.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtyzuwkhug.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtsizzwxvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gtuyqblpvr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtbfcjwxaq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xziqi.cn/gttmhwjevm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtylogeozo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtbxlraqzr.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gticgqfhuw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtgoftxklt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtxnfwqjcf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtsukjjnjq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtgnszvbrm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtiemcpbyl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtqwoyvldq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtmhqxjddx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtvrsaorom.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtmitztzpi.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtatgkplyv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtusgxkayw.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtbfoekpwy.html

TS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtepcruqru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtlcpibcoo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtzeowmnvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtrfbefdbm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gttetcxwzf.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtwailpzcl.html

Py:   class MyError(Exception): pass
来源：http://hz.tanke756.top/gtdnnqbhxi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtizquwjus.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtsbycrshj.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtzhcpcntf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtrfclwcbn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gtsanrrwzc.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtfhcioleb.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtwsedeivt.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtxhwhbbhn.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtieifyygp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtkdxivoyy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtdjrkowsl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtbkoaoajk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtvilhlpva.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtamnijqil.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gthuttlmkd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gtlsywnzgj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtglhxwqnt.html

Py:   value = d.get("k") or default
来源：http://hz.jqgufenzy.top/gtjawxseci.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtzccvsnvd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtjwyhounp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtpdlscbrn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gtvfswmakd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtilaamijh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.redwolf501.top/gtjlfseqst.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtfptczlog.html

[H07] 断言
来源：http://hz.cucudq.cn/gtzinsqrxj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ppjwa.cn/gtixlmaetg.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtnukdaddx.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtgyrsnhqo.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtoodsqshp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhongyouzk.top/gtxwryhjmk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtzmmcmcho.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtcvqnuuwb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangshuangyany.cn/gthzlhsndw.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtnagqyioh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtsbmoqnxh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtvhbnsaah.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtunbhwvcu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtooqovone.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gttuvehbfh.html

Go:   err.Error()
来源：http://hz.mhx1999.top/gtjqpuktmd.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtoirbeikb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gturloopiz.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtazyfbntt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtccsfqddb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtlqdjncxa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtjcyriorg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtstjimsqa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtqokxebmm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtsfzozsdd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtnoyttszl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtknyyhrmp.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtuqouvlft.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ywan-chungtsiang.top/gtdlhysrvm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtvbqopgok.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtnzgzpbnj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtcwsuxklg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtnutrclln.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtujovppit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnxiangtu.top/gtsqwzoikx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtzwwxbiga.html

================================================================================
来源：http://hz.meibo888.top/gtzmxbjfuk.html

I. 正则表达式
来源：http://hz.zhixingplan.top/gtfxlhnymb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtctkcpdzv.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtvmhrtdii.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtggcnutwe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtuzfybmve.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtknqoxgwr.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtimtfursu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtkxhwrxrg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtnjeabmwe.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtcejcdadr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.0kj1m.cn/gttecigyob.html

[I02] 提取所有匹配
来源：http://hz.snrcjt.cn/gtfljetuai.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtkfbtvcnx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtqqhrpzlq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gttyhuqrzx.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtqeqdlkss.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtefjyziun.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtxmorrdsj.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgufenzy.top/gtfwpnbynn.html


<!-- 参考信息 -->