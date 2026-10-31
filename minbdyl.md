代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ku.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yk.asd995.cn

Ruby: s.capitalize
来源：http://au.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ug.huanxung.cn

[E18] 模板占位符替换
来源：http://wd.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vh.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://as.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ty.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zf.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qb.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://li.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://un.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yw.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://fr.asd995.cn

Py:   s.splitlines()
来源：http://xd.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bh.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://zv.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://bn.huixiangedu.cn

Java: s.lines().toList()
来源：http://jf.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://xp.newstarts.cn

Ruby: s.lines
来源：http://za.wgjwhj.cn

C#:   s.Split('\n')
来源：http://nz.newstarts.cn

[E20] 判断字符串是否为空
来源：http://qm.szsharing.cn

Py:   if not s:
来源：http://hm.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gj.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mo.9csxet.cn

TS:   if (s === "") {}
来源：http://vg.521024.cn

Java: if (s.isEmpty()) {}
来源：http://zn.nicolike.cn

Go:   if s == "" {}
来源：http://hr.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://ft.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ht.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://jz.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yo.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fv.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tv.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ci.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fi.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ex.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ag.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qj.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://hk.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yr.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wj.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://au.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tg.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wr.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rr.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://db.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ym.shtwfgs.cn

================================================================================
来源：http://uh.jianghongdianzi.cn

F. 文件与目录
来源：http://au.gzmigu.cn

================================================================================
来源：http://hd.gzmigu.cn

[F01] 读取整个文件
来源：http://ol.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ag.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://xf.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sp.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wh.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fa.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jj.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://af.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://tx.9csxet.cn

[F02] 逐行读取文件
来源：http://mt.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ae.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rf.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ic.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://po.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kx.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fj.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tx.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dv.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://np.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ye.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vb.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://es.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vy.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uz.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cx.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://eo.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lf.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://rt.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xl.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pn.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wl.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xh.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yy.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vl.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ha.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kc.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://kh.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://py.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://cm.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://sa.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://pd.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mz.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rs.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://md.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://pe.asd995.cn

[F06] 删除文件
来源：http://me.colortex.cn

Py:   os.remove("a.txt")
来源：http://wr.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://fk.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dq.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uk.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lh.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://bb.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://kp.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ew.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ej.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vi.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rm.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yw.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://od.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aj.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tp.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://va.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mp.nicolike.cn

[F08] 遍历目录
来源：http://qb.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cy.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ou.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://jb.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://sw.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://la.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vt.nicolike.cn

Ruby: Dir.children("dir")
来源：http://uf.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://cn.panjiajie.cn

[F09] 获取文件大小
来源：http://qb.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://hy.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://wq.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://yy.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ye.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://az.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jf.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://wb.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hs.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://cm.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qi.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ol.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cm.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://cj.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ti.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sg.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yn.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qk.bjjhwx.cn

[F11] 复制与移动文件
来源：http://zl.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://me.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jz.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sn.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oy.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mn.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ir.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dz.gzmigu.cn

[F12] CSV 读写
来源：http://gt.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xr.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gg.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gk.huixinmuqiang.cn

TS:   // 同上
来源：http://te.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wa.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ws.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://re.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vs.huanxung.cn

================================================================================
来源：http://zw.jctech888.com.cn

G. 面向对象
来源：http://xk.huixinmuqiang.cn

================================================================================
来源：http://yv.colortex.cn

[G01] 定义类
来源：http://zd.chemitech.net.cn

Py:   class User: pass
来源：http://nv.jianghongdianzi.cn

PHP:  class User {}
来源：http://ri.shtwfgs.cn

JS:   class User {}
来源：http://tq.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://kq.szxytkj.cn

Java: class User {}
来源：http://tx.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://kt.yuexingan06.cn

Ruby: class User; end
来源：http://rn.shtwfgs.cn

C#:   class User {}
来源：http://ux.asd995.cn

[G02] 构造函数
来源：http://jb.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ou.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://oi.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://bo.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://wp.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://wk.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wh.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ey.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://sy.yuntaijiaju.cn

[G03] 实例属性
来源：http://iy.asd995.cn

Py:   self.name = "x"
来源：http://cz.9csxet.cn

PHP:  public string $name = "x";
来源：http://sw.colortex.cn

