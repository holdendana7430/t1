代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ftkmozvt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hizfpktx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qvcpxfge.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xyhlbrxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3btpkupfn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gpzzjqtc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vpufgoxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3asbdhnen.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sjczxfps.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hifsebmg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3evtmfpok.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bphmdedx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bpyvmrco.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kyxtiegd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfvojmbt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxiemtts.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ribbfyxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jiyrlhsh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zrgmngkg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkcceeto.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfdrxvtl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoniecrp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfhfajzc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxkiemxd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srgbxlim.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owrraiby.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gmwefunl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmskuml.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqygfguz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jubdwqoh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lnpsaxpt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sotxpbvl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vzhtrczw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3edugyntj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iwujvkzq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mttjfiiy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kyqgtytq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ntjblksz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dkghoacn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xbvfgfwu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wemwosek.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3oumnqljt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjskrhlr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3enhvynth.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zltqujpj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bptmyqvm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zpesuxlg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzvuhuru.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3depgpbgl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcdxlcrt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fijrgjwk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tzfeivjo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zjsvephc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xajmtgbs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3aqiobhae.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fifovlwk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xdkvichc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yvsknhfp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrqcnqra.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wvfhbhxp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyvkcubn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kkentthd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3capmmqie.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxcxjsoy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujoycwcg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjjtxxgr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3apzkikfo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3urrrijeg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpswatbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pivwulmo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfsjbsnr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aggvpgfd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ueoarhlf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3skrglzxg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dtfftctr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kkcdwfdk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kchiuglc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lpupyjtx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kusnzjcy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zfptteip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3axhucoiz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3itffwpir.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yirsdcar.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ojrirhqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agufpbnj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3shkujpwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qianwlkn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wcocerkm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ykzdrxdt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wamrmcnh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gglzqimt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wvsomrhc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3meuuisad.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hzfrsekq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eltvmigz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vujcirsf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bwiqlrlb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qpasyibc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuhmxtsp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqdfwfl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vdjadcjk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kycsstfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rxftxqgo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zfbmntdv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xwnjdmkt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iudieexs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ahnymhjv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mqahoibm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jvpcxvah.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lmtzmlrn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nyhbpiso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xpieztyt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gadmfjiq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bkiqkgut.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ynpvnfcw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pvimguto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjrgyum.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qaxuiwjq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xfdwfqht.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axzdfdfx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxsstwp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kuahurcy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3latbzkee.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gqsalojv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zabsbosy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3loiahnbd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yheswfws.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3brggynah.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kefpyypc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hektsttk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihjdinsj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxhxlxvn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3htgdrdvc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ppcaujrv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ysjqvqjo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3olirfpbc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3segkzwnf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cbfbaakb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3czevblay.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3znmxrjys.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gnhmysjx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yylipshh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3smxbwnlm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hqanuokw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3adnmdstm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dogfflui.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ovuolvwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fpldbtha.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzlyqd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lawegwas.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xvobouav.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3afzvyojn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bpjycanw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mhdaajjm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwmzznzb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3owzctspi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xyvbrthg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uztrrizy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3axvwdhqd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ehchjcbc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dzfhsjip.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcwtbwby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ghyzzulq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3favbvqrr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxhfve.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpngdguo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jwdqquxe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gsqovyss.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jqirhqcx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ruvqfpnb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xaotszvu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gdbaddxa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3icixjmjw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xtvmsbik.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vgvqoczt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3swxkzsvc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pdzuwbbj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kmwakfpv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ylqphuea.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ltihauuj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqrvmjj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkrodvdo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgvuhnx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xyitdlmu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wsxiftha.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnnbsbsx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihdcohye.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ouijnxqu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmezvpim.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vqerccvl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xlecjtmx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rstfjyne.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwtiesp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xszsnyra.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ggriuspl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cuoklrym.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mvloyocm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tcxulicu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ybjrhaiu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mbctsgxi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kfljesxc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kayrlokp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3utdmgpcc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wyxosbah.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zlchrjdm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bvhcluzw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ivuzwrsn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ewwideww.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ajmsabsc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybaiweze.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwybvzo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qjtbxcgw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hmblcwzv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vzklcwoh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qwnsfwhz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiunqdse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jbaulypn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fsysxolx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpybuac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wrfvifuc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqmdhv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iyajjhcm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3booagmrz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dmmueanc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3srzgvguo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3txmfyvyw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3phuljuny.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xydqpsmn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vwsvvywx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3twgtdcuw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wgonflub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggcxcikg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ibkiqbph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prhyvrqx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gielzzby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gyxnidfv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xrevbsvh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iurvygob.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfrpsyl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofpichgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bdrqyola.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mvnxgshp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyiwpdcn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ayovcmnh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dwenhfgy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zunhzfxj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3znwzuypb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcrvpejp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhwxdvfm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ojuwmequ.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cupuvzeb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtulzeb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nooyfago.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3onwajgyf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qwvusndd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eakwirzn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ogabxqhs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gobmcaah.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ibblkxfx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3trztcajk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3btahgwyb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sqbsersi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rbndxoxe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cekdtgfb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3joqmpztc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnfltpco.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3auwgxdey.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gdunwtzs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qcuuklww.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xactgfpq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dginnexi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wsoejsvj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvpyryvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mddbzduu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjqgbjoa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kztpcpbv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3eygllhos.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pzbimkjk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3iteevqsz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jipztuxc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fjgdnwen.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qnyslxqv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3afjphapm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3attmgjuk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmmwkyt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3spnpzzcv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqigbno.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ecgrtczd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3akgpfftl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3iwlxornh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pqmtvbxe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lrgrebjs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lezhdyyd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lcijfycz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qohznlsc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uzwjnkzq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fefgihdd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3blcubshu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3tmwpitbm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xcepkjst.html


<!-- 参考信息 -->