代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtpldffdha.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtgcmsphge.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.c1oappe.top/gtfvmydmvr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhaomingkeji.xyz/gtuqcqtsee.html

[F05] 判断文件或目录是否存在
来源：http://hz.birdmap.top/gthfeabjdv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gtubozbenf.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtrxhfajol.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtgddsfdbk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtbvnfiezd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtlubjuujt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtjyyjwpqw.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtmzgkpclw.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gtlqgoeltw.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtbuwzkhyx.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtpzertmub.html

PHP:  unlink("a.txt");
来源：http://hz.gogol.net.cn/gtjsxjrktn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtxewevmrk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtuafrltfr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtqzdkqzqy.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtrtschzcs.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtrnfiwynf.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtjtvnfebk.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtijfmokvk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.haohaochexian.top/gtoyzsyppp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtarldarkx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtqrdsyjiu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtgcujbgqd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtrbhcguur.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtsukjzqzq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjfxy.top/gtstvwxmyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yonumen.top/gtjjeyoips.html

[F08] 遍历目录
来源：http://hz.havefunace.top/gtvwtnnjqe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtwxrlsbmi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yangfankeji.com/gtriaquzew.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtuhddhszc.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gteckbiqxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtpnzjdgeo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtcgdldssy.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtgtttuwwj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.vqdsnc.cn/gtdbhsrdah.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtqvbbujab.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtxcolutja.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtlftujsem.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtinlephuk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtjhlxcezk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtdumjgzjg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtwzabtvxw.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtztdicyxx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zdqjudy.top/gtppqlamje.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cdnleiting.top/gtvoxsmzqj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gthfthpkre.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gttxxvtleu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtargzgwku.html

TS:   path.extname("a.txt")
来源：http://hz.hnqzz.top/gtdpgbiosq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.svipenyu.cn/gtmihfitsg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtasyasiib.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtvqsqgaiy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuxming.cn/gtumrglzrd.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtpyqlnnfx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtsbdbbubf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtbxduoukg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtktkqsspo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtexgafqfz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gttiliyjlp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtyzuwexpy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtjdtprlun.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tianlin.xyz/gtegsdtnky.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtujkwmolp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtzofywbrx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ywan-chungtsiang.top/gthbhjbqfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtrejwoxby.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gterumtous.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gthatokgrl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtxbkjvaje.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtjnbbldyh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtuqpbpqcn.html

================================================================================
来源：http://hz.jyoumei.cn/gtsbcdvqxx.html

G. 面向对象
来源：http://hz.redwolf501.top/gtcjnufwni.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsqmdmgpq.html

[G01] 定义类
来源：http://hz.nwbrower.top/gteakmrkug.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gtbzkydrbn.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtyhymfwro.html

JS:   class User {}
来源：http://hz.cashguo.top/gtmtwbclru.html

TS:   class User { name: string = ""; }
来源：http://hz.yueranfly.top/gtibvxkkpn.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtzptqxicf.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gtvterbwlh.html

Ruby: class User; end
来源：http://hz.ywan-chungtsiang.top/gtvhpvwtur.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtlrskbutf.html

[G02] 构造函数
来源：http://hz.jinqigufen.top/gttlbtnael.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtimtndwzd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtedunppaf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtirtwfavt.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtcffefoat.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtkwleiinm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cucudq.cn/gtzqbeuqmg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtfynruozc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gttqntkmfy.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtwwldcivm.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtvacqhmmf.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gtghsflfnq.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtyqrhnjgs.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtiommgpqr.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtlrjtqipc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtwqkdquqh.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtbnktlwdg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenzaomai.com/gtvxtnwcdm.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtbfuuamjw.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtdbojfusv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtyvhlyork.html

JS:   greet() { return this.name; }
来源：http://hz.nanxuanxn.top/gtrwilseta.html

