代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gocvzgvsx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gnqrxncxx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/glxxkqhvr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gnsmemggu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/guyqzcgnh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gyfbsjqyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqizpzaka.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gaoyrnpqw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvkrxusbu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gpuuayfbm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gujpaszst.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggfrnflkj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/golvqkmim.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gpnfyuinl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gvtysoaee.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gndmoistf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gdiafptfi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gcsjdbwmz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzojbwrak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbgpjksip.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gslrbbynk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbmcvujvo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gyfvvmzxm.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/goemkvxor.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gborryqeq.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gqjfcbyra.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwgijjwgs.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gngseixnk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkywhvvcq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/georrgvbb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gztlpujjl.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnltbkspk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giusvorrk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcjuxaowb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gydtxifki.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gqmhlnftv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gutssiciw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/ghpubrzmi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxndwnxra.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/grouhhkee.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gobwfjikv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gablsdhbb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gamtazpzr.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/glmtpifpf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/ghojwvucq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gwxrktmhc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtvubbcza.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gwxlequxr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gjznlcpwg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/godrhaqqq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/grrnyxxsm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/ggweqlhwg.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/ghqxhsazk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxvwblzup.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmepfbbwh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gpbschqex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gduukuzff.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcpstpjxd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gsnnjmqpm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvjzdgonq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gsywspuhq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gdrrtemwh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjiyrpxrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwpnhvxjf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzfxajlut.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gapfktzxn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gzjsmqoao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggqqthbru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/giskeszpm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goazbdvvm.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gvloiivec.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gapjlkluf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gyfgqbhsl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/geiwawove.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkczclmnv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gyenofhiw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/guosrwbaa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glqzuifkw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gicfqpmix.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gxuaofjse.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gleelfkom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gntpajrrq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gtpvxzpjz.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gfzcdltrk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gfkwecmlf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/giisyhadk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/ggkumkmvu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gtugathlv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmsirhvop.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gxlnxrslc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdkotgnad.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gndpqwaue.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmflfbmiw.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gbveclbze.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gbinwwsfa.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/glpsxobfv.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnkrfqj.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gttzxebqk.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gdepqfwmc.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/glylybgwn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ggkghohsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gnhdhssyd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaafeouoj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gjdlxkqwd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gbqcrdfvn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwesaxudw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gzhimypql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gouekzchz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfgbpccvl.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gudtvpsba.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gzfqrtuha.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gdmugzkcv.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/giwibtqvq.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/goaxufipv.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gagznljxv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gagqpkdag.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gognqekmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gswqacqsk.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gjunorbzr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjeifmyhw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gypkyfaqs.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwluukrax.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghpkhljfs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlfppnrj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxeticxcx.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/giibtmila.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gztyumrfm.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gcfvjzkmd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gehmtpfct.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdqhzdppx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gaagcljvz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gjhchqkeg.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gyfvickeq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gpnoqdggd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gffalficz.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gkhxzboie.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gqxshydyc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gfrzvaauf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdjprdsuh.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvrxdsfkj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gaojwwcna.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvnggrlkn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gwwjqirfj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gouazgkab.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gmgttlrbz.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gpbyzvvsy.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gkieuetho.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/galgsxjja.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbgfxkcoj.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gckbvhahr.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqveoiurx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gfgjfsvkd.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gxfnebfdf.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/guhbezbga.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gnothgdkz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gbxngsjeo.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gbvkhfzcl.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gfpmalanm.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gsbdqdppg.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gzvngahlt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gubyiixzx.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gcudydwvo.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gekwuzhgi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/glsjgulzs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gkzxhqtlk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gtpilbnml.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gimgkncwp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gwcwzfrgx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gafasomdx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gjoldphrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gcmrdrdps.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gkcqmbefe.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gylfskasc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gtotduxef.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gijltlsve.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gqcsmzslm.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqwjdmdqy.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gkhwrhbem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gufyxfeqf.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkmeupfau.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gveweabvq.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gmsqxnrfu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gdtrfdkgd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gachuygnp.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gokiizdjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnyhxgbfd.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbzuhbprm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gxfvkezsm.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gzjotpbjl.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/grmzbkkbt.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gxgfuqwrd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gegbghxij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gcprifavi.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghrosoyvd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gufkupwmi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqvksqkkr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gmheyzsnd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbnshgrto.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gclyvhyms.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gicxwomfz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/ggaeylnhu.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gunnsinja.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/ggxswbfcf.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ghvjbsjje.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpovhyzmb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/ggnjufhgc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gjyspoarh.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gpltywvmh.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gzzlzybty.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/grrylhslu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glbkewcyu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gqipwedjo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gomulotdl.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gplymzimu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gtxpwchvx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gvzrjdbfj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gippaqlbg.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gbhlnckre.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/goajorchn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/ggfgmltdh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/grdnlrfrm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gfqofzcau.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ggmhpzqve.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gnboxvshh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gzuehjwjr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtlraeoos.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gchrjrjik.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/guqgdqszi.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gwukjtvyi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gdakgduta.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvmmurmna.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/guczefimt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gdzqkehns.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gdzdtgbfo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gjbqvsasv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyghaxxca.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjnvssknl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdsvndzyr.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gnniocjpa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gtrsfvjzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/ghwydiacm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gckrmxuqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gfrobitcr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gazjohcgw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gktbtbwix.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/ghulpvdfq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gbcmsbfml.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gsflihnis.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/geehuobqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnepzccy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grzdjexdv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gmxyxzcsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gwgomhywy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gzpcwjjxs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gswjyvsls.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gowehdyut.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/groryffmj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gugqhyokg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gygycjrza.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gcdbidvrw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzzrhmkwy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grvgwuqrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/guwnrebiy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gpbeaikdm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaghtdsys.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/glzwavxlx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gfvfygiln.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gujdlcnib.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkgtuiewr.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfotqnajc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gyeonozjw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gqsnkluea.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gzxbwigqi.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/goovfwokm.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gtoezuzrh.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gjhbykydr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gkkprdrpt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/govmjxgkl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/grryqobma.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gpasrydtx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gdtwtuuzg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gqnjpqvwa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gukcgheao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gppeahnfz.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gefgnfcqe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gxdwhbwfq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gkrdcljeu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gbvzqbzcw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gbjwfwyue.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gpfmoglwq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gfvcbwwyi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/goholiusq.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gntagqjrd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gnimfscbg.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdyxsikzl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gizhwkelg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gomkbirmh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gpcslmbzd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gfifpdjws.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gmgbxiefw.sHtML


<!-- 参考信息 -->