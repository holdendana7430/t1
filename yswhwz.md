代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtywmnvutu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtoyyjwdmn.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtpotsappy.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtewvldurw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtgvkilxnx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gthwswxvlo.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gtbmdxlpnj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtdyumznpr.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtawoszjpc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gthvqlzkcn.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtobhlwjfr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtzdhilipy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtcmtadhbx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtuxiyqrbo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.svipenyu.cn/gtpfymvcyr.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtnkmlkwnz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gthyadsgsb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtrusqobgr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtkbppvzco.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtafoypiob.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtuvzyhpbx.html

TS:   path.extname("a.txt")
来源：http://hz.dianchejie.cn/gtwteaxkma.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtflylvmjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtugnugwim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtijcxmnjj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gtmgmxjlrk.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtqwguukvo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gthibxksmn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gttenvkypi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtodqadfze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtksmzenkd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtvseujsmo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtlzzgsxbl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtsfytiqoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtvvkpsolw.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtspxrdmdc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigufen.top/gtvcmaapxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtzogwbmhn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuanzhike.top/gtdmdhqhmy.html

TS:   // 同上
来源：http://hz.pycfn.com/gtbvuobwst.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtjzwklcve.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtwpfwuxze.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtliloxdir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtekknzfec.html

================================================================================
来源：http://hz.yueranfly.top/gtrpdiezrw.html

G. 面向对象
来源：http://hz.ydzc1.top/gtvdperhgq.html

================================================================================
来源：http://hz.jinqigufen.top/gtsqkxxisi.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtubtposzs.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gteyiasxqt.html

PHP:  class User {}
来源：http://hz.zhengqikj.top/gttzfrryui.html

JS:   class User {}
来源：http://hz.sweek.top/gtgkkpdckd.html

TS:   class User { name: string = ""; }
来源：http://hz.redwolf501.top/gtmeblvyuk.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtvgavdsaw.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gttevnnigl.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtmkikcvsu.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtvzchqwmi.html

[G02] 构造函数
来源：http://hz.52xcode.cn/gtrbhoeihu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtpqjhuwnd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtkbklszrt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtuuyxhtea.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtezixgfex.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtgggrsawj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gtmbinolxw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ivvv.top/gtrmwfyjiz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gtmvevxjxq.html

[G03] 实例属性
来源：http://hz.sweek.top/gtnhulsnmz.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtyromdiij.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtmtzxscdu.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtygayyird.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gthwfelunc.html

Java: private String name;
来源：http://hz.sweek.top/gtveshbkzw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtwvyojdgq.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtbndqstuk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenzaomai.com/gtftwrkrbi.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtibsbutfc.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtnhosljkz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtxowmrxey.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gttaxxfsxu.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtfbsniwft.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtdbelgihe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtcfhgcqnl.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtqxsdngah.html

C#:   public string Greet() => Name;
来源：http://hz.redwolf501.top/gtlakftkmn.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtoaxnuujl.html

Py:   class Admin(User): pass
来源：http://hz.kuanghao11.cn/gtwgawoalf.html

PHP:  class Admin extends User {}
来源：http://hz.hnqzz.top/gtgsofcizf.html

JS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtpumrcvts.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtrxmbblkd.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtnzymoxwc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtwfrqpvso.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtvorkzgnr.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtnmteebdp.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gtwzgbesqn.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtkocjqxqr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtwjiyskmw.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtibwwdfej.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gthnjcfqpk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtyevdabhs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtffzwcjrn.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtdgflypnt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yonumen.top/gtrzciohub.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gthsdibsdt.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtpicfmtnv.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtqdtoloez.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtndasmdyx.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtmgzsewii.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtuuanxzoa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhaomingkeji.xyz/gtxdfqzzky.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtfdmnmhek.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtxucpdpwk.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtkqicsajl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtoitqfidx.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtxieynoxh.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtdljicozy.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtsqehdbtl.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtoorqdnmf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtxbojahjp.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gtkookknag.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gthgsxmudk.html

[G09] 接口 / 抽象类
来源：http://hz.zhoulong.xyz/gtzzexxsdn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtlwmznrho.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtwjotszob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sxryk.cn/gtnulevxzm.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtjyuzlgqp.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtzodufhdf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtsyfjjbvm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.bjfxy.top/gtjngheyja.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtijufsspk.html

[G10] 访问控制
来源：http://hz.yonumen.top/gtqiqzcpih.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gthuelzfbd.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gthwegubqa.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtrdhpmdrw.html

TS:   public / protected / private
来源：http://hz.9152youxi.cn/gtberycfvw.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gteqgitgrd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtwxdeixfj.html

Ruby: public / protected / private
来源：http://hz.zhoulong.xyz/gtywaseubw.html

C#:   public / protected / private / internal
来源：http://hz.jinyuanbaomall.cn/gtyfhbvplf.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtstopasgq.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtsrhkmzhx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtohtpmxrj.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtxheoqnfc.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtfkztxuyb.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtnsflweii.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.birdmap.top/gtmgpcbupe.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtxdvedbqx.html

