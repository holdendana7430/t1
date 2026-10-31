代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hj.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uo.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lx.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pv.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ne.huanxung.cn

[E19] 多行文本按行拆分
来源：http://xu.hnjuh.cn

Py:   s.splitlines()
来源：http://ra.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ee.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://xv.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://zj.asd995.cn

Java: s.lines().toList()
来源：http://hk.521024.cn

Go:   strings.Split(s, "\n")
来源：http://ey.huixiangedu.cn

Ruby: s.lines
来源：http://ci.szsharing.cn

C#:   s.Split('\n')
来源：http://vx.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://po.colortex.cn

Py:   if not s:
来源：http://gv.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xw.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ti.hnjuh.cn

TS:   if (s === "") {}
来源：http://at.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ah.nicolike.cn

Go:   if s == "" {}
来源：http://oy.huixiangedu.cn

Ruby: if s.empty?
来源：http://jv.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xp.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://sz.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tl.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yw.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ex.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jc.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wp.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://vt.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mr.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ft.newstarts.cn

[E22] 字节长度与字符长度
来源：http://xn.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qf.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fm.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xb.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gc.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ca.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sj.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://sr.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kj.gzmigu.cn

================================================================================
来源：http://jm.newstarts.cn

F. 文件与目录
来源：http://rh.asd995.cn

================================================================================
来源：http://zl.asd995.cn

[F01] 读取整个文件
来源：http://ed.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ts.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://qc.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pe.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ej.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fj.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aw.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://oa.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://fg.shxzskj.cn

[F02] 逐行读取文件
来源：http://dg.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nk.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gr.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lr.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zh.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xc.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gl.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nh.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dt.521024.cn

[F03] 写入文件（覆盖）
来源：http://io.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jc.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yr.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ny.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ur.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jy.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qt.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://tb.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fm.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://jg.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pl.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sr.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rd.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ik.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pd.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wi.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://li.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ao.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sb.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://mh.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://tl.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://bs.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yd.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ea.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://rv.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://hg.bjjhwx.cn

[F06] 删除文件
来源：http://yn.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://bm.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://az.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vu.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bi.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iq.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ow.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://fw.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://am.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://br.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ml.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jw.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nz.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ez.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vy.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qi.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bq.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mc.nicolike.cn

[F08] 遍历目录
来源：http://eu.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ok.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eq.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://dk.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://ui.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xz.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kr.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://nn.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://sx.gzmigu.cn

[F09] 获取文件大小
来源：http://rf.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://os.colortex.cn

PHP:  filesize("a.txt");
来源：http://to.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://ut.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://sa.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hx.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fa.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ao.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ff.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://jf.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qx.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ey.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wm.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://es.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gr.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ek.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gw.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qd.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://dd.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://on.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cx.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://is.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bw.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ak.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tn.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sx.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zd.nicolike.cn

[F12] CSV 读写
来源：http://wf.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vy.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://js.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fl.huanxung.cn

TS:   // 同上
来源：http://at.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wa.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://in.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oh.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xp.newstarts.cn

================================================================================
来源：http://pd.shtwfgs.cn

G. 面向对象
来源：http://cg.nszjky.cn

================================================================================
来源：http://jg.haigaiapp.cn

[G01] 定义类
来源：http://qq.szsharing.cn

Py:   class User: pass
来源：http://wi.yuntaijiaju.cn

PHP:  class User {}
来源：http://ca.asd995.cn

JS:   class User {}
来源：http://fg.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://on.wgjwhj.cn

Java: class User {}
来源：http://qu.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://ek.shxzukj.cn

Ruby: class User; end
来源：http://ti.wgjwhj.cn

C#:   class User {}
来源：http://fs.huixinmuqiang.cn

[G02] 构造函数
来源：http://mh.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://dw.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://og.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://po.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ax.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ca.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://yp.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://lr.hahajie.cn

[G03] 实例属性
来源：http://jv.9csxet.cn

Py:   self.name = "x"
来源：http://ny.nicolike.cn

PHP:  public string $name = "x";
来源：http://dp.nicolike.cn

