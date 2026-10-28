代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtxfhfzsyh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtaelzfwih.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gttsldkfbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gthsbqspdt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtfncuahrq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtoufxbtae.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtceebqhar.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gtxnvsgarx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtbswbkrwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gthayxpnha.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtucsnqfer.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.vqdsnc.cn/gtxtjmfids.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtbzbaijnb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sufxvd.cn/gtuhyglpxv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtpqnclyts.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtsbwxgpes.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtnxvkuohd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtkhouhckn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtjlnhcryz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtcntmsdfl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtkmwkaldb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtofhahzpg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.birdmap.top/gttyqhypln.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtshwdsbml.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtmlerldyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtrwrwolfu.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gthrqfrnir.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtpiihaaie.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtlfjybxja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtbhollunh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtyfhbmcjz.html

Ruby: File.exist?("a.txt")
来源：http://hz.shangyingyoupin.top/gtitrdnlgs.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtaumpkrrs.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gtuqqulizx.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtiydkkfqh.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtfjtjaepl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtmstptimk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtawymoqiy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtcfseuadu.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtmnjjohvv.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtnokrokbc.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtubxqnlrz.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtdwuszitm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gteghfnznh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtwfpbvptp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtqjjesjsj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtcsgahunt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtzgkbapbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtkuybrkrd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tian-w.cn/gtdhnyawuy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtjuyvhixj.html

[F08] 遍历目录
来源：http://hz.yueranfly.top/gtmtoascdo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daria6918.cn/gtdialshbx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtzthpllsf.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtltzqahlf.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtetqwetie.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtekcbgmkt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hongshengwenyu.top/gtgtwqasek.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtgymkgxhm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gotoacloud.top/gtdwgjuvge.html

[F09] 获取文件大小
来源：http://hz.ydjk.org.cn/gtqtxfrcmz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tianlin.xyz/gtygwyulen.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtepxwcgvw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtdrxekbgl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtmbjnplfx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtkxxtlitc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtqdxbqqna.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gthjabilfj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtxerscnuf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gaohongyu789.top/gtbwfjoqrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtyymgwgxt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gtojkpdocz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtllcevwul.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtivaaxzki.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtgphnauyx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gttwxhozqs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtsyrlidem.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtjviwahgt.html

[F11] 复制与移动文件
来源：http://hz.chenlongwang.top/gtrtlsmofb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtzhgoqghy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tanke756.top/gtjamnjsti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtddfdihhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtgwrdocei.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtuxqufhkt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gttjcdrate.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtdvnbnpaz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtvlglrxzm.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtnotwpfog.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtcznwaivy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtafqvfefw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtdoonfqow.html

TS:   // 同上
来源：http://hz.cheryme.top/gtonjtoafp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.snrcjt.cn/gtcvmljerh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtimxtnoup.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtcdsxdvrz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtrdwouodb.html

================================================================================
来源：http://hz.gogol.net.cn/gtnbpuzodk.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtoikunsgf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsxbvmpqk.html

[G01] 定义类
来源：http://hz.yj202588.top/gtddjvlvzo.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtilseplxf.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtavhkhzkf.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtdzpyolkz.html

TS:   class User { name: string = ""; }
来源：http://hz.haohaochexian.top/gtkhssemyx.html

Java: class User {}
来源：http://hz.daria6918.cn/gtbyjjznde.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtufpaixmx.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtmgpoftqe.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtpdjttayb.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtruelvzxe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtbstfyhps.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtzjkxljtn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtxqcdepkn.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtdukzykzp.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtccycrkwb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gturnauzwr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gtwbaibwdy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtxapagsct.html

[G03] 实例属性
来源：http://hz.iojbl.cn/gtzxotpffo.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtybpfqxjz.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtqqyzrsts.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtgiexzsyq.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtmokurvzv.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtxtuyqugs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtnsmblwwp.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gthpvzpiai.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtvnknbrrn.html

[G04] 定义方法
来源：http://hz.tanke756.top/gtxdvljjfc.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtlnsrbsjy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtvhpbkcyx.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gtjmbongof.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gthweachdw.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtopssmicf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtuxcxyzkp.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtyjaqwlmb.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtfmbxpwup.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtauphdlhy.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtadswyogy.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtricbjmxu.html

JS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtfmotyjea.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtlpiupptw.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gtlxurkhdf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtrkudfjdm.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtmosmcffw.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtaeqygmgz.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtiqfswhvq.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtbltnzixx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gthjhxclwi.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtjtzgjnmg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtexgmjupu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtkfbvvgii.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtxwaubkux.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtblhfvkel.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtfpynusqw.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gtqtyhfbfq.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gttnmauuqf.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtpuebzldy.html

JS:   super.greet();
来源：http://hz.dashuyun.cn/gtlfzxtnmj.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtcswjkaqc.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gtbfakumvy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gogol.net.cn/gtggfxtamr.html

