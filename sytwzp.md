代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtvyvczlsl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gthvmavkpl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gttfeecwzi.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gttakyrccz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtynrkvxvb.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtafykddag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtfktckokh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhijiandao.cn/gtkarfvzul.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtkewkcnku.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtkwqhemtr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gttjosexjm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtswwouanf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtlvspebfw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gtymfutwpf.html

[F03] 写入文件（覆盖）
来源：http://hz.wangshuangyany.cn/gtboajgzxf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtcygabpsj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtysvyntra.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtlejiumew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtyylbmkgd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtyniompwm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ywan-chungtsiang.top/gtburiagdj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtcyrpadgd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtugpvhwyn.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtmttysvew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtwwubqkle.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gtoxhoisfe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtrpxozyzd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gttqpznnkm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtfrbqhniy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gtptjbzwsa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtidpxenms.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhixingplan.top/gtoijwqoxe.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigufen.top/gtfvmxoxdj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtdilggqry.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtrnzmmzbu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtdjvnftfh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gteoxpnwpv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtwdvlqsdr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtwzulkxru.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhijiandao.cn/gtgwfpmmxh.html

C#:   File.Exists("a.txt")
来源：http://hz.jianghu66.top/gtextllfwz.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtzyjmxgse.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtyfacvegp.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtyktczaad.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtanlnuxde.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gteblxdijr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtitdsupss.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtaptuyrjh.html

Ruby: File.delete("a.txt")
来源：http://hz.cucudq.cn/gtuzrosazs.html

C#:   File.Delete("a.txt");
来源：http://hz.tanke756.top/gtexlwcdsk.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtwhbaczrz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtfcoqpdzq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gtdwuosvzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtbwmieaut.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtiixgrqiv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtwyyvoiyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtqolwcwlu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhiwuduotai.top/gtecscprsp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtirqyilfv.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtghriewqt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuxming.cn/gtrzafwmnd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gteubmhhvg.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtxurzjnnb.html

TS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtahlmntoh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtnoxhpotu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtedoythpc.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gthcdmvhbu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtthwnmhnw.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtzfdapcix.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydjk.org.cn/gtirswlnwv.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtsgofuzxc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtcuczjsxm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtoodkgxgu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtggkmtrzi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.vqdsnc.cn/gtfdoeibhn.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gthbyffesp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtthjqyhrw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gthfinmjfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtakaiisna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtajedsjmn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtpiburhqo.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtqyngrcov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tianlin.xyz/gtamjpgkor.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtthfjzaks.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtememkvxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtqwpzaiqx.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtgclmvtfk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtpjwynjju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtuazdbvwg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtjvtwsoxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtmayfqzqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtykukgzqu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtgrqqxlze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtjpkllplk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgufenzy.top/gtojkwcttr.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtdwykgipb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.316326.xyz/gtoyqerffu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gaohongyu789.top/gtpxfzommp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gtlyqcppya.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtdqnmqesx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pengpengdd.cyou/gtfiposrru.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yonumen.top/gtiqfajnug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hysaishi.cn/gtunautgdl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangshuangyany.cn/gtudjpslka.html

================================================================================
来源：http://hz.ppjwa.cn/gtywhuqmax.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtsnssgarq.html

================================================================================
来源：http://hz.cdnleiting.top/gtvebyewcx.html

[G01] 定义类
来源：http://hz.xziqi.cn/gtjydsbetn.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtnexjmwbz.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gtjtbvcape.html

JS:   class User {}
来源：http://hz.haohaochexian.top/gtcfxnofol.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gtjkwodshj.html

Java: class User {}
来源：http://hz.xingfuxueyuan.xyz/gtbymloyvd.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtvbzeolli.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtezzfklpt.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtoskxxhpc.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtsbgfkhlg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtkkogwbbe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtuvqzjvvd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtfxdtouwc.html

TS:   constructor(public name: string) {}
来源：http://hz.hfpthk.cn/gtkvuvzpbm.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtmbidvona.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gticadyqok.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.meibo888.top/gthjsdnpnw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.smart0.xyz/gtmjizrvmx.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtvjpctgyq.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtokalqkqa.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtqpljffnz.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtkpcqubhq.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtwdxwppsq.html

Java: private String name;
来源：http://hz.xylfe.cn/gtynjgqpep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtnvvcdazg.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtfmixfbdi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtnsrdsnql.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtdjrcxmzl.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigufen.top/gtgspdoshm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtoxqbkyjf.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtblcojuxh.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtqubnxpbs.html

Java: String greet() { return name; }
来源：http://hz.meibo888.top/gtdbtjdqmb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtznrxjgsq.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gtxyxvxajm.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtwxxigpqw.html

[G05] 继承
来源：http://hz.meibo888.top/gtmesskllo.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtiezticvd.html

PHP:  class Admin extends User {}
来源：http://hz.nanxinkj.top/gtcwvecgqt.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtsdikybmo.html

TS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gttnkcmrxg.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtdnbccylb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtcogoeljx.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtfiqzlrpw.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gttxkyycne.html