JS:   this.name = "x";
来源：http://wz.colortex.cn

TS:   name: string = "x";
来源：http://bm.chemitech.net.cn

Java: private String name;
来源：http://gz.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mw.haigaiapp.cn

Ruby: @name = "x"
来源：http://ly.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://ge.huixiangedu.cn

[G04] 定义方法
来源：http://gj.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://tq.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qr.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://ds.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://rp.asd995.cn

Java: String greet() { return name; }
来源：http://lf.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cw.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://rv.521024.cn

C#:   public string Greet() => Name;
来源：http://ne.shxzskj.cn

[G05] 继承
来源：http://ty.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://zv.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://rk.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ml.521024.cn

TS:   class Admin extends User {}
来源：http://av.hnjuh.cn

Java: class Admin extends User {}
来源：http://nz.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cz.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ze.yuexingan06.cn

C#:   class Admin : User {}
来源：http://mg.nszjky.cn

[G06] 重写方法
来源：http://ab.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://lt.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sf.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ia.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://fs.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://cg.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pk.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://xi.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://pl.muxihuayi.cn

[G07] 调用父类方法
来源：http://ci.yuexingan06.cn

Py:   super().greet()
来源：http://ey.yuexingan06.cn

PHP:  parent::greet();
来源：http://qt.huanxung.cn

JS:   super.greet();
来源：http://ox.muxihuayi.cn

TS:   super.greet();
来源：http://hl.szsharing.cn

Java: super.greet();
来源：http://gs.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vg.colortex.cn

Ruby: super
来源：http://qk.newstarts.cn

C#:   base.Greet();
来源：http://rm.haigaiapp.cn

[G08] 静态方法与属性
来源：http://cv.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ru.hahajie.cn

PHP:  public static function f() {}
来源：http://hc.asd995.cn

JS:   static f() {}
来源：http://li.yuexingan06.cn

TS:   static f(): void {}
来源：http://rw.huixinmuqiang.cn

Java: static void f() {}
来源：http://qn.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://su.wgjwhj.cn

Ruby: def self.f; end
来源：http://yo.bookmarksfly.cn

C#:   public static void F() {}
来源：http://xk.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ie.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://sb.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://au.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gi.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://li.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://of.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://yg.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ey.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://qi.newstarts.cn

[G10] 访问控制
来源：http://zd.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://ln.newstarts.cn

PHP:  public / protected / private
来源：http://xo.521024.cn

JS:   #private 字段；其余公开
来源：http://kq.shxzukj.cn

TS:   public / protected / private
来源：http://kz.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://lz.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://ky.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://jp.newstarts.cn

[G11] getter / setter
来源：http://js.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://ie.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dm.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://co.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://ac.colortex.cn

Java: public String getName() { return name; }
来源：http://wq.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vb.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://qu.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://iv.haigaiapp.cn

[G12] 对象转字符串
来源：http://oz.521024.cn

Py:   def __str__(self): return self.name
来源：http://ny.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ie.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://bq.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ei.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://bf.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ao.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://pi.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://gr.newstarts.cn

[G13] 判断对象类型
来源：http://kx.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://cv.bjjhwx.cn

PHP:  $u instanceof User
来源：http://wl.jctech888.com.cn

JS:   u instanceof User
来源：http://zk.shxzskj.cn

TS:   u instanceof User
来源：http://ci.jianghongdianzi.cn

Java: u instanceof User
来源：http://gk.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xq.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://pn.hahajie.cn

C#:   u is User
来源：http://rg.chemitech.net.cn

[G14] 数据类 / record
来源：http://tq.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bh.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://vj.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://it.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://fr.newstarts.cn

Java: record User(String name, int age) {}
来源：http://ur.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://kv.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ay.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://ia.huixinmuqiang.cn

[G15] 枚举
来源：http://yy.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rg.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zq.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bj.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mr.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://vx.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oo.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://bw.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rc.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://zf.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fw.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ve.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://zn.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ly.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qd.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kf.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://gm.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://ba.shxzukj.cn

================================================================================
来源：http://lr.szxytkj.cn


<!-- 参考信息 -->