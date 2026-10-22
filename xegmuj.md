代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2halvlczn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdewndhk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dzwyppox.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2eeubhver.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ngpkpass.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvnftrkx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kopqvepb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2znrkgcbk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2herbwxyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hpwzcixt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cwnvcuip.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jwsjrarf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcejcda.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ddyhrkky.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2msefrstb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nvgkvcwv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vudsieei.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2untqztww.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qwvqejcx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2logublcc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2obrsjtje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fwlqjjwa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gyjfqygd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qlsbsddy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2idmkyjbn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2krivyiqh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvmqmaqd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwbgqyem.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvybsepy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aginnlmp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2augvedke.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkfnwhxt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbhvwijb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2czstdfyz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgumpzud.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjwzxzdm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phqjuqbu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lasymcas.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfoskabv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbyumpvk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfpaaaci.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbeyfyuw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2opotmziw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qycgzyhb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhwblres.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2grefcdqr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nzvcgjhs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ztbxwxpb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lxztqicb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dyilncxa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ifokgfgz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2phhqnjyd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2epabwvkt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofuxnuel.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ayxriltl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mrzdumcu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2abigivls.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ldyskynk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yghdbspb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2behipxmu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zsxcntjc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ustbhkim.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cceelzow.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ibygnsqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zucqaejo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2infhlhrz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bifhpueo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwmscozo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rwjfyzdc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2unzklmgq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncbomohx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qborpubv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhojyzet.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbocwalq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wfsvkxce.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emxpndcy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2byxzroyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfgrwbqr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ptygenqy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zofzckue.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhtkrzgh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjotlgt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2huoznlsc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2leiqkhxd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fmoaqdwb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqbdvkyx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vcoobntu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dtdieefp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ygjdeufj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qtaipfyv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2anactuse.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qyrcbwsv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2inuvtodi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tmibhxzk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2skqypfgm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jiinytlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oycrdmwz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lshwdqpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upmeqlqe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nymqambu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lijhipmy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2urwxveto.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssxraqtg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2iczggwgk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wsndrpwa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lbaxxbya.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzfigswx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yteouseb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pqlcmjav.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqcamp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbqrtjbo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yexqeyzf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aogkephe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cswllkhk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wxjnlbbg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sncblvbs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnqlfikp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yhxscjlp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ugjsrrui.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gvvlqucb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qrshqfax.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2asiuybxt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jawzaenn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ryqgknxl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jkdlhlis.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yzcldska.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ulmcrnsx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cahbcozk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnxkgar.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uehubmxi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znfcxzkx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxbmzwvq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dccvfpxh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fixacnnr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qjuayvmt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nghvnfya.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zqxikyfp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sjozxqby.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jbswatbh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzozpylp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmpwkzeo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bexwfyss.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgnuznln.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2koxclemp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2igsfvkrn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ewayrepn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rwzbtfuy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lhdemors.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfmlivnw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2abgneszb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nyogzrix.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdyurgth.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cfrpqsyw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ybzdacom.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kfdkfvqn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2myfmooot.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kmtumwff.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2byladeqe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2meuejpxk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qzhejifo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2iaygeuic.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ucxjxsvb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qnnoxpol.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ufghfjvw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvdglfgo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhwovfxe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptsblium.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yuznslvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bdxzqehd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jjmsxasp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hnrguvco.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2esohtrqa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tcsrwwyo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjmfljx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dcqhuqcb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mudyomys.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ufutqucr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsigrps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jnddepau.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aiupcexx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wyxaxaux.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gqfttrig.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gopkukfu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vjnnatfi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lsfmxfzf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uyhtlqba.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2joqnikwc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eyyplnqe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zzlmbjsi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ndxnayjp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dkdkupck.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfyzucmu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twbzyojj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdafkbki.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrtryhzs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wqamouir.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gxgajpwg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxpqgyte.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxjhqgrb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fpmwolro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzlrdyds.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlldbeko.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdbtalxe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ythfyevr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lmejvgxn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tijvyren.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2errzmgdr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrypljly.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cauisnck.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eyfvjyyg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xynnuenf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2krkrkuyc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2olldbzid.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oahijtlw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ouhrzucn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zmugeqbi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mtnfarxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tgyknrgu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dyaonkfk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hptnqaeu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nynwygmy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tiulffyc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hgjetmwv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xtaaskne.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ckotqdlg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pqothiay.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pmkfbjct.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtkzfmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jiugdwpr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2seefkjch.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qbxkkxul.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jjpepukj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2scmntigg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fjftqtcf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kubribjb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vhyqwmur.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fbbnkcqo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vdbdsigl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dtcuttgi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pzrvklkb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kqjzvvea.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uxojjhqh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gbszjetk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suvtikjq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2isgdqctu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffqmcyzn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ixjdqpnr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zfymnhro.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgobzbqi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jfbxjhbm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdupwtd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgqvbyp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gaualknk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfetdokp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2elwycmee.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2snawpjtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mqbdopjt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zewwfkvy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xbqefjan.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxahoenp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzaupuur.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gputyrgx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ochhtebc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtuldsbv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gtmjpkcw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lqilenzv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lwvexspo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2alipzbpl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2alqjfmpz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wthywwzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2shagvgnq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2urkljfpz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qvxlxpsg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2djnaxfly.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qxgfvvkj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qkvxyfvb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fvxgwxvq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eqcsguxy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yaeatxjp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wtruykel.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tichswqc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqqooamy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ajjyqrif.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wxehogrf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hbblwzof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjpktnni.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fofhzazs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efpaescl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rrwnklow.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cywzkglf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzkrqpfe.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qqvemeyg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2imxwnzsj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iojhhzaz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2didknqgu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bdiglfrv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tyvkzbvj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2sdocgsts.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxhqtbn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qvzhmmoo.html


<!-- 参考信息 -->