JS:   this.name = "x";
来源：http://gb.bookmarksfly.cn

TS:   name: string = "x";
来源：http://ov.shxzukj.cn

Java: private String name;
来源：http://ho.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tv.lnxyls.cn

Ruby: @name = "x"
来源：http://qi.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://mc.szxytkj.cn

[G04] 定义方法
来源：http://ps.szsharing.cn

Py:   def greet(self): return self.name
来源：http://ii.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ht.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://iz.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://rf.lnxyls.cn

Java: String greet() { return name; }
来源：http://pd.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zw.lnxyls.cn

Ruby: def greet; @name; end
来源：http://gt.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://yw.521024.cn

[G05] 继承
来源：http://xi.nszjky.cn

Py:   class Admin(User): pass
来源：http://iy.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://kd.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ag.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://bf.huixiangedu.cn

Java: class Admin extends User {}
来源：http://xa.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://in.shxzukj.cn

Ruby: class Admin < User; end
来源：http://gx.shxzukj.cn

C#:   class Admin : User {}
来源：http://vf.hahajie.cn

[G06] 重写方法
来源：http://gm.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://up.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gm.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://ac.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://qk.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://hj.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sf.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://fc.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://cp.haigaiapp.cn

[G07] 调用父类方法
来源：http://ma.bookmarksfly.cn

Py:   super().greet()
来源：http://qj.asd995.cn

PHP:  parent::greet();
来源：http://ym.szxytkj.cn

JS:   super.greet();
来源：http://xp.lnxyls.cn

TS:   super.greet();
来源：http://qs.gzmigu.cn

Java: super.greet();
来源：http://kh.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lz.bookmarksfly.cn

Ruby: super
来源：http://dw.hnjuh.cn

C#:   base.Greet();
来源：http://qh.szsharing.cn

[G08] 静态方法与属性
来源：http://my.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zn.szsharing.cn

PHP:  public static function f() {}
来源：http://ql.lnxyls.cn

JS:   static f() {}
来源：http://yf.lnxyls.cn

TS:   static f(): void {}
来源：http://nz.lnxyls.cn

Java: static void f() {}
来源：http://qx.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yq.gzmigu.cn

Ruby: def self.f; end
来源：http://yw.shxzskj.cn

C#:   public static void F() {}
来源：http://aw.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://ng.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://jz.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zh.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bg.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://ix.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://zm.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://vh.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vs.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://xu.jctech888.com.cn

[G10] 访问控制
来源：http://oz.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://se.colortex.cn

PHP:  public / protected / private
来源：http://xd.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://nk.nszjky.cn

TS:   public / protected / private
来源：http://pr.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ar.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xc.asd995.cn

Ruby: public / protected / private
来源：http://zr.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://zy.muxihuayi.cn

[G11] getter / setter
来源：http://dl.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://mh.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rf.521024.cn

JS:   get name() { return this._name; }
来源：http://bv.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://bo.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://uf.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ao.hahajie.cn

Ruby: attr_accessor :name
来源：http://kz.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://rn.bjjhwx.cn

[G12] 对象转字符串
来源：http://hf.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://qi.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ap.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://nq.521024.cn

TS:   toString(): string { return this.name; }
来源：http://uf.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://ex.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tj.hahajie.cn

Ruby: def to_s; @name; end
来源：http://op.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://nw.nszjky.cn

[G13] 判断对象类型
来源：http://gu.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://ji.wgjwhj.cn

PHP:  $u instanceof User
来源：http://bg.hnjuh.cn

JS:   u instanceof User
来源：http://nr.521024.cn

TS:   u instanceof User
来源：http://mh.bookmarksfly.cn

Java: u instanceof User
来源：http://uk.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ug.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://fn.huixinmuqiang.cn

C#:   u is User
来源：http://ir.huanxung.cn

[G14] 数据类 / record
来源：http://te.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zg.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://mr.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xq.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://bl.nszjky.cn

Java: record User(String name, int age) {}
来源：http://oy.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://fr.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lp.521024.cn

C#:   record User(string Name, int Age);
来源：http://um.gzmigu.cn

[G15] 枚举
来源：http://ei.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rf.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ew.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mg.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ty.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://oo.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mz.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://ia.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kv.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://qh.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sc.521024.cn


<!-- 参考信息 -->