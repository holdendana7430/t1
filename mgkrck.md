代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxgcclc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hpjstaku.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rtcjqrxp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fcokkftm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mybtlfzh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2erpxfmpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umqzdhir.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2liyfomfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hhngcdba.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vvagbnju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cymaysba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dktwbozz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2genmurhl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mlloavez.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcjoyccr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smfavabu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozovdbqh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcwtowgt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qdafvvys.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smuxykeo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hitugufa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jlkxeqjt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsnvoddj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqikioga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blzfhlsd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwsdpzix.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rzbjnlnb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txxswlcs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bblcxbkh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdaasxfg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vsvcyxrj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzbrjez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2amurxxuk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ztlpfgka.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nbvvlisq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ndlwaqht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2llyjkwer.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bjcyfbnq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ttwrniyc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bevoxtzs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dcwkyqsr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lufoojiv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ywgydckz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jgcyyonk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wtdbsxfj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kigopkpl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lupmfojr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2znjvgnnn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jpuyahig.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imntgoxu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zwxxxoyl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aitfofas.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2doxsyadr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cratwbud.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2daprsnqp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gaqzajwe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nqiorcfn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2grkhcgnl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrkzotmx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2khouptwe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2raynbfzn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rrrrtzqz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tnnotccn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wndlxuyb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpfpwmlm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iycfmkkn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jruezplx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlaejwcn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fvxfdlkg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndqwxopv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpfgaicb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lnooxnhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2erifbpse.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nygmkodk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2icwhsdyl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rylxbkcq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fodviduu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jwadtwvn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2okehhorj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ltldgflv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2atputkxh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2timcjrxw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zfzonfyg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2usnyzykq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shdwfpsh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xpzbvpst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auqopncs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2asxirqlc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fkhjinsa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nlrmuhlx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xivemexm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vwswvkrq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qoamggdz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2titimjzp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xdzcgalm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bypxpowd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfncipst.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2aazgadpx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aazjljhu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kenpzoiv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2goxczmbl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lwvjxcet.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2skwpupba.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wquldclu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gsobyfaj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nqlvstrp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hesnwurx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ycdhjxvf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lductunh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvpwrnms.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rmuckiei.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cwqnsvdg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qsivowoq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nywhdexi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wuuisuyz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lzqkwtoo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ideqqypa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pylfgatl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fgygehdl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2toglolpg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dhdcaxne.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tiqohwwm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjfqjln.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fyajdbey.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aopieesi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xkaytlae.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sqhunklp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpbseaub.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtgdpwwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wgduwanb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ejouivcl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bizzimjx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hiwknekg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wxvnxspl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzwaosv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imzdlxtn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lkaphfgx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnlvfik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2slbhykph.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oizoukju.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bcugpkzm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dphoqflo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cjnaxdby.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2phzkffpb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kklgwpfc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ebfuukbs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zsyelefj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nqpnomxb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yvtyprrr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2orfattck.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lwxsecoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ennkycqh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hejmgypf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2henkxcrw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnfprllo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rasaishy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kpbutane.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aowjetcd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwkrcubi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ppsxrsfm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bkwktjru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpevxnjm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tgvupoas.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkoervrv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdukrlgn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2swsjubjj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfpahzgr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzvqlszo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2frqsocio.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rvhwhfra.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cuxntqzm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bxivgmkq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2stuismft.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pgtwptng.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hhlvmpde.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2duzfdvpy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hpxokjoy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rvnvubme.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rxcdfsuw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mlazibqn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wxuxyxui.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azrotfkr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdvjjgt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2svpkxppf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jtyhikge.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpduwrhk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikusodrg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fmlegprr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vafslycy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jauxhkoy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2penfvkqw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ayasmlqf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rgppxviw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2drsknmje.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2skjiikdr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfodkord.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gaarrohj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jzoeacfy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vtszkchr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2prrtbial.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2alcroopu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2sbfjaefh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cudocqod.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2boeqxuwu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cctsqphd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2labfrtwb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xmqzfjrw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2czqwlrmh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nuhyrorf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kszdeedo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2unajpnmr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wlsflbey.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhdbmp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xtdufdjx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2clhmxyvp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjqjmkyc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pwujepje.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pznqboop.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xvxyitqv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ufwqnvpl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qknoilcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwdlvzal.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zvzlkkhn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fdbtfqpe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cgftwrrk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rufygsdi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xueeuyjn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2swthtqbz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mlpiujxq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vsufztqr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mavjznyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvtibmpy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ngfedivp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbjvcric.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ydtplmwq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2henwyktx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afzxolpe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrncdwzz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vhbucbom.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukeqhrrk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pqetyngc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfhbftlp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmixzbc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dmfcyykv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2koaiytnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhusdzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whkrizdd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvymgftt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsskxwwy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vkzeqvey.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2akeohkmk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxejijgz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gigteelw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qoyzejsr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vuceyrze.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kkmbigwf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gdafffff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fphtpgsx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vhidneou.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kabpxbsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gidyoasq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gppjccse.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uaorkimk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ccwvsuih.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnztlbna.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nntxtonv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2euihvwug.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nuabiars.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hyarafjo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsrhkxmq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hykkposq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bzkjpbyq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gzzwopts.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zkkosmrh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yfpeqlgf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltteedyo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xcqdiwgc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bzekkjxw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2badqnokc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hrfrcjyl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ijfsdioj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xlbisauc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fehvneea.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ovkwmrun.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eyveumqh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cjdoxbby.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjfgzxd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oviidaoq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2deruwujz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2letuknth.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2voacqsob.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zwsberww.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wcyflsdz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2nydyttyc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lvoggmpi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xwotlaju.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gepphtgn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jctkwpmi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2webgdyar.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dysmlnwr.html


<!-- 参考信息 -->