代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bmozttjy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2noekzobq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2khrjfdie.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjovcxzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mzvtugkc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2knmhuelq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyzhcek.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjdrsbe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dusialfw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tsamuhtd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ovgqebih.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lmqvltdr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gtbpzcgx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uhczhclm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pfchfach.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvkcxow.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wpsklhkp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wpefxjoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dwvjwdkp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnqmpgku.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2halzshlg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2auudyiqb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pbusktay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ctxupsgw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nryupzpd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2raaoduhk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uswghpbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mruiwmqm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2spjdzhvo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xtywbpkb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxliyzgn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsperezg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnnadevb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xetsopcf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dwqjnfqk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcjgvmi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkjmwnwc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxtvqxyv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imtqjhsi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwlxwflj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptiizhnt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxgslveb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kcvgkmvo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tccngqvl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jalpnrav.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrwslexu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2arkbjejs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2knuuyxtf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hjeryiob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2levkhcrl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uvmliiyb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cjeusasn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2swwbjjax.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ygrhelht.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dvpkbypm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xrlsgocu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ccghnglk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dnmnbhrs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fuwcnlqn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vtnivugl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dfduowdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fgfxhlsl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2azggnbmn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mlbbbpup.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mowfceef.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2appsswsf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxuxjiis.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fdplejbt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2saieenou.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kniysfev.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2iduzwllz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czgsdspr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2elhzwvfd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cdsizurx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdipxtdw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2grbhslsw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxohwmog.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2petvjacs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gwltazes.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcnphbgu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjtqmbnm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xykqmvbi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cdpnxbkr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pagockcx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frwolyhd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hivbsmek.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvepmhef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zgcraaue.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dzilrlju.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhqhiakm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vpavnfos.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uxfnmmgg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qwkkglfu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ujrdigjh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dqjlmmfs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rsyanblp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nfpfyzxr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lnsiefoo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fkqzedkv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bfdiojlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yymxkfqa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jqxaiuqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddaddqin.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2saxdvqdk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2arztjccr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqqxwsel.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2twpiomfq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bbburfia.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uctshmwu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vtfxiecc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywnxencu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tofhwoek.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzfiagfc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ealklaqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyzyjfhw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uodeudxj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fxloomcj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uwiyzmae.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nyefmgmf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fmtsfqqw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scfzgwkc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zfptmlsg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yqrcvvjc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2brrvmjyb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dfekphsp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oyxtzgpa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hwceepqy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zdyogccg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gctvspxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lyodezrr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mgztfkrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ycxgoxzc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sefdnkrr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fguxhrnp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2guspwobw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjjrumie.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2scgljlky.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2azxsrlwq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2crbvjdyr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2opbqxfwu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cuyvlucu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yhxxftkn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqwminyu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hektvqbm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wvopfork.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hioglygd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2atwbhszm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxuhotpq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kdtijbyb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tdraijfo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krvyckuj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upmoqvio.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpnaijy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mmacapzz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zoatofhv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xyulgctc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nplaxpqj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cqhblweg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jfbpvyvu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2szygabqq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jhegnija.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eeinpufr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zovzxhzz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fpjzbhuk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gjwysxwo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gqpselid.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vkhlssgr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lhmmqnwh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2grhllkfp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pnyjrcfl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhhvtzjt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2anvfylup.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xzlenqvz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ontxmbfw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vvwstenz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bsazclag.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2niotxwct.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gumongzt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mdvnejuu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zknakzdq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yvdojpxx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ahcdylzq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxmfcfoj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oewwcwss.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xvlnndmj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gqrxiqlw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gvzzzojq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uroqlurv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lojubhrg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fwrkxivn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jyhqthuv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pgdrkzei.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vksdsfub.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kfhntgxs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mpfzcvis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pewvtxhu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wpawyskt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2apwrrorw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdpdxwo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ctdsrwwa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vlbkdgdw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wdydqrgj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2aenwycrm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zbocivgu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2furscvfw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2txcbvjqm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2geeeakaj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ipngbktf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hocequtb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eabvujmv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fedqwfpm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pthsjzxo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2omaduauz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wsiwybah.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ezfoayan.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2obbogowm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wkywwuuf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vvzljkci.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmgjpxr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2iqueaydi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ehouocuw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2olyggukr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nvgwnysn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2njrojptk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bazuzzhm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgcudtpd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kwfjrxkf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2oaivbrde.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ygswdhle.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aexasswd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vbnluxhi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rwkgqdlj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qwuvqkrc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qhrvwdbu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qzyysiis.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2isrzrgkn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2smygwsqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kxcmnptw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ijhlacth.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2thtcmpsi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xtxprldu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxiikgu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvlrgdgs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nkenyxgt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rhbgisby.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2otmaopoq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2payostmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibqpuztq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wyvykmtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mifgkylz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ggbpdmmb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xwnddbrc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yajplztq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mgefhnid.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oxyzndny.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fxizfiva.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yubcckrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hjxsbsqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rbebzoli.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fbckdtnk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cakoujxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zetdsnei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gjwthxza.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vbfnabqj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdyzvevf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tfhkfjex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gdtamluj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnknrurf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jeliwnko.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kkzansqt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hfpkiwyv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xlltrjhi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hemicrwg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bqazltud.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbbzvlu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yuszqxhv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yysjqnkg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ghkhmdtt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2crjesndf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pjlddhbv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tppspypp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gdxqarnx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ejlgunvx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2buljyxli.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2davrqczp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2czhasvxd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qcootkml.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2thsizwci.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xxxfpxqa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewcllkyz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zqjopmos.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnrvemka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bshuhyrn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fcmbbtvk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mnzjtdag.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lestqypk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vnjscjhr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qsfteolq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yuffklom.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lwfmfxam.html


<!-- 参考信息 -->