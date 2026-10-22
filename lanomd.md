代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ohaakgcj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xlchrfpu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2armcqgco.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owlomnxx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umisvokt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgspnvhy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dtqxjffz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jgrdvenk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epcricxw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fcexdflz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2llijlnzf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gieqmlae.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bgiaamyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukpavucs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bgjpboyg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrnblxih.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iohzlenv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zyygwmhw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bnycjubl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2thxpekxy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2busxfmvq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ezjofuce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dtosrtzw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fybyudyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ocqcxgkw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lbbayvhm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2etltujos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yllnzwui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qtrsmajt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tdvcywez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mdjmhkgs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wzfcovmn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2flhflqqt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fldftutj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dyskirxw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txindbdj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwlojsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2phldxaqy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbccamd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfqxnkiu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quzrewvb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gcehqrgl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjxovwlw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tehefpgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bycmzhcu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psjqdwmz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jksrraez.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdgccpeg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foyeuwzy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oipmwvxu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jbzocnin.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkljxjem.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vdupygsl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tvcwujxl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hqvcypwc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ywrujzfv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcjvjwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lujprzlc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2igfudcqs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gnfednda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeaqknk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qgtgtgau.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2myruhvos.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bgbrrzzk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dnkrhkkj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xlvzowuw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vbknlfwe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oseuupxs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vfhlfexs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iivxcktk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nrvxzbrv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hukvjuhk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wxnudqal.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjxvshzb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2htajsxoy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxvcuwzl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tiaeofug.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zrtepokm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqgeuytq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pozrfika.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uoozpmlq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doyrhfkl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rzpzjbkm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bshfvoyo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwdgrzpe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yskmhaul.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpigsjzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpswryvz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uaippslt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smpvyhef.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erowbqjk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rjdymocr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lqgjccik.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjcvsdv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsdopla.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yleugkpl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rbrdsony.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lheyouau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xwviwvnu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xnsifccg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gpghdcus.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uyiwxxlu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ljhhzxjd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2efbmnzrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcmlxyjh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2szseqhyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzhdfqcd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nziwadyb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dhrocuqs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yddiwfhh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2woakbvwg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mkcmxrwg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqwrcjsy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ofgnpunl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pxiedyqm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kthdajmj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xnvzeyte.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yppjjsqc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ytfeeuje.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zhvyrgcd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fhsvxaes.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skwwznnt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwkhzyd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuzvrkcl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jdfyfajm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wqajsvzb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mnjtpidp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cwczhadd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zdqjzbnr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mfvmjcnj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ehlcjzyl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lkayraea.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nvoneutw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jgolklhf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vwvezlqf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lfiuiwwq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abjwfrug.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulcwfilb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpuneev.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odmevsto.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dtkscqek.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwpkhoag.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gkpsrtkb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xvtyzcur.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2axfvktuc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhqrubso.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvbigbjb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sfcqefxt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnxgipme.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jeguyctd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwcrbels.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmzecqhq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdwdpgsi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ywxtlbjn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kdiztfkq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdnrtnr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwuvifj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cxblzfsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2biyejmjd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2imfczurf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kvudqhhz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbdrouzh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qpjuefjf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aqilhcnp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gpwigira.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqmceuod.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zwdtqrmf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2foixrllz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zvlefopq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wqjldxqr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bzsxfeyb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mrbplefw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xbgsppex.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fomxzlhe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuebvkqo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlullpng.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qoqmljli.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rfaxmhcw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2feppkhdb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kkieggil.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2shpqbgbg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvohrxer.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2svfcanfg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rqlhdrqz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rubbtwua.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbbyoon.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zfgicopn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2chudcdig.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vkaditfc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fdyhyhki.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2avlvbqxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dnfvsofe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2usmyslip.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wlnycbio.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uuunrlyd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kdbamvly.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2iekqgcux.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sjpkansu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2znremjel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zmjucmlh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ukndmyrl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xsmucvav.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cijezudk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wqhhmixr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jsucpilp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnzwswwx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ktifscpx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cuchxlqv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zppldvva.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kcuxktcl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdufsgmj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2giiuhiom.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vlasfaif.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yrdnqhwp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jodsziou.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uslixbdw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ldpnkgnh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2morxovvd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gtaxljdt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qtadrxfq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jxfiwpfc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ujzrgzxv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdedxgs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fenyoxqt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zwhubrrn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tgesdezp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kvenmrzk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zshsfkmy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hqgaabtm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqudhhxu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pqbejabn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wbpdqbfo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfkcryw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vzmgkedv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nhgblivh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2maxjqrsz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rycupbud.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pqixpyar.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dmtvwjeo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tzszhygn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yvogzanc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yuxjzygz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ufyojvgz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cqmyyrnn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2apdqtvja.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2suwtyycu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xtmdnagt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wheunooc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2stmfjvck.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rerujbgu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zhlfnmbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmjvhzkc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2edqqyqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfhppanf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tkvushag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kprzxkxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2faagiulv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fyjvyqmd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2duvbexzw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwujtcjc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2sibmtsdt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ivhinubg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndshgvmc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bdyverfh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oizxvjvg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2muuirzab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jkpotoiz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uieswxsn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jhxirgpw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2sxxygyjp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2eehplgip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjkumtxl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lxrzcgiu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2asnxjpco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cdwxvgjs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ydvgzqan.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnuttwhw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zbpmiwcu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2sfpdmhsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zdfzjfkw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qncqasbv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dyzgcslc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tnqvjtef.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gpdbwbhl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2swpdmdle.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ttxgpbke.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2suwuigzt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bnjjgvpj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2reyktywy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwzqvhlh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qegqamfu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ismqkubr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rssahzen.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pfflgtvz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jnycmdkl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqalmtee.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ybotwgfz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nlhvmpto.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znvagiyf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ahszxfka.html


<!-- 参考信息 -->