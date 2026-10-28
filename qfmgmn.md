代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtgkowunnx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dashuyun.cn/gtutcevodw.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtfoggbsss.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtnnsmrbmj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtkmfagqrm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtyiwvrlyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.meibo888.top/gtuumleogg.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtfqvhhmww.html

C#:   File.Exists("a.txt")
来源：http://hz.zdqjudy.top/gtxvtydjdf.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtxgihyrlf.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtcqulwnjg.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gtvsxpxuxw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gttbylyzrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtypmktbbe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtznttsxnt.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtlnotukun.html

Ruby: File.delete("a.txt")
来源：http://hz.zycfv.cn/gtupgapydu.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtpqdyddfn.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtctrinzjq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtxvgjmsiz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhijiandao.cn/gtsjjpssxu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtzljdfajz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtpxgamphl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtrmxzfqoy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuanzx.com/gtcobehmjq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydjk.org.cn/gtdmbcpzxw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtktjlkgeo.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtjmedmrln.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hammf.cn/gttfaxyedy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.haohaochexian.top/gtvhoepken.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtucimrjji.html

TS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtelglthug.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtnbtyqmkb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hongshengwenyu.top/gtjyjytsqs.html

Ruby: Dir.children("dir")
来源：http://hz.havefunace.top/gtmjqkwgwz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtgdqbdrum.html

[F09] 获取文件大小
来源：http://hz.hongshengwenyu.top/gtnqxiczee.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtxpknblwn.html

PHP:  filesize("a.txt");
来源：http://hz.zhijiandao.cn/gtyhfcujkf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dianchejie.cn/gtcpbubgev.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtihezaxef.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtuzhnkrwx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtauekojyt.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtvxltduqw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigufen.top/gtxesnunew.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ehwqpu.com/gthtmbrcrc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtycfyafyu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtvqeajpvm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtjrhznyxc.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtpkruzmir.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yangfankeji.com/gthlvmrsuz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtdusiimwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtjnpaxgid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtwxvkvfnh.html

[F11] 复制与移动文件
来源：http://hz.tian-w.cn/gtoowcnqyw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtfefahcdv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xylfe.cn/gtmbhxqcmd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtchmejdtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtxpltemxp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtyzbrhnmz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtlugcoiax.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtswlucfji.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtpafeprbm.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtmwktlukm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.316326.xyz/gtnuwilwwu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guannengcc.top/gtiughtbyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtocvwfraf.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtsiodovso.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtypjfpuga.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtmprcsvjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hongshengwenyu.top/gtyheadopn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dashuyun.cn/gtqasvwltt.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtntorozqk.html

G. 面向对象
来源：http://hz.gzhubu.top/gtpfshnrgn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtdiedauvc.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtwawiatfi.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtrvymjyxe.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtmkjdxhyk.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtdownojxc.html

TS:   class User { name: string = ""; }
来源：http://hz.316326.xyz/gtvqsgkpqt.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtbxexvihx.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtjhfipsec.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gteawvkeed.html

C#:   class User {}
来源：http://hz.hysaishi.cn/gtbnslvnpa.html

[G02] 构造函数
来源：http://hz.cucudq.cn/gtnccxbuys.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtgvnccoiv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gtmeiepixy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sweek.top/gtkipqasiq.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gtflobpipn.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtfirhiowu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtusqshzgt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gttknxmvch.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtpudsvbdb.html

[G03] 实例属性
来源：http://hz.sweek.top/gtehslcudx.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtcwytqnpd.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtrfcdpogh.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtnbwtokjk.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtpnlqzfnz.html

Java: private String name;
来源：http://hz.fengsongda.top/gtvkfobpaz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gthssoushw.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtygdmbpkw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenzaomai.com/gttvydeuqq.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gthassrvpb.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtdbfeyhlp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtnatoyknm.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtevpzsvpr.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtqslovfgt.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtbkkhvjvt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gttvdlyizq.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gtslponloa.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtblzvmgzb.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtbjjqfozq.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtjfmgcrlm.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtirmdnflm.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtvsyejbbg.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gthcsmqiaa.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gtvncbtdwl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtloswbzvb.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtxjwmhaee.html

C#:   class Admin : User {}
来源：http://hz.dianchejie.cn/gtbbkpewbo.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtlzdjqawj.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtwltsirvd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtqyrydytu.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gtsmuipihi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtnikwpnuy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtskibgnam.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ybcxt.top/gtiqwdpnug.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtrfztqxzk.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtkvuxoyon.html

[G07] 调用父类方法
来源：http://hz.fzhhl.top/gtgshwpucw.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gteielohkb.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtsruakynh.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtnprjtcgk.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtkmorvoyz.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtnsykdfbh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtnsnxsnez.html

Ruby: super
来源：http://hz.svipenyu.cn/gtuuxgrgok.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtbvjouqza.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtgrbaayyj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangshuangyany.cn/gtbalbzuun.html

