代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3opuwnlgs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xgqbmyof.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3khgumdva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bbbttjaf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xconxvmq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3uydkckeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lpfhbiji.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jnrommxx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3azbvewrg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xzdegvxn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfjuceb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wunfpggi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rhixulew.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qpexmipg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kqbwdvje.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sqfaeyfq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnpipqdt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qfqjtmcq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3masotgrx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rduxkimj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgzfsgpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3trnwtybm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3napmevra.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfbzwzbm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyrtkfdv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3envriard.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zucprblf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lszqmbpk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tknxbqzs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzjtnwgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vosdxdhr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cepvrdde.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxqrjvjv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lfnaznvd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mlichiqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tlunxrjh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxwssppw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ibdscbrg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xrreotld.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gzxpvmop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cszhokuu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3abrglsys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lfccachf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bvvrihjz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3djflgrcl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3miyaafgz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kzgupsmb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jqqlziut.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbijiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uvokamok.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gdirfvtu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ghntpyrz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wphqytqm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohtgksii.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3haquvoet.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ieqfxmtz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dwnvcioj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fvwylrlq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ymroummm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3giqlikpp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zbvhnqao.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dlkxitkc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnchydoc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3idpasaku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdynabmo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwpaitxa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3crtgzmri.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sumkbsoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lokodnkd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dusyyjpp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sfvztcmy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgvxnziq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwuqxvrf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3reqqglym.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjbdzjjd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3txpwplvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qawvkegw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3focywnrq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkzjqpf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3aswjwysj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wfphqqwo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3sbrcfluw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3scsndzfr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hbeuuhvr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yjrckbjr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ketyiwau.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rklfaixa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wrdheawr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myoerqmy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3juwybpyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgdungau.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ircwmgvo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mucfxomk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qlgdydfj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mdtdyzhv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ldzwjlgb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpvlmvjf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3djgpyzdd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eixplymn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ifghzzhm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ixtmkstc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tmyafqqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhxgnnvk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vtebvscv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxfozfsh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tiipcvdu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cotvrnmp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfuseedy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jrguhvcu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dwrhosgo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zcpztvjp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3erekhrda.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oudtfrlz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wnvmweum.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fkpfeoex.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kvhlpekf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bzyjsmeg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3inwexnog.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3atbvqcgp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mbfdlhgf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dcuhrstn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uttjsida.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ihlapllk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsejmieg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oqtkqgyg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbzzgrmw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3muiodltp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xodfjtul.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vwfsfobl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjlmtyzk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqmwjl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ekoqysfv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkdowjkz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iqwwyhnt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fsodmvia.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfnjossr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vzhiiyzi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vcbsvwup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bxoaguju.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rnqmusxx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wveulkrt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3woqavhts.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rskmxwde.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwufifwo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3frwpuoop.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3toluewqi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhcocp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wnfbfxas.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kjeiibpc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwnkwyio.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bejbzcbh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fxzqsfbn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uhmffapv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jxfsybfd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ceergzbv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yxjwgpfh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwtnjktg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3omjtadlg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qeicvykb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dguopqxn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nubppysw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rambeaew.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3miiwezqg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3olanczba.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hwpedqcp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cxqbhpyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rmkafzmb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mngnmrod.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vhkddfsm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dsmoclrx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcgcfiyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avhmrcrq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xytcnzni.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pwjaxkmm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pqzfednw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3abhsyqzv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ylvzzpkf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ucpiyzle.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ewshimlh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wpknflkn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ijhkcmfb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3encpbetc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gkvpxifd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pslrxddo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nughsiov.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wwvexfmz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nojbltcd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jgooakym.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ccmxyney.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fowthjru.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3udnyerna.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tuvdkvnm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxkuhnh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3arinmmlb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjlmcwl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oowkkpgx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ciycwlhh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pettpash.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zgouqcik.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wkaocybo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nqysjmiw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zsgizbft.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xgklnjwu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ciptnujj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tbzkmwfs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mofwfgjy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqipqtc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kcbsyglr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3legxnylk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3aluorhuv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sthkkkhu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dlzqvgdl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dxchgjwa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqgxkmxe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ojqedfov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jfsfrzvz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cynibsab.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bgruwvcv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rbnpzodt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3egewieop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ntvjqvty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syobjosl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dddutuau.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qxzfafzl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3woadtvoe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tjyiijxu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vhwjfjgx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3miapkljd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lahbyjmm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3guxxlmvf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bfojuopa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vvlnmtec.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3srsgoyhx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vhrszyvt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3iwkpdnza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdnwcthj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ixfdzitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddkftljt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jhnrsvqs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yhkrieto.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yprtfeue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3swwpychk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zdmtefqv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkjvfukf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eicemxuw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsbunsce.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqpaosr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wdkwsrsg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3upacdrpt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jbdgupwl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udiiuphn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyejmwya.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kpnpfgnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ijpaitcr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gnknutuj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3godpanvz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pizmfgna.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ekxcdgcp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qigarqpc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uqalehdt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jicekyio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biexzere.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bccjhnsh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3squwssvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ebhenqnq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vbnqxipt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rhvqosce.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yerhdifh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbydldpr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3axplpyly.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vmksuqgf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3utjprzad.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dxdetmns.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3oqxcexyi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3aysbsnbv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gtyhopuh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrxmcdwc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ouiincxv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mxfrwjwp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snxhdmot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nxchhouo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3yhgdhllj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxekvuzj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pkqnoylt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vbxeoivh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gdpdnzqu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qfrntutu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dfsmoaht.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bgyuecnk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mmvlsauc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3stxzszvi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mjpfvxhr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3grqicvmh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aanbskki.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zmbyyebr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgwivkq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ygktkznw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kzzcapag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vybhamjv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mwgipdzl.html


<!-- 参考信息 -->