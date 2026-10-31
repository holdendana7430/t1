代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oz.hahajie.cn

[E19] 多行文本按行拆分
来源：http://dm.gzmigu.cn

Py:   s.splitlines()
来源：http://sw.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gw.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://zg.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://ui.bookmarksfly.cn

Java: s.lines().toList()
来源：http://ai.521024.cn

Go:   strings.Split(s, "\n")
来源：http://mk.shxzskj.cn

Ruby: s.lines
来源：http://ak.9csxet.cn

C#:   s.Split('\n')
来源：http://mg.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://lk.521024.cn

Py:   if not s:
来源：http://bb.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hk.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wx.panjiajie.cn

TS:   if (s === "") {}
来源：http://xi.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://eo.shxzskj.cn

Go:   if s == "" {}
来源：http://td.haigaiapp.cn

Ruby: if s.empty?
来源：http://wf.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://le.hahajie.cn

[E21] 超长截断加省略号
来源：http://mi.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gd.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ns.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qy.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dh.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fw.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://it.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hn.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ic.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://af.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dm.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wr.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://um.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oi.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lm.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://wr.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xc.jctech888.com.cn

================================================================================
来源：http://wo.521024.cn

F. 文件与目录
来源：http://ue.jianghongdianzi.cn

================================================================================
来源：http://uj.panjiajie.cn

[F01] 读取整个文件
来源：http://te.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wb.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://qh.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kh.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sy.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rd.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xz.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://hc.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://nd.shxzukj.cn

[F02] 逐行读取文件
来源：http://kq.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mp.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rv.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qb.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iy.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dn.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bf.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sa.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ga.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ap.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kb.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wt.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wf.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zi.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xs.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bz.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ll.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://so.wgjwhj.cn

[F04] 追加写入文件
来源：http://hd.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xi.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rr.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://as.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ll.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://up.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mt.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rd.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://qg.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jf.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://li.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://wc.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ii.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mw.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zr.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://os.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://jo.lnxyls.cn

[F06] 删除文件
来源：http://xt.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://zj.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://qg.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cn.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ou.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://al.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://bf.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://cg.asd995.cn

C#:   File.Delete("a.txt");
来源：http://xk.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://sc.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jz.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gu.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xb.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://if.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://np.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jw.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ll.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pw.szsharing.cn

[F08] 遍历目录
来源：http://wt.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vr.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hx.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://rf.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://tv.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ie.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cd.hahajie.cn

Ruby: Dir.children("dir")
来源：http://zo.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://lx.521024.cn

[F09] 获取文件大小
来源：http://bz.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://xf.9csxet.cn

PHP:  filesize("a.txt");
来源：http://tf.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://rd.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://ms.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ix.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://la.nicolike.cn

Ruby: File.size("a.txt")
来源：http://ob.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://ap.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://gi.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mr.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://su.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ba.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ma.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ls.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bo.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zf.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rb.wgjwhj.cn

[F11] 复制与移动文件
来源：http://xe.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://al.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fd.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gg.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wj.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ep.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nm.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hm.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://my.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ro.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://po.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bx.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bz.9csxet.cn

TS:   // 同上
来源：http://ag.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dt.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gg.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mj.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ga.yuntaijiaju.cn

================================================================================
来源：http://xh.jctech888.com.cn

G. 面向对象
来源：http://yi.jianghongdianzi.cn

================================================================================
来源：http://zi.nszjky.cn

[G01] 定义类
来源：http://km.bjjhwx.cn

Py:   class User: pass
来源：http://zx.jianghongdianzi.cn

PHP:  class User {}
来源：http://fu.huixiangedu.cn

JS:   class User {}
来源：http://hb.colortex.cn

TS:   class User { name: string = ""; }
来源：http://vv.shxzukj.cn

Java: class User {}
来源：http://wm.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ci.hnjuh.cn

Ruby: class User; end
来源：http://qi.haigaiapp.cn

C#:   class User {}
来源：http://nh.nszjky.cn

[G02] 构造函数
来源：http://ez.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://jr.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fv.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://rc.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://iy.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://pv.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ar.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://xm.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://md.bookmarksfly.cn

[G03] 实例属性
来源：http://ny.bookmarksfly.cn

Py:   self.name = "x"
来源：http://eo.panjiajie.cn

PHP:  public string $name = "x";
来源：http://bq.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://aj.hnjuh.cn

TS:   name: string = "x";
来源：http://hi.huixiangedu.cn

