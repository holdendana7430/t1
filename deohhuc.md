代发 wailian999

Ruby: s.lines
来源：http://bg.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://fg.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://iq.yuntaijiaju.cn

Py:   if not s:
来源：http://ty.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ap.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vp.szsharing.cn

TS:   if (s === "") {}
来源：http://qs.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://vd.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://mb.521024.cn

Ruby: if s.empty?
来源：http://by.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://do.hahajie.cn

[E21] 超长截断加省略号
来源：http://py.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jv.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ml.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sg.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hv.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ry.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://lx.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ha.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bk.huanxung.cn

[E22] 字节长度与字符长度
来源：http://te.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fr.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ui.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lt.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bo.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yx.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://hu.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ef.lnxyls.cn

================================================================================
来源：http://gf.521024.cn

F. 文件与目录
来源：http://bf.huanxung.cn

================================================================================
来源：http://qe.gzmigu.cn

[F01] 读取整个文件
来源：http://gl.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://an.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://zj.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://et.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lj.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dw.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gx.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://yv.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://ej.colortex.cn

[F02] 逐行读取文件
来源：http://fh.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dr.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cy.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://do.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jo.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fc.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iz.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://os.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wx.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://yo.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jc.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qq.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wy.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vl.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ws.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ki.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://dc.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gk.wgjwhj.cn

[F04] 追加写入文件
来源：http://pf.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vk.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pr.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://um.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pl.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://he.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nt.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gj.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uu.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://df.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://io.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://hi.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://ug.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://kd.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cb.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iy.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://wo.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://op.yuntaijiaju.cn

[F06] 删除文件
来源：http://jk.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://jz.nicolike.cn

PHP:  unlink("a.txt");
来源：http://rk.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ul.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vl.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gl.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://ey.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://dj.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://vc.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://sr.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ft.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://px.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vy.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lf.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kk.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dy.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vw.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ab.jctech888.com.cn

[F08] 遍历目录
来源：http://di.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kk.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jv.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://vb.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://bl.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yo.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wh.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://ry.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://jm.jctech888.com.cn

[F09] 获取文件大小
来源：http://po.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://kj.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://kl.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://zf.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://qk.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fn.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qt.newstarts.cn

Ruby: File.size("a.txt")
来源：http://mx.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://pj.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://jt.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://un.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fi.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zt.nicolike.cn

TS:   path.extname("a.txt")
来源：http://gs.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zt.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fa.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dp.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://az.521024.cn

[F11] 复制与移动文件
来源：http://za.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zb.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nz.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qn.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yc.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zp.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ap.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://if.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mi.9csxet.cn

[F12] CSV 读写
来源：http://td.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mj.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ee.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yw.szxytkj.cn

TS:   // 同上
来源：http://my.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hs.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nw.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hr.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cg.hnjuh.cn

================================================================================
来源：http://bq.panjiajie.cn

G. 面向对象
来源：http://vm.nicolike.cn

================================================================================
来源：http://ad.colortex.cn

[G01] 定义类
来源：http://og.muxihuayi.cn

Py:   class User: pass
来源：http://hg.newstarts.cn

PHP:  class User {}
来源：http://av.panjiajie.cn

JS:   class User {}
来源：http://jf.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://aj.521024.cn

Java: class User {}
来源：http://dj.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://ta.lnxyls.cn

Ruby: class User; end
来源：http://nb.gzmigu.cn

C#:   class User {}
来源：http://nx.jctech888.com.cn

[G02] 构造函数
来源：http://lr.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://nr.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://wi.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://bn.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://fw.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://fn.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zt.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vh.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://rg.colortex.cn

[G03] 实例属性
来源：http://fq.hahajie.cn

Py:   self.name = "x"
来源：http://bf.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://mv.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://xo.yuexingan06.cn

TS:   name: string = "x";
来源：http://kx.huanxung.cn

Java: private String name;
来源：http://es.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ha.bjjhwx.cn

Ruby: @name = "x"
来源：http://oz.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ui.haigaiapp.cn

[G04] 定义方法
来源：http://oz.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://zz.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lg.hahajie.cn

JS:   greet() { return this.name; }
来源：http://bd.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://zt.chemitech.net.cn

Java: String greet() { return name; }
来源：http://mw.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xr.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://ql.521024.cn

