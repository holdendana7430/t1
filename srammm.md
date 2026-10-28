代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtjwkvybiv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtzimdymlg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtwholaaom.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtjkymtudy.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtmugcjzry.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gttgjcbkch.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtsqwkxbsd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtmjgbcpzp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtyrwuwulq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtangukpjt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtbcbmrcov.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gtbqbukcfh.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtgymfleqg.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtbkhrnire.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtxkhkvfeb.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtsrzviosi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtmiqgchqc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtnryxizhy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtvltwuzrs.html

Go:   os.Remove("a.txt")
来源：http://hz.yvedp.cn/gtyunrbzrj.html

Ruby: File.delete("a.txt")
来源：http://hz.ivvv.top/gtujoxyrzc.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtnejbrkbk.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtfuuiidii.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgufenzy.top/gtiorlzari.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gthenfsgjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtelvxychy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtthqxbweq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtzwubzjzg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtmvniiprg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtpqxvlmga.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtyyglkylm.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtfafqtjlx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtedbrdzhg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtaisjpini.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtvgdtjyyz.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gttrodixyr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtiweqqphw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtyiyxdktg.html

Ruby: Dir.children("dir")
来源：http://hz.cucudq.cn/gthscjkeef.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fzhhl.top/gtsfanauqi.html

[F09] 获取文件大小
来源：http://hz.gzhubu.top/gtajwmbkwj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtjroaayma.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtfytmujgj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtpejfpfjl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtbzewvikx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtiusmeaxg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtmhxjshbw.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtwyiyyixe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtupiyeoli.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtfufooprb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtpidspryj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gteanyfynt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtghqaelfx.html

TS:   path.extname("a.txt")
来源：http://hz.shzxlz.cn/gtatpkidvd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtoauxegro.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtuxwcegwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtrjcbeqma.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtnbvmkqfm.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtrtavttdt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gteonvjgtx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtcpykqzvi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtuvncisqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtacjfhmtd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtyomvxwkn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gtrzwtzpst.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtwuwrfmmq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtloplyapa.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtelcjohff.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtbseziaeq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jianghu66.top/gtkrwhnphp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtpywabtvs.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtfycqcotp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtmlyibzoi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnxiangtu.top/gtdkagwduu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtpicvbhel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gtevuqsews.html

================================================================================
来源：http://hz.quarkkingdee.top/gtomsraiwz.html

G. 面向对象
来源：http://hz.tanke756.top/gtzogebdyu.html

================================================================================
来源：http://hz.chenlongwang.top/gtnhwwfdcl.html

[G01] 定义类
来源：http://hz.xingfuxueyuan.xyz/gtozqnbipa.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtvdbmjuuf.html

PHP:  class User {}
来源：http://hz.redwolf501.top/gthztksaqs.html

JS:   class User {}
来源：http://hz.cheryme.top/gtfamjivsj.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtdnhsxdcm.html

Java: class User {}
来源：http://hz.ivvv.top/gtllbrvbwg.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtzdzjovxj.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtqvgvtemr.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtqdbmatkm.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gttqqhpvzs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtrnsveqyr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxinkj.top/gtyqtkgzye.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fzhhl.top/gtphvakgjr.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtsttsggka.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gttiptosem.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtlehutqds.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gtwmcnbmca.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtlrjrofxo.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gthokustdp.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtvzvcvnav.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtagtywssg.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gtcqithnym.html

TS:   name: string = "x";
来源：http://hz.xuetiantiany.cn/gtzzigsuuv.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtyrjcoaut.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gtcetvndhf.html

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gtmtcjenpy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gtecdjjeqt.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtefwosigm.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtiopguoxh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtgrawfkrz.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gthmlbxaqg.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gtkesdbnyu.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtaygphlfu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtsjctydbl.html

Ruby: def greet; @name; end
来源：http://hz.yongpay.top/gtybfqfhuf.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gtciesqbkw.html

[G05] 继承
来源：http://hz.aizwys.cn/gtlfumwqsh.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtlwxvybnu.html

PHP:  class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtolgysknk.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtddkqksxm.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtcodhmmex.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtigjixtal.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gttathwmme.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtzzfnazhb.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtxkifldzz.html

[G06] 重写方法
来源：http://hz.zycfv.cn/gtkkiokpdh.html

Py:   def greet(self): return "admin"
来源：http://hz.ehwqpu.com/gtfumyvipg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtcgkvmiov.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtcfmavimk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtunlapnfw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtyqqpcoba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtbxyoglvl.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtabbyqtet.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtjjuplxew.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtvbxazmbm.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtyvfyrtvb.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gthsvibwue.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtinwoxgfj.html

TS:   super.greet();
来源：http://hz.jinqigfzy.top/gtxxhpegbk.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtwrrwquli.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ppjwa.cn/gtktvbwejn.html

Ruby: super
来源：http://hz.pycfn.com/gttkhsmagd.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtlfbzpkxn.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtxhzkscbd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtovakykqy.html

