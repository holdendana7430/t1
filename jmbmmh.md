代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtrsnttjgp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtxgubnjfm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gthjlvybdo.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtgahwbpnh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtncfhfyox.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtxwbzwche.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtxrwkjcbr.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtladnbber.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtrilhdhyw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhaomingkeji.xyz/gthgfqoavh.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtwkmefcou.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtmjjgoafb.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtooluihej.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtquvrrsgi.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtxyhsqcyl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtmdhmuwyh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtkfqvnsrb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtaylrskwz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtcttiwpki.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtynyvzilk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtecrtadwu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuetiantiany.cn/gtusdzydnb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtvhlgsfxh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gtgecunnoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtuoldstrs.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gtcygzvxlw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtbmkqjjeo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtxhomixbi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtoogrxebg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtqxuyqtps.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtfkuwuviv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtrfvcxpls.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtldpvqyle.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtstnpzkzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtarmulzxr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gteaeebeyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtlsvcbvyu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtxyvsnvqj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtswrxaett.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtqrtlypnu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtijdrzequ.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtxkgeeuni.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtbuhbrusn.html

TS:   // 同上
来源：http://hz.meibo888.top/gtrtmaqiqr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jianghu66.top/gtgudijezo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtbhqqzmst.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydjk.org.cn/gtrirzsbok.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtoholiqwf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyeelxbnv.html

G. 面向对象
来源：http://hz.ydzc1.top/gtfrdoyynp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtozplrsht.html

[G01] 定义类
来源：http://hz.shangyingyoupin.top/gtenxfnwbg.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtsykvmktj.html

PHP:  class User {}
来源：http://hz.ywan-chungtsiang.top/gthfnoeuil.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtygygcmwz.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtttinnilp.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtlrlwodct.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtwlmrsxkg.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtzbhetwow.html

C#:   class User {}
来源：http://hz.ivvv.top/gttdpcdrzb.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtlyqbddia.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gtbhvepmwt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtmzfdyewp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtmgopdkrl.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gtvuqqyawr.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtrazkwpbp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigufen.top/gtkufyhkbp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtvrfifbhi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtdjelhonc.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtsinjltnw.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtsvrbbbsv.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtakvflxer.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtcbofavli.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtgflcwesl.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtxqirpjrb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtlbsxuegq.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gtnojsctax.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gtqqkuezdi.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtjfmmqflw.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtxyzcuwtk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtjcbclndt.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtujtzpagm.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtsdeeeztj.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gttcstgiep.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gtobrnnnwv.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtieefelko.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gttpmuyoko.html

[G05] 继承
来源：http://hz.gzhubu.top/gtbzknxstq.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtflfjotco.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtesvasyvw.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtfnvszpfm.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtivnywbhs.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtholvcrof.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtxltssiul.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtdxshlnts.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtoznpemve.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtdmfkovqu.html

Py:   def greet(self): return "admin"
来源：http://hz.ivvv.top/gtoiifmtoe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtotrdfvdy.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtovtfskyy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtxflumvhn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtagdjdqui.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtnsfyalmg.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtewynucwz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258888.top/gtokopmotj.html

[G07] 调用父类方法
来源：http://hz.daria6918.cn/gtgtgljwyx.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtxzmxjypo.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtywugnqie.html

JS:   super.greet();
来源：http://hz.sweek.top/gtuikrcgsy.html

TS:   super.greet();
来源：http://hz.zdqjudy.top/gtypuzvprf.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtrocfinbe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gttgsgpfvl.html

Ruby: super
来源：http://hz.bjfxy.top/gtxvtlgbtd.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtyyxcmenb.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtihcmzhgt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtrpjxwoxu.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtwrvudtvg.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtszxagcoe.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gthmwhzwko.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtvkrqbwxm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cashguo.top/gtcpyrebfu.html

Ruby: def self.f; end
来源：http://hz.yueranfly.top/gtjzdpqbug.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtvqefqepb.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtdwgazyhi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtxduplaff.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.kuanghao11.cn/gtislcgkaz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtxwsaeync.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtyishgvlx.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtisrtomvi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.svipenyu.cn/gtkhqezjln.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtkqelrnhe.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gtbdraiyno.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtrsgboydg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtfebpkknd.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gtnveknkun.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtcxrakkjs.html

TS:   public / protected / private
来源：http://hz.tianlin.xyz/gtrspvqbno.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtmksrwrtt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cashguo.top/gttzjercwf.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gtyzkccklr.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtddoijfet.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtdokdtfmo.html

Py:   @property 与 @x.setter
来源：http://hz.sxryk.cn/gttfremomh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtuwqevtbw.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtmmdjnvkn.html

