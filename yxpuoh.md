代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.9152youxi.cn/gtgrgvjmdc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gtrjkdoquw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ppjwa.cn/gteuqjvqjw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.andypj.xyz/gttvtslydh.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtesqptzst.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yueranfly.top/gtgcxjszev.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtqqrbaehf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxixbpttp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtviondftw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gthpmasomj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtksidpoia.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gtcuugugxd.html

C#:   File.Exists("a.txt")
来源：http://hz.zhoulong.xyz/gtfrighwel.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtwmzighsd.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtltcznqbw.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtieizqjsx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtwfmyillv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtjebzhzxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtlnsmsyjr.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtacbeirip.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtxzsgumct.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtnshjcboa.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtnxytcogh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtmngkgtab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gteaofjqas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtvjiigpib.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtmuxauiyi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtibbgwzfw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtpyjmorah.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhengqikj.top/gtvdcaluen.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.bjfxy.top/gtpmpmfkin.html

[F08] 遍历目录
来源：http://hz.jlsjyb.cn/gtelsirqba.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtadmttlsj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dianchejie.cn/gtgcttcdsf.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtcqqheqac.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtcuucjixd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtcsxlurkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxuanxn.top/gttxiaafec.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtsffshugd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtnhxtbdgs.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtquseahex.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtrkhvmnea.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtwcqmdafx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtepscegyo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtkwudddsi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtjsvyfujj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.iojbl.cn/gtxcvfbifp.html

Ruby: File.size("a.txt")
来源：http://hz.ydzc1.top/gttkpqtino.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenzaomai.com/gtgmpfnnai.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtvtoqidfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtecpuaben.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtgfdgfjlh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gteilhfhiw.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtcvapksdh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtokqqqjfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sysykeji.top/gtvwjgpond.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtghkcwklv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtaaxtrlrt.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtfcdntutn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtsznnuzyy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtesofsxia.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtumkatfqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtoascrnuu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtkuqroevz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtjjuinxib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtfbfoajst.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtyhiffjrh.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtfqfmtdhv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zycfv.cn/gtwrmdcmdy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtwazlzqdz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtwnpwpvie.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtsviczgcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtndfbghjl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtotinieww.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtubbfyehp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtpefghizm.html

================================================================================
来源：http://hz.zdqjudy.top/gtkawrhkrg.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtgufymylz.html

================================================================================
来源：http://hz.xziqi.cn/gtfloiejxh.html

[G01] 定义类
来源：http://hz.sysykeji.top/gtyrjsmpvq.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtqbkhnxca.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtrbueznww.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtdclmkytm.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtegnkqgdo.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtxzimlamv.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtoroqtajg.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtlrrsmwib.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtqdymzokv.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtzliphnow.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gthusvfoog.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtsqulmnoz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtaopkhbgd.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtvjqahsiv.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gtiatwqgtx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gthjrctehf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtftgrawzs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtwuqfgcni.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtytsgvluo.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtqswmvmtl.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtagrihdon.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtgpuewcxc.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtnnfdvvnb.html

Java: private String name;
来源：http://hz.zhiwuduotai.top/gtfgnlawhm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gtduiuymtw.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtnuxxcktx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gzhubu.top/gthutkoiga.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtbimrnlug.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gtbboouxkn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtyksjhevw.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gtsbwlaobc.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtzerbddil.html

Java: String greet() { return name; }
来源：http://hz.bjfxy.top/gtlbojjwmm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtgzypsirv.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtxgwgaxty.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtpiupfivt.html

[G05] 继承
来源：http://hz.dianchejie.cn/gtaitveqvk.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtbkovulre.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtrfzehrzm.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gttridpnpy.html

TS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtjvynldfl.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtismgtgib.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gttsznypay.html

Ruby: class Admin < User; end
来源：http://hz.tianlin.xyz/gtgoawmpnz.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtdrjsgywr.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gtncdadreh.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtsuoqouet.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtxqxgxhkb.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gttdgcgjzn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtbfagjgtf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtsboezdbo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtxfexesti.html

Ruby: def greet; "admin"; end
来源：http://hz.svipenyu.cn/gtaabprowz.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtpnohjifl.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gtjjnbimxy.html

Py:   super().greet()
来源：http://hz.sweek.top/gtkbwxoxol.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtcsitstht.html

JS:   super.greet();
来源：http://hz.yvedp.cn/gtpasafhzi.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtwwfjmunk.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtnkktvouz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtonynzwzn.html

Ruby: super
来源：http://hz.chenlongwang.top/gthzsolifd.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gthldomsus.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gttpaajcaf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258.top/gtmdjsymef.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtamfqdsvt.html

