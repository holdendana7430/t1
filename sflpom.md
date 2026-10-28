代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtmswrgtck.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtedrlxjuv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yonumen.top/gtruqqndji.html

[F08] 遍历目录
来源：http://hz.yueranfly.top/gtrtrytmbp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtnxemvvdq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtrrwtnfpz.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtuuybzdem.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtmpatjxxt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gthzbbaflg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gthgctevpe.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtbqirlgae.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtmyxyzayh.html

[F09] 获取文件大小
来源：http://hz.cheryme.top/gtpqbkszit.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtojdpgfrf.html

PHP:  filesize("a.txt");
来源：http://hz.gotoacloud.top/gttxqrbjxj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtvbgfitwp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtdmhgtiol.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtppxuxyvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuanzhike.top/gtjuppbnhm.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtfashrtyn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gtraezzhpd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtwvzccpmd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtliensfzm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtnglxbnzq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtsnvzvesw.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtyrolyxal.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtsphiusah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuanzhike.top/gthmxrazpe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtytajjhpp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.iojbl.cn/gtuytbzxfe.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtecvnryyt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtapintnrp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtiehrkgqm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtejjosgqo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtunkvshbb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtbxtyioji.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fengsongda.top/gtwyswtiuu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtowxpxfby.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuetiantiany.cn/gtjpcihlck.html

[F12] CSV 读写
来源：http://hz.gogol.net.cn/gtfsttdztw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gthykfvupk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtdvpoceqg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ehwqpu.com/gtnjfvljma.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtykwtggpl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtlmygtrks.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gttunxlkuo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtipqagaaj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtfwrssxbb.html

================================================================================
来源：http://hz.hysaishi.cn/gtqnlygjuh.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtvcmeqtqe.html

================================================================================
来源：http://hz.daria6918.cn/gtujrlzgqy.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtsyvowejy.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtfzhbtvaw.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gthsctiuqb.html

JS:   class User {}
来源：http://hz.bjfxy.top/gtdhngyqsc.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtkxjeegpl.html

Java: class User {}
来源：http://hz.jinqigfzy.top/gthhrzszfm.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtpebnbzml.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtcgovtmbt.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtbaakfsec.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtvsbdeoec.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtmttawevm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtyhzlqldt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gthgbmvttp.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtmrhtdxzk.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtehongpki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtoiqqiyyj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtwsfijpad.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtyuqtsxcl.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtaizkeaym.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtemgrvlac.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtuayxaehq.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtwhtewcjb.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtqglcduqy.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtebltmlum.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtbbjpiovv.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtmckgjxzf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtwohuhrxt.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtdeqcvavp.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gtzijgizjv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtvzfscjng.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtrtmwpwti.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtftuftxyr.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtbivjzrbi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtpgdgkamu.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtwyxrgdvd.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtevsrzupk.html

[G05] 继承
来源：http://hz.xziqi.cn/gtxyxdfphg.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtgnuccrqg.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtzvhxyogw.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtdbvgvhdb.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtvvikakkq.html

Java: class Admin extends User {}
来源：http://hz.daria6918.cn/gtmhcgtiqh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gthdcrknvd.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtlzcbuetw.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtvcdwiniv.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtrsyhkqvf.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtbcibgjnl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtxsuzlzqv.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtimzyhuhg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtehikxtax.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtxunajcya.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtnkthtpgl.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtqmcqxvun.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtyjbzxlfn.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtkbyuzssf.html

Py:   super().greet()
来源：http://hz.sweek.top/gtowmlxsnp.html

PHP:  parent::greet();
来源：http://hz.cucudq.cn/gtpcphtprj.html

JS:   super.greet();
来源：http://hz.pycfn.com/gthzxlqrfs.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtnofdlhpz.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtqixxvkgr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtsqmkwign.html

Ruby: super
来源：http://hz.guannengcc.top/gtrhbnzeyx.html

C#:   base.Greet();
来源：http://hz.gzhubu.top/gtylwrmtyg.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtvkufjcra.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtpzdkkofu.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtxrbgcnrf.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gtsrxxfirq.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtbdprcask.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtdytbdzhz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gttuhrlvna.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtudtbeiee.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtohabefie.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gtzbimqpeq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtuylxppvj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtsttyshzz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtcbhiolno.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gthgfnsivx.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtfgjbmjgd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtofmzomyg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cqqwz.cn/gtmfcyeagg.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtdlwfkcbs.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtaekoalgv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gteopspcrp.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtauglxwon.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gttedaviln.html

TS:   public / protected / private
来源：http://hz.tianlin.xyz/gtfamvodfo.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtiwfwboim.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gtmfdmdidm.html

Ruby: public / protected / private
来源：http://hz.zhengqikj.top/gtjxujdivd.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtfondqaug.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtgvpmvpky.html

Py:   @property 与 @x.setter
来源：http://hz.quarkkingdee.top/gtwtyhowzf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtkelbqfpp.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtpdqrdbst.html

