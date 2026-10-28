代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gthtllvzyh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhoulong.xyz/gtzgnkbqsx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtjvtlkkkg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtjhbtcgkg.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigfzy.top/gtampwxsia.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gaohongyu789.top/gtfemornui.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtkvkwvjwj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtvwbclsxn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtevantwzv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtjlswvrjn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtraaxazdv.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtsygcvpag.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gttwelnhme.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtfbhbduke.html

Py:   os.remove("a.txt")
来源：http://hz.shuidangran.top/gtwnzkppse.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtgwfbqgpi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtutgchyuo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtebvwoncl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gthjxzotgo.html

Go:   os.Remove("a.txt")
来源：http://hz.yueranfly.top/gtlwdpoocd.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtwguxojza.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtwfommjgm.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtzxduwyjg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jyoumei.cn/gtalcfmmnd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.c1oappe.top/gtkxthcayv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtvagayjkw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtbpuktaqx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtwtcvzzfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtvmfgsmia.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtvjlvnjou.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtzuzhaurr.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtgddxazaw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.dianchejie.cn/gtoeknnsxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtzhmvwiez.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtmfeovoqn.html

TS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtxmjrmzsx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtgxrggmzx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtsovpqixo.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtseixwkrl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtjgxtpjju.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtlbapabiw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gteaojcnza.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtryjzesml.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtcyjhpcgu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gthcdufnjb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtuzmfrwiw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtvovapink.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtgftnnlkj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtkapijdzw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtunsvwayf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtsnnrrhdm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gttysfonwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtszpctfrs.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gtupubsbyr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtjlelpnim.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtowyrumwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtjctbqzpl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xinyue.icu/gtgtkwjyfc.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtvliawrya.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtodynhuea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.havefunace.top/gtqrsgziyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtdwoazlsl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtvhdqluep.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gthjaztiep.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtalbizlht.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtkazanzlw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gthifqltqc.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtfqjgvagd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtjgloyfqk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yangfankeji.com/gtncvccxll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dianchejie.cn/gtqnjgbpox.html

TS:   // 同上
来源：http://hz.pycfn.com/gtmenfzwhy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtffmrbgno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtsqohvpys.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtnxxokdjc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtobskkoql.html

================================================================================
来源：http://hz.andypj.xyz/gtocojnuoo.html

G. 面向对象
来源：http://hz.shuidangran.top/gtzsdzjpfg.html

================================================================================
来源：http://hz.yvedp.cn/gtyvlafnxq.html

[G01] 定义类
来源：http://hz.xingfuxueyuan.xyz/gtjgtmnqxs.html

Py:   class User: pass
来源：http://hz.svipenyu.cn/gtvxssgwcn.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gthjosfcpi.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtzztfzmhr.html

TS:   class User { name: string = ""; }
来源：http://hz.chenlongwang.top/gtjhngwutg.html

Java: class User {}
来源：http://hz.snrcjt.cn/gtsobfoqyq.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtjxniidgc.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtkmgzftgw.html

C#:   class User {}
来源：http://hz.pycfn.com/gthhheaerc.html

[G02] 构造函数
来源：http://hz.cqqwz.cn/gtglbtvngo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtgbjcbcxs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtgwvtywgf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtdavzfceb.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gthlgcmwwg.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtmgoorjgs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtslwiueix.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.birdmap.top/gtlxidiivj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtberjavmh.html

[G03] 实例属性
来源：http://hz.sweek.top/gtjuxttoci.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gtuozrvjzc.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtrseddryw.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtrbgiqggz.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtazpmseze.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtiidhwaoo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtvcchwbbj.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gttjjdqqwz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtmikqxhto.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtyacegecv.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gtuunjymov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtbimqfsqj.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gtakakczno.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gthkuhrzbb.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtjqntaxsl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gtuedjwcre.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtmkigdiru.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtbrjzrvpj.html

[G05] 继承
来源：http://hz.zycfv.cn/gtremrrsmd.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gtrbpskqbi.html

PHP:  class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtdulveiev.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtasjkruzs.html

TS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtdurkthpq.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtmlcoxrpx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtgdukkcse.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtyxoyejii.html

C#:   class Admin : User {}
来源：http://hz.sxryk.cn/gtatjkmbic.html

[G06] 重写方法
来源：http://hz.sweek.top/gtyugsneir.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtnstdmtjm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gttnbgpeje.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtjrbxqpaq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtiyjriizj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gthojmldyw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtzdkufggz.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtvuupayiq.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtlfjozshd.html

[G07] 调用父类方法
来源：http://hz.shangyingyoupin.top/gtgdtprovk.html

Py:   super().greet()
来源：http://hz.xuanzx.com/gtkcazeniv.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtviweswcs.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtrfrukgmy.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gthpowsxbd.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtnbqlyagd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtczxasraw.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtcpzlztkp.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtpfywjjaf.html