Java: private String name;
来源：http://kz.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://da.chemitech.net.cn

Ruby: @name = "x"
来源：http://ga.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://tq.huixiangedu.cn

[G04] 定义方法
来源：http://ra.521024.cn

Py:   def greet(self): return self.name
来源：http://xr.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://at.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://ww.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://as.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://ox.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lj.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://jx.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://dj.muxihuayi.cn

[G05] 继承
来源：http://cs.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://ta.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://uu.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://rv.hahajie.cn

TS:   class Admin extends User {}
来源：http://te.hahajie.cn

Java: class Admin extends User {}
来源：http://fv.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vq.huanxung.cn

Ruby: class Admin < User; end
来源：http://fj.szsharing.cn

C#:   class Admin : User {}
来源：http://vs.shxzskj.cn

[G06] 重写方法
来源：http://fz.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://pf.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lu.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://qh.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://gw.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://lk.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qb.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://wh.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://yk.shxzskj.cn

[G07] 调用父类方法
来源：http://dd.yuntaijiaju.cn

Py:   super().greet()
来源：http://zn.colortex.cn

PHP:  parent::greet();
来源：http://kr.9csxet.cn

JS:   super.greet();
来源：http://jp.bookmarksfly.cn

TS:   super.greet();
来源：http://tn.yuexingan06.cn

Java: super.greet();
来源：http://fg.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gg.jctech888.com.cn

Ruby: super
来源：http://zl.yuexingan06.cn

C#:   base.Greet();
来源：http://qh.shxzukj.cn

[G08] 静态方法与属性
来源：http://ny.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ej.gzmigu.cn

PHP:  public static function f() {}
来源：http://yw.wgjwhj.cn

JS:   static f() {}
来源：http://ky.521024.cn

TS:   static f(): void {}
来源：http://ju.hahajie.cn

Java: static void f() {}
来源：http://gm.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vl.chemitech.net.cn

Ruby: def self.f; end
来源：http://uh.asd995.cn

C#:   public static void F() {}
来源：http://pg.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://uq.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://fh.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dr.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jf.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://bd.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ee.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://qv.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://th.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://yt.colortex.cn

[G10] 访问控制
来源：http://pj.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://gp.gzmigu.cn

PHP:  public / protected / private
来源：http://li.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://wv.wgjwhj.cn

TS:   public / protected / private
来源：http://is.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://zp.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qe.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://yu.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://cf.huixinmuqiang.cn

[G11] getter / setter
来源：http://cw.521024.cn

Py:   @property 与 @x.setter
来源：http://st.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bj.colortex.cn

JS:   get name() { return this._name; }
来源：http://hm.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://jk.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://na.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://il.szsharing.cn

Ruby: attr_accessor :name
来源：http://ae.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://fi.szsharing.cn

[G12] 对象转字符串
来源：http://xf.521024.cn

Py:   def __str__(self): return self.name
来源：http://qu.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sg.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://cg.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://qm.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://be.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://st.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://om.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://fx.521024.cn

[G13] 判断对象类型
来源：http://qt.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://ys.shtwfgs.cn

PHP:  $u instanceof User
来源：http://wf.lnxyls.cn

JS:   u instanceof User
来源：http://hg.muxihuayi.cn

TS:   u instanceof User
来源：http://zc.chemitech.net.cn

Java: u instanceof User
来源：http://jo.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uc.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://sb.nicolike.cn

C#:   u is User
来源：http://nc.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://yn.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ha.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://un.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qc.521024.cn

TS:   type User = { name: string; age: number };
来源：http://pm.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://kq.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://do.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cp.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ja.bookmarksfly.cn

[G15] 枚举
来源：http://xy.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mb.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rt.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zp.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ex.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://lt.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zg.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://vh.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kb.asd995.cn

[G16] 对象转数组 / 字典
来源：http://nb.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://id.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://sl.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://ya.hnjuh.cn

TS:   Object.entries(obj)
来源：http://hn.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mq.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://an.panjiajie.cn

Ruby: obj.instance_variables
来源：http://zz.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://sr.shxzukj.cn

================================================================================
来源：http://zz.chemitech.net.cn

H. 异常与错误处理
来源：http://ht.shtwfgs.cn

================================================================================
来源：http://ui.huanxung.cn

[H01] try / catch 基础
来源：http://rv.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hw.yuntaijiaju.cn


<!-- 参考信息 -->