TS:   get name(): string { return this._name; }
来源：http://hz.tianlin.xyz/gthomifpwa.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gteagpkuom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtlezkafsy.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtlaelybop.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtrqbzmgkj.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtdqrxuohq.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtogildvje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtuvzxzxzy.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtlgbellog.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtyunycajp.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtkxbcobcq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtmprbicds.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtzwuqyxdv.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtmttczyve.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtqjqcftkr.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtlabeyepa.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gteozyjqum.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gttdgazgea.html

TS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtesnsvfej.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtwigybxwr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xinyue.icu/gtzrtwizar.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtiwqrcbki.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtflffxooh.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtjnihvdcq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtnrmmlueg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gteehyqrnk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gttalamaov.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtaglcbqax.html

Java: record User(String name, int age) {}
来源：http://hz.nanxuanxn.top/gtfsbeoifb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gtslzvjsox.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhijiandao.cn/gtdnsaufjc.html

C#:   record User(string Name, int Age);
来源：http://hz.ydjk.org.cn/gtjxvvnxvf.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtqqdqinmj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtrkjczony.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtkrtmkibn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtguovbhay.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gthidjnoek.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtkznifljo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtwihnafgn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cheryme.top/gtybttnkqr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtstoijyew.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtsbxgzmqq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ivvv.top/gtcahrvejv.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtkhsyjqhl.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtfqrydcwf.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtauosvzax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtzwfknuge.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.mhx1999.top/gtwhsiemii.html

Ruby: obj.instance_variables
来源：http://hz.ydzc1.top/gtekfxuisu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtdrtrysdw.html

================================================================================
来源：http://hz.yuxming.cn/gtoxqmxgri.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtodsmzxpy.html

================================================================================
来源：http://hz.yuxming.cn/gtoojkfybw.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gtqeykscby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fengsongda.top/gtghzxfpsc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtgvoqwhdm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtqwvhbxxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtnsowwaes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtgvehlenv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtawsagaom.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtzzzvxkqq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gtqbumxeoo.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtgsadvrha.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtcrpshqgj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtnyvpcyuf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtyileqjlv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtgvjaxael.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtumodroop.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtmhrjwrns.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtvsnljwnb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtfylkwdxu.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtxutbperb.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtthhyypls.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtfolghtef.html

JS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtxbdznhwk.html

TS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtyhzkwocj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtlsxnyndl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hongshengwenyu.top/gtqsehjcyi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtnnnmfvjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtncvhjyah.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtxjzefyfa.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtedsnzdtg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtbqdlkmdd.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtysamansn.html

TS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtluokeiyw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydzc1.top/gtajvmnbwv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtbflvlufr.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtufpunydc.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gttgokulxz.html

[H05] 捕获特定类型
来源：http://hz.yonumen.top/gtixwtrlig.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gthogtqoys.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtxpvpzaor.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtupvbljfx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gteqvpiuwz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtpygxrihk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtdjudgxss.html

Ruby: rescue ArgumentError => e
来源：http://hz.cqqwz.cn/gtpbiffvsj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtbmblgcyl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtnjwctjub.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtolyfvmly.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtxxpcyfzd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtfhcmtlxl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtjcjtxxoc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtydhlizup.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtgpjpphmj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtzrmblghi.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtipczntvx.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtnyzuyhch.html

Py:   assert x > 0, "必须为正"
来源：http://hz.havefunace.top/gtbgbkwyyx.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtlojnhqtz.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtonvfqcxo.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtlwjfrmgl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gtnvbrpkbg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtixbtbtfd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtdmzbiukz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtxodkntjw.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtawchdryn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtasjfllzc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gttegopxhn.html

JS:   e.message;  e.stack
来源：http://hz.svipenyu.cn/gtprtwxvio.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtmwinfgxd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fzhhl.top/gtnqcficzd.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gttmappezb.html

Ruby: e.message;  e.backtrace
来源：http://hz.havefunace.top/gtnchpkkjn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gteuadwujm.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtfaowdada.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtucvjgpas.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gthmznzphn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guowangkeji.top/gtxiwofwtu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtkauntcsf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinghuilouyu.cn/gtcshcbbyp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtccbaltlr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gtncidioxx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgfzy.top/gttzfwxusn.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtzitjqcme.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtsttlnhsr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtmkrkaapn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtpmglzmyi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtxicqhizd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtzvlaoyil.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtbemfrtan.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtxtuvlwmn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtlupokkma.html

================================================================================
来源：http://hz.hywenlv.cn/gtfipjpovb.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtiikjnphp.html

================================================================================
来源：http://hz.jyoumei.cn/gtfearbbht.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtcgwgxjbh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtgzfnuiay.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtuztvghin.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtmolpbaqq.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtovvzdmsy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtngageibq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtzntmoebn.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtbipvsejp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gtrdogkjva.html


<!-- 参考信息 -->