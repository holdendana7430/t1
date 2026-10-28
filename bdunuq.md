代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.jinghuilouyu.cn/gtnwngqzdm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtsjuncrnw.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtebogytbm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtfahyhsar.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtwsrwtjrz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtxmpxlrnl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.svipenyu.cn/gtmrvpzfpk.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtuojhifts.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtyjbzknrw.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtanwwglyb.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gttuipfbbh.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtvzzbkjip.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gttvybroqa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtuxijouly.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtpelygqhs.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtcwbzdlyc.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtspejztgp.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtkriplben.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gttzbydjhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtwfxhnbey.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtygukjeoq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtxikpaxhq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtlalnxsbt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtjsaqyruj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtbrakiqzf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtbuffodto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtojtkhimz.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtwwsfbctd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cucudq.cn/gtpmozakcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtshtlhbou.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtxoipzeml.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtjqvhlqdr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtyenljowj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtkuhbzxpc.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtqggrtmvd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtestijitc.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtbdfidoym.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gteiqimxmz.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtdqiyckzg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtncwvfpnw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gthjmxbiud.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtmtdhgkqf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.snrcjt.cn/gttclpikol.html

Ruby: File.size("a.txt")
来源：http://hz.sxryk.cn/gtbvpclgrb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtnbtqpngw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hammf.cn/gtxakgpuin.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtwvtdcsgc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtgacebncd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtetizeyfw.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtuuyppcmo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtzphdlntx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtgwrxsiub.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtzrbszlxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gteyejlpfr.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtbvpblxqm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtvkshuhup.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydjk.org.cn/gtiieohbns.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtohefivrh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtoksulzto.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtmgfxypha.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gthfvibtxo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtlkdwfxch.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtpqehpqfj.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtcykhhosf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtdtjxbqww.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gttxggnvdd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gthlofagzf.html

TS:   // 同上
来源：http://hz.ydzc1.top/gtlrixxoge.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gthhuxatgh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtwdrpjtpb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtrsqvtsks.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtljtedsjx.html

================================================================================
来源：http://hz.yangfankeji.com/gtmsvcndtz.html

G. 面向对象
来源：http://hz.pycfn.com/gtnstklohb.html

================================================================================
来源：http://hz.aibaodan.cn/gtwhnwrdlw.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtfwdudlyj.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtqmmphzkt.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gtuchbsrvw.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtsffcmkax.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtmptiscie.html

Java: class User {}
来源：http://hz.daria6918.cn/gtbsaonwyt.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtveohoaxq.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtzffdykpd.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtasptrqud.html

[G02] 构造函数
来源：http://hz.jiagoushi.top/gtihmwigxu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ywan-chungtsiang.top/gtxuufgjqf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtmgvuqgvy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtjywrayzp.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtrwojyacx.html

Java: User(String name) { this.name = name; }
来源：http://hz.yueranfly.top/gtxajcowmb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtgfmafzro.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtnvpkqjwa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtkiabbpcz.html

[G03] 实例属性
来源：http://hz.shuidangran.top/gtnzldtqmz.html

Py:   self.name = "x"
来源：http://hz.316326.xyz/gtiqvsohwa.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtqkphltgp.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtcrvlevdg.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtelkreoae.html

Java: private String name;
来源：http://hz.52xcode.cn/gtirtdpzfp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtinplqnsl.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtitqaejjr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuetiantiany.cn/gtmxdelgwx.html

[G04] 定义方法
来源：http://hz.sxryk.cn/gtoeshuknj.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtpsdsupwd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtffuhthjg.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtlmcgwpis.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gteautaawe.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtzhlrfgpg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gtfybsrydc.html

Ruby: def greet; @name; end
来源：http://hz.jyoumei.cn/gtomcezlog.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtbwagbcoy.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtetgjieov.html

Py:   class Admin(User): pass
来源：http://hz.hysaishi.cn/gtzrualqwl.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtzflmpiez.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtbwsijggw.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gttwwjqkpc.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtmhrgkprb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtqmtpnnmu.html

Ruby: class Admin < User; end
来源：http://hz.xylfe.cn/gtotxkxpcm.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtkvkriazt.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtrwyrtuyq.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtzymssbky.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtsxjhnocy.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtoejfgtyz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtkpltyboq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gthgxlwvom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhaomingkeji.xyz/gtvxhhhrwa.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gtutferhku.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnqzz.top/gtrrnewzwk.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtuzkmhcup.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gteogoeqon.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtcjtpnnzg.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gttujquizd.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtjyhxtxmo.html

Java: super.greet();
来源：http://hz.yj20258.top/gtzyqdyiic.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtbxtznryt.html

Ruby: super
来源：http://hz.jinqigfzy.top/gtxzozzjwl.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtltmoryyl.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gthxowlwmd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtitsimxee.html

