代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3aabunswe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrcqvkmd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qzqbqbhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3achqndlc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zaxxegzw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uzpztpfu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jimjxfxe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3phmzkifw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jchhpddl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kqrxbfup.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lgjbdouj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buydmjqu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kckfsnqp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwsoqpbz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rznjqadg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xllccbdq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rmovwrtm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucalgyzj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ezagkoha.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ylwpfavg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ubkfsbzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3slubsorl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ifhaqekx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bshfppct.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eotdzyeu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pbzwhfjk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lrpvihnh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ewppwgis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3chmhgnyf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ixbmllpf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xkhbbkom.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxbfwjyc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3shugeond.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3egydfwje.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pejiiems.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zecjvjeg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jzizqsqq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iegvkkte.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxsrbniy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eaipkogj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phfmizbc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mincabdd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbfiyeji.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqyzjlod.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3raldrdzm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nbcplwyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgcrkf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzmqmkga.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mltkcowa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3uppypnhf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjqzcrbv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jjzescey.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osqxavrq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdtfogal.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uztlhopi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrvldoor.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lppmkjsv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdfkdmii.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qtwhpgev.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3giowhndn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hoxvlyou.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3badspmxm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gktsvfwu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bymlmgcd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3khnawato.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ocuuwafr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jntoxkia.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3twjiqvka.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxyjupp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtftsgim.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3crhlgoiq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqtgvcu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjnpmlm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3npkjdows.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3toonozfl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3czjkbyqu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jdvsiddm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnehcigv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkepxfjy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oltjzwcz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hzjrnwet.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3igfnwlxe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kbonbhus.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stvbzoim.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gedmtxsn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gjhfmqoz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hriwmpye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uvrqbkrf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eubfevgg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwgpfubl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvkezw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igakzuru.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvcwaumz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kconujfz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3reinncbe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvcujtav.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kfuwoooa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhiuygoo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptacskoy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3esfsvsyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fliwotwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjqismtj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3swpzibre.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lythebpj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mrgahdhv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dnpavkdp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vqojszoy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bpsdkazc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gxfjuhtl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ppwvngoa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tldeihxn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3obhagunl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvzlgtzp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dkwcdorz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtcxexgk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qqqykqix.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jvxlotai.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhnqabbr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3glhgvrer.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oyrohjux.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3agwfmonv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lpwzkvqn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3emydqwru.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngzlbebe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lvkxkldi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3oalkyepe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3aaunqnqw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ytwsjotn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrfexych.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irtppcup.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vurewfle.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aearutqx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjiathjn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3plmtgzav.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vbzlzhxj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xzwljmup.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yxgzaaoo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mhgvnlfp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3krcfayrv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cefkxojr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pmgsajnc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xkvsrthr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ykjapoki.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wajhxkdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmmljnjc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kppjynlg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezxadpvd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mbqwftnt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3polklkkc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bjmsgppk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mgwocnbp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3edueigep.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tseornjc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nvnaigst.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sbemcckr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlrlwyhs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3phjigayv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ytjbncdm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aejfbldg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmgpixgx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cfjsbiby.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kclvvnvr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xtabbnfu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhlqnos.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecugfbla.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnungldy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vnxwwxqw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dxjzvqpy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3acieceki.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pgnthosr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3czflomer.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lqbemgtx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hafjtiin.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ulmqgnhv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewtnpcqy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pvublkbr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fpfgnefw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwkkfvlw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ltxefxpf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3paebeswj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptnxsqzy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nkwyraav.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsrwpazr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kufgjwpa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dtghcomf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jpuxveuk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngytmpii.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3grgvbiuj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gsdtoafl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gjfmdwvv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mbjhllki.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sinjkupv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxhsjne.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ohpubfcg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdolap.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnvbxzsz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yteiamib.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3djnznjru.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cwjceuzi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cgteynxm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pfswqkte.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hzxchnzt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3erfetdia.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3faqhjhsp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3osrnvgom.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iyzlklmo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mauajhts.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhqoiegx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tvsqyrra.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cjrbcaas.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jcskpvge.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3itrvlxvw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wulpjcta.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcwpfdop.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywadodlz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wffwhivf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3inrrunwx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3egfooxmq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksbtwytt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lacsryvm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnkhaqrg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhhyxndh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fqmwzmbn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3benatszt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3uesdkykk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cgnhothz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mpqkhjkc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gumgrrxp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oduddecu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wagubtxt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ogplrzdx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uxxretyr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cjniabii.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3svzfjqid.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pxdhuxwv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hvehxlrh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bregkfjd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvibmgho.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wqtggiut.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nixcooks.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3okfvptfq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3krttevap.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjgsdelp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uogvlhkq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cjqifvdy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bsrvnuxa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gsrkaarx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvumzgm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xaogwvbc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvnmeunw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ydmknaao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3saxcwwgp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kffyvtsc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmradzcm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gknaoliu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3iwktpnpb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdlezbfh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3nefkwato.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3klirtcle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzhtbnxn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxanwoyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgcvwrla.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3aoekuocn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eehkmuee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnwxqht.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mooiyugr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvwbikbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3szjkhcbk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xazliank.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3oxqxbduy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fhnubjdw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3svdxggtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wavywzpb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szgwsoae.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3weuvbqtl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvqyisp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mparpucz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gjxokctx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pyqscpto.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3anvnewwg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dvdirioa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3paeulzaq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kpuhnxaz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cfirifcp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biafrjwt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3unnjyykz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fqihezmc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uuuvjcul.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cfkoostw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kzehxbml.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lcgoyhfd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bhfuvqdw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3webektwy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjsudvzu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3luilbpbe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iznjivyo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeajhpfi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjxnqbgf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hmgthjmh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fviaetah.html


<!-- 参考信息 -->