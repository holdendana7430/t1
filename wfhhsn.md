代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nvvbythw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apkbphfn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gddrbtbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdwpwjxm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gadzqjdt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qyjvpmxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcufulpm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3usvgmydf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hojlwkdn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ysguvbvu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gjypuzrz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqwupygi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mhwbvrxf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynwpvlxu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bgxqviai.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gybraxtb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phipgjsz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bviexdon.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqwdocj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mloujhew.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3smngvyez.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gflcviaq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pdgjywxk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdcwfeu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgognb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dtfhyhsx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3axjvjdlw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3awsakpsd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3frnrnjdo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wzsmqyxu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3shozxsnq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3koenkoru.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nrbsceyh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3paknxqbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kxcekbzm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xbnotxfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vejbhcfj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3aiibgqky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3edvhqmxc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hdhslyyj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cvryslkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dafzywaw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdxcgfvh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfkbxxar.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrpxepll.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uyguttdg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ravodvxs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urkbvqfz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkemlefz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qxcsvtdq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohvzggls.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3toqkinps.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abygyyla.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otznlkop.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjuutvja.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgonkian.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drxjxnen.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uqeozmde.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3koduxlur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ndvraufq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3npcfjojf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lsgsmlji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xxeudgoj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mmwfehqu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3swxuryow.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ohtfprfj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3coyvbprn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rnlzwzdp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lkggldmg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3biphyjyp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dnqjlcvy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ceyxvfni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ecadviax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3unvzzjzw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mvhvydff.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nufipdqa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xoekrwhu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knwecfah.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqleztnk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fhnrvwoa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ciupzdyt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3psyyukgk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xeugcnjy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mubeegqq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wxwwsber.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3utodttli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuuyhfmv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gotvlfyv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etdezoxa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrswbaqn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vraqesrs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzyzpsuj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqyepsof.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgyddiah.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbzvmypt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqupbfgg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dokufcot.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlnjkiyi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3picgnxds.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bulkverk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fekszuox.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrtmcrmt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3oofiuoaf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3yhrrbxur.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxiklbq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yhazsxjf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3unwpcsir.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dsuylcta.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3aadkglmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3heelecre.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bywadewu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eiuetmgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyeswtrd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pytrnpqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxevynln.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xshcyvse.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rynrhyni.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3izksfsrt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3svlxynsr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mqbzxwon.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmptwetf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gvinguzr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xohgsosd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dxvrxwzk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwhbeqfu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3euiwelsz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtxlyxap.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tfkxiiar.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uanxfuel.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eltgprdn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3epsmaxvp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbzfjjge.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oyvvhmjt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aopjmhsr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3alxprctg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3byyvknax.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vtobdtfq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jecrovpe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3whtugrop.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lnzaoxsq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rnbvjjxj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kdautbuz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mykxfztk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ppeixwov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjgjncis.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsyqkdb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cjozmyjc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utzbexmt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uexzrcaw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ebqxomkt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xypecivr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3otpboams.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zeohsoqo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ykinaenc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bwfqguck.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jettuidm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vllxivrq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qvquxylg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3olinngqy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zyzaglnh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bjebdcms.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pizngybt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfvxjgl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yifaekja.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jylhfruw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oargzdjg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pahbkyea.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xuintryu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3clgbxyrr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ccapxlax.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tjftwmdn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3svgnoqwk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hpslzawv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gcntzmpv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cygnpxqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3osvralxa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mywqlvlo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cabckerw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kpnxguwf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ujlyuzjy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ztvssvwk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qilmvmfv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3iuhwyzsi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3amirxifc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yefdanml.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ezzawyip.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bqomhuez.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kcntblpx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tfmgfixg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dchlzpnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vaohprqp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ifxgbjhm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3toubhizp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rmestdep.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zwcjoqve.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjptzozg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3spodrwup.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rfbexrxi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wcllbgkh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hgfklgut.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ppcggnch.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aaojkdoh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3chtzvfgk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wkpgaope.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3crfjttfw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3brdpvzqz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gfizjwjm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jowwhofw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxcedehv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbjpyvmv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjfrftkt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ppoeprud.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qvtuelwd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiwledmd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jarviavx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wdwpiveu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkdqjgr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrjhkeo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eziwjoop.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esojqgpk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jzyfpzov.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjbbbhus.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jncdwhei.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmthvupu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3klyyaros.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ogorhddr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rbafgwnt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlcmlrls.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3khdharlv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cjrnwico.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqeppje.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dhphfftw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qcfvydbb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pzqirxuc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gcaiakcu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mrtudatq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3isuyfybj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otdjwfhi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3etpwsciy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ebintjgg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bvzdewom.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kcmqergf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vhzayesr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajiykase.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3leyovmhb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbngrhex.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3igznqobq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3caiysfyg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3oprpbzie.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3paxwnmhp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lqaszlzc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3skkfzarc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qnucekgw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvibdacr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbpsrnnk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fojuifuo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fgyfigve.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dzvevgvw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gvwtsjoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrjfzkql.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gdvakydl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhzhziou.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ttxlodjx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mugitlic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ddecaxgm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3najvqtqc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yztnclha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ydptjubf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3avfmpwvs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzfappxh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ryeytgph.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dcckqtih.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nrdppjtg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vvlaouer.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ltznappj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjkynjfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxynrpmt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3iejdwole.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cynxypzd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mfzvurfo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kvihtvri.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zvkvvriw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mzxqkvmt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3klugikzr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cjtqszak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3texlymvz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kalxxsld.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nwrmtskn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kbetwqfc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3waeruvjf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rutmtnxi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eiknhctv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dccxzpsz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3acdokckw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpwhyqbf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tbydlell.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmcfiawm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3orjcyypp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmmwijuv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3sywwzbew.html


<!-- 参考信息 -->