[G08] 静态方法与属性
来源：http://hz.hnqzz.top/gtiphhfhey.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtimkzugik.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtsahrgqac.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gtwfasucbw.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gthgdnjmro.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtbemdkiyr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ehwqpu.com/gtnnceqqaz.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gtkauvqvck.html

C#:   public static void F() {}
来源：http://hz.mhx1999.top/gtswdtaknn.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtdlziukcw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shzxlz.cn/gtcrofzdji.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtcchwxkvj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtqacuklrg.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtiaygvzhb.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gttifnudac.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtjivrizrm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtdamydikx.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtvjyvuppp.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtgsxkcgqe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtbyktvxlg.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtkfklozdt.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtjfctmzzl.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gtduqtrbsj.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gtgpkqgosh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtakbkmggj.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gteydufnzk.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtbpxnpvfp.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtauedsoun.html

Py:   @property 与 @x.setter
来源：http://hz.52xcode.cn/gtkalbpxsp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtbnqjgbvn.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtklrlqzcy.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtolgsvklg.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtlegduemc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtnkmxkvqv.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtdyyalmet.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtcukerzbb.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtwolgrjxs.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtolivfwpe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtctzaavgi.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtwgqmfjno.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtfoonuidl.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtszwanara.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtsvygfpkg.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtsenuhsna.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtyimtqtou.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gtvnjweqwl.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtotpzagyv.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtgpclcyvr.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtzqyzxtbj.html

TS:   u instanceof User
来源：http://hz.jyoumei.cn/gtghgxkqei.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtawalxqsa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtmvbxcvbf.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtofxaerbo.html

C#:   u is User
来源：http://hz.fengsongda.top/gtuzqegdep.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtpqtcbjou.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtskuyjoeb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yangfankeji.com/gtqyjlzqwc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtbtdlzfpo.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgufenzy.top/gtjmvhenib.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gtjnujkwjt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtkmquhdpv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtbtyyauso.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtlmqfcrzs.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtcxwvwshe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtqfmeiime.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenzaomai.com/gtxjmfzhmy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtvhfsruqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtrerjhinj.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtrdgxkjym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtkkxyyczy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtyjmkmgfj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtgtobhsjc.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gthnxufgjs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtqqpsefgb.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtyiounpjl.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtfxmrnwfi.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtpiyddaqe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gttbmitanj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtsppzfcxx.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gteonodsnv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtfmlnukmd.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgkpxbpty.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtlxoxkayr.html

================================================================================
来源：http://hz.316326.xyz/gtorxnfjzg.html

[H01] try / catch 基础
来源：http://hz.smart0.xyz/gtoqhwmkvz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxinkj.top/gtzgdyklzf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtfaigpyvx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtgiocvlqv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gttutrnsdc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gtulqrurva.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtugijsztz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtoqjnjfep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtifyaeiyt.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gttrktqlcj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtnqmccgkn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtrfefwhru.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtnhwqsehm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gttnjaxhjj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtvvuufaoh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.9152youxi.cn/gtcygybhil.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtjstybbzj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtfiwpzlfz.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtxrarualc.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtkajmksog.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtabzqrofv.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmuhchygc.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtnhihwekh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtizwyqxqo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuetiantiany.cn/gtpzyejrca.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtayucatwc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtbiigkrqy.html

[H04] 自定义异常类型
来源：http://hz.dashuyun.cn/gtovtywysg.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtgogakdei.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtxgpyxbpb.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtkgfygyqb.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtsfhfkqri.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtkwudhvuw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtfmdtowwi.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gtvvzjhdfk.html

C#:   class MyException : Exception {}
来源：http://hz.tian-w.cn/gtmuxrdals.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtwihelups.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtwhgjubpe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gttcnumejn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gttzmddvur.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtotptumkt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gtmhgksbrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtshiurxik.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtvhrajvdk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zycfv.cn/gtfpoacdjy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtewbzxczt.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtsdgkfczs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtogegmvbj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtupravqte.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtqahdbbni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sweek.top/gtrizxielz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gttnamvjpr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pengpengdd.cyou/gtefnwgdjh.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtlfwlaypy.html

[H07] 断言
来源：http://hz.chenlongwang.top/gthvsvikmk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daxiang520.top/gtjnhgoiab.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtancfhtip.html

JS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtnahcnwwa.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtnjlvrezz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gtuefrnuvs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtzdhhahgq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtsyywwamy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dashuyun.cn/gtroqbkdti.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgufenzy.top/gtbaqlwvla.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cheryme.top/gtcpedljjf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigufen.top/gteuqgrilk.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtlcpgzzqy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gttqrsjbtf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtumfttpcy.html

Go:   err.Error()
来源：http://hz.hnqzz.top/gtvlrhiqnj.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtxrjvovam.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ppjwa.cn/gtxrxtoxds.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtckmbovbv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.feifeiyinyue.top/gtftbiwwuo.html


<!-- 参考信息 -->