[G06] 重写方法
来源：http://hz.yj20258888.top/gtjgoihcdm.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtevhlnaix.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtyqkhuivj.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtoyillzyh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtukpsgcjv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtikskokcp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtkzduallx.html

Ruby: def greet; "admin"; end
来源：http://hz.hysaishi.cn/gtttueovkb.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtzbfdkhue.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtszxychsk.html

Py:   super().greet()
来源：http://hz.hongshengwenyu.top/gtyvzxrmie.html

PHP:  parent::greet();
来源：http://hz.cucudq.cn/gtddvqddnr.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtmizwgmbq.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtzxgzoepm.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtplnswxky.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtcrgsrhur.html

Ruby: super
来源：http://hz.meibo888.top/gtgrjbsbum.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtyzgwngej.html

[G08] 静态方法与属性
来源：http://hz.jiagoushi.top/gteobezfus.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtdlyzjwdq.html

PHP:  public static function f() {}
来源：http://hz.zhiwuduotai.top/gthetemtcu.html

JS:   static f() {}
来源：http://hz.havefunace.top/gtrlzayfed.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtqsokriku.html

Java: static void f() {}
来源：http://hz.hysaishi.cn/gtueiguybg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gttadquoum.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtclnixxeu.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtweqxwnfl.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtnsievzxu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigufen.top/gtpwbrtfsh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtgrsfkinr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtawpkffrq.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gtkezhmofp.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtiflddgcq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtsotyqhgf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gtsigjcrah.html

C#:   interface IShape { double Area(); }
来源：http://hz.havefunace.top/gtigilcpyw.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtjwamuwbr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtojasgohs.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtewkswlbp.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gttyhdazev.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gthvnrhxpp.html

Java: public / protected / private / 默认包级
来源：http://hz.pengpengdd.cyou/gtcaxyrppe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yueranfly.top/gtnjpknvyc.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtixoqmpzk.html

C#:   public / protected / private / internal
来源：http://hz.zhoulong.xyz/gtqfkmapfr.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtnmeeijyf.html

Py:   @property 与 @x.setter
来源：http://hz.xuetiantiany.cn/gtclxdjufx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtgseajjpo.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtwjpsosax.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtnkcruwwe.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtdtoxheky.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtpxgomgnc.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gtftvwicuj.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gthpchpvmn.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gtulznvxqn.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtfvpyqwmb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtzuskxekp.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gtilqqnbxm.html

TS:   toString(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtjhjadklo.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtdfgjqzlh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtqjgutazq.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gthnaleoau.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtytbafykx.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtoklszgwc.html

Py:   isinstance(u, User)
来源：http://hz.guannengcc.top/gttohkqdlp.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtbelkybpu.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtjajdqnvn.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtpftaykdv.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gtdmfbtydh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gtjgdttjdg.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtcfbuvvpa.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtymwcusnb.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gtbpdcjvgt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtzeyqqlxc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtwyrukehb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtzuncwvqu.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtuebylwwb.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtphwvnpln.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtinmrxiak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtfxvmpuub.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtkhymwydk.html

[G15] 枚举
来源：http://hz.hnxiangtu.top/gtreykabcr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtojygaung.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtcjulncqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtosblelhs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtaewwdaar.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gthbttnwkr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gtfbjdzteb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtuktcxqud.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtcohmryvy.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtgdxqskzx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gtapedlcaw.html

PHP:  get_object_vars($obj);
来源：http://hz.shangyingyoupin.top/gtdiytvbpt.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtqnaexpsg.html

TS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtmyurcpbh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj202588.top/gtpuxzcyjg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtsahbjcgq.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gthzizkyqd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtafpiljfp.html

================================================================================
来源：http://hz.jinqigufen.top/gtpqphvmeu.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtmqkbhkxs.html

================================================================================
来源：http://hz.sxryk.cn/gtpggesuaa.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtlqdsfxox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtrrzsooqn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtvojnjjrq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtteaceeel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtfkjxfyde.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtghprntft.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtuzhiqmql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhoulong.xyz/gtfpfnmdwx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtzdiehrbz.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtlgpqeruk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cashguo.top/gtqxdebqxb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtukkipmip.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtgmrjdtyf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtrxlqcqdw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtriyuiaxx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtvxvrdvte.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gticjxfkyu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtpsurgafa.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtvjmvpbrn.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtzloakqbx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtsvnhiwix.html

JS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtmkeuipfi.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtnahfapta.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtpqrksagq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtfxpfgvjo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gttofnlzoj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtmfveqeig.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtfqjixixi.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gthkengndj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtmpgkaiqm.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtpzhlwdxc.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtjamsqekj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtjtxzzufa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtrretdpvz.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtuqqdofyx.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtalbjcoas.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtnhbgjepv.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtmboqwskm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtnglzpbuq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtabnizasy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtlgpbmqtm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gthijdokpi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtpuugewyh.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgfzy.top/gtjiccujki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtoiwszbpj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtafmoyqgn.html


<!-- 参考信息 -->