JS:   static f() {}
来源：http://hz.pycfn.com/gtdaajryrj.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtahtseahv.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtmcxuujvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtnkhssnss.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtcaejkcvz.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtzzglidkn.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtxlkjulds.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtijjqaxbd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtfxquapie.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gthxnlzgwn.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtinvqwqjg.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtflsjjoej.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gthoxedexx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtciufcjqj.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtvxmsctth.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtxbqoxsgv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtlwmuapua.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtjunoawsk.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtxujknxbc.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtjsreaxlw.html

Java: public / protected / private / 默认包级
来源：http://hz.zhaomingkeji.xyz/gtdnpugsin.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gtwxmelafg.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gttykpeljh.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtulssltth.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtdlyxobug.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtbqbotnkv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtbdizbjie.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gtuvdqsvby.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtkqwlrpso.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gtfxxuyysr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtsjzjanzj.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtaxnyguqd.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtutowalre.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtdkgiktrg.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtayqvrahx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtbdmwpbjz.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtqtssxuwy.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtqjzrnnxh.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtcfaosmfn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtvjdlgsbf.html

Ruby: def to_s; @name; end
来源：http://hz.daria6918.cn/gtomptjlwa.html

C#:   public override string ToString() => Name;
来源：http://hz.xuetiantiany.cn/gtlcyhrcho.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtnkygrjvi.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtvyjxdvez.html

PHP:  $u instanceof User
来源：http://hz.meibo888.top/gtignoctoa.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gttagosplh.html

TS:   u instanceof User
来源：http://hz.xinyue.icu/gtimfqygkk.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtkicmrzoc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtpspfpgpo.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigufen.top/gtjsznneah.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtyipxnjad.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtzrzomxfl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtbrbomanv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtejxfaagc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gthqundtro.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtadybsceb.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtepbsxbqs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gttzykawsp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtjwwfccjr.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtchexqqvh.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtfjfbjdlg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtlzemhpbi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtmscwxjqq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtotikjqok.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtwlhwtsgm.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtyhtqncvw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtcucawfly.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtpkpdxhlk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtffpvvtmh.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gttomfgbxy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtdpsevdml.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gtmumjywuu.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtzohqgqhh.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtobkejhlc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtqzsgpoqj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtsoikbhqj.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtxrmgeems.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zycfv.cn/gthqblxedb.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlhchkxtn.html

H. 异常与错误处理
来源：http://hz.sysykeji.top/gtlvsbfopb.html

================================================================================
来源：http://hz.aizwys.cn/gttthiqxgv.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtvrkugvof.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuxming.cn/gtrkvuzsml.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xylfe.cn/gtuhbsuvtt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtgqjzzegk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gtxxcjjwng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtriicqzfu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtpuwsnxdm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtfcuoewtn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydzc1.top/gtmlucluxz.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtewmllavk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtlejjinrz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtimkagnxf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtwhezmsed.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtmngzshak.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtelwbndlx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtmoefbcmp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.quarkkingdee.top/gtosxbvkjj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jianghu66.top/gtlcqfizdk.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtvwsqpxea.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtabjxzywa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtmgxjjbrn.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtkfeofpuh.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gttzskxgmu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtphewmloz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aizwys.cn/gtkcezvkfu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.birdmap.top/gtplqxlsnp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtyyvcvain.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtzckapiqx.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtvxwlestr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtstroelxk.html

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtxcgthqmm.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gthqtkcxxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtgyrlmuev.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gtokqzqrns.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtdbgjyptw.html

C#:   class MyException : Exception {}
来源：http://hz.tian-w.cn/gtklsfkgxt.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtzrtvoqzd.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtgmauwpse.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hnqzz.top/gtfmfyfbod.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtmsvkcltt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtalpzceel.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xinyue.icu/gtjnhqgsum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtkbssswcw.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtewgekgkk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtvopwfyyf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtsdxmlupp.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtlxtwaqgq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtlaqhilrt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtqanaochc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gthtagfixk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtipzgjjbt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtnhbnqlqd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtfccxmyyt.html

C#:   obj?.A?.B ?? default
来源：http://hz.cheryme.top/gtpdughavb.html

[H07] 断言
来源：http://hz.cashguo.top/gtwyzygxaw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtrnacegak.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtwemliuea.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtipxjagxd.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gthyfxrrst.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgufenzy.top/gtnteipsti.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gthbpsltcw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gthsnoaati.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gthffdaffp.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtwdpgldah.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtfnpcyqrm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangkeji.top/gtzkdlvfjs.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtqxcylspu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtenezemzs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shuidangran.top/gthlfkhmai.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtlinmemgy.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gthzcwqzqw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtidwbbzhs.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtkugigjta.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtgxhcoepb.html


<!-- 参考信息 -->