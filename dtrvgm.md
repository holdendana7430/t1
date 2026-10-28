代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtnsqxudlr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtraibjrwj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtmzvvdwbj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtslknagvd.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtwjyvtzzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtplaeykku.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gthdcycvvk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtmzypvben.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gttjtlrrfc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtiteaxluz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtxkbscqtp.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtakkzgexc.html

C#:   File.Exists("a.txt")
来源：http://hz.meibo888.top/gtautmrsrs.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtdzwldsgc.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtqamolyzn.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtpucwgrly.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtzuphvujq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtozsqppei.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtkbeigman.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtcgekozkn.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gtkirfpvrc.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtypngwuzu.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtguwzlzec.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtwnwjkpuu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gtscmuwgos.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtetidebls.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtkiynwgyl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.iojbl.cn/gtpjiwbdhg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtyzxxmdla.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guannengcc.top/gtspfkipjf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gttqvxgshy.html

[F08] 遍历目录
来源：http://hz.fengsongda.top/gtodnjussp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtyxpvvpng.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtpualnrtw.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtebeqtqbf.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtdwrbpntq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtzavvrjwy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtqpuvxvih.html

Ruby: Dir.children("dir")
来源：http://hz.pengpengdd.cyou/gtzypgdztu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtinaccfzg.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtybhqonkq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtyuwmqakg.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtcockhtyz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtxjptzdbi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtxefaxrag.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtjlzvskyd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yueranfly.top/gthwfpvbmw.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtvkohyghi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gtkpnskwlu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhongyouzk.top/gtnfdkbcff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtwefksmtq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtkpmcdpgx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtnsanmsjx.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtrgxvvovf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtixvjrsfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtqcuuutlh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtrudjbboo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtxrogrrpb.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gttwemcqzq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtjcgtyyfy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gtbdrzshuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtlxxwetxf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtwqvmqqil.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cqqwz.cn/gtiprdxhva.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtmwfhsjgs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtxgixgdag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtpntjvkgh.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gthgtrxtic.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.52xcode.cn/gtgqajqnpd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtcehxcptk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cashguo.top/gteapseqcl.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtqgsfsqda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.iojbl.cn/gtplswctgf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtojzawtks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sxryk.cn/gtwnmvdpvd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtkmdohpqu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtttpehvuv.html

G. 面向对象
来源：http://hz.zhiwuduotai.top/gtqejvsfcv.html

================================================================================
来源：http://hz.tanke756.top/gtyyyciaei.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtlqooermt.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtzubdeoyp.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtqmqovgzv.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtpkxdduyn.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtzwjypdxu.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtakdgtodf.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtkkzsftoy.html

Ruby: class User; end
来源：http://hz.sweek.top/gtfftipnyn.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtxmdxpowx.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtnnmkvcju.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtmxyzynku.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtmponlydt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtuvvovrao.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtsjwdtgwx.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtpihqvhjm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.redwolf501.top/gtxvluupua.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtwelnahtb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ehwqpu.com/gtvkqodfps.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtgzwrnkdc.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtbsoypuxe.html

PHP:  public string $name = "x";
来源：http://hz.andypj.xyz/gtkpyflqfs.html

JS:   this.name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtqyofacgf.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtwhdzknqw.html

Java: private String name;
来源：http://hz.xuanzx.com/gtbrlxgsxw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gtrdhegblr.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtcynqknkw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtcxkuqfxs.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtoykxjcvr.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtpanbhnvx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtxmliplbe.html

JS:   greet() { return this.name; }
来源：http://hz.0kj1m.cn/gtxinhpqwu.html