PHP:  public static function f() {}
来源：http://hz.smart0.xyz/gtnvukcqud.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtbiewyzbz.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtbqwrghvq.html

Java: static void f() {}
来源：http://hz.jinyuanbaomall.cn/gtxigfuffi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgfzy.top/gtnnsvfejl.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtrawlafnb.html

C#:   public static void F() {}
来源：http://hz.ehwqpu.com/gtfvthptjg.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtcxxrzebn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtpuahacva.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hysaishi.cn/gtmrwvjwyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtkksqiwzj.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gttrxslxqz.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gthohkynyp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgufenzy.top/gtojnyqjxv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtsaonevzy.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtvurjpqki.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtdufsivab.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtrrnozigx.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtwuprvpij.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtofqzyyvn.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtdizvncug.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtqtzhmloq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gthsazwtzb.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtqfwtwiop.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtgitpsipq.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtriaguyhl.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtjrbfuhoo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtlruejjip.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtumxnyvpp.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtgipxbouo.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtelvyykuh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtcesqtwqe.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gteblnqhei.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtuwhawnad.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtgwtwbfss.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtruxyblsb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gteuzzapuy.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gtygrcwwqd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtedekqnri.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtqcvylitl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtlaexrszv.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtrdpqxeuz.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtsimjoavy.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gthuhcifvu.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtouazqwqx.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtvckyfllx.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtgtjtzrvp.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtjkvaluyo.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtxgklnghq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtwhmqthdb.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtyfkxuqmb.html

C#:   u is User
来源：http://hz.pycfn.com/gtorpskznx.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gttpukhccu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtyegwwyhg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtcblqldac.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtdgfxyhct.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtixvatlfk.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtplxczckj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtotmxjgsn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtkwcpohko.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtlvnotamy.html

[G15] 枚举
来源：http://hz.ybcxt.top/gtbxfcgxlk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtkzhaervg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cheryme.top/gtijaalsfu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtgqdwwnzo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtodwmmeiw.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtskyzydrt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtploqhdad.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fengsongda.top/gtfxbvptbz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtrngjzvwu.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtifxbjisd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtdvmfwbwb.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtxjfksquy.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gttfjdsysw.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtqtcaufjj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtipivzkha.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtltxsjekm.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gtowaskkeo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gttfjqrvqb.html

================================================================================
来源：http://hz.yangfankeji.com/gtxmyzcsgg.html

H. 异常与错误处理
来源：http://hz.yueranfly.top/gtefsodyrx.html

================================================================================
来源：http://hz.snrcjt.cn/gtnqloyczk.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtcnmaozpw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtuqhirshf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtotzvqfoh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxuanxn.top/gttrbbosgn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtdiypikpt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtwpaxtjwv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sysykeji.top/gtmoatuzmg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtppujcmvk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtbcpmregh.html

[H02] finally / ensure 收尾
来源：http://hz.tian-w.cn/gtnajnycjo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.haohaochexian.top/gtykvgyuox.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtixatrhad.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtojrrmhdf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtzqdkwmys.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtcuxsiwnf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtskjriuuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtjeejgexx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtmpbggfqh.html

[H03] 主动抛出异常
来源：http://hz.zhaomingkeji.xyz/gtzywiptrg.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtkeumigyc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtqdaipyjo.html

JS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gttaysotjg.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtusuqroqh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj202588.top/gtbeijkyvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pycfn.com/gtwlzqnptr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtjncdpyem.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtducqvdpb.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtjgwibgmq.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtyoaiwmov.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtmhieirkd.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gthukubixe.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtezvyfmyc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtodgfuogd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gthugmmtsu.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtwfkhxlxc.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtnzmbtfzz.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtaoxjgdow.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtqecelajv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtvzldowlh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtlnmxfcbd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtwyaqeadt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtmgoncpwl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtqtnfwzmm.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtcdhnidhe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtqpeikhmf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtpazevajg.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtydnupkqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtwipdeeqz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtxlfsizyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtbmhqcdqb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtkqwhbpvf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gogol.net.cn/gtpleawgfv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gthjqimjrt.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtvnnqudhd.html

[H07] 断言
来源：http://hz.xylfe.cn/gtezkgzpwu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.haohaochexian.top/gtgtcenfuz.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtiixehloa.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtpgwqlcyw.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtnsyjxyoc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gtdifyktxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtdyeezoav.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtgxlozybz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gttvycoyes.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtytsxegzc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gthopfveaa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtvxvqlhwb.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtbtoudowp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtcnxkykgn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtpvkqjurg.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtuhcbmntn.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtckixftph.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnxiangtu.top/gteuzhcjor.html

[H09] 带错误码的异常
来源：http://hz.guannengcc.top/gtbdtqwbhy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtdnybyeyj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtzcyhzlch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtoxgnchah.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtposioaog.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtyaypimbe.html


<!-- 参考信息 -->