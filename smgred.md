代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtknezchzj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jlsjyb.cn/gtrrmaqdoo.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gthivrdjde.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtzogdfbgm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtdhmjxmts.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydjk.org.cn/gtzzqjepea.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtrydiowax.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtnvknkmaz.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gtvwcstzza.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtnupdiuir.html

PHP:  filesize("a.txt");
来源：http://hz.zhoulong.xyz/gtpwznzdaz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtcwhitvbl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gttmsmofqx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtavvukuxs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtwujlbjru.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gttojwsjrj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuanzx.com/gtrchwzsgm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gthiqplxwf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtcevshlab.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtutciyzel.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtebipatnt.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtdmpbvaim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gthxkeicrt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtvbplbrmj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtfwqxnpdo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtxehoawlo.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtmqbzwvgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtmlrprwmc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnxiangtu.top/gtpbquphlm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtplxdynkn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtvtfgoetx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gthwzvkjcu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtcocsoknv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gthgvyhrhd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.mhx1999.top/gtjmxaciyt.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtskdggqaf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtywsctwvk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtwatmbkwx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtaluxvzkz.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtwnfpyybo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gtvmmifabq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cucudq.cn/gttlvstfxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydzc1.top/gtepecehte.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jiagoushi.top/gtaehvmept.html

================================================================================
来源：http://hz.iojbl.cn/gtwaifvetx.html

G. 面向对象
来源：http://hz.hnqzz.top/gttgtxdtip.html

================================================================================
来源：http://hz.kuanghao11.cn/gtqiekplfs.html

[G01] 定义类
来源：http://hz.ydzc1.top/gthdhevudu.html

Py:   class User: pass
来源：http://hz.yuanzhike.top/gtfaaroqcn.html

PHP:  class User {}
来源：http://hz.haohaochexian.top/gtujoynfxq.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtndtusfrh.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtlqiikowv.html

Java: class User {}
来源：http://hz.gogol.net.cn/gtmxtzrziu.html

Go:   type User struct { Name string }
来源：http://hz.smart0.xyz/gtttuqmzty.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtintrvzom.html

C#:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtzqfhylfb.html

[G02] 构造函数
来源：http://hz.iojbl.cn/gtwrcpterf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtsbhuajsx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtltwtcykl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtdknwiyjq.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtimnmobql.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtkownbfli.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gttruhfmjc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ppjwa.cn/gtxstmasup.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtupzzyckr.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtvgnxzwtx.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtrquekhzs.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtoebealsx.html

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtraqkllmj.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtpkdjebfq.html

Java: private String name;
来源：http://hz.gzhubu.top/gtixvgppeu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtnnumnyhg.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtwbbrbpmm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtstyxwekh.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gthyvxsbni.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtiskxhjhm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtsttnphuv.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtfzgawoes.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtjfaxlwqc.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtjvgvbimu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtezolpaan.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtmjahgxuy.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtytygmvta.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtzyasicvt.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtyyuctqsc.html

PHP:  class Admin extends User {}
来源：http://hz.52xcode.cn/gtoxjgncxq.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtljqtwywh.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtgczjfmfy.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtwjruxhqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtfleecmsf.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtxyngxnxf.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtndqvoaxt.html

[G06] 重写方法
来源：http://hz.nanxuanxn.top/gtltibasta.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtklovhkjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtrfsoaixd.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtcrnpdzwp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtnyhlxwcm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtclichzwz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sysykeji.top/gtzdnmfrme.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtkzqugtek.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtxegqlnsd.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtxxzdhgmw.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtuheqaydz.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gthexgvpzh.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtdzfpihgs.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtjqrhvqbq.html

Java: super.greet();
来源：http://hz.yj202588.top/gtgelsafcx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.bjfxy.top/gtuofgeywe.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtoogjexdz.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtvsnmpspw.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtsqtzctkm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtfcczicjp.html

PHP:  public static function f() {}
来源：http://hz.aibaodan.cn/gtfjjkduvi.html

JS:   static f() {}
来源：http://hz.sweek.top/gttquwcabl.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtpjnlnvbt.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtvgtfsnaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtugccjcwf.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gthbyhnvaa.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gtoaaymzsr.html

[G09] 接口 / 抽象类
来源：http://hz.gaohongyu789.top/gtcierzszn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtjfhmhtif.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtomqeshfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtlgsqqddq.html

TS:   interface Shape { area(): number; }
来源：http://hz.guannengcc.top/gtrligbzav.html

Java: interface Shape { double area(); }
来源：http://hz.yanxiufei.cn/gthwdeuqbq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtfivyfdcc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtxwcoaawa.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangtech.top/gttxsxbsft.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtqtljgsau.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gterbqqsmu.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtxuslvtzi.html

JS:   #private 字段；其余公开
来源：http://hz.ydzc1.top/gtlwqgouqw.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtmpvlvgmo.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtdbhzcdgh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtbshczoin.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtabhmrkzx.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtlwiclbnl.html

[G11] getter / setter
来源：http://hz.yongpay.top/gtsmkzienh.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtbwxtuvqr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtfihqacmg.html

