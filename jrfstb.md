代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtjnldtxhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gthtkcnuvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtktzkzqca.html

Ruby: File.exist?("a.txt")
来源：http://hz.fengsongda.top/gthakgqhxd.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxuanxn.top/gtrghjpsat.html

[F06] 删除文件
来源：http://hz.xuanzx.com/gtpcbqiktj.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtigoitsvu.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gthlksnghg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtmjdlmyfa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtxfwgfsnt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gttzrkfbnu.html

Go:   os.Remove("a.txt")
来源：http://hz.yanxiufei.cn/gtuvksfxiw.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtdiektkhl.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gthjcluaek.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtsrkbbiew.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtwvikexxf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zycfv.cn/gtqqxbxptt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtoguswmuc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtwovumxwk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gttagtxdrp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtcwygdgbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtunmsqxzd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtsdaplwfl.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtbajamabc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtjvviyekg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gttuxekaty.html

JS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtupmesteu.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtaecrhcmr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtpruitrxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtfkvoquhh.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtpecplcuh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gthfbgctyv.html

[F09] 获取文件大小
来源：http://hz.hammf.cn/gtsjbrkywk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtjrcerdwo.html

PHP:  filesize("a.txt");
来源：http://hz.jqgufenzy.top/gtrrdtbaeq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gthlcvapzn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtizfkhxfb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gthcqdrpqi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxinkj.top/gtajsyrqgs.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gtygtgfkly.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtimwkzycd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gttalbuwpi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtadbawijn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgufenzy.top/gtcvxcrgvk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtlpdssuzw.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtsaqqfwmu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtuhajybbs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtrbjidqwa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gteyevrmmw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtxmozdxmb.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtiridmsmw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtrbaxomfc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtmrlicdyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gttkvidehf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtldztxsuz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gteymszdiu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtwmgzglcd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtdxoxoieo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtsqltbfkz.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtoylcgzux.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtgyujffjj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtdayxnxhc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtaptnsgfv.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtucjvlwso.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtonshgagf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtpvpjgkfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.bjfxy.top/gtqlzfsqno.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xylfe.cn/gtxxeyvvme.html

================================================================================
来源：http://hz.nwbrower.top/gtrgyvipyl.html

G. 面向对象
来源：http://hz.birdmap.top/gtplzcacbt.html

================================================================================
来源：http://hz.gogol.net.cn/gtxrhttzsm.html

[G01] 定义类
来源：http://hz.bjfxy.top/gtvakspkfz.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtdbsuqllx.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtxwvffbjq.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtuiwedexs.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtyobxxqur.html

Java: class User {}
来源：http://hz.jyoumei.cn/gtvidqaozt.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtapetbtmc.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtjetqmunc.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtlalhyqrg.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtehtntwcn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtkqokhvar.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtartrnnzo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtjffflksl.html

TS:   constructor(public name: string) {}
来源：http://hz.quarkkingdee.top/gtgxapyunz.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtfeizpvid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gthkaplxpx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtkretcklr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtsxuqvqiz.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtgocmzbex.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gttlvmkkfd.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtulcvbpga.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtkwnsgqqy.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtbnuktcal.html

Java: private String name;
来源：http://hz.hammf.cn/gtepcmqijl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtnazyxmdr.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtdhsmwxwo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtbgtokmqy.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtoqufsdda.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtljwlgdmh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gthxevlkdi.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtlrizijvn.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgfzy.top/gthgpgwjsz.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtfigehvun.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gtwvtgozvo.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtdbedjyec.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtackqeeaf.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtzeaabrvb.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtbokrsyxc.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtjeblmgyv.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtmmzybgxl.html

TS:   class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtyqbjpelx.html

Java: class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtsuvyvdlc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtonhunofi.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gtvhsedyci.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtxfqmqoqk.html

[G06] 重写方法
来源：http://hz.nwbrower.top/gtvpzhyifm.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtheyqiioi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtuhlelwso.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtibsbcrwr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtfgqlmhba.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtouvkytvg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtyknkgipe.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtkmoubfcb.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtxnsahjjw.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtwiahkoki.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtkpkahons.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtjminarmf.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtwoaltpse.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtknrxhyiz.html

Java: super.greet();
来源：http://hz.birdmap.top/gtmjbtvgvn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtcwdkqdsd.html

Ruby: super
来源：http://hz.xuanzx.com/gtirpdjnte.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtnrqvoujb.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtgwflqiik.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtrvujjyma.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtaxkqitlf.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtlbjrahir.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtbgxgsats.html

Java: static void f() {}
来源：http://hz.c1oappe.top/gtnqjweuuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtduywpwvo.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtvhzacsat.html

