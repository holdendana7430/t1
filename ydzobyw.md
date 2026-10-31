代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://am.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://di.huixiangedu.cn

Py:   s.splitlines()
来源：http://ah.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dr.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://hb.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://nf.hnjuh.cn

Java: s.lines().toList()
来源：http://zl.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://lk.gzmigu.cn

Ruby: s.lines
来源：http://eu.hahajie.cn

C#:   s.Split('\n')
来源：http://ip.9csxet.cn

[E20] 判断字符串是否为空
来源：http://pn.jianghongdianzi.cn

Py:   if not s:
来源：http://qk.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nj.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://er.huixiangedu.cn

TS:   if (s === "") {}
来源：http://in.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://cr.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://ub.bookmarksfly.cn

Ruby: if s.empty?
来源：http://mw.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sj.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://wq.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gb.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://op.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wt.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yb.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ui.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://lk.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://by.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gx.colortex.cn

[E22] 字节长度与字符长度
来源：http://va.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ty.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qm.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ua.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://si.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nu.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://xb.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tm.shxzskj.cn

================================================================================
来源：http://bm.hahajie.cn

F. 文件与目录
来源：http://bq.huixiangedu.cn

================================================================================
来源：http://bp.colortex.cn

[F01] 读取整个文件
来源：http://ll.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tq.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://mz.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mr.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ww.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ls.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zf.521024.cn

Ruby: File.read("a.txt")
来源：http://op.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://qv.muxihuayi.cn

[F02] 逐行读取文件
来源：http://bx.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nn.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ng.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tf.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ll.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ay.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wu.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mp.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ac.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kr.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pq.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qx.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rl.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jg.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gq.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://co.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zc.shtwfgs.cn

[F04] 追加写入文件
来源：http://ni.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sf.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ba.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dx.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dz.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fs.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vr.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iq.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://at.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://cu.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vp.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://pn.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://sq.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://mt.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xj.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uy.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://fu.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://ib.huixiangedu.cn

[F06] 删除文件
来源：http://aa.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://rz.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://qb.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xs.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hg.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wt.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://px.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://zk.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://ir.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://rb.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nj.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qp.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sp.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gd.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mx.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vv.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ei.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cs.wgjwhj.cn

[F08] 遍历目录
来源：http://fg.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jw.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kh.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://zg.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://ca.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cx.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jl.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ec.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://xe.szxytkj.cn

[F09] 获取文件大小
来源：http://vs.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ec.szsharing.cn

PHP:  filesize("a.txt");
来源：http://nf.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://bl.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://ub.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bd.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wn.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://lv.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://au.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://df.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pe.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rw.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uo.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://vv.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ju.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dy.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kv.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lm.chemitech.net.cn

[F11] 复制与移动文件
来源：http://jl.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ko.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pm.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xh.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pz.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://te.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://am.9csxet.cn

[F12] CSV 读写
来源：http://ev.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fm.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uk.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gu.9csxet.cn

TS:   // 同上
来源：http://ey.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ro.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vi.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qh.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nb.muxihuayi.cn

================================================================================
来源：http://cz.521024.cn

G. 面向对象
来源：http://kf.szsharing.cn

================================================================================
来源：http://zf.jctech888.com.cn

[G01] 定义类
来源：http://vx.huanxung.cn

Py:   class User: pass
来源：http://ga.asd995.cn

PHP:  class User {}
来源：http://aw.bookmarksfly.cn

JS:   class User {}
来源：http://wm.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://ep.wgjwhj.cn

Java: class User {}
来源：http://fa.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://rk.nicolike.cn

Ruby: class User; end
来源：http://py.colortex.cn

C#:   class User {}
来源：http://th.newstarts.cn

[G02] 构造函数
来源：http://gk.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ff.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://hc.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://za.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://vi.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://jp.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iy.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://my.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://pn.szxytkj.cn

[G03] 实例属性
来源：http://dr.nszjky.cn

Py:   self.name = "x"
来源：http://dc.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ll.bookmarksfly.cn

JS:   this.name = "x";
来源：http://lp.asd995.cn

TS:   name: string = "x";
来源：http://js.9csxet.cn

Java: private String name;
来源：http://bl.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ph.muxihuayi.cn

Ruby: @name = "x"
来源：http://mf.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://yu.yuexingan06.cn

[G04] 定义方法
来源：http://za.newstarts.cn

