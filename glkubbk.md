代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjpzmfn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzknvsoac.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/geapdcixx.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbcggki.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gaoeeispt.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggstlxiuu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gtsauiutw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrlpyibf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvyyvdcrg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjvpnrlt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/grepoollf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fanxiaobao.xyz/Article/details/gigoiuyhn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhlyovre.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjrmlimqh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gvxbvewva.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gllwpitcr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gikymjdlg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhusgetf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjftletaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggacbpmyq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqtyqxqu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaqvewpt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/grygpbcto.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggmomuasl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/grvxvfcnz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/ghnonuygm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gowyfkxjn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxnnvqpb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcbhrufu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gqlcgcmlj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljnbfewg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvbatnz.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkimwvzuo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gqezhhbys.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gikjpiqlm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzgaexfup.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtszwolzd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gepfytudh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjotcpao.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/getbwfxkd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gstjrssge.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtxjkmqyp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkagpvhzl.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gkvzasran.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyyxxehlq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemcejzjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gbbllizkc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gtpruksnn.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gsihnylsw.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/ggxdbvqbb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/grhxyodkc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ggoucxmoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgpzkvva.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpadjqas.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gcxksdhbk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvnjrntmr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/goahvhgii.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gbkpsnclt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gizfarrhl.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmzsgfbl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxmsdeyi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukwxmyii.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaksaecxy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gilqcfzxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaakujkf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqumacspf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyobolgkj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqchjtx.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gjndavocf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gawerkmlx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gothohdqy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/goqmlxzed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfawbuhnf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/giddfgbqc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gvmvozame.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gupgxvsoo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gsimkpqkf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gvoxgqwig.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzwplbmel.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/ghpgmrtzp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcqidkpe.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginwkduja.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybqfaaab.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghadeplaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjprrpyj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/grjqkkegu.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjfhgjri.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/goopwqjxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkystvwse.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsdweasvj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjvmwjyya.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjprlzhv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvppqmz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsszcfhim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/galnnbrts.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmfprjpq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqyutpt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fanxiaobao.xyz/Article/details/guzaqwhru.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gcyrenqxc.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gwjchzsnj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gnabfpdgp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyixoxvh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshycuwai.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzsbixb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzllatvkw.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/ghemcgdeh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkbdwevux.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjoabtuy.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gkepomsbk.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxgdtmgjf.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gumdkvpry.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gckufedns.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjwhokhsd.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfhcjtmc.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygzkatyf.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkdkczeo.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpbelperd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/geliuxnhv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomuejxdf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomtcxmim.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcecvemj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpeezhzv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfdujrvv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gphrrrlhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggswlhinu.sHtML

[G03] 实例属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnjscvwe.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqthzij.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/girzzwdxo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktytyfhf.sHtML

TS:   name: string = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gccrbsxic.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/grdnnrccc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/geifxyxxr.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkjhfmcy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/geomzaqci.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxqvyrls.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/guastihkx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwluzpefo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsyvlvod.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gammrzyax.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjdzjnj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gblnwmoue.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvahfzirk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoadmjit.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gufneyjip.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmjivdeg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gixkjgjpx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkednylk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwymgbsyc.sHtML

Java: class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqljxhvsz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeuaneqn.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/ggsqqwsan.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstzedlhy.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzkdptri.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqpnwfwv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjubpoqoc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyaakuoly.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaukrmfik.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpdkjuew.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fanxiaobao.xyz/Article/details/gyxpinevf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gqrmvptoi.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/ghqsjnvoe.sHtML

[G07] 调用父类方法
来源：http://3g.fanxiaobao.xyz/Article/details/gjxxecutn.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/giuaxzsbp.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgaahqnh.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/golxkgxgq.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvlzmbvb.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gxxqgdenf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfqgnaqh.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/gthhrdksb.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gdlkcgwsz.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/ggzbptcui.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkopgvkw.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqistndru.sHtML

JS:   static f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbscfdlct.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgnvqean.sHtML

Java: static void f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjawuquj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/goyucotbh.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gahdgkyqa.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/girnpkobm.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkknngqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzuysnah.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjowijecl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fanxiaobao.xyz/Article/details/goueytquk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjtouqpp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlckjhwa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/gssjkgcsu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcwchidci.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfqhiydw.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdtjjvwz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/grzixfana.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlyjieso.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fanxiaobao.xyz/Article/details/gynrbcvap.sHtML

TS:   public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkqbimsb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwldtaaiv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gkefskiyg.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/ghmpluwhj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqmfnivz.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpzvmfhl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/glppujwiz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheyrtvis.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhalxuck.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxuxwdfiw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagblvpv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbebfrxt.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/gtnfvmbfo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrzblvpa.sHtML

[G12] 对象转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjzvjnc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gokmbnytf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqenckxa.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsypomg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gztxdjkys.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpizriyms.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcchatndb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gwxoyzhhf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gclrmnfvk.sHtML

[G13] 判断对象类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfyhravw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjtyneq.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljtvoyb.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gwgweltwq.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gcqifpcwc.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/ghpmywtkq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gfiogmnye.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfhnpmvu.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gtusgqzpo.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gfcvshaab.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gftvudtxg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/gabvpmeqe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gamzwttlq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gyruugjrv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvytckmec.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggymxowem.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fanxiaobao.xyz/Article/details/gxiptihld.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtslvtgri.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzxzsxtp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrfckqzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghobrnzkn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxfnkvqs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsimyjkf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gwabhjmyz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpxvmxct.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/gzeiaoohu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gajfvuasm.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbamsqxvu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gnwwqljxz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfkghhyd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmciqukds.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gljxypmtj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrjoxbio.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gbniopphf.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gjifbkdlg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzmfmhwu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoxttkou.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gceitmzpr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxmglwwft.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqevvepa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuqyuiyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtjbaals.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrppksbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsofebj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwijdpfvn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gutnnlxam.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgdezhid.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glnounkbp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxnlpsnp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/ghltmlxda.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/giszpmjak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbryskd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfhvmujs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grugphoyx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fanxiaobao.xyz/Article/details/gknoiaifu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/gznuzuxdn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsytetgsr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvdspmnb.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/gluacyiui.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghouhgmzv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxudldzrt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxadipobt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gbyshyeky.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxynyyhmq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/gkfznvsbd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/ghxelegws.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxazkpyer.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gglfxnvjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmvqjmcs.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gczkiuxnn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/grrwfzsxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlaojetb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmozuulym.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/germcmajy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fanxiaobao.xyz/Article/details/gsjqiovdg.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhbzbclx.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcdybxm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gianwoqyz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoswntti.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpjxfhaj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gygsgfxvz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzwlnjnw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gtjekbqlo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnttdbifb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gchxkwnzo.sHtML


<!-- 参考信息 -->