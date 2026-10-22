代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ohgivjug.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cfmefkwh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2puiwhnek.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yxwprmpf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkhxpnr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2euirvuhq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uffpxhch.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yhtxwfaj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kcyneltl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wmypadpk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vfesncyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ybehfxuv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tqeqqomj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nimvzeoj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jhzjcedv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gwhpgfyi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nfjdmaxj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2bzroxtid.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eobgnddi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zoissktz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijibgnll.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2shlcqokp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ddugwrso.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2autyxxef.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrzuily.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fuyitypp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbumflzd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vfeygpdh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umrokpwy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgcqoxbi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yiruayzf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnmpcers.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtbyynsg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nuwtaerb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wqwzioeh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fzbwidrp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zuxezkbh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2maotnsao.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bibpdyxi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2toxvgrhn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nnmulidy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eyfoqhpe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wfggkeub.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2poppetsr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iazizkoe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ckdbmoxf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ucncmeyv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oiqgzgzd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ijrjqlae.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wuszpndc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xettzwiq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oihpgldd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hambajpo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psrgeyid.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agkqamgk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xsrvdwio.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2odoopwqh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jdqmzpxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xzlxqwek.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhyvkrnf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ydiayfks.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iqwjxhwk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvdtgodz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czjpkvxe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lemyiguy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvwwaaih.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hjfdcccg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evexqguu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mysdirne.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2usdkbkbn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qixgpyls.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zehroluu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qzhgxdoh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smczvcid.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izribmor.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bpdeumzh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pfhofdml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trlomrqw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aoqrzgby.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gmkfrajp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvjtyqo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vtvtfllu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vudutnmq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2akmmyslp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xgqomfow.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bqqjlwoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vwcxhgvd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yridqjua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqslchqn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2irpnzkby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgucyfbn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2biuvflqa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2twwxvneu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oplvxsfe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qrsntabr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ancjmitr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2illxeqie.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eiemfwyy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vwaesopw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ficktqrp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofnvgmmc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vnrdndgp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onyhvjdu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqyamjex.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opvezclg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2frhkkira.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vgmnxpzf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2miwhweid.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cevuxkxv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vgqaqtvw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cctjcrrc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2taqfkvwe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lygyupbf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxutbmvb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2juszdhtn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qwtjjpqr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ryuyybhw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fenxbubu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ahetamwb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aujsbnsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmepvcho.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gceblspg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dghfdkhr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrlncsx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rdqvxtqg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yoczuqns.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aftvbmen.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fhonkhsa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rowgtqae.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgynjjbz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzbgmzkj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2voapbadd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yljiicdn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vevkkhtn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkqjzmld.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwpqtinp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqcrbfri.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yalcueag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vyxtrjdo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flmpmczj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nupogdsj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kguvgkxj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ajavnike.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhoqgwhs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pbtxpkfz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tebihesk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qasnjmxn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yilycxza.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nywuqwzg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dvrsppuz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rayuftpi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2oocwlvrq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zvidpixs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ymdvwoey.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kbcfijka.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlqzil.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cctzvjqa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kstjtgph.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdjjiwqw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xugsrksr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2izukrzwn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zsybhhqj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpgsxnqw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hbyqnoym.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sflqoduo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yggicmwi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ggvqiqgv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tacebzrz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmbkwtb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nifmhctm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hedxfbuu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xbantjcf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wiaddntz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nuyiovoc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2odjxpcyo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2flstjaju.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mrdxomqs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2eusjuwsr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lbdpsodx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iqlvnfbn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xzgakyln.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lprfvgij.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ysjuxywa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjausffz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2choepkhr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qanqwgcw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qifqfhuw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gbghyrer.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jprnxvlk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwsihac.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ycjkbchz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rtewxzun.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhvgwbim.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oufhkvlw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czjcxnau.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uifbovlp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pixjgjwc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2npbgueqc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2icixijxx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yobosntg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfunqpv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2npvkwznr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gbfstldo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wjodbxzj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mwsjyimw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qszxigjs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uevqkmoi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pjskyfpc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2znmnkfgo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ryercqdk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jqfhaeyi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pudngwtc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2plvkttpf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjklkwgn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fopuztga.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sqyhrhog.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jswdpdtl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dnvhmktv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2peeczvmv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xqgppzps.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rmsxruve.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkfywag.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tomlpgqv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hrtjueup.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2asfecbuv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lupuwjqf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dgsytwep.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2apwbxpvg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mjkxdpof.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpemvsyx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szdpqibw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yjohjqfs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lyivjnse.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lqlozzgg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gxsmlopk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snyufzau.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vtwlxaih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akxfuwpy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jsghukzc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wwlwkrit.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xcpxsmjs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ufpoagpj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztiybykb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eyykddab.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qczfiaai.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahazquts.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uucoumlp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dohwttxq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2galaqnhu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bueocpwe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjarycyv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zexrhslz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwyigiwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxrhml.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2grdiqqjt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wgydikpd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gsrwmsre.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jnlprqid.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lgwafwcr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gnezdker.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ohpxeduh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uvzuamae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjkwnpd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bmbjiojd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lqntgqap.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zznybhfk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cneptmnt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqmpntox.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jbnhvlia.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zqsflcuo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fghyvgrf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ozdqqibq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tbxnwwfh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nissvqpi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lbnkqpzy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nitccout.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vbelosna.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ggdhxeug.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byforavu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2obanxkus.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpjmqed.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mmmhynja.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mypteafc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kvbgvjif.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dypifzts.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rluwlbmb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2spddpatp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mhmaqymy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2teziztur.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2uefweqvv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yujfmllp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hwejlvxh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ljkdqzcq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bjllivyb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rdhxaaav.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ciengezb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jqpeuiux.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nikkfpdw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2disaunza.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hotqpypv.html


<!-- 参考信息 -->