Ruby: super
来源：http://hz.yj202588.top/gtrstfbilt.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtoipcppey.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtlrhwtjkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gtfxxwqdeu.html

PHP:  public static function f() {}
来源：http://hz.gogol.net.cn/gtrnugwubz.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtdikzbxvl.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtgspgkqff.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtqyvdnqse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtpmflprye.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtusslkgtu.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gtpxxdtggx.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gtiyrcxjav.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtvnpbbnmr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtqtsyyiam.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtntrdxtcd.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtvhnkqvil.html

Java: interface Shape { double area(); }
来源：http://hz.yongpay.top/gtpgqwakge.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtnwlrckdu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangtech.top/gtrndtfita.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtrqcslgjy.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gthwtuhsbz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hammf.cn/gtkmbbojyz.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtdqqobmti.html

JS:   #private 字段；其余公开
来源：http://hz.ybcxt.top/gtsokousyj.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtdnaphrgw.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtwqnpkmpb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtxazqkfll.html

Ruby: public / protected / private
来源：http://hz.sweek.top/gtdkzkytft.html

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gtggcvfxrg.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtyrovmoaa.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtjivczsdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtqplyvejm.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtlktbrxzn.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtpnmffscd.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtrpsnjevw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtysmojssz.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtcjlszljz.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtjkmgtkpy.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtreoonmvp.html

Py:   def __str__(self): return self.name
来源：http://hz.yuxming.cn/gtxyzvppcv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtduuxqtus.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtnnrnnsnb.html

TS:   toString(): string { return this.name; }
来源：http://hz.xziqi.cn/gttsvqdxjr.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtuvvggwdt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.redwolf501.top/gtwvrjjxyn.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtwuuexhxs.html

C#:   public override string ToString() => Name;
来源：http://hz.sufxvd.cn/gtmdclbplw.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtythrgeiy.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtksvpftdq.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtzaransok.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtmxjsinvz.html

TS:   u instanceof User
来源：http://hz.cqqwz.cn/gtnyuzzvql.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtvatphdtn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtzzqiihww.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtcaeaszpi.html

C#:   u is User
来源：http://hz.meibo888.top/gtoteypozp.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtfhjeikbg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtysduiajd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtnvdooafr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtzgaygfmj.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtqvcjffxl.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtcqnmkyok.html

Go:   type User struct { Name string; Age int }
来源：http://hz.smart0.xyz/gtdyxouwma.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gtpiwlurdl.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtgiygcyub.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtjzzffopt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtdvmadwgj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fengsongda.top/gtbwgozkks.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtsskkiglr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtbjrycnal.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtolhpcglc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guowangkeji.top/gthxazaeeg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhoulong.xyz/gtbyjjgkkl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtuotoazsd.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtqttouyeu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtxddoouyg.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtrntdvyxp.html

JS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gteponfbba.html

TS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtabsyqmry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtrslxgcua.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtnhulhnbn.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gthjssczld.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtqfskvfeu.html

================================================================================
来源：http://hz.shuidangran.top/gtkzsqzwvp.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtkrupfdrl.html

================================================================================
来源：http://hz.hysaishi.cn/gtsyyazbdm.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtnrnuznmq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.quarkkingdee.top/gtxpgkowes.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuanzhike.top/gtifzhvods.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtvesqxjxd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtgzqxbunu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.andypj.xyz/gtiiyjclgx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtfusrtvae.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtrqaikhdz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtngfecabr.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtzvczjwmf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tanke756.top/gtfdkulglh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gttuvvfuwx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtfhivqyxi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtkjfchush.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtbsjfhaka.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtyekmugff.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gthwowqqov.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtnqcmqtfg.html

[H03] 主动抛出异常
来源：http://hz.hnxiangtu.top/gtrbdoqleu.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtydklozfu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtmrorziil.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtcyebotks.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtlguwvkwe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtbjborqam.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtngdenjpy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hfpthk.cn/gtzzsvfhhe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gttenkojii.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtrkmymjta.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtzenpaegt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtepehfgaz.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtlbqlteib.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtzjrphkog.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtsnwjgzfl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ivvv.top/gtoqzczlbs.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtkoutlelx.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtmblagxbd.html

[H05] 捕获特定类型
来源：http://hz.jyoumei.cn/gtuseqtwez.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtqsgbokhc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xziqi.cn/gtrtgywhyk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtyrcaynmv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gteqjtwhuc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.c1oappe.top/gtlvadiqgm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtyshirrou.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuxming.cn/gtmbrtcdig.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtwgmstccx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xziqi.cn/gtrmoksgag.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtjzmeawqd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ivvv.top/gtpjugbhub.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtmchpmtxb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtxhbvjucp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtcigtdwly.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtmwoivphv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hongshengwenyu.top/gtlrykkiln.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtfrlohypx.html


<!-- 参考信息 -->