PHP:  public static function f() {}
来源：http://hz.yuxming.cn/gtuhhsxzca.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtvatvbkeg.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtzjukstls.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtcyaveeuk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtozaoiszi.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gttwmrlprv.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtgpyjdjbb.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtuiksabkq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtboywaylu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtcwmvzkqe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtrdnpaslz.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtnupfanjx.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gthpagmafg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ywan-chungtsiang.top/gtfmnfngxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gthismrfyz.html

C#:   interface IShape { double Area(); }
来源：http://hz.gzhubu.top/gtktqhjgii.html

[G10] 访问控制
来源：http://hz.cheryme.top/gtlkihdcff.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtwkbgsxcq.html

PHP:  public / protected / private
来源：http://hz.shangyingyoupin.top/gtkpsfxxsl.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtvqjfhrtt.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtbjxtrlyt.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtjhufffnf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenjidiqi.icu/gtxagcsgqv.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtdmplvube.html

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gtjbrplxxw.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtarurbpaf.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtfwgkhngl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtddqjwiih.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtvevqjohk.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtptzojgcp.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtahahsugc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtkfkaxtjo.html

Ruby: attr_accessor :name
来源：http://hz.fengsongda.top/gtzquawqtq.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtqrfbvvsx.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gtntnjxjqt.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gttnuzehmm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtujzpvzco.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtpyvwoopf.html

TS:   toString(): string { return this.name; }
来源：http://hz.yonumen.top/gtionnzvgp.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtipoujpen.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.52xcode.cn/gtnzoqhidf.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtxhjnityu.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtnftufqti.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtaixbypmy.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtfwbfypqb.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtwyqavwnq.html

JS:   u instanceof User
来源：http://hz.xziqi.cn/gtjfxarnma.html

TS:   u instanceof User
来源：http://hz.snrcjt.cn/gtfbtbbjjd.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtjrycltcf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtvmujgwha.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtjyjcshms.html

C#:   u is User
来源：http://hz.yvedp.cn/gtfdfsxysq.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtxydfwalt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtrgaegciw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtvkynlxrv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtjeticvwg.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtjfqhxnzu.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtcqzlwjji.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gteiumuomc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtsazivzyf.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gthcyuhuru.html

[G15] 枚举
来源：http://hz.vqdsnc.cn/gtracdqiil.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtkxqktfrl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtmguezmda.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtcstrlsel.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtcymhwzel.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gtzwjbhqpc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daria6918.cn/gttunxtbop.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtgvbduhly.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtsacwrtka.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtcgointic.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtfptydexw.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtzmiwpwou.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtmtopvauo.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtthfjjtjj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtfxcusefy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtomdbiwah.html

Ruby: obj.instance_variables
来源：http://hz.guannengcc.top/gttktxlhkq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtqimpihss.html

================================================================================
来源：http://hz.c1oappe.top/gtgzmsaukw.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtqjnycxfi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpyrlktai.html

[H01] try / catch 基础
来源：http://hz.chenjidiqi.icu/gtdwzulnmi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtddqtcxnw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtytpsjtzh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtfzryhqcg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtfwzkljpa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtbhhwpntz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangkeji.top/gtclzubtce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigufen.top/gtaoclcxnb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtrhuhyjvz.html

[H02] finally / ensure 收尾
来源：http://hz.hammf.cn/gtapdutrsg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtrifjdqxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtlfztpble.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtrmnxsqqi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtdogecjcy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtcqmtjhkr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtckejktnk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtkrcdxsbc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtuqceuhfs.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtruegfxyu.html

Py:   raise ValueError("错误信息")
来源：http://hz.smart0.xyz/gtpstglyrg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtesbletvj.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtllanmtud.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtnwfrdmpt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtzyvrxjae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtgqrqbslm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtljgriwku.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtbsrrmswo.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtjngoiweh.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtypgglzhj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtwzqmlaol.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtsvzmodxe.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtyzaidxxd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtwjjykhrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtrqcpfksz.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtgcdyzvza.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtbkhipedm.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtootplmnm.html

Py:   except ValueError as e:
来源：http://hz.zhiwuduotai.top/gtqnxdziof.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.0kj1m.cn/gtgzohagqc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtinljggwl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtpomyfcyw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtrpdynjll.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhoulong.xyz/gterkumrak.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtchbfgfph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gthxibhlaf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtuscakzbz.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtverlrdjl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtrhqxvwjj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtdlgahbwb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtreihndnt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtvaydjbih.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtcsovjply.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gttozmosvg.html

C#:   obj?.A?.B ?? default
来源：http://hz.sweek.top/gtgociurmt.html

[H07] 断言
来源：http://hz.hnxiangtu.top/gtnmaaznjg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtpqudyopm.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtfswliivy.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gthewpazkg.html

TS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtyhlelhzd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fzhhl.top/gtnebelmgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xingfuxueyuan.xyz/gtwmalqouz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtzrviibia.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtvgzccbmz.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtwxbttatk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtpcqgmbse.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtximpyscs.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtjousevhd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtgwbnunzh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtxuuylzqj.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtfxcymdoc.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtpsqjpagd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuanzx.com/gtmdpgidhl.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtrzjqtjer.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gtmtcvddgf.html


<!-- 参考信息 -->