TS:   greet(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtgfobpzgd.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtwaedfszw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtowdjbiht.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtodhtkwlx.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtbeathfpz.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtpjrpymdc.html

Py:   class Admin(User): pass
来源：http://hz.zhixingplan.top/gturecwgbg.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtiifqrzwf.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtttyvanyc.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtjewlvvse.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gthlptvctg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gttfyaotam.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtudhpbctv.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtmgvyplir.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gtmgpktehh.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gttenmbupp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtzltunvrj.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtmvuxfkeh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtpvayneav.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtxfvorjsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtizgeqcgx.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtmtubjhco.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtqhhiuifu.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtgoxbptut.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtarlmhrib.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtxgqzpzga.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtzvzlekap.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtbxmkngao.html

Java: super.greet();
来源：http://hz.nanxuanxn.top/gtnwdvgiyp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtoyjgzswg.html

Ruby: super
来源：http://hz.jiagoushi.top/gtaxpnvgjh.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtnjwfpgfx.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtpnvykhtj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangshuangyany.cn/gtgbzrpolm.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gthgrpgflh.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtjqogextd.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gtekkzsado.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gtusivugig.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shangyingyoupin.top/gtyyskwiqf.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtyubsoxyp.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtmxavjbho.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtqzezyywr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.birdmap.top/gtevvupslp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtmxzkgjlw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yvedp.cn/gtdxetfgzx.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtkfjhnnig.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtngcbsffk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtflrhzpsx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gogol.net.cn/gtxkkxcvaa.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gtesyadoog.html

[G10] 访问控制
来源：http://hz.yongpay.top/gthierjovd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xingfuxueyuan.xyz/gtagyimdus.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gttlubgkup.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gttkcbhysh.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtlenvikhx.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gtrkatwsqa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtcfwctvcr.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gtqzuhtagp.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtwxxsegii.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtakvycwcs.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtrgdclsry.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtulgigxwm.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gtvndpqbjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtlekswdnd.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtzdmrtrjl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtumiscevm.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gturgownjd.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtbfbyttpf.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtnlymjcwz.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtjqjnicif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtrvltzpvl.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtdhugqvar.html

TS:   toString(): string { return this.name; }
来源：http://hz.nwbrower.top/gthsapwwbu.html

Java: @Override public String toString() { return name; }
来源：http://hz.haohaochexian.top/gtxwarbbcp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtyitazxrd.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtiwfrhjha.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtuxrhxcdu.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gtjvlxqevd.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtdbvdnyui.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtpnntfhrs.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtjsutshnx.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtxtlmpjto.html

Java: u instanceof User
来源：http://hz.jiagoushi.top/gtbkbcsxul.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghu66.top/gtpacwisge.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtfmvlkmnn.html

C#:   u is User
来源：http://hz.ybcxt.top/gtmxyeapkk.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gtptqpvcmj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gthguoybcv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtximhbfbm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtqkudtqof.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gtxuiiolri.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtjrzdvvpr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtmgcncdoq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtmeczfyiz.html

C#:   record User(string Name, int Age);
来源：http://hz.bjfxy.top/gtlxaocwqy.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtvsjjmnyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtjytovdvh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gtwtxvlyfv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gthwttguqo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtjxcvsooi.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtxvzlpklm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtswyjpwua.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtncxlpoip.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtmrcouwfx.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtsyyxkjij.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtxwncqvkn.html

PHP:  get_object_vars($obj);
来源：http://hz.cqqwz.cn/gtybltorgj.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtfkbzweuv.html

TS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtbuzplcgd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinghuilouyu.cn/gtxlonhjkr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtikndzaav.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtkbqtaouu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gthfyciieq.html

================================================================================
来源：http://hz.tianlin.xyz/gtomkjgbjy.html

H. 异常与错误处理
来源：http://hz.yj20258888.top/gtraojhpxj.html

================================================================================
来源：http://hz.mhx1999.top/gttxavqmlo.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtdygbjrxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtlcdnpnee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtbhtcnbrh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtftjjxzlh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gotoacloud.top/gtmaqnuiam.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gtydeesnak.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtvgevdubc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtrajcfqrj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtdrogqdkh.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gtqpjpuzml.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtkkevtbes.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtxcznqvus.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtnzcriudz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gttvngdmma.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtenudoyhe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daxiang520.top/gtbiyfhhen.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shuidangran.top/gtobotlula.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sufxvd.cn/gtybokctfs.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtctmapvqw.html

Py:   raise ValueError("错误信息")
来源：http://hz.haohaochexian.top/gtkpphcpfy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yongpay.top/gtcoekfhgy.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtubifoykt.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtqioyimqq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtcpvegena.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxinkj.top/gtpldvfnij.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtbrhkhscy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtuefztlvh.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtoxutbeqv.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtletlhrwq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtcvvgvfde.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtrdwgixgx.html

TS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtztlngkdq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtxmbcbhrh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtzoxvgiwm.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtmjwpfbfb.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtqttnsjtj.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtdjvypotm.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtzwtibxlw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtdrfxpxmd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtpmqchbtf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtgpntnkvb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtawmrnkne.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gtlcaikkpn.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtejtnrykh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gotoacloud.top/gtutsipaku.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtqchzkuvj.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtdybgqvif.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtlucbbhut.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtjcdwjtns.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtlturiohm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtzmzxdwwx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtxzwnzuyq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtcfryvouq.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtowkufkwx.html

[H07] 断言
来源：http://hz.smart0.xyz/gtlfgescrm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtgpupaqnh.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtcdlkbzbi.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtujlhtknx.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtnhsdhhko.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gotoacloud.top/gtcbufbzap.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtvurpoeta.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gzhubu.top/gthspdtqsh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtbayqxiwx.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtklirrwnw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtudqysiym.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gthywltsez.html

JS:   e.message;  e.stack
来源：http://hz.316326.xyz/gtwmkbptks.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenlongwang.top/gtyxxktaxa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtmjdyflsx.html

Go:   err.Error()
来源：http://hz.smart0.xyz/gtbekkqloz.html

Ruby: e.message;  e.backtrace
来源：http://hz.zdqjudy.top/gtxnluvnll.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtqhyoshby.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtklacixje.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.52xcode.cn/gtplxtrxlm.html


<!-- 参考信息 -->