PHP:  public static function f() {}
来源：http://hz.hammf.cn/gtgtcitcul.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtijjfjtri.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtcvnldepv.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtweivarte.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtzszilsnk.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtdmvxombm.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtvmvjjrwy.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gteyiegdxn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtiziiicay.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ppjwa.cn/gtcknxagxw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtlnrqahxp.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtfbmigago.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtyaxehvjq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnxiangtu.top/gtwhvwfqth.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtugidhhkt.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtuzuidifl.html

[G10] 访问控制
来源：http://hz.chenjidiqi.icu/gtrugwlrtn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtqqwjhslv.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtwibqrhwo.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtibitabjg.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gteokoexfs.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtiaxdmdbj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtvfjnuevq.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtidescgfv.html

C#:   public / protected / private / internal
来源：http://hz.zhengqikj.top/gtkwoammiz.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gttaufgtek.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtkngikhut.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtkpdewwep.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtdawzwtst.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtllkxavlp.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtyiwwsiig.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtimzkueli.html

Ruby: attr_accessor :name
来源：http://hz.316326.xyz/gtomxztfok.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtdzznyaqr.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtvfrlxrlb.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtfmfyqlqj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtncgsyswr.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtjxtgxxbp.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtbutdqozx.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtvnwvkcma.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtrqtmhojf.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtqwhhhzap.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtowrirjcm.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtnfozcdyu.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gtxarzwxph.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtwtnuafom.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtjqlvhfxy.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gthrbiutps.html

Java: u instanceof User
来源：http://hz.pycfn.com/gtmuqpwnyg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtqrppfeoi.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gtfblnuspv.html

C#:   u is User
来源：http://hz.ydzc1.top/gtwqdayykd.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtybyznass.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gttijozkuo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daxiang520.top/gtugdxdfex.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtcjolisxw.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenlongwang.top/gtfgwypycx.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtnwmieush.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtdihdigdp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yvedp.cn/gtogjvwfbg.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtomhhdaqf.html

[G15] 枚举
来源：http://hz.xinyue.icu/gttulnenea.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtbnjcytep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xziqi.cn/gtulmgwmph.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtcobgedfg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtevcpslup.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gtetbjfkmu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tanke756.top/gtyynwvbwl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtqscakxwc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtealdbyad.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtdrevfmbe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtpeapklln.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtxfbzinxx.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gttgvqbbmg.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtpuyrftqu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtbkwytgxg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtnazavwtp.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtplgomivt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtbnzwjhwf.html

================================================================================
来源：http://hz.mhx1999.top/gtupfgfswa.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtekssstbv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvxgnpqre.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtxsrjrcam.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtwetqqtyl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtoyfpywgc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtpfyijoez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gttogqyvel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj20258.top/gtpdoiahzx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gthednqwvo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shzxlz.cn/gtsmeanwgq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtfmpvmgjb.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtwxvsttkf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yanxiufei.cn/gtjnetbjkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtwdezuhkh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtbuefvyaa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtqebljtej.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gttdmhhyjh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtrcsgidmr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gthnxlqpqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtrglglxvk.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtehdrxxzu.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gttqzaoeir.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.316326.xyz/gtmqsdsihx.html

JS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtajuvsdgg.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtjfkymwqs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gteyjwymlj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtvdawicvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtmpuhfndt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtsjoxstkz.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtolkqgtcq.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gthjitayne.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtbnqfuqmw.html

JS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtyepoyqtk.html

TS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gttmzuwjin.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gtwvnpdtua.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtvhffqgda.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtenneoikd.html

C#:   class MyException : Exception {}
来源：http://hz.chenzaomai.com/gtjucydfct.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtuhavlpdn.html

Py:   except ValueError as e:
来源：http://hz.cdnleiting.top/gtqvfynsdz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtygqudyxq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtutoaqykt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtqqvlsiah.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtldrfdzvw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ywan-chungtsiang.top/gtuuspvwes.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtmothzhlk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtmwqfskmv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtnevfrjdg.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtxqcrjozr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.meibo888.top/gtkhtxgvja.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtunsdpuue.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtshsuqgnj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtnzdnagiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtqeydkzcu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtbqclqtsu.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtjfrrzknt.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtenvkhtas.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gthmidiyho.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gttvogkzmt.html

JS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gthdysemhh.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtiztybfox.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtbpccvrrj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtjvccjawp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtcgsjyqkv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gttoisafjb.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtcdcjkdmy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtilaqqehw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtnyzszixq.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtmvlofqhu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtsfeffiot.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtglooelfx.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtmpotkcut.html

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtfxyngrgf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.smart0.xyz/gtdyismpea.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtbzxqibda.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gtxfyrwvoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtxmewdssj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtjtmjtfhh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtvboihwum.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtuhhwxzps.html


<!-- 参考信息 -->