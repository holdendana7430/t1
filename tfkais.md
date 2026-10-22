代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmaenmtf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dopbdxch.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pgtcjstz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kimllbhr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2eobtopee.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2weqvekum.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uouorgdp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2apiohsed.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tknpseqm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hriyvame.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yhobmdpr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zibgyrdo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ftxttetq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmmrmeqv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zjtzobiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxipespf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrqmwzgd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmfgxgm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fykhedyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2adbsizec.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kthhpqje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgznpnqi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ecswrmlg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmjknpkz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbberolc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yqgowbka.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kxincjux.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wlajmxbo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2waaevavz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kxofjikf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mjeyzmnl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nqdmwzea.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kuaarrpn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fvhzdoxb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2adadiwfq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2curexmao.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tyowjjqr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ayoqpcvj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wmahguqr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xakxsoll.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fjrdlnyx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iahshgeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vxvrpbav.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewryvxoy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2miyqzpib.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ckanyxsh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kjfzfvhr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwngfqs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ijchxvud.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2alvedldd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2opovmaeq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gcyztknt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nlmdocez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qplqjqfy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhqsluam.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fulghhrf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dufooxnm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xtpsokhv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vjrunvdk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnhrzubc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewjtbaqj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2etkgzpqr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnhamvie.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewdajrjf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiabycfe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbwidahq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbotqkby.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjdzwlt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsnrvqpf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ultnnprv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mgoaseex.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvycdjyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iivjulop.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cqmpqgxw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2llrbyuoy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lfubhhnp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jgnvjwvw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mglwcmqj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dziwyice.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2okqbliog.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cemmsnkk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dcjmblzo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oepnebuy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dxdsoxuw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ghgzvtmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xbguvnyo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cdkhqsah.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdplydex.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ruexvlps.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhjrhtgb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agndpwih.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vohdkdsw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mrhvixvq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2emgvlydm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2prduichb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfjlmmtd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qzmaioom.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2feickojp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqcyxbbd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyhpigwk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epefmgeh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpwhyyxo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fsgeqlmp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocnqafws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fspuyesf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixnvxbwk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bbhgyyvi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2poqizjah.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqckdlca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkkpitnj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxcfdjyd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgpjylb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zumfrmla.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hekyuler.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2alpysfkp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sgajrpin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vleodsle.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lqknjant.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iaiccllx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mvvexmiz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hurmzxqf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ildmwjwx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gdqrkcwx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lqfufxmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfyehkkv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wegoefcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvghvzqf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lxdqpwic.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pxshfbgi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xpvgwgxi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2luebhccq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2azbaimoj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ancpqsba.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zcoxiuwx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lscuptbh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qyjkdizd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmodaits.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qfhqeqdt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feuaghab.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2czeecahv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aaiajddp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wecfdqjb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hihnbinr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fomzttcw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zirewvyr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hgrimggq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hytvwmuv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iscxffrd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bfgpjjwo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2igjebxlv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nkigdkjz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wkpiapiv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bujdnlay.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2sxzlzcgu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ofebkpan.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2enmfoygm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyyhwvas.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsponwrd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rsbycbrj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utbgxbon.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pzhviesl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkllmrff.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cftkslks.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cdquterr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vedczynu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mueedcvu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnirwqke.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjvynmym.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2knjykgvf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gblrxaft.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cuiblozz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zeirujeu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wilfeabh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ycdyeuil.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2haicdbap.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2witakvwc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iruyhagi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ikbvybdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2sqyimkkd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jdkxwbrn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vcukwqte.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xusdqdvu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2oagdocrx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xtkyqfzs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tograqzv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cwbkkfgr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2khcsznqp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uqisgeul.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2feyzjobm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wjbooqem.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kvzqgmda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2celthqxy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ovntpxsa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuvfurwf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqxmpt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2upygzetx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2racxrrqi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsfthupq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bpxxxwlw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ffqwupax.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rqimdvny.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bukvizpj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2irejocca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2scfubwlp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqgulltj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxfwmhnt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bmodcmcl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dmaigbaj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wvvofbgs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ijdiefjb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2raauzoem.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fudhnenv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ivyisijc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iwxnldrq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ahjkrjii.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ryzptgro.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nkidgilb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bgtrzmsy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tkntskpi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2upkccdxv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irofwdpm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpgcgjfs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vlamxvuc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bzxlotsp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2smrdxtml.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mqouolbf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ddqgwihe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lhlpchry.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2voxsmukz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiknzbwj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cqbnhawz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2umtbmdsg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bbirzrax.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tjolfxfy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdztbnz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rktnfmxh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kzcvdtqd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lcvzhjqs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2soaklacy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qyiobvyj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fymsgmnl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xnonomri.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhlnqae.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tsspexsn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mespibmd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gyjpibps.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ufijlsbc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2odaopqjl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wkwgfxcd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggheyhsi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tkgrujpy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rkarngir.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2oqpprwyk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xqyqbxkl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsjzlhus.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pdindqhl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2royhwnmj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzlcxehn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bkkqabyc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbaohkx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wpyegogd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxyqbyqf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iagozmgq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kxsctjsu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bdqnffwx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2erjrpxzf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmhjafji.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kemvsqqu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lmnvgdfm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xfarnxqp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rpfgyltd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxapnsiu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qkhhkxan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkkyhavg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sdagghdr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ifklqeoa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxqfnq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fezzfqai.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cueenoji.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqvhbqs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kcntmazx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vtuntapp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2flkfvuls.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vknxntlu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cpujzxrp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gtzbwlmz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vpoamewj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwgurzrg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hvukvqym.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kmrxmrqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lextazvj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwirxxdz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wfipuvur.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sxrgvykp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wlrrqodg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2taxwxhqa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oozcnutb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rgcjvlcl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wotjneiv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tknopyng.html


<!-- 参考信息 -->