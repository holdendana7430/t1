代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vm.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hm.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pg.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mb.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bb.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tu.haigaiapp.cn

Ruby: s.capitalize
来源：http://cw.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jg.gzmigu.cn

[E18] 模板占位符替换
来源：http://kh.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://js.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wf.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dm.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fj.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gg.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://us.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zo.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xc.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://vw.muxihuayi.cn

Py:   s.splitlines()
来源：http://vk.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://me.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://zi.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://gv.wgjwhj.cn

Java: s.lines().toList()
来源：http://ld.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://qp.521024.cn

Ruby: s.lines
来源：http://tt.nszjky.cn

C#:   s.Split('\n')
来源：http://hh.colortex.cn

[E20] 判断字符串是否为空
来源：http://dw.panjiajie.cn

Py:   if not s:
来源：http://qm.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wv.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tp.bjjhwx.cn

TS:   if (s === "") {}
来源：http://jc.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://ey.gzmigu.cn

Go:   if s == "" {}
来源：http://pg.muxihuayi.cn

Ruby: if s.empty?
来源：http://ds.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vu.hahajie.cn

[E21] 超长截断加省略号
来源：http://zt.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sa.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nt.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rg.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ei.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ya.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://kn.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hw.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iu.521024.cn

[E22] 字节长度与字符长度
来源：http://kt.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hc.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lm.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gz.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yu.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bb.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://is.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://ow.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cc.huixinmuqiang.cn

================================================================================
来源：http://vq.huanxung.cn

F. 文件与目录
来源：http://eu.huixiangedu.cn

================================================================================
来源：http://nk.hahajie.cn

[F01] 读取整个文件
来源：http://fj.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ba.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ia.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ay.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fj.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zp.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uf.asd995.cn

Ruby: File.read("a.txt")
来源：http://on.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://hd.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ae.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gm.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jg.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rm.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gs.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wm.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tb.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qr.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jk.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://sh.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ga.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yd.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://us.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dz.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://en.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mg.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://wn.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zi.bjjhwx.cn

[F04] 追加写入文件
来源：http://tj.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eo.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fm.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tw.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yl.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ml.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kc.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ot.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wg.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://sb.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vy.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://da.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://ka.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://qv.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gf.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pt.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://mh.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://fm.yuexingan06.cn

[F06] 删除文件
来源：http://to.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://hv.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://an.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vk.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rz.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sf.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://ki.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://xb.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://qw.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://rm.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ek.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://db.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tu.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://te.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zu.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mc.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bq.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lt.haigaiapp.cn

[F08] 遍历目录
来源：http://rw.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ob.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://et.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://os.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://yx.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nr.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cz.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://ez.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://lg.bookmarksfly.cn

[F09] 获取文件大小
来源：http://ah.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://jd.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://rr.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://kh.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://fh.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ot.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kg.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://am.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://pn.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://mo.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ds.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pr.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ch.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://ab.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hh.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ew.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cr.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fe.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://nr.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nu.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ut.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vp.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ok.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ww.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uw.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tg.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xc.colortex.cn

[F12] CSV 读写
来源：http://el.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yu.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pi.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pd.colortex.cn

TS:   // 同上
来源：http://sl.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ip.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zy.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iz.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sk.wgjwhj.cn

================================================================================
来源：http://gs.shtwfgs.cn

G. 面向对象
来源：http://hr.asd995.cn

================================================================================
来源：http://jq.shxzskj.cn

[G01] 定义类
来源：http://dw.yuntaijiaju.cn

Py:   class User: pass
来源：http://vr.yuntaijiaju.cn

PHP:  class User {}
来源：http://iw.jctech888.com.cn

JS:   class User {}
来源：http://rz.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://md.hnjuh.cn

Java: class User {}
来源：http://lz.huanxung.cn

Go:   type User struct { Name string }
来源：http://qw.colortex.cn

Ruby: class User; end
来源：http://jo.nicolike.cn

C#:   class User {}
来源：http://va.bjjhwx.cn

[G02] 构造函数
来源：http://as.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://xw.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://ff.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ic.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://xi.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://kx.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xr.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://nz.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://vn.lnxyls.cn

[G03] 实例属性
来源：http://uz.521024.cn

Py:   self.name = "x"
来源：http://nw.colortex.cn

