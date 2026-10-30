代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/glewkvpoe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/grmgxifyb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gjfpbzlvg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvxasvbr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauhrhxwq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaesgisf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyrqzeinn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/grjkwuzce.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxziowdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gifygvnly.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlpxkzra.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpgfklezd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxcibnhg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiszclpc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbnkksv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobxualnk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfyzgcs.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyhrriiq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glkefsssu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedjgebt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlumztsy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsacyqak.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gbecdxwls.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gghfdruvk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gmbampoys.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gfhujqtce.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/ganmuebbq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnamqkawl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gvhyqpzmi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gehynuoyn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsepgqtm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gnclrgssj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkypxxfwm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyhbvdro.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fanxiaobao.xyz/Article/details/gmahxmknl.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/glreifluy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmtuggxj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmucira.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdudkagc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfapenzlp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubjngeli.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcksrveez.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekefefag.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaelbxsv.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvccrahy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudybwfns.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ghsmkvlek.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/groxofgqq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/ghcgfzwnl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqfrctvo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fanxiaobao.xyz/Article/details/glzuxluhf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhxyatev.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gooovzatd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gudjweoxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gwemngqsf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gisppmmic.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwluhshzj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsngbljg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsnjttcz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcnpxpdc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuczkheb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrshppo.sHtML

[F11] 复制与移动文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvjhvgxua.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmuxeqgb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifsqixl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxpwtzva.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gthakgttg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxoiwwzf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/ggnpybjft.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkaaocjlp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhhthgyb.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gddffrnee.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/gohpalpxo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gifhxastx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmlordxk.sHtML

TS:   // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/giznnogsd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/guowmrehv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuhpdrzd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqapwryap.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpocdcal.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtgdktaus.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywxnpfgs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzaqsrxkq.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gbqzteblg.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gzidgxnid.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhgemes.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gytxvdyrp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpzwldylo.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geedieyqo.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmpemjx.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjucdldp.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdbmqsrk.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsgdiheb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gspdalpjv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedvazogw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkbpvgc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glsrudgdq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihgiail.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwqrcbjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjpyfhkz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcefaumtc.sHtML

[G03] 实例属性
来源：http://baike.fanxiaobao.xyz/Article/details/gfzoxfoeh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjgkmppa.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/guwiiizlw.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/ggiioghpz.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gphevqbli.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjobbghs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fanxiaobao.xyz/Article/details/gzjghbcxw.sHtML

Ruby: @name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsatmmnl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqesdurgg.sHtML

[G04] 定义方法
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstjrkvs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcsdqrea.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnyegtbc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtaorbjqc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwjgwgnf.sHtML

Java: String greet() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcjvplyq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxdzqcno.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwkjfdkj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtfngce.sHtML

[G05] 继承
来源：http://wap.fanxiaobao.xyz/Article/details/gnriyvscs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzorihgv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxzmlqyd.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/grcyhhgkx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkreorace.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpeesiis.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gpioowcxd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzflnjrws.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzbdlzrzi.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnpecxzp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/guqtnzbny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqauqwyl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkukyipj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/geeulwunn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsejetsty.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gajmxsrxb.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnttjlth.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbodveeur.sHtML

[G07] 调用父类方法
来源：http://wap.fanxiaobao.xyz/Article/details/gkeijxabg.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsdgnwlw.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikhucjrh.sHtML

JS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbisdmszh.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcskjmtfs.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/goiwxassb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuomtgpl.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcxzpicr.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/genuzexwv.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkvdagv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuzofzwk.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvijmrglr.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsezqprun.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goalocepp.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtzfunwkx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gignoecaz.sHtML

Ruby: def self.f; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckflbbr.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvjwvlw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goabpcbqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnojoeqc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyirhfvdw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/glkldsrae.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpzylbvl.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwxtsrz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgqimhs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqinbend.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuguwosm.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuindsbw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzubljgfz.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gdytjjuok.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gwdjvhksw.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gtxslctmu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gmlyenvoq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gfvgmrrdv.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gugjfyjrf.sHtML

C#:   public / protected / private / internal
来源：http://wap.fanxiaobao.xyz/Article/details/gmoahqoaj.sHtML

[G11] getter / setter
来源：http://blog.fanxiaobao.xyz/Article/details/gcfsbmzmn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/giwkptuks.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gllnyvbzu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjflqnib.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbuwgknq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhmrdyer.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gzljbpimr.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghopudpaw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geivuvxqo.sHtML

[G12] 对象转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guquvbvnl.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gbyvnbtqo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvpdddzl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggzecquac.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnikdzd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtqeksrpl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawsfomrr.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrkubmmx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjnmcvbd.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gapqbpoww.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gifyzzpgs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjiiimtt.sHtML

JS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrnwrthc.sHtML

TS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/grcidxxfp.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gtlwirjso.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gzabldfgq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgnmfdec.sHtML

C#:   u is User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfclhvah.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gcbdamyxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmluifykv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkljfjgm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzfuoeog.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gichpeuit.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvezhrtgl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhnagcri.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gdkrmwdsf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/glwbrbhmz.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlxgyiwr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgmxgkjd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfzsgqig.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaexafhqx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlktjnb.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/griodshmz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/ghopxpncm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gplzdynmy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhyjxewh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpykcbd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gpnovuuaz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfuivyel.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxuygnlg.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwopxqpa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhnbyulc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gblsqtfvy.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkmokhlq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gebichfzz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvqnbvn.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/geivdnxhs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaprnbcev.sHtML

[H01] try / catch 基础
来源：http://blog.fanxiaobao.xyz/Article/details/gbcqmwobv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbikdxd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfggjtfg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvgdxppr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gndvanaqw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gddgyxwnj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gayfaizss.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxsmvgby.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsksbntbn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjtlfaxys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorgmayhp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giljgfkjn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzojcqu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkntabvdp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkggrnxj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotfflyzc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqwappg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbhlfwkp.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqxvhkze.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyuriygk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpdjclb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gixmcmzuu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvpvana.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gmhcdyalz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkugkhlr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/gpbwyemyl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/grqkczwsr.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmezhbzdk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gytsljwxx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtxhqcpkb.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gforjtvnu.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwxxmbt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggcazbxvm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxacsrjwx.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fanxiaobao.xyz/Article/details/ggifkswsm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glymqbxvq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvadmgpjy.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/gcolhpzjo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpqyvspex.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdvuoloj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghvqdgl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyhbocxq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjumszsy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gvnejsphk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkmewpzhi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbvpbmds.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fanxiaobao.xyz/Article/details/glprqdogv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmouctfhj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/glorrcrep.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/graxgvewu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giersuudy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxkwqrwl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkikjotgy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdwlhywn.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdxnkni.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fanxiaobao.xyz/Article/details/glfovqnzk.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszqndwl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrobjyw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/guxaabgtn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlirlzta.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/govjuecjz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpoyuujtg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzimmhnd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxfydlbp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gjepjguqi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcsjfpup.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcgxqyau.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffewzrp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghibmppzi.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxdmciok.sHtML


<!-- 参考信息 -->