JS:   get name() { return this._name; }
来源：http://hz.zhiwuduotai.top/gtcueuozpj.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtglnijwfj.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtlstcgakg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtxezaiima.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtrdbdevqc.html

C#:   public string Name { get; set; }
来源：http://hz.yuxming.cn/gtslfjuzqb.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtzptqyadl.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gthwkcfyru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtsdkrdufd.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtcqyixaxa.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtwmmqhzwu.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtlccbwflw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtvbvrktsn.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtzgzwsggj.html

C#:   public override string ToString() => Name;
来源：http://hz.daria6918.cn/gtwiygqidp.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtknjzvzmx.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gttrzemwws.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gtmpehyttl.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtiglrywea.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtsbpoknoo.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtuzxqowww.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtggokfxll.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gttltfnkje.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtcovnoghm.html

[G14] 数据类 / record
来源：http://hz.birdmap.top/gtmxszhtqv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtfccanaqe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtbegllzzh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtnibcgxcg.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtoxcxintz.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gtxddzjxex.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtmdkmooem.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtfkyvqold.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtdmlyncop.html

[G15] 枚举
来源：http://hz.tian-w.cn/gtgswqmfkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtgwplxtnj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtvsdfuscr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtobllvpps.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtqliyhkyd.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtiupjszax.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtfpbnnfyb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gthbihxhlc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtdpclhkgu.html

[G16] 对象转数组 / 字典
来源：http://hz.gaohongyu789.top/gtjotmxndc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtvjohrvyo.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtwrioaxjw.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtwmzvycix.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtkrwmooop.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtnpunoalg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtelpfqqlc.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtmjxbqqyh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtkifmfmxv.html

================================================================================
来源：http://hz.yj20258.top/gtqfhfnhst.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtllgsqjtr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyhjoychl.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gthkvbgtbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtsredqfnx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtyghckgck.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtlgjxtoio.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtiexgvzsz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj20258888.top/gtkwdhdgyn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtzwggoqfr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtxthccrjf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtmvoeyuce.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtmvpeycmy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtsctoejbg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtbmpidrok.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtzaazurkx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtngzowzlt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtizlwcnvm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtcatxnbiu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtzvrxvxgi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtsvkibpks.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtttqrdonn.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtgkhqfezs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtbwaspcvk.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtjnlcgzia.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtpedojbxm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtxpfxeqgm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtuhzorghw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtmwbhjwki.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtyodkjbzm.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtknfxnuek.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtiuinamds.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gthjqenvka.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtybiopewk.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtdpqjevyg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtyinsiijd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtfqzsoicw.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtjazyfvwk.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtizukycjv.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtynemmtfe.html

Py:   except ValueError as e:
来源：http://hz.tian-w.cn/gteysyqlvg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtuuerivlj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtavenlmvb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtsptjwrau.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtkfeczngc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtztekfkyj.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtiosnuzew.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtnahcsluh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtzqylbsju.html

Py:   value = d.get("k") or default
来源：http://hz.dianchejie.cn/gtldlcnojv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtdauyntgi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtoacxzqcr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtxukhlwwt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtqsankrlo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtarxjxmhi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gtocfwulqa.html

C#:   obj?.A?.B ?? default
来源：http://hz.sweek.top/gtchhdzobt.html

[H07] 断言
来源：http://hz.xinyue.icu/gtrknflydm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtqetwrkki.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtjiytzaiv.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtonvdxkfe.html

TS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtqwnnzluj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtamxxhslt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yongpay.top/gtbysgzzqw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtsswbazru.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtvztsopbl.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gtxwgobmaw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtbqkwpinu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gtolbzhopa.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtlfsgvxzq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtatyunsol.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gtcwwtqojl.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtsdgiujai.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtypxnswnt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtpyoliyaf.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtgvgxxoms.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtrzzmzmal.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtuzxvghxj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtkcpmygma.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenjidiqi.icu/gtrnodmjqb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtpvmrhsqu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtkqewmnzw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtiauycqez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtjskgjwrp.html

[H10] 资源自动释放
来源：http://hz.tian-w.cn/gtzarygkcn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hysaishi.cn/gtkdgtnwmx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtwstswypg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gteowcsaag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtltxkrbdd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtrrqegblt.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtnpvqpzpx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtlhrzfoxh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtwmbqdabj.html

================================================================================
来源：http://hz.aizwys.cn/gtqqamvlym.html

I. 正则表达式
来源：http://hz.zhixingplan.top/gtjzwlluxz.html

================================================================================
来源：http://hz.52xcode.cn/gtwzfbcnhn.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtqmkiyyls.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtrtihrpuu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtielsmyzs.html

JS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtmzgkflsi.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtxlglzevz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gtgylfjzqs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtqmreapjb.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtfgdpmbcz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jlsjyb.cn/gtuqakrwic.html

[I02] 提取所有匹配
来源：http://hz.jinqigfzy.top/gtasxygans.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtauletqzj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtxtjoebiu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtgwjfxrfh.html


<!-- 参考信息 -->