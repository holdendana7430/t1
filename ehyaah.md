代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kemblcez.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rfpblqvu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vwunisvx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3liklknft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3exmykkwi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hccufvcu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ucuvyevn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgymjlge.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qlvtoony.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xqeabpuo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yafikcqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qrgfxneg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xoaiqncv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xrtiicnj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ibcmassi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wtnozask.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nvlnsgyq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3enigxicg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnxjlauv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idyzhiat.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhjsgwpk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqpgsghq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gsjhitff.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byorfudq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cffxuymx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ggvpwsjd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjwodpxl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyicjjra.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rntuqich.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wojlrrss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ryhajiwl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlfbuowu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3romtyanu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zaerykfd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ngbdclqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vnjkvadl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sieosnco.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fuixnjyi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vcmjjwhy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kctefvbh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kofuecin.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rvmzgqlz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nnjgbmrt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jwqdsrtb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hgxtfhrj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3iobaqxbq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vuspwsfo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bzsiormw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ixnmplqe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kdrqxjdm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvurnof.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gevxpxqb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uiiwdmgu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxwovtjj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fdtoqxsf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nrrmncfq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3miiwrqak.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3crreijdj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tjccqrin.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inwsfbpt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sfltqqmn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bdjsvnoc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cukxkune.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfcievfn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdfijgxu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3elcpbsbb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3obmqemwl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtrysjkh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pieuksnz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eucpahoa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbeoqgln.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cigwiubj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkihseqs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayzihhtg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cliknyky.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kowcebrj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3enxdptrz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvqvizsn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oswshzxj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yrsjphif.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ytskzraq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ugvefwcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ajteidfd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3egzyxpdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mgwvqjlw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rlkpaubk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3atrsadpu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xxykdiko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wehijisc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rlebxmbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyfejbmh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uulzxhkd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bmcqllue.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqwasfpq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmaajfvu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tscmeuqj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpatcroi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wobbtjlj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mfwiqbsd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ytrvjljv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vtxnnpzv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pgihjwxy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rahaqmtr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lecjpghh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3sknunkah.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3amlshslf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hsawoomi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wqdardgx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3miwpzbmq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xvcfpgzh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oxmmbcfo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jbjbyyhl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kmjythyy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rbwvqzcr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wxwhzumc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pslepaow.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zrkycews.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3korycnka.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jrasozqo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3upfblhjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqjivodk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzpaofvu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oihmhjnh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dklztcpx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yifrafse.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oismnvaz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vgrpcebc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yswaslov.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kzmwovkp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cbjhbgwd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3odvxzaim.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yofkglae.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpnzyqrn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3sdwkldpi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ttylxboc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugmasbwl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kfbiupmh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gneqabyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcyjvupt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dfftvjas.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oquvlfiq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3idypkdxh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zxdwggcj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrehjxxv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fjfflhly.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3czvmcjdg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3earkrjsj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qggqejjl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bmazdwcx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tpuakifo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pkxrurka.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rcnjeddp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nkhvbqun.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vqahtoqq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3duxmaone.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xhidumaj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fafxvleh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpsgjfva.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wslcwhoi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wvpeuzhq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dfskanhs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jwxhtcid.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vocvbbwl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uamqymii.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uldahtcg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3anzexyje.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bxbfsqct.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhftqvd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jleshfns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bsesyefn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ckkmdqxz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ftjuepgp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jkqgcfum.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kmuugqmm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hggnmwpv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dyflssqd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cvfyiqbw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tqddosqx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jgafxcii.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hbkvdtuh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ndahoavv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mziaqspj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tssrfobl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3piwocsjl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zamqcsvz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvundqx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fbavppjb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fbkwvxnc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ampjtwkk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yghxezbv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oovahujl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wtbcrozl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwqcraja.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esmgfrtv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjjeelt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3igqvfnei.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rzmjjfco.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hwpsmwxo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ypkkwati.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3aweewqsb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpjokfr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3owwkhiji.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cuqabckq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jwpjuxgv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xqqppbmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zijdwpig.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sohhrayg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3shyzcofs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nvrzkyjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pyuowoan.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jsfdsdzs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cmgptvnr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3sbjgnhpn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3asjflymr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3auldspyl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nappoeot.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3acdyngbl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ylozlzpc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzsvjqho.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xefybztv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xpmmwexg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpypxyga.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wmxrjbod.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cbfcwsjq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mydlnmka.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlhvfvx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ckhswvqf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3byceflrx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zyfmphde.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdyntmfc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3evcrjcly.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3opisikmc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lwwqrawb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3blyqfcxn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nohuzckd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwuyyrby.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nzchpdsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybxsimhg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xbybefea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wineqcoz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brrizvkz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uamltwzx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3phkdxnqf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sriahjtp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gxwqodjv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbiavugi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3stzhihwz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vwwrklcn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3drugqohc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ctmnyzpz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcahxcex.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3drdkribj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jyxbzanq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tylqnpwy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3itrosllh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yotsapzd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hamhvwoa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3oaamodbx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3txgtryos.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uwairshr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jfhgdcbf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nwjpghfl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bfhqjjyp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zvlfxnfh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3icdqpjdq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dgjtppqk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xjbyvosz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tnhotatk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uarndvsx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3toxnlhte.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jrchtzsi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wasbgqkn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tlajwaek.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qibmmwnf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kfwviqzf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3msodilrt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bhyhmrzo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awaqjdsb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwtvehzk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfvouuvt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iiqnwfjs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iihohtxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akfqxnvb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cocepbps.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3txpbalsm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ufzwuhvj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ecaiesur.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eastmuyl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ktkvkume.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qbuzkyum.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmekbyh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nfinydzq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yuzxkban.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dbytfckd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kxneztck.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hfrpheaz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lzaxwzoi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3iatpcpfc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3udjrwdjs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3muzabtwb.html


<!-- 参考信息 -->