Py:   def greet(self): return self.name
来源：http://ex.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nr.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://op.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://oh.szxytkj.cn

Java: String greet() { return name; }
来源：http://xn.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qu.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://qd.szsharing.cn

C#:   public string Greet() => Name;
来源：http://vm.muxihuayi.cn

[G05] 继承
来源：http://pn.szsharing.cn

Py:   class Admin(User): pass
来源：http://ga.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://zy.nicolike.cn

JS:   class Admin extends User {}
来源：http://dv.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ds.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ut.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gx.colortex.cn

Ruby: class Admin < User; end
来源：http://lz.muxihuayi.cn

C#:   class Admin : User {}
来源：http://kt.521024.cn

[G06] 重写方法
来源：http://ul.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://rn.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xh.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://xn.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://mq.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://qc.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nv.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://sb.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://qp.szxytkj.cn

[G07] 调用父类方法
来源：http://xv.hnjuh.cn

Py:   super().greet()
来源：http://in.shxzukj.cn

PHP:  parent::greet();
来源：http://zx.jianghongdianzi.cn

JS:   super.greet();
来源：http://vm.szxytkj.cn

TS:   super.greet();
来源：http://lv.nszjky.cn

Java: super.greet();
来源：http://qv.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ks.gzmigu.cn

Ruby: super
来源：http://hr.szsharing.cn

C#:   base.Greet();
来源：http://ce.nszjky.cn

[G08] 静态方法与属性
来源：http://ef.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uy.newstarts.cn

PHP:  public static function f() {}
来源：http://zq.bookmarksfly.cn

JS:   static f() {}
来源：http://pt.9csxet.cn

TS:   static f(): void {}
来源：http://tn.bookmarksfly.cn

Java: static void f() {}
来源：http://yy.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ry.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://ve.asd995.cn

C#:   public static void F() {}
来源：http://kq.colortex.cn

[G09] 接口 / 抽象类
来源：http://wr.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://fi.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qu.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ys.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://oq.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://qh.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://si.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xn.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://xs.yuexingan06.cn

[G10] 访问控制
来源：http://ew.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://yr.panjiajie.cn

PHP:  public / protected / private
来源：http://uz.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://bm.asd995.cn

TS:   public / protected / private
来源：http://tr.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ct.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://or.bjjhwx.cn

Ruby: public / protected / private
来源：http://wl.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ud.haigaiapp.cn

[G11] getter / setter
来源：http://uu.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://co.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mj.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://ih.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ol.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://pa.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pj.shxzskj.cn

Ruby: attr_accessor :name
来源：http://tj.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://ko.chemitech.net.cn

[G12] 对象转字符串
来源：http://rj.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://hn.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pa.huanxung.cn

JS:   toString() { return this.name; }
来源：http://al.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://ok.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://el.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://py.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://pv.colortex.cn

C#:   public override string ToString() => Name;
来源：http://tt.szsharing.cn

[G13] 判断对象类型
来源：http://kn.nicolike.cn

Py:   isinstance(u, User)
来源：http://aj.muxihuayi.cn

PHP:  $u instanceof User
来源：http://jx.colortex.cn

JS:   u instanceof User
来源：http://gh.hnjuh.cn

TS:   u instanceof User
来源：http://rz.huanxung.cn

Java: u instanceof User
来源：http://qf.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fg.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://ht.nicolike.cn

C#:   u is User
来源：http://eg.bookmarksfly.cn

[G14] 数据类 / record
来源：http://tg.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mo.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://as.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dg.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://ko.9csxet.cn

Java: record User(String name, int age) {}
来源：http://rm.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://zr.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yh.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://be.panjiajie.cn

[G15] 枚举
来源：http://pk.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mi.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wq.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ah.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jw.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://ym.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xx.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://xu.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://td.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://gu.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ib.521024.cn

PHP:  get_object_vars($obj);
来源：http://uq.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://fp.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://wr.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ku.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kp.colortex.cn

Ruby: obj.instance_variables
来源：http://hg.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://eu.chemitech.net.cn

================================================================================
来源：http://sv.haigaiapp.cn

H. 异常与错误处理
来源：http://kj.yuexingan06.cn

================================================================================
来源：http://au.shxzukj.cn

[H01] try / catch 基础
来源：http://uj.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vf.huanxung.cn


<!-- 参考信息 -->