PHP:  public string $name = "x";
来源：http://wz.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://oz.newstarts.cn

TS:   name: string = "x";
来源：http://yq.shxzskj.cn

Java: private String name;
来源：http://es.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gv.hnjuh.cn

Ruby: @name = "x"
来源：http://hc.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://ld.jctech888.com.cn

[G04] 定义方法
来源：http://vc.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://og.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ij.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://rz.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://pt.muxihuayi.cn

Java: String greet() { return name; }
来源：http://wa.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pq.lnxyls.cn

Ruby: def greet; @name; end
来源：http://ko.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://yq.bookmarksfly.cn

[G05] 继承
来源：http://nr.szxytkj.cn

Py:   class Admin(User): pass
来源：http://xv.asd995.cn

PHP:  class Admin extends User {}
来源：http://xq.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ys.shxzskj.cn

TS:   class Admin extends User {}
来源：http://bt.haigaiapp.cn

Java: class Admin extends User {}
来源：http://xh.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vc.asd995.cn

Ruby: class Admin < User; end
来源：http://gj.hahajie.cn

C#:   class Admin : User {}
来源：http://ar.panjiajie.cn

[G06] 重写方法
来源：http://cc.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://pv.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bj.colortex.cn

JS:   greet() { return "admin"; }
来源：http://rs.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ve.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://eo.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://na.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://wi.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://rl.muxihuayi.cn

[G07] 调用父类方法
来源：http://ee.huanxung.cn

Py:   super().greet()
来源：http://qv.chemitech.net.cn

PHP:  parent::greet();
来源：http://vv.nszjky.cn

JS:   super.greet();
来源：http://ul.shxzukj.cn

TS:   super.greet();
来源：http://dl.wgjwhj.cn

Java: super.greet();
来源：http://yo.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pw.hnjuh.cn

Ruby: super
来源：http://lz.521024.cn

C#:   base.Greet();
来源：http://bp.9csxet.cn

[G08] 静态方法与属性
来源：http://ua.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sv.wgjwhj.cn

PHP:  public static function f() {}
来源：http://wg.shtwfgs.cn

JS:   static f() {}
来源：http://sg.jctech888.com.cn

TS:   static f(): void {}
来源：http://ma.yuexingan06.cn

Java: static void f() {}
来源：http://db.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vu.huanxung.cn

Ruby: def self.f; end
来源：http://di.chemitech.net.cn

C#:   public static void F() {}
来源：http://as.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://mm.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://nm.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dd.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uw.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://cu.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://ay.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://qx.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ab.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://pk.szxytkj.cn

[G10] 访问控制
来源：http://cb.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hx.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://bf.huanxung.cn

JS:   #private 字段；其余公开
来源：http://dm.huixiangedu.cn

TS:   public / protected / private
来源：http://vv.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://yo.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tk.gzmigu.cn

Ruby: public / protected / private
来源：http://nz.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://aj.huixiangedu.cn

[G11] getter / setter
来源：http://cs.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://ro.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ab.szsharing.cn

JS:   get name() { return this._name; }
来源：http://de.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://ou.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://ym.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://py.hnjuh.cn

Ruby: attr_accessor :name
来源：http://gm.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://xv.bjjhwx.cn

[G12] 对象转字符串
来源：http://gs.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://ao.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://at.hahajie.cn

JS:   toString() { return this.name; }
来源：http://aw.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://od.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://vh.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sf.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://mg.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://fa.bjjhwx.cn

[G13] 判断对象类型
来源：http://yc.asd995.cn

Py:   isinstance(u, User)
来源：http://tk.haigaiapp.cn

PHP:  $u instanceof User
来源：http://pp.9csxet.cn

JS:   u instanceof User
来源：http://cn.bjjhwx.cn

TS:   u instanceof User
来源：http://wg.yuntaijiaju.cn

Java: u instanceof User
来源：http://iu.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://au.nszjky.cn

Ruby: u.is_a?(User)
来源：http://qt.huixinmuqiang.cn

C#:   u is User
来源：http://qy.bjjhwx.cn

[G14] 数据类 / record
来源：http://uz.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zk.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://at.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yn.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://uz.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://yx.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://mk.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ti.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ld.shtwfgs.cn

[G15] 枚举
来源：http://hg.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bm.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bt.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dn.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jn.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://og.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zq.asd995.cn


<!-- 参考信息 -->