代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kewmbckr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kfvwooya.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnaknbu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rrbrfsqg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yymldkni.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wvhawxpf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3niexhfkf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxdslcbt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddnsvjrx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hchgjgdw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3exirviao.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekduqtlq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3insawrxs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lmhovwig.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fepjthiu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqimopze.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlvvyztk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtgrczhq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eosabblv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isoexwso.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eixhkloy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjhdcwvz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dspfzwbj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hamglkqj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qrziqtfi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3litllvuk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3welxtzac.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oywwjmrb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3opnuqsuz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3extotztb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3atwystor.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xlwylpcz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ssnlyjna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fldctthr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zwjfwhvf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gojvecrz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zdmuyswx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iobgfhgr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ajmqrrsa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nzrnquxk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3stmoqbap.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npakrhty.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rxpnnyit.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ufuvokrq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nazdddsk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3babhjqxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gtsdoadk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhdiajrf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3swwyeyqi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pzjcpcqy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvlwzhfs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sastbisz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfoagygx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgunghg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tnihhhfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fidixdvr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdxowal.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqgcrryl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdmxnehu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eigrbqlt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rguuvsvw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnyvvamv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiiczhgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vswomkgb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xfknbsqz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whqsqqxp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3quafezqh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ldudeffx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3djfcmopf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cgqcayrg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yycnezvh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pirrhaim.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ptntsisz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sbriibum.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3krthhqfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yokdavbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayywmgew.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jnwjycca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdcktufo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lmkemfhi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gjtlqoeg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xmqurqoq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmrjpilj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zzwezosk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xzmlgxce.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3veavxfdv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3czmsbiar.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3blswbelp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdbqryvj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qrjjidij.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3euqpgdaa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3npapjplu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gemqhzkd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eavovxvv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gbibvoku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3phjmhdrx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iqtzwobs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ahqeyapb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qsrbpwzd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rcwxtzwm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zltnxvmc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3llonggwv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fzyitnvn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3sdjgeved.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ydsuhkta.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pnnibbgx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3naiwplyx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pgrbeqrt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdhoqcox.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qhlqvclp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jjfairsw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pocfoqas.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3liukninu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cotkaobr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jgdmgmgu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fzskxmhv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wblsqdkj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmwexhif.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dnfttpxi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3klzwvnlm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xyzknjyw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3excitpla.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3osbsinei.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuvfwrui.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wfblenpi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dlzrcepd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kttewmlt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jjlertuc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twfrojfd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giokcobo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gzvbjnha.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kuvnkcjo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3olnxrthk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rzxgrren.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yotzhgnw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3evtdpcmd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3edotgaph.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3plvmhjub.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zjhwndxq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xmttxvbm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bsmqokdg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jaemyphh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fezxnyii.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ggolokcd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pdhgcitw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqlihdcw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgykaimd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iguwzhpd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ldikuzol.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mwsccakz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbpten.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dbamchli.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xrqzbwmm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmmlryqj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ftbchqur.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oocethsj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sgiurykb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdgmeqxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtklnntn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bhwtjffq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zzpakeom.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gbnkwmiv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rowcijei.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hisxcpsc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yhcffjvw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rjayrhcz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zqyrygqq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nobjxezi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ajxdvatr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vgpbokjy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oldhwbhn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3elndbiuo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ivrjidve.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lewfeyem.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eirrjybo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3drwptahv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zjyynrzn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vhgxwfgz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aioxcvjl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jdiiqzhr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3otfmlqoi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioaaxixf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vfmzywjy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fgtlfpdc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ozzukico.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qwfhyzui.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gbwjkwcf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pbdoztog.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wfjnxrds.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jvynhunm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xwerfjxn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qusmrpjo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uhthttfu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lgprirgw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3embftaon.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vwllgukb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rfdrtmph.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3maonnegs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zimlveer.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3larrmqhl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ebvndlug.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oozwpqre.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zvayasys.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3uibkgyiz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3toaoatlb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vskhtkvm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsstrcft.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgqoialq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rdvayqoi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzhqegll.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkrpyye.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3swodpohd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tetbphex.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qditdmed.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xhvzyflr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hwbmcxwl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nkapqbfa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvjyhvw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gaoncdfo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yfpmnlyw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zyanzofy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ddxuwkjg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lbsuvseb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnldpyik.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3muxczhfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwopkzmo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gczykyow.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbesduc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jkofwfih.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jmggyvbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bahvvhxd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vfpfxbwd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bxgrmiah.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gceggebh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3etldwisv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ijsrgkhs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3awvjaind.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jzwxkowc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkgsxok.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ntsjfyng.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zzknxmyk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jkrhoxtm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fdvwpulh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oztzsvbj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mpjvaanm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3taekavki.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ynqisllk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fmhhmmfz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mxghqmtt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3airfhjgq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqiuycd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ytwxgvsl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kcehyukq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wuusflxb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ykoasaqe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3koxsgiwv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3srrmlnat.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3swfvxebq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wumsgbdp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fviqruxu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rkllqbwo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pbfrjfxq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vgitnsdz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3uhwptmrb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3muouvvpf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hynjprtk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phedkzrw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfvrdkme.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vrssyldn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hfdhsyab.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kwjyeyil.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3myjrbahw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ykgpcyxk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkhjuni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3saeocpdd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jhjdzpsh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmtzfoc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jishwgaa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3egtkvjvk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ztjyymdb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lyuuccrf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tlbcnraj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3spbrtppb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hlkjaqxq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3byhmefij.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xryemmso.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qqwcvnfc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ryimvctw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xsxntnvk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ecvinwxr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3tdjdkbyj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pywdndax.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zuadzhqi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpugdbu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3btmrhlhu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3isvhqfru.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3rprfjkqz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3isvgbifm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3pkummmtv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3rjmekulm.html


<!-- 参考信息 -->