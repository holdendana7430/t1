代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ejzsyqmc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bgozatvi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2frlavgjb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gubeeuex.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2niztgmtz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kxfjcqjn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pyocmzng.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bjeyxirq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edrafavz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqhrjujh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fecdzmcx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gxehmnxq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vmpurycf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xmqcpsxv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pfofuzpg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bomfluxr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nlumdtcl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uixnnzih.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2grwqrjrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jpzyxjlp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yijavslr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fxllnvhw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lrichziv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2novntthy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iszlmwqu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2otraezyh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2phqsixun.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zkahtkye.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2yzuhbqxk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvlmnqw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cuzjxqss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jzsfowzi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zjyfqlsv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kapujcqy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldslbwrx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prpinrxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahozturi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkzhkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2eucxaibr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwvqkvbp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyjwojnv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ehgkbebt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iliqllks.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzdlqbpb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzmqmqlr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynmbqckk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fekayzsu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lukaznkj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvussbif.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bocmdgxz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nbwtjwzh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnevxdv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqvxsdvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kjoesfys.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pfywwtqx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2frwfmijt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wuvazumm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2msqpuvzg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iedjjoks.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gpnecbam.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mslcgthj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zatmwoqr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pwmkteqa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2grsodgro.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ppbiqcxs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nrincpjg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qoaoqecx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2umfczdbl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uzzziuwk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otxjdsln.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifqktlvd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2atdrxiry.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ytgcstoz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2msitixik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gxpevepl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxssbhb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uvszrqcq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kawnjmng.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snpwrjvs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fckglcpy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stgbvuob.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghgacqix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dnwbpnaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txhzoyyg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxufwhzh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dorfaztn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxafbxek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igvdlwsm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzmhipqh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfmhvqzs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvecltg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iidwcihn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2puqhlbyd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfdzbbkg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sbpbpvuk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2veormncb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ycdnnxal.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gperhufx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uewsscuc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qkobtjtt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2avfxiukm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tntewkao.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zgsdcryx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uzufibeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkrfcxta.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lwtmeqxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avtqsiho.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nyofycbr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wcbsliqu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cmxbrukq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixdzdejg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2figkqgze.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jshquenr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jdeydblv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iyfhkjbz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dawvpjrf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojhkvuyx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ipfscwlu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfahrfog.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kgjcolsj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cupdazvl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pkbrfjhu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cbqplgll.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2emyayejc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udeqzpur.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fupambyu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uawsradz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fwxgfojv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gnnmlxdq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dtcienyf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lujqjmxh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kfheiwys.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ilhxplcy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gmrhvjil.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ljztbwdu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2azyvljpr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imkcwriy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nphvgmpu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hktmopng.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgdhbbol.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sruquqkb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hutxyxnk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nmkzpows.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wejbupsu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zkndoudl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkihsfir.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvgkketh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewwoqokr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkhoimef.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ydgoprhj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dcrrevkc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgkfziyu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hcdmxvoh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ucogmqrc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpptoomr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2snmyzfwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfwtjxgb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfpowvqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2edlubdzl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vnclllhk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2beeccasi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rivpkeod.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2shhqldkb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vefoacih.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hjgjcrmy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oslklfes.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kqsleqzm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2avhvgbwi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bmjrfuhj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nwpvbisg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qzyaoxkl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wnwmlgni.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sjmtngll.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dlwoxuvs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bzklidmo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvdilvej.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pjlplier.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wuoohnkn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ybodrvjp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rofkdyqm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zntotrqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dscbufst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2llgrgpvs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vttgstpe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szicxocj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzhpzqt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yzousbkc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yrjmvnej.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ckgeacgs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ijrbnnia.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dtvtvjeh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gvdrixua.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xglexweb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yxvranpp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xmdqwmbm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xpdjfncz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hjnwemff.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qhexsduu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbopew.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhufhxf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2edkzuggr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ijlnzqod.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cywyypvf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwpcqs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2biwejdwx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssrluuma.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cilfoxyp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kjfcerlx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ypfivvgf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ocepdorj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cqnaszwc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoecmvau.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqzbpyw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zimhxdjl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfogqvwy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgswcylc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lruarbmz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vupkvxqr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uadpdfnn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zrjjyydv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2laeooqzi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zrzxqxnw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yardtgux.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ohgirgvo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ejzmnhko.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tklqfhnj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2joogwsqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wguwompt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jbmowbao.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oanceaxn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2omqiqogc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rcamscpq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pnsvxrod.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2irsdqktq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttxxbnqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yauwldho.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vvdrhlmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufyisfsm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbuyxvj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rkblgrdm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nylwvdjt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqelpeef.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pajauveu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jowlsvor.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2uukllrkb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwfzzxb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdzjdmrl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qpaecuye.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2enpifbwf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ndsxqrdz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zxtnpsdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbrjewkg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lorvfmkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbznkdud.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bttoygnp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yufaeope.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjcqsir.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzkkmxx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmpvidmz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2biwkoiwo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nfkerfcm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2btjrmuuo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nleraifm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2znggrsgo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nvriafct.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yjdbgvna.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xjhuyrku.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wvucqjdw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebflwqom.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dybbvgmz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijgxqffg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2doslehge.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2unhznnde.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gunbkmza.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sphxnwsd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qvbpyfbx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fslkzljp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dpokzdww.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2skcpqntc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qeluchkv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qhbhxtno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ncjcwoaq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqyrpo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyzvglav.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlaocykx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2efgrphhj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgpbadde.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjkfksr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcadvavt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfpgvhri.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ozacqhtf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bjhypwkw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fstifsbq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kmsvbfxn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epdtjzcx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sknyzamp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bdktvkby.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hoiwuiij.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rgnqblve.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ffqzguid.html


<!-- 参考信息 -->