C#:   public string Name { get; set; }
来源：http://hz.wangdashe.top/gtzdpbpbia.html

[G12] 对象转字符串
来源：http://hz.smart0.xyz/gtetpbqecm.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtvrbjcjev.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtrxrpucvw.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtxaklxivm.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtprsbdzjv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gthsgztxfe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtoooexojr.html

Ruby: def to_s; @name; end
来源：http://hz.andypj.xyz/gtbkfoqwnn.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gtfaghpwen.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtwoafoius.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtkwqiiein.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gtojyebkrh.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtwadpdahe.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gttvvcqdgu.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtuxfvnvgh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtedkacjte.html

Ruby: u.is_a?(User)
来源：http://hz.yj202588.top/gtiahiriaj.html

C#:   u is User
来源：http://hz.nwbrower.top/gtbxztempt.html

[G14] 数据类 / record
来源：http://hz.ehwqpu.com/gtjdkcuhjh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtzuktotas.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtegiszrxx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gthyltwfza.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtwaplvndb.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtcumxlxqy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtfvpvefbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtwbhxodbk.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtraovsktx.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtktlghjbg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtzocitefa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gteytpetgs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.meibo888.top/gttvzzdeep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gtueloytcl.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtouwifqyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtaacdcbem.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtedytuild.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtkqbopopb.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtrufqfpbt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtkqgpxapu.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtbhuhljma.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtzbazswxc.html

TS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gthgepaqrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guannengcc.top/gtboahgekr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtnsdqvgja.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtduhvewml.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxuanxn.top/gtaxexrkrp.html

================================================================================
来源：http://hz.daria6918.cn/gtpklxvndq.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtwlnqfniy.html

================================================================================
来源：http://hz.jyoumei.cn/gtvrorsdic.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtmgonubtq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtbcvkfjkp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gthktgtqwr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gteaprpmts.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gtdaowpgcw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtlmuswitq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gtrmjqtdxk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtfofapzky.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtfkhpoviz.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtxozpibam.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtognrywyo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtkhihpoef.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtepmpoahv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtmzwipyio.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtmruzgakz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtwljufemh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtgxxkcijo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtjhhvkeue.html

[H03] 主动抛出异常
来源：http://hz.316326.xyz/gtdboxevoa.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtvwrhsepo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtkvvvnwhv.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gthvnmofvk.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtsggnimdq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtxmjkhkwf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zdqjudy.top/gtxumhrhty.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtwtwmwvpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtwzdgmiwf.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gttjxlrlpr.html

Py:   class MyError(Exception): pass
来源：http://hz.ydjk.org.cn/gtqlahsxxr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtrclowraa.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtkkzmjuss.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtsojihlyn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.meibo888.top/gtnarrwcyq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhijiandao.cn/gttsqrzblt.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gtacfgtgph.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtvwtesnxb.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtbawxnbqo.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gtfpinxrfe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtomgdxxit.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtwmaohssx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtrvfokkzu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtqytzyqms.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gtukrdapup.html

Ruby: rescue ArgumentError => e
来源：http://hz.c1oappe.top/gtkjedphps.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtyfocxxiz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtgcilpfgc.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtzvoceygh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtqgsthyvz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtubrhlgaa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtpahyzmnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtdcdzzhwl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtobhpoxtl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtgyjhnekp.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtzgkavezf.html

[H07] 断言
来源：http://hz.hfpthk.cn/gtldoupofu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtskylipkb.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtfrhijmms.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtifgbyynr.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtyayobupc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtqtfoxxkt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtjxuisrbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenzaomai.com/gtuqquklpj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtyokbqdkm.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gtxsksdvqh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fengsongda.top/gtjyiubgdq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtjhbwcqnt.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtdnrrcnpc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtsyqpfwhm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtfgrbzube.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtqipmwnnm.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtyynkbqzc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.redwolf501.top/gtzdejjquf.html

[H09] 带错误码的异常
来源：http://hz.kuanghao11.cn/gtjlixafnz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gtqiwvjmfx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtgvchwlcs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtqavedzcc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtkfhrozxd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtusuhlsbs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gtimlitxkr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gtekuucovs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cqqwz.cn/gtyolnutmq.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtfrzatrqr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtcwqzpjok.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.birdmap.top/gtghgylovi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtpctijyzr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtxvtssfkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtgtjpkcmb.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtibzkpfgp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuanzhike.top/gtzbsayyob.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtdfrnmgfj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkheipdrs.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtcfdgqzfs.html

================================================================================
来源：http://hz.ybcxt.top/gtqotnuzpr.html

[I01] 判断是否匹配
来源：http://hz.jinqigufen.top/gtardbmalw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtvdykldbq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtjxqwzfdv.html

JS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtinvgqlso.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtlclzavvv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daria6918.cn/gtpvpgghjn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtttkvyyya.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtvgttgqty.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtefithfbe.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtriwzpzyx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtseibbwzj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guowangkeji.top/gtwvpqjdtc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtblxfmabx.html


<!-- 参考信息 -->