C#:   public string Greet() => Name;
来源：http://ut.yuexingan06.cn

[G05] 继承
来源：http://qi.lnxyls.cn

Py:   class Admin(User): pass
来源：http://xi.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://pe.nicolike.cn

JS:   class Admin extends User {}
来源：http://ap.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ya.hahajie.cn

Java: class Admin extends User {}
来源：http://fn.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wz.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://dz.huanxung.cn

C#:   class Admin : User {}
来源：http://zp.huixiangedu.cn

[G06] 重写方法
来源：http://aq.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://oc.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vi.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://zh.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://df.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://lx.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rv.asd995.cn

Ruby: def greet; "admin"; end
来源：http://yq.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://zf.hahajie.cn

[G07] 调用父类方法
来源：http://yh.jianghongdianzi.cn

Py:   super().greet()
来源：http://mv.chemitech.net.cn

PHP:  parent::greet();
来源：http://xs.bjjhwx.cn

JS:   super.greet();
来源：http://jq.gzmigu.cn

TS:   super.greet();
来源：http://kx.panjiajie.cn

Java: super.greet();
来源：http://ji.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ki.jctech888.com.cn

Ruby: super
来源：http://nv.huixinmuqiang.cn

C#:   base.Greet();
来源：http://tr.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://wx.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ft.hahajie.cn

PHP:  public static function f() {}
来源：http://mh.hahajie.cn

JS:   static f() {}
来源：http://ry.gzmigu.cn

TS:   static f(): void {}
来源：http://ei.chemitech.net.cn

Java: static void f() {}
来源：http://av.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ua.huanxung.cn

Ruby: def self.f; end
来源：http://wj.9csxet.cn

C#:   public static void F() {}
来源：http://mx.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ar.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ca.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nt.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nx.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://bd.nicolike.cn

Java: interface Shape { double area(); }
来源：http://hs.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://vp.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gi.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://xm.panjiajie.cn

[G10] 访问控制
来源：http://rn.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://uw.newstarts.cn

PHP:  public / protected / private
来源：http://je.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://wp.nicolike.cn

TS:   public / protected / private
来源：http://dr.521024.cn

Java: public / protected / private / 默认包级
来源：http://iu.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yc.huixiangedu.cn

Ruby: public / protected / private
来源：http://hl.colortex.cn

C#:   public / protected / private / internal
来源：http://db.shxzukj.cn

[G11] getter / setter
来源：http://lu.huanxung.cn

Py:   @property 与 @x.setter
来源：http://wd.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yb.9csxet.cn

JS:   get name() { return this._name; }
来源：http://fm.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://mf.szxytkj.cn

Java: public String getName() { return name; }
来源：http://jo.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sc.9csxet.cn

Ruby: attr_accessor :name
来源：http://sf.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://vn.chemitech.net.cn

[G12] 对象转字符串
来源：http://oi.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://jc.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pw.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://jr.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://ed.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://rd.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qk.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://lh.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://kz.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://hm.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://pz.nszjky.cn

PHP:  $u instanceof User
来源：http://op.huixiangedu.cn

JS:   u instanceof User
来源：http://lc.muxihuayi.cn

TS:   u instanceof User
来源：http://mh.9csxet.cn

Java: u instanceof User
来源：http://tj.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ao.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://mr.bookmarksfly.cn

C#:   u is User
来源：http://lv.huanxung.cn

[G14] 数据类 / record
来源：http://ai.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fz.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://yy.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://em.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://we.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://rh.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://oz.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ez.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://cr.szxytkj.cn

[G15] 枚举
来源：http://mi.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://je.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qs.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qj.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ps.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://kv.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://in.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://tv.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xj.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://br.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vk.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ce.colortex.cn

JS:   Object.entries(obj)
来源：http://us.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://wk.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cs.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gz.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ab.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ub.wgjwhj.cn

================================================================================
来源：http://ma.bjjhwx.cn

H. 异常与错误处理
来源：http://ly.bookmarksfly.cn

================================================================================
来源：http://hi.colortex.cn

[H01] try / catch 基础
来源：http://oj.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://po.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pl.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qq.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rc.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kv.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uf.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bg.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xg.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://xz.gzmigu.cn


<!-- 参考信息 -->