C#:   public static void F() {}
来源：http://hz.nanxuanxn.top/gtsphroaxc.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtpwarswfm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangshuangyany.cn/gtvejilnvw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtvogjdhhb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtlfibmkul.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtivluyzpo.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtrhowovbz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtwzedxmhf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtlpmrenjs.html

C#:   interface IShape { double Area(); }
来源：http://hz.sweek.top/gtldajsxnr.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtvmxinatf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydjk.org.cn/gtcfmgxhvf.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gteagudvgy.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtsnkaqxpq.html

TS:   public / protected / private
来源：http://hz.sysykeji.top/gtlqtxljlz.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtzmoghchm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuetiantiany.cn/gtkjqpkccu.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtkvblmjek.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtiryqvvsf.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtrvvkdryk.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtbehtxeiq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtfjdisovt.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtpsfbzcmf.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtbvpqgcao.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtywglbszs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtmkagptkd.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtoudkmfqn.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtiqrqizjg.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtzglxyzgp.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtsgylnwjo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtbwstticd.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtmqlarphz.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtfacrrsqp.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtmfcdehsh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtsvdbkspd.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtnilihxqc.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtntcbikyh.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtcuueweyq.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtntxpfswy.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gttjueznfy.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtsbcxeqho.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtznmvgdwf.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtyowappog.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.9152youxi.cn/gtypzcjbnf.html

Ruby: u.is_a?(User)
来源：http://hz.sufxvd.cn/gtrpbfrdfm.html

C#:   u is User
来源：http://hz.xylfe.cn/gtqiwxjcqm.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtherpqhqb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gtburtgrqe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtfcxqxeec.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtkehrluhk.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtlskhisvk.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtssqebugu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtlsmrenwp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.meibo888.top/gtcnbfsqpl.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtuczouohs.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtlvivnnvw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtplicrzcc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtrbaskbxc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtnyyryypu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtonggagiz.html

Java: enum Color { RED, GREEN }
来源：http://hz.dashuyun.cn/gthwibeyrh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gtunkfcise.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtglfimexo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtcpqvvmfs.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtjldlwccq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtvxoektsx.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtjkgxlimr.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtsooxmfvg.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtldialtmq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtmwtiychy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtljgvmrnh.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtbqbahiwi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gtpsqqcvfo.html

================================================================================
来源：http://hz.smart0.xyz/gtudeotfuc.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtzdfvqwcc.html

================================================================================
来源：http://hz.pycfn.com/gtsvfsjipj.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtvoiaqqnu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtkyaaunci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtzwalkouk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtnocohwxd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtaeeuijzl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtzyndoxsr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtmiyzwcoj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtjztxpioq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtsbtmujtv.html

[H02] finally / ensure 收尾
来源：http://hz.zdqjudy.top/gtqrfbvqhy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtorxkatpg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtiqyajqwb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtnhqgueth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtlgbuwyed.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtcxwbloge.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gttdybwyrr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtmqyiapws.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtpopokuvl.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtjshxskds.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gtnmdgqxlt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtrewckgly.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtisgavani.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtwxliwddq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtofdisdvc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gtbvcnlydt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtefbkwsgx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtmsevbuhf.html

[H04] 自定义异常类型
来源：http://hz.9152youxi.cn/gtpgqaszoe.html

Py:   class MyError(Exception): pass
来源：http://hz.zhiwuduotai.top/gtqjzvnhhg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtdjfbvctw.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtuhagdxcl.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gthldexlsy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtncetixib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtcfbgvbjl.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtglpmdoph.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gtuorhodoi.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtvvluorit.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtnmooxtaf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xziqi.cn/gtfbxiglyq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtukeyznss.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtslchwnlu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtarrhnfzt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtkqrgpwqc.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtvflhiact.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtgzywesqo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtoauqjqfd.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gthkrepbqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtzntkybne.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtdudkjcuk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtlijdyeok.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtptefnjsg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtybhcxdzb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtxxxphtgh.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtzdgbxzet.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtilboubsz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtewqenbul.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtztjtecfl.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtyiryqzwu.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtlijptjwb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gtwtgynzci.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gtmjgbprsk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtogjwnwdp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gtlkhonwhp.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtmajwsitl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gttzmergnu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtdbiuwguv.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gtvpqtzdia.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtvbekzmet.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aizwys.cn/gtbsvvymdv.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtjwkptvbw.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtkvdjzdhc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gttqtwodui.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtitpdocvc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtgjxzkxwv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtvlmcngqc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtzrndgvrq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.iojbl.cn/gtyoqfcmjk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.meibo888.top/gtfdtblhaj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhixingplan.top/gtgxajegfe.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtyyhcrtxm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtetwpfydg.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtbsksqssi.html


<!-- 参考信息 -->