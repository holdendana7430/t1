代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtreockrsg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtpdlnozwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtiisypeub.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.feifeiyinyue.top/gtvrprknuq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtiewhtlsx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gtoevleyeo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtwnidocmm.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtqymdhfeb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtdxknnpyw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhaomingkeji.xyz/gtovzsamas.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtxybrssny.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtrjxzkzvp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtmjcxjrvc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtqaizdgsp.html

Ruby: Dir.children("dir")
来源：http://hz.ivvv.top/gtqbvilcwq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hysaishi.cn/gthtbydrqf.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtlsuklrwb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtsvhegunc.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtymesmbcx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtymswvjdw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtnmgorkdz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gthbovdydt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtptcejqso.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtrgqogoen.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtieurmwwe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtecppdsga.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtsftadhfr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuxming.cn/gtzolwbywq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtyqphmsba.html

TS:   path.extname("a.txt")
来源：http://hz.gotoacloud.top/gtlzbspxwq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtwngrtjny.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtanqasmgu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtsoabplxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtxmobdbik.html

[F11] 复制与移动文件
来源：http://hz.ivvv.top/gtxqglsdch.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtvwtjofjz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtxzednpvo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtykawyqug.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtltexruqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtsawvvxcr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtmjbcdfgt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtvdbszghv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gttaleivyw.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtsulrkbjl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gotoacloud.top/gtmsfgpjpn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangdashe.top/gtqmzchpqj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtuypxvrqo.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gtxpynxicg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gtcstxogff.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtupdzdpen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.haohaochexian.top/gtbxlzbvoe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtxvjbmogb.html

================================================================================
来源：http://hz.zhengqikj.top/gtcxfsrxaj.html

G. 面向对象
来源：http://hz.jinghuilouyu.cn/gtxiwdypkc.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqzkdwzdn.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtizzubeyc.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gtugunhocl.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gthljrvptq.html

JS:   class User {}
来源：http://hz.guannengcc.top/gtuusirugo.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtdbendzme.html

Java: class User {}
来源：http://hz.hfpthk.cn/gtblovbuec.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtcccnovjs.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtjtrhnvwj.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtjwfhvomd.html

[G02] 构造函数
来源：http://hz.yj20258888.top/gtaelsvxtr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtmhfvacua.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtzgxubhyo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ybcxt.top/gtyoyoelni.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtieayuvyz.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtuwlkpbgd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtycbtveks.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtrybqmnrl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtshfllzkg.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtlimyfffm.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtnhmeruvz.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtekskxmhs.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtvzgjjmyb.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtbttkxneq.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtqbydudqj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtqohxaugd.html

Ruby: @name = "x"
来源：http://hz.ehwqpu.com/gtiavntcnh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtrdikdwst.html

[G04] 定义方法
来源：http://hz.cheryme.top/gtcijmlowf.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtycxbpzzo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtrqikxlim.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gthntpvfxa.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtpcknkoul.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtrspjnnyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gttxaiosvr.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtjuciffvv.html

C#:   public string Greet() => Name;
来源：http://hz.daria6918.cn/gtnvruqbrr.html

[G05] 继承
来源：http://hz.cqqwz.cn/gtruoioaim.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtplggcqtg.html

PHP:  class Admin extends User {}
来源：http://hz.bjfxy.top/gttcowuwtp.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtsunnbzxd.html

TS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gttrxjahtd.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtbxszwstc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtkswrirns.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtvnkexuai.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtzlmabras.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtsvvjzcpy.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtabowvjxd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtsiosldxb.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtutyuozdk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtnyymdqsk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtpntvzoli.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtwexwrvue.html

Ruby: def greet; "admin"; end
来源：http://hz.zhiwuduotai.top/gtgfevthex.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtncdymwrk.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtpcwhyifa.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtyomwgbmm.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtwrahblag.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtiwnhyrpx.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gteosdyaec.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gteqejaump.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gteunehgog.html

Ruby: super
来源：http://hz.yueranfly.top/gtttkffpns.html

C#:   base.Greet();
来源：http://hz.cdnleiting.top/gtoeqobyjw.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gteidjgznj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtmpiwjjqz.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtyaqzxzns.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtoxsvgbtj.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtjpubbsah.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtpdbjhmqa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtswikgwiz.html

Ruby: def self.f; end
来源：http://hz.daria6918.cn/gtqaurimde.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtanxmudxz.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtjnqqdawv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtgernzeny.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hongshengwenyu.top/gtihopuskk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gtmspwkyic.html

TS:   interface Shape { area(): number; }
来源：http://hz.jianghu66.top/gtufrhchkr.html

Java: interface Shape { double area(); }
来源：http://hz.gotoacloud.top/gtrdgudaup.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtdilbcurb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ppjwa.cn/gtltiueqdp.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtrxutvgim.html

[G10] 访问控制
来源：http://hz.hfpthk.cn/gtnhuykipv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gtdqvgyqbo.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtjcylrqow.html

JS:   #private 字段；其余公开
来源：http://hz.aizwys.cn/gtnyjhswwh.html

