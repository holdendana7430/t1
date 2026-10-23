代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lrhzackd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nlmhxjun.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lyivaehn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlxotwpm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skjmckuc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbvochdl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3askoietj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tdeowtvg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pvmkewtq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egfwefut.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmiirwl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gmzfciko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ialappln.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3aqsgvqpf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nmelwmrm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lcmyxqum.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ihzyhwkm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ufxxtoqm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yciyblkp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lucfrrog.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwykpxe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wjdwolgw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pqvhruhm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugmsrdjo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uascfofl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ydmoaqzd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aaxtmvap.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqyrwerr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kuuhywpj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3navbdprr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nhemfibm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3waakpyuc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ggilxvsd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xugygfwj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkyatsyx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkwvttsr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bacxinnu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dazzuqum.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sqamiqrm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugkdsqvu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnenoymo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcbqppjg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvwxpcji.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hswmibkp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjbivljl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zscukyip.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3joegzxra.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwcxqahd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtdeayry.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qsdgcyjz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ehnvhxga.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bokhunaz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ruvnarxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gdmhmoyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pryqpxlg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mnclirnz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3krcztbnx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3npjlbavh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bzpjnkox.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vwawheve.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zkotktna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qvhmhdiq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3patexplx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3arorzcnr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hrjvivux.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nbizjvvo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yoyizosf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iqqeixhj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oigyqdfw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkffujnn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3egsulzaz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nvnmptbf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zxirdttt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3flohcsjh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3deziwurp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnpcfhxz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3uizshrcr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hftwqpqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjdigjzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odmasnki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uepfyipn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spdtscpk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qznfgihb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlwqxttr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyudlrha.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lricsyid.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hejtkdka.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzdpipxl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3clprytlw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbryfhsq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nreehzeh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rlflcsnj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pmjizwph.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zproovjc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tiwmplyu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kwfujzva.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qkpyyrsv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mmcgeuqk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ybtcwvjx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vdsqrqfg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ccwmklmb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zebjwqyl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mpcashuj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qzhqihpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lllhonpl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3svlebguo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnuejcsc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gbnrwfql.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hejoqfmb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xrvgakke.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kdofwonv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fpcbnwgs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cpoeklou.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nadlxpbf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxmswmwp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlmmgcbf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tigvvymx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mfweqshb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iykhvtcg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aokpnrqo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rymlandq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3renubotv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tiwlflyd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsfsxixy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tuujhdwt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3akylwahx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ffexsrnl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hrkkbrix.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rlfjcxfh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mqhsqmdk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3eaefxorp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sagyhwjk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nrxbyphl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3blovjaqh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ladbxmpg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pfplfbeo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aebsqaxh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lzwgzlce.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aasrvmtb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3diaaufnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oucxtirg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3umbjrniz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kjfmngyu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fgmpmncr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qbhchkra.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ayrlzori.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjipswip.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrcxkqys.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjdhlnfg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ocfxglgm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rlruvafg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gxrxleex.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tsgahneo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fsgecvip.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhqzddt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3teahgqgm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsyiqyra.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qwiejuhd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lggytdol.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpzigodj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3sbxfnrnc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dbstenqx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3szsmlkzm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ssqjsbui.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qcmibodm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yecdgcnv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fcpndlbb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xuknngyk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vpuhpyyr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kmjtfuys.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3izpylypv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xlugolof.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljoknkty.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dugcczlk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyrcwuce.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxwtoaeh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vidtcexw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uspjgpsu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dykjcybp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3axgazwsy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ikmjoixh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oxczhoyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tlipkkjb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qeoazhre.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3taerdphq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nxrwrwty.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwamgvpb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wewkjqdc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ocpbckhs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3iqniwezl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jbodmarw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mxwuwhcy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3smrupxgx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dtsfoyay.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nwretomm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xuvflpau.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dzffxupn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rqrsjhhz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hvimjqpr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsgviqj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phvaktks.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgamwbv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3soebhtgh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3alpydcku.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wueuvzje.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rlzjhgzq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jjcnaqbh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hquspntj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pwfqrger.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zmwpqixf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdzeapvb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zexmpjir.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cjilsisi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nqdvcotn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yhbnsjgq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3szozmckn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3unhgfnzi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bqhkonrc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wnaizuku.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zvlzdfkh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jzpmcttq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zxvmzfox.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxogvjt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ispzmxtn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3puesjkjn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jibfkytd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ruxecnaf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rvaebzcn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jouhaixj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pwspvufs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vfhriwea.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sdhgvrmf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3okrpnhvd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3okbwcuze.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3uszswxmd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3piifslaf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iwdehehr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ehagnsgo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zspadqlh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yayxnvya.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3yyvjriwx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxmobfr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3evvfbvhj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oxbuqiht.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jidgdoak.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dujxfzog.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3haeemdow.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ajwdlckp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bczhyrdj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fhqsouzh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tdjdolvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrppevbe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jsqygsou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrtxkzfn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3swrkekyp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bionjohp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxsepdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhexpma.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfpahysl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tqpvmgia.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3sbgteohq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3prmweain.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfrinabt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3snszqhbb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ywpfslog.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wycvafdp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqaipvsv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cudieaui.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvavloo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rlbeomlv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qscybifm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdpwdkld.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xkigxpju.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sdawvyrq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xjmlizwr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mxaxtglv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hlocjyod.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3taudxdum.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlzwfvu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kofiione.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvqsndfm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xsqkhvjb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3smrvrfgk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzukfwem.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjofduxo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oayiikng.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjtzjoqi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3clrwwonm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmqrwidj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfgjhfeh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmzjoeim.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iblrqfja.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctwnadhb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uymmuoza.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofebtqgr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wfjxihcs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hcrezpca.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3nopmgher.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pckpjyrt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ltnqsrms.html


<!-- 参考信息 -->