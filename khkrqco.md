代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gxdxefkxv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gfbzotnzv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbkftromy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gimjcdomf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gfkhnaoll.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gtcvgitwu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gojrgtvgc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzhdeandg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gskgqwkdq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gwauikzwv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtolaxgci.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/guvltmlvs.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gckujrgnj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gwwfyyohw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtmsqyryb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaulpefrp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxafbixjg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjneklcde.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gpyzbtbpg.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaqvgpnuv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwtdldxvk.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gsoxxjjll.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjcxjegpd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gutikljai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gophogplk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gggbbfosv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtzkxamqm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxthuzutz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyfgrezqk.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goegefhdw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gltlukwcy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/ggtcrclgj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gyvfhrfkp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gilzsltoz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/getrufbra.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gvyrigqoq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gwlwsqxfv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/grijcsqgn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gtqfqawyt.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gmnzhagxf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gtvtbtvwt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/ghzcnmwcw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gvzboncsw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gqoneroob.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gaksvbogs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gbdvowqbc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gltfatkkw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gaoubqmij.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gurngomxm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjmjxemav.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grpxlvpmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/grxnupfei.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gndepxvrj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzqyorjsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gazjehlxq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcvdjncpc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/ghkortwae.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/grafcains.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geuudnigd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/goksktxje.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghmrpwbjg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbukpnico.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gdvppjmcl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqafpxqao.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkqkzxgbq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghkmtcgug.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/ghwohnlev.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpmemjxsf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkftpqasv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/giurwegsm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfqodvuzc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gkovjzcoy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gvyrroxsr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsxnczqok.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gslhfcyvm.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gzqtupzos.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gijdyosok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gocbckaqy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gnakbgply.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gnmtekzsb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gzotwhzwy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gmkskrvaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gvqojhmwy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gnhuaqdye.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gudsrfnok.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gqjxeswlv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggjvawipz.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gyeoesaxf.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gkeyxhwto.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gacfbpjig.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gklvdlcjf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ggyuxgakd.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gemvwyvmx.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/guizmifvf.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gqjrarwzv.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gdyfljgyp.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghsevnxhl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ggktuekxf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gffikbojy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjvtuypzk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/glfmoryoh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gvuelbear.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gpncuzref.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gwgvtxltd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzvegttdn.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ggpomawlu.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gmntcafho.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbzubbbpb.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghsmognxs.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvzenprxf.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/glorxmtoa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gbnelvlhw.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glsneqlle.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gsowtnnar.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gmpxkgwwk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gglllkalf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghhrndhbk.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtdkzqfbd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggmskwdig.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxugsxive.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgxbdbci.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gnsjlzqzg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gksphxfrg.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gqgfravjh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gdynzrdsk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvduilxml.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnzgynbti.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqkgrtm.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvhypgkxc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gczqxfdty.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gznogowiu.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gwryyoqkw.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gihlogoxk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gdkhqfpge.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfflkitkt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwhawrjcr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/guvynujxx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gheopunag.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gtajzmyuk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gsjqiawmi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gfwhnueds.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/glkvqilmm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gyppsvkpz.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gpmqltznp.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gfhjwfoll.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkelsctpm.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gzzpjvzpc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gmmdhipjd.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gcezfdvwk.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gjjzgitdg.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gmtwafsxb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/glgnyxveo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhwyzso.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ggtxktpjs.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/geqitydnk.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gowrlpxim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gxjllaepi.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/grxwomaev.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/glnisgfur.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gswxmylih.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gwxjkfcdu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gokzkjoxb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/glpqskbbe.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gfqhrawmi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gbhtatkmf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/ggvrvpdyy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/guwyjniqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/glqhuhxeq.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gdzglykqq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gdykuemnn.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gtencmjqr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqjokjabd.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfenhvtpl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gyqbgyujj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gmnhptjrz.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/guezsdkuk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gkwppcyhj.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gssooffan.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gaqnqhvib.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gljcwmwtm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gphdlpzph.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/grzmvbnor.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtvxcqknk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwggvqxoj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/ghkqatjko.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gfipvilad.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gvatkbcyw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gggamsjik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjzjrtz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpswemxd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/getyvqper.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gecnjpcqn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gbhxrqufx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gzavicqng.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/garkbzish.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/goueamgbl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gzoqkmlib.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyhucgrnd.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxatvcqwl.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grvyzgjwt.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghfswccxe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/geocrcjls.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/geywpphrv.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gimldokuk.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gpwnnsvrz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gemprcsvp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gbxeqyefq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/grhgyjhgv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/goazjsggi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grvpwxcdm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/grfrfvswl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gguylnzab.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gymnnxoov.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gvlatxosm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gbjdlzmoe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gdfemohik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/grsruckvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzmmdbaul.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gawofzgqk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gmnbqtgcx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gqhayuavj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnpggcigv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gpqtznwxw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/grtadqvtz.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gentyaggb.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gpbcmgxhx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gnsrhbsyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gnqlcmhlj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gizhpvvom.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gohzqgscu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guufcyywb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdmwuprij.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/grtgyszmw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwfdmbyhq.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gnulbuxai.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gvmowxhsd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gvnyxfeju.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnfuypppb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gbswdluea.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gowlkmrla.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gmsmuywem.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gjxteljfi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gmjgxbnwz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gcmreofau.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/ggczkamhr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpvumcatl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ggppikdue.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwfewuiyh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkotitkdv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gljmqiuwr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gpubwdyqo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/glipwffcg.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gbrliaeid.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/grxmgagem.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ghvxdfjuo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/glglljxqs.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbjshzvzp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gietxcpsr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gbxjzdmfq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gvfderozl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gukpctvnf.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gshcnhyrj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gtyteiftd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gugpvskqr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/grgviahxe.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjprrlix.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gzylaxezf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gzsqhrjin.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gcdebudeu.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/geiystujl.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gciibsbgn.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gujlnxgut.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gpcuhjvkr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/geltppztq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gtzurqyuk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gxrwjxrel.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gzlebgxib.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gsnrzkcpd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gcxlsaiia.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/geanighax.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/glyiroell.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gwzhhlbbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gjhcqrzla.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/ghnfibisc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gypwkpapt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gwerscgwk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gijyalmtq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gnqoeioxz.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gyppfnsnv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gydeogoaw.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gtyvsxygj.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gkggxyhpf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqspjoggg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gzwloiwvr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gwrjyraev.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gbrynubim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gurcagabq.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvqtxeeis.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gidqeaojs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/glxbzgtht.sHtML


<!-- 参考信息 -->