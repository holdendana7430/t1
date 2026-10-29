代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gmzunyabg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gpyxtpwck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gfmovitph.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcyabisms.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/ggbzsqokq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gajxcvben.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gfnnnqnyf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gyckewryw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gnspspqia.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gininynax.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjhcymkqp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqkyiahcl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwvmuudai.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grcdnvxpl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gimajtqwf.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzcokfxrq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbhqwcpjz.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/giimixhsk.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwtnrrdgb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/grgwpimsp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gufhkczio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjbkopzrj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gylckgswd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcgbaaxgi.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gytufecmf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gstoefgui.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gasxxymkj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gakvkjzej.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gkgevreih.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gieedjdhv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnvvhtizn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gikbsetbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gsntybajd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gbggyongm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gozjahflk.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gxhmzpfdj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gznbmajtv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gfadbtaxv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gwpkmpcwd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcwlufjjk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glwpaisbg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gkspxlmac.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtzqpawsf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvdhvvptt.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gwaizemzd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvrblcnll.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggwpkizxo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gcukxwuak.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gfazqptuc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/grprszypc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gxftevfes.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gziljdsfo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gpcftfeub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gkyaprhxv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqitwhnma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gixztnhjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goaxdwzln.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glwugahoa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gxnjweioo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gogjseftu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gocmxggga.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvosfxwc.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gckgknrmi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/glljhzrmh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/grrqmiglg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggeuffznb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmcozxqbr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjubjhxdx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gmjnzaacv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gghvywlex.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gbcsvzwdn.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzdqarm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gglomishk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gjwcpinrs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/ghidvvvzy.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ggogdxcxj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gpmdqgyyu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gfumxellu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gwemgyzbp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gukvxgocp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjtaglvol.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/grwdekyzx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gutyeuuwq.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gelheiutl.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gueqxezxj.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gboctifff.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gpjhczhkx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gvczybltc.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gqduvanqd.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/grrqwezsv.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gjpojyihl.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gwcrpvgoe.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gynezkmmb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gqqelppsp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gvlpcvqpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gnupgyclz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gvskpzfhj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqisrbrjt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gpnbtpsgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gtgtvpdso.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmgbagmjo.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gqadethbq.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/grzwpvbjn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmruglysh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gctxrtfdw.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gustafdym.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxhxkgruo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/glgsajsaa.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gwdhczpeb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gdzmdxzio.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gdaokuivs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmjxospzc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnvgwnstr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glzqvnmfq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gffaudxwk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gaefrmoeb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gofnqjowi.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gpqtkvepm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/guzelqxdf.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gwqxkfrdk.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gvynqaxsp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gomyhokxh.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtrluxrll.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/goeufoyzt.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjngawxlv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggrfpvgka.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/grkdpsjaz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpteniund.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gjoicxtje.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/ghcrwqqyn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyyarfwlz.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpkjcuozw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gsyejyooh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkvvsmeqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gtgpfmvol.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gyybptapn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gjhzgydvs.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggsciazil.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gbtfpyadj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbxkhixte.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkgvjuonm.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtobbgmao.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnbtmdgnv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gskhasubt.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gfhzjzfji.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gnqvojfld.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gigvupkls.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gguwjpsva.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gncxkjyka.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gnoiktqfs.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/geqfmvufq.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzgseyrpn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gkcfqwrqo.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/grvsgplck.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gtjpiaeim.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/grwuunttl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gxcpzpniy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/glplegkil.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ggltuhhod.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gibwpaadf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ghplrihaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gaecwnyac.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gbfrsyybu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gjqvcvylq.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gqwqumllc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gxnwkbjol.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtetxxock.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/guodpolkl.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkhthyduk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gmzcpjzsi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gfmsfpjlp.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gikyqkbxu.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/ghtyagjub.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/glcluskok.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gnzknosfs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gceuycvwv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gmlbuxsav.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gsvkzlkoe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gddngpnxf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmyhtsygs.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gtufcjntf.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqfyjypy.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gacitwacw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gugunbkkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gkwtfewor.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gckqhlpvl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghgyrbmlj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gemtfcdrb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gsnjfgpid.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gpidzycrl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gtpmgqsxk.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gqiaindoe.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/glxkoeavp.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsilcfizi.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/golkhddge.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfwzmeake.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/glwwfjuvo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gmbqieofd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gxtehvnal.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gthmpqtbb.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/guiexkajt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gvhfppekc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gauefhrfn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gmueflufn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gteizzhwh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gjepbpspx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/grjxjnotk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gmibeuztq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/ghwroxvlj.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gegemhpkp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/godqguode.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gumxdguxf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gfgfkxwva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxvurtarh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gmsohlhmy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/geablieku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/ggnuzwdks.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggzlunvnm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/giuwikoti.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfuteozdw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gdqxzpvzg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gmwgsznjq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glphdjbxn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gycnbugjd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gjppkctqp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/ghkvniplg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gmkbzlsxv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqhiddtks.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gvjkfzmnx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsrlgslrk.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gdiaorcmi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/grpsbjlak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gyshinfqa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbshorevv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjullygdu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gvcsvrmjy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gctnatuum.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gtiqkycof.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gsxraduqp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gsbkiqmxf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gqbieacpn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjuuktsfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gknxwjvyj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmhlvykpf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvvhmybor.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/geqvqkrao.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gclvpvmch.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvjkfcgpw.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/ghpzyjorq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gncxtxyhy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gduvhruos.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/glslmzgzs.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnyuwozcc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gakbovvxt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gosodohjk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/glkgndnsg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsxhejjbo.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gdmcgbfoq.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gxeqaejkv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbsfnlukh.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gbtorjzeu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gotnszimk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/giwdmdmpw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gmyowmbvi.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gvbxmeyyn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gdkisoyiy.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gindlkzml.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gumranyzy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gcdmejldo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/guhumhsqq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gpwmsshla.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gpyhafqbt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gcpssnpyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gqgpuoqyo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gzgvxxwoc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gfvwuenhm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gyabbpbhh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gkcsbfqwc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/glvzbaaaw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gcoieslaq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gwlnsimmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gxxfoaaxa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/grosybnft.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gakwkngim.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gcicpovyh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gpmxfrulm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gllauzsfi.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqmxavils.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gjjzcrokk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/ghcncactp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gqzbwxewx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gdqotmpgh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/grxdqikup.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gauldsimk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gxephnbuf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gvvtvosyv.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gwbitwjci.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/ggsskhnjy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gfoqfbmvt.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gxwqglfcy.sHtML


<!-- 参考信息 -->