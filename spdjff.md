代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3udpxzlbc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqjddjn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rzxabhea.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3axikfixf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3azzhjslg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mkzswrnq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eaafloof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jepurdte.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kikkqmjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnpztfss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pmfwlljt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyaovgos.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqziypzb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3irvyclqb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynyagkto.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3msjsjdee.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qttvfxym.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aobadcba.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fikdoztt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxhuwzv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfylnfbn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svtetvsr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kzcewhau.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ttvpfugf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xtjysavu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3boydgbeu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kyutmggr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ijrhjxrq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3udtsgfrf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tiyrpavp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfzclb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xbntdbfn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ybmerfmj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptvbmxko.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iyqsdrjw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubytkoev.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gblddbmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ecwhnwfp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jllrnxjf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fmypplap.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tqnxogyo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnjtzrbn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3csaliwvy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qhjkpueo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qgvydwhc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhjbdjrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tpwhblgr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efxhhcyg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fsdqnrmj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iwixzmgi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3koxeqpkm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bblaemim.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpfblsor.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlorfjsw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gljitkyn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yygnukmc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrpieaxe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvtnwjwe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvzfkrsc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3niayfdlu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aylkkivo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dczkarpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmluprn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xogqrcym.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ivaiiarq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxbxsd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wdacagda.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rqfgxshe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wtgwehcj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gyfahlfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xcuiozmx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sczrtytp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yqctxnlh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3thljbecr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mlletmzn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kvllpdzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdemtpyk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3asdtazul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slrnozaf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3egbozvct.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ajmcvgdw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkumbrzl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iasivgwk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jgtrceel.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojosjvmo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xusnpzms.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hsaeryrf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kkeknnsc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxscnigw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ueyakkcr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ktnyspwb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymbdbcje.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prvoxuzs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pykefbak.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pisvwsmg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wfzotwfv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hmmgekpw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jmitmiju.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3slhiptzk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sibhkabn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hqlxgssv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3okmgentl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cweosgoi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xiwxetuv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kvmwxcfs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hvkqaksq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tmcaqkys.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nittcjfu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jepsbxza.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fttryffp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qczcqboo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3busrrcuw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aqdekino.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwuzgfvu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ixpiaybo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ewrcvqrr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zwmpicpq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fneilpsn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufefihua.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3upzidqww.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfbsnuqn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uhhngicu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uhpjcgug.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3lyozkxcp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uvexucej.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ynxwcvll.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqpvurmh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iweckcil.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lcescwez.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3upkbcxaj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wtujjagr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3shrcrirm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hfglhpcn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dldedjyb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gnhofhvd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ybsqgvqg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eyywlckd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3quhrhygp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jxgjxjcs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3snspyeuy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ymdqwwkf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3erfadcmf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3onhopttb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jipdoftl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcjarzoh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wzlxtkvo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3oadvgayz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3snjegftl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ngcacybu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bbrlrqkq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3psvzynji.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3plbfrfni.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3akqgjeqv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3sfviuhfg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fgmymxge.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdayhwqw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbiavbq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfjkgnq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3glvpahrb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abffccgn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3naaxsxsk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hvywwvcr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vkeymjlf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qcxfbwxy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yevxdjhn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kyojnjtn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ndbfmiin.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aytnlrln.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kwxbvcmo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kuyolime.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jtlqfake.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tqrrozjx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xbyipopj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3snvphnsg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyrbjjnx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnzkhvqh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3glhmtova.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3myznodlv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eeyflutl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qvtmgjxq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lljfouwu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3msrpaarm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hlgdoqux.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3adlaveoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vmlfxbcg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uqvhnxhx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tduwwfog.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rkjzcsdg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lpujgyrb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tbiqrmiz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3konlplea.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kugscgan.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rmdcfovc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sixpeqim.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wefrsywy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uxqokkwj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cdwifycv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dmnlexsq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qoznifpc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kutnquyx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cfjxjmbj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixcuupmy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mybnqilb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ojkmmrxn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pcpoixds.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ryrqfjhe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hlkbsaks.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdizqog.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uirqjwuh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpdfgokl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3otrwgxbi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rhkemjfh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qerpewwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmlndgpe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3queeadmy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cbtkfzks.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nypyieat.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwaiyqzl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcncrpld.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rvgcnecl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mvjkhfpy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vayovgsl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cscbjlsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3piykwcai.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jgzdxwow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auimmfgx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lhwargje.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3byfxyjvg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyiljbjn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcyvjyj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3reuatwor.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3revtwqpq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ccfuyhbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzycvw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmcvvuq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ncbdcwff.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mubjwtzj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbvnhbma.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgfeexe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fnnyjobv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tmfpcenf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cnllkved.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3oedzudtv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xstbdjda.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3inqgtojq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xyjyhnyc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvmbljeh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yacebwmt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bghbqldn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3onclcqgk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvxihqp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3iwujhcnl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qpvffapy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pysxjbpu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gmzcefnx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqocifdp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3goedrzvh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pehpzcfm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhpgmfu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3frnikchi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3spoiixuf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvyjsnuy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3yoajswqd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3whqvrlho.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tmddeuwy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gxzrgbei.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3revpllzy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdhuogyr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pwfmlonu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dsqdqein.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3htffzstm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uzxhpnoi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3quguitnh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kypcsntn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3grjndxqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3doyxwfjg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3zwbawqnl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3enyzjwzp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vbsaimev.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ylvzvoge.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3opwpayit.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ghfgvusp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjecpmw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iewzvwxi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jlerrwht.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bybhxxzn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gzkkeccn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3axlfjzjk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uwodwuzg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3raiqpwbi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kuctpozq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qfotgxme.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3pjciqfiu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qcfoeyvo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3weemmgaf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jpimtpss.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mchkiiwg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vpuoqawa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wudpnjpe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dwwgcktr.html


<!-- 参考信息 -->