TS:   greet(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtfjbjerrq.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtivyqccak.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtksqvepxo.html

Ruby: def greet; @name; end
来源：http://hz.ydjk.org.cn/gtegegfbem.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtujzdmyvg.html

[G05] 继承
来源：http://hz.ehwqpu.com/gttpcfrccp.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtijuzirfk.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtqbmfldbc.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtdtxpfpuz.html

TS:   class Admin extends User {}
来源：http://hz.havefunace.top/gthtvmbcsr.html

Java: class Admin extends User {}
来源：http://hz.zhixingplan.top/gtqsqlttrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtdpkakzwq.html

Ruby: class Admin < User; end
来源：http://hz.gaohongyu789.top/gtbrksqkqv.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtxcdepzad.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtkzxgfxfk.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gtmxbuswlr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtogfwbkbc.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtwweifgkh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gthvsojulj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtyqoxbddo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gtdgaecegs.html

Ruby: def greet; "admin"; end
来源：http://hz.dianchejie.cn/gtjubzmrib.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtxaadhvmh.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtafjlkkro.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtzkwqztvm.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gttxockmlo.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtdceyelqx.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtshhrcwhi.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtimoehpiv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtcdqemtik.html

Ruby: super
来源：http://hz.smart0.xyz/gtramvqrzn.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtyxfhxsbk.html

[G08] 静态方法与属性
来源：http://hz.yangfankeji.com/gtmwmkfuya.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtscvcyass.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtnaumormu.html

JS:   static f() {}
来源：http://hz.shuidangran.top/gtekwuabgj.html

TS:   static f(): void {}
来源：http://hz.jlsjyb.cn/gtucyfhpsk.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtfvlkkecm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtyhmyovrl.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtebsvxbtr.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtcyymencq.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtknvjqiyv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtgmfrqkao.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ehwqpu.com/gtrjalsclj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtbcmegkml.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtxjhqbwmx.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtwefsrjpp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtgemvcytl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtooocfdii.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtkwlppojy.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtkjcvbdge.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gthhjzchev.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtsmaaluvj.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtiquonwus.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtfjcettuy.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtxfdsrrfc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtqahelfde.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtehgxlkpx.html

C#:   public / protected / private / internal
来源：http://hz.guannengcc.top/gtwzzrfhyl.html

[G11] getter / setter
来源：http://hz.ywan-chungtsiang.top/gtghvcemdb.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtzfvxcnwu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gttdthycjt.html

JS:   get name() { return this._name; }
来源：http://hz.yuanzhike.top/gtbhxbibyf.html

TS:   get name(): string { return this._name; }
来源：http://hz.cdnleiting.top/gtwynvzmhp.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtlkfqrczx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtbfccjqle.html

Ruby: attr_accessor :name
来源：http://hz.vqdsnc.cn/gtzxdqmeyz.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gttdixlbcr.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gtntvtbgtg.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtvtqpnily.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtosefsldp.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtsefbgzlp.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtbeertbzo.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtbgunqrut.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtvlakuezc.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtguvtktrk.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtawcalovq.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtmbkkeiup.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtdslamuxd.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtilbuehmr.html

JS:   u instanceof User
来源：http://hz.ehwqpu.com/gthhjxwlds.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtbxntorzo.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gtbwvjpetk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtfwmcwely.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtnajwrlgq.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtgidhukny.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtgnlftwro.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtoyaolzvd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtwtezneti.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtioxcxxax.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtdtzvqrpy.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtogohboqt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtxjwmonpp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gtzwvanujb.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gteeoiyjff.html

[G15] 枚举
来源：http://hz.xuanzx.com/gtmypxhigc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtivpnoswf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtmdpunxqv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtxghoaaju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtodxifzdd.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gtvlydzdbz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gttptakfvp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtqzwnsorl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtiiqsszpb.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gteowmcsnp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtidaldwbk.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtezcpnekp.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtrsmxmwhk.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtujizwwyy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtrqcuiqcp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtouiikmli.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtmjhwqban.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj202588.top/gtdmtmvfro.html

================================================================================
来源：http://hz.chenlongwang.top/gtjpciasqy.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtamrdoshd.html

================================================================================
来源：http://hz.birdmap.top/gtxlnmrahu.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtgjuooamf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtwmmjyusk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtwwddlepo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtqpxcmrpp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtkgjeovwn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtwmfdqglc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtlekuproj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtzhfqfjnf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hywenlv.cn/gtcewiwszv.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gtcnhwxzvi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtmnamdrgu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtqblcyfjf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtutrpnnxv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtltignxum.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtzllyuxxn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gthwzynlvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtowezdrgy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtzpqphlgo.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtwzoxspis.html

Py:   raise ValueError("错误信息")
来源：http://hz.fzhhl.top/gtuyddspou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtvbecgbkl.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtikdefxca.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtfgdvsudv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtjwnsnlua.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtorttvwcx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtfbqrjacv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtmgxmrqef.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gtoorxrpau.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtubxwothu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtodajujhm.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtmmvadohs.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtfnyndsap.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xingfuxueyuan.xyz/gtnbzknndd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtywznwrsd.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtjsedapvg.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtueiboamc.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtnvuoofhj.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtjlofbpva.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtefnfcncd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtpcroadsl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtykkhakah.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hammf.cn/gtixrpffel.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtmneejyrl.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gtriimfnpy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtghrrfiod.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtcmcjfjnp.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtbjtzqflv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtdabbbfar.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gteasdwmez.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtuidmcanv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtujbpdmuz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hywenlv.cn/gtlpflpjfo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xingfuxueyuan.xyz/gtcqzkpwyk.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtoaahqnmb.html

[H07] 断言
来源：http://hz.ehwqpu.com/gtkycbdrdx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gteqjrgkvz.html

PHP:  assert($x > 0);
来源：http://hz.c1oappe.top/gtiffywtov.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtadzyljdm.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtfwfnmlzc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gtqxgalcoj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhongyouzk.top/gthrcarjei.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtqssiyhgo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigfzy.top/gtvgcysioa.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtadyvyjpa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtnqzealvi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.birdmap.top/gtnwtqzwwq.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gttfvnmkls.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtanbyxbpj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtjnprthvi.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtmhbcvwtj.html

Ruby: e.message;  e.backtrace
来源：http://hz.0kj1m.cn/gtuifpszfc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gtqeeahjxo.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtkzasddho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtweckzeco.html


<!-- 参考信息 -->