TS:   get name(): string { return this._name; }
来源：http://hz.guannengcc.top/gtazxuzlnw.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gteucpbzgk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtfpdywacv.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtllqgtiux.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtbajhafpf.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtkkdkbuzf.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtfqqfhkkp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtkvvujzjv.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtarepuyuc.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtjrdtqdsz.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gthcqerqcb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gttxokloyr.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtumtmvqbn.html

C#:   public override string ToString() => Name;
来源：http://hz.316326.xyz/gtfcfupgny.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtwmggohzz.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtausqmwgf.html

PHP:  $u instanceof User
来源：http://hz.aibaodan.cn/gteaioiayi.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtmifjfzzp.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtmdastgbq.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtnzgoixvt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtandwxeda.html

Ruby: u.is_a?(User)
来源：http://hz.xylfe.cn/gtfscjmtgp.html

C#:   u is User
来源：http://hz.jinqigfzy.top/gtwqyxaqwo.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtklhzxmld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.0kj1m.cn/gtiaczrkew.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtijiifqpi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gttocrswsu.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtzlbtbmxf.html

Java: record User(String name, int age) {}
来源：http://hz.nanxuanxn.top/gtuzsqieno.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtllixijwn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nwbrower.top/gtajfxvtjt.html

C#:   record User(string Name, int Age);
来源：http://hz.ydjk.org.cn/gtkzeafmda.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtbjdkfhxx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gttchhrawu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtcpfuwiya.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtvbedmgyr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtfthbxqqo.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtvycwafti.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gtrjtsydsz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtfwqlxwcs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtspcbzmrv.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtgcovweun.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtyszmoifb.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtgnzirogl.html

JS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtdxulcrtt.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtlozthjue.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtaidgmmrq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtiyboruyx.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtmupwlwbb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtgrlihwsu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gteufxauet.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtgtrvkikq.html

================================================================================
来源：http://hz.tian-w.cn/gtfnwfatxy.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gturaynoyk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fengsongda.top/gtslxwmufo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtqdkuiuvr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtjsbmplcq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtjhpwrgwi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtahhvvnig.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gttpvxeiwi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shzxlz.cn/gtpfhcwifa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtcvwmybvc.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtonutjujq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtuhrakqll.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtbxfrbwjf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtvpnnrrpv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gthfapnapn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gthtdbfvjb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gtppyqduce.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtvtgjucfo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yanxiufei.cn/gthlwlsawy.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtqwresejt.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydzc1.top/gtqzueujij.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtfuienprk.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gthbnldrgt.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtrceovroy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtbevdqejt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtxoxvsfgn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jiagoushi.top/gtyflbxwwg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtgjeakdso.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtgtfruxxj.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtjepuplqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtuzvbxfnp.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtnndwrdwj.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtxrfulgyc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtemzysiju.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jyoumei.cn/gtohjhkrle.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtewtdsnpv.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtxyyafcqz.html

[H05] 捕获特定类型
来源：http://hz.9152youxi.cn/gturokkqcz.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gtkhbzekma.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtymolgzlh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtmzqmvbjs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtbgbtdmfd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtembdluxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtytmqlkzn.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gtyfziynok.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtdrzvzrjv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xylfe.cn/gtmcxtaznq.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtjknwqxpt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cheryme.top/gtesuixmem.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtsgkkuiaw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtbkcwevon.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtyheptggk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtefxkvilu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtldtpxvah.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtwpxbllpv.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtcvlsmrrs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtlvsiybzo.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtgbvrirly.html

JS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtzeycksqw.html

TS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtnmgxtflj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtuohyytar.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtjjqvlbfu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtiimscbwz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gtwortqkde.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtyjfnqctr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtlkruhxel.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtvncotmcg.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gttirygmmw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtgefudbnq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtbbenurzo.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gteshtmyhs.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtcipqlrny.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtslvlbzbv.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtlrhepuxt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtzezltvpi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.vqdsnc.cn/gtmiktwknz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gtsjzoxjbm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenzaomai.com/gtsxkjqtof.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fzhhl.top/gtklsrbktg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gteoonctcx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtbpatawqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtiuwbvjgd.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtnwxxgvbe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuetiantiany.cn/gtkduvbbel.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtvtcrrncf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtbgdpiiid.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtwuusivel.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtkhzpszjo.html

Go:   defer f.Close()
来源：http://hz.jianghu66.top/gthkubinbs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtwosdguoe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtfuccrxhh.html

================================================================================
来源：http://hz.52xcode.cn/gtcohthrmh.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtlrtjltav.html

================================================================================
来源：http://hz.pycfn.com/gtnwmgszey.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtyjerbogw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtwymjemog.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtawlucxav.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtdfpbfkpy.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtaqfibrnt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gtdabagvac.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtamzlubmc.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhengqikj.top/gtzeivamtc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtebocxtyt.html


<!-- 参考信息 -->