TS:   public / protected / private
来源：http://hz.gaohongyu789.top/gtecbrjmuq.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtzztnywro.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtmgqudxek.html

Ruby: public / protected / private
来源：http://hz.mhx1999.top/gtbhkdtlpq.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtdhjoxxqr.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtearncebq.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtwdijglkz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtvojekmps.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtofxmezeh.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtlcvywwxl.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtulshicqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuanzhike.top/gtgibvwehi.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gtnahlxwoa.html

C#:   public string Name { get; set; }
来源：http://hz.jqgfzy.top/gtknztvjyg.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtsdbocnct.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gtefbyofbt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtzqgtvdbn.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtkdfoifyk.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtaggfrlpl.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtzvaxcaun.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtnsmlkxvt.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gteccthwmq.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtfmtjsirr.html

[G13] 判断对象类型
来源：http://hz.feifeiyinyue.top/gtdmdknfjd.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtsqxqrnap.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtgwhlomvz.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtxdvqddha.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtrivhpoli.html

Java: u instanceof User
来源：http://hz.iojbl.cn/gtsidynpyc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xinyue.icu/gtfecojyqx.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtakrvxihd.html

C#:   u is User
来源：http://hz.daria6918.cn/gtifzyrldl.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtsisawory.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hammf.cn/gtiwrnxixh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtmxoqnzgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gtsrnqnora.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtymftmgpx.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gtndmfzktf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtfrmzjpik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gtzbudfrkl.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtyiamqbmr.html

[G15] 枚举
来源：http://hz.havefunace.top/gtskwyophp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtowkdrzyi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtmwvexosu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtkfzbezbr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtraqnchsg.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtunzqcvpt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtqoidkbln.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtagdgxwav.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gthpkrkxmm.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtvmgrshzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gthponahxg.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtyjrhsway.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gthcsrioys.html

TS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtyphjdgfc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gtjwxoxqko.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtryxdbehe.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtgddkiabc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtlmfktdje.html

================================================================================
来源：http://hz.hammf.cn/gtbqrdrywf.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtmxazidxs.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthiskuxov.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtfnlugqqq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtmybbdtal.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtwbsdzwyo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtwtrkjoay.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtdgowlmat.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtxtbfqwmu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtdaraazqw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtggymbljz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtyasbrvua.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtnwozvwme.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtjlsjclmx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtdnkxonro.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtgplbnipq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtqtcmxnel.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtkkedteqr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gtpxsxnduh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtpyqkzerc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtoyouotys.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtbatttoip.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtxiuhezxw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tian-w.cn/gthjgkqbou.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtnmzgaczj.html

TS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtgbewccrh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtliydvitq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtukuoduzw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gttdmfulix.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtythdnssd.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtbluwonpo.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gthqaslcck.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtdbympyuy.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtnxsgeukc.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtmjbxatsa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtgflgzgmn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtzzegmtwl.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtnulecawk.html

C#:   class MyException : Exception {}
来源：http://hz.birdmap.top/gtknzqybwp.html

[H05] 捕获特定类型
来源：http://hz.zhongyouzk.top/gtdkgqqxzn.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gtgmkojkhi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yvedp.cn/gtjooylosv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtydyeqjbk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtgyjgzsjj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtwkqaywln.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtsyhxdzat.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtvaajmndt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtnxsoczdv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtwzxnsxck.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gttlbnakrx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnqzz.top/gtpakdjulh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtjcbxqpxh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtuclgohmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtadjvbfpb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtqdlmzbit.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtmqlsnmqz.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtwhnektwm.html

[H07] 断言
来源：http://hz.smart0.xyz/gtenzosyyq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtvjkmxwqo.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtdcvesnlp.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtgioqfdbs.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtnqaffouu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtubapysgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtdoxrdjtl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cdnleiting.top/gtsvmngvzh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtulobpbvb.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtzmmaqgox.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtuhrrstca.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gtwmoxfvws.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtvqscepmo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtslpnjtru.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtbphutuvg.html

Go:   err.Error()
来源：http://hz.jinqigfzy.top/gtheagmfpa.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtppzmuknv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cucudq.cn/gtjegqwojv.html

[H09] 带错误码的异常
来源：http://hz.jinqigfzy.top/gtvxvuzaxm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtgupkwjia.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtfsbgyxgl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtftvmdlqx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtpzgwnozz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtvfuqphus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtgtlhclim.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.316326.xyz/gtcgpqphyv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtkynybuav.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtgrfnfbvj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtybsqukaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtefoqumgc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtgtjufmft.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtvoslmjwt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aibaodan.cn/gtsuckniof.html

Go:   defer f.Close()
来源：http://hz.sufxvd.cn/gtbxjjzhtl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gtgzqkbofw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtbuejkccb.html

================================================================================
来源：http://hz.yj20258888.top/gtbhqwmgfq.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtfkuignot.html

================================================================================
来源：http://hz.yonumen.top/gtetwewjlv.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtscxohiuf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtrcdyjjry.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gaohongyu789.top/gtnlsqsphg.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtpavcspxn.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtxciycipa.html


<!-- 参考信息 -->