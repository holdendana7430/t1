代发 wailian999

[E18] 模板占位符替换
来源：http://kv.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eg.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hj.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wk.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://va.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zc.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hl.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://om.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bk.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://he.haigaiapp.cn

Py:   s.splitlines()
来源：http://vt.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://or.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://nv.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://oi.bjjhwx.cn

Java: s.lines().toList()
来源：http://lu.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://ke.bjjhwx.cn

Ruby: s.lines
来源：http://gb.haigaiapp.cn

C#:   s.Split('\n')
来源：http://pi.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://db.hnjuh.cn

Py:   if not s:
来源：http://ee.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pv.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mx.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ar.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://qd.nszjky.cn

Go:   if s == "" {}
来源：http://ha.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://nh.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vu.colortex.cn

[E21] 超长截断加省略号
来源：http://mt.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xa.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zw.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://di.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bm.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hd.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://wq.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oc.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ij.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://xi.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yd.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://el.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vp.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://io.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rr.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qg.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://dt.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tv.gzmigu.cn

================================================================================
来源：http://mp.shtwfgs.cn

F. 文件与目录
来源：http://yh.bookmarksfly.cn

================================================================================
来源：http://bz.szxytkj.cn

[F01] 读取整个文件
来源：http://bz.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nr.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://gk.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://at.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zi.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://il.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mh.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://pd.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://nm.shxzskj.cn

[F02] 逐行读取文件
来源：http://ca.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fd.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://db.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oc.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ad.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tb.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ix.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mb.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ju.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://nz.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://di.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gd.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://na.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wq.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hx.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gd.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://cv.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ko.yuexingan06.cn

[F04] 追加写入文件
来源：http://ia.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://no.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nm.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iu.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ip.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vs.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oa.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lj.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://gu.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bm.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://es.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ng.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://bx.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uf.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ia.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://rw.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://js.huanxung.cn

[F06] 删除文件
来源：http://id.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://zx.hahajie.cn

PHP:  unlink("a.txt");
来源：http://he.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://th.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ih.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xm.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://jj.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://wb.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://ve.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://iw.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://el.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zj.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xh.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ol.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fg.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ij.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sm.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sy.jianghongdianzi.cn

[F08] 遍历目录
来源：http://aj.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tp.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bj.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://rb.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://by.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yd.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lt.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://ip.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://dq.panjiajie.cn

[F09] 获取文件大小
来源：http://zi.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://zq.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://fx.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ia.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://fq.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yn.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ny.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://hk.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://fc.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ah.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cl.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tz.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hm.521024.cn

TS:   path.extname("a.txt")
来源：http://nx.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://un.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ng.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dq.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ov.521024.cn

[F11] 复制与移动文件
来源：http://ql.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bj.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mt.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pc.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xj.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nd.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fe.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pn.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ck.shxzskj.cn

[F12] CSV 读写
来源：http://ud.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yu.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lu.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rq.shxzskj.cn

TS:   // 同上
来源：http://tn.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rw.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ux.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ly.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cm.chemitech.net.cn

================================================================================
来源：http://is.hnjuh.cn

G. 面向对象
来源：http://qg.newstarts.cn

================================================================================
来源：http://kh.szsharing.cn

[G01] 定义类
来源：http://kh.wgjwhj.cn

Py:   class User: pass
来源：http://ll.shtwfgs.cn

PHP:  class User {}
来源：http://cs.521024.cn

JS:   class User {}
来源：http://lo.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://gk.huixiangedu.cn

Java: class User {}
来源：http://wc.panjiajie.cn

Go:   type User struct { Name string }
来源：http://ta.lnxyls.cn

Ruby: class User; end
来源：http://ae.szsharing.cn

C#:   class User {}
来源：http://xh.jianghongdianzi.cn

[G02] 构造函数
来源：http://cq.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://jk.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://of.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://fl.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://kr.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://yq.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ca.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://qr.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://yx.jctech888.com.cn

[G03] 实例属性
来源：http://hy.shxzukj.cn

Py:   self.name = "x"
来源：http://nb.hnjuh.cn

PHP:  public string $name = "x";
来源：http://wu.szxytkj.cn

JS:   this.name = "x";
来源：http://ow.haigaiapp.cn

TS:   name: string = "x";
来源：http://gq.colortex.cn

Java: private String name;
来源：http://qh.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cb.colortex.cn

Ruby: @name = "x"
来源：http://hv.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://nk.yuexingan06.cn

[G04] 定义方法
来源：http://pb.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://pc.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zm.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://tp.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://zs.nicolike.cn

Java: String greet() { return name; }
来源：http://cj.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tq.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ch.nszjky.cn

C#:   public string Greet() => Name;
来源：http://pe.521024.cn

[G05] 继承
来源：http://wa.nszjky.cn

Py:   class Admin(User): pass
来源：http://ew.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://mi.asd995.cn

JS:   class Admin extends User {}
来源：http://sy.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://yh.bjjhwx.cn

Java: class Admin extends User {}
来源：http://un.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qu.lnxyls.cn

Ruby: class Admin < User; end
来源：http://lv.szsharing.cn

C#:   class Admin : User {}
来源：http://nn.asd995.cn

[G06] 重写方法
来源：http://ly.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://rs.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ho.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://ir.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://yj.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ks.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jv.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://ig.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://fu.jctech888.com.cn

[G07] 调用父类方法
来源：http://fd.hahajie.cn

Py:   super().greet()
来源：http://hq.huanxung.cn

PHP:  parent::greet();
来源：http://qn.521024.cn

JS:   super.greet();
来源：http://du.asd995.cn

TS:   super.greet();
来源：http://rk.huanxung.cn

Java: super.greet();
来源：http://mc.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ed.hahajie.cn

Ruby: super
来源：http://vr.chemitech.net.cn

C#:   base.Greet();
来源：http://ay.panjiajie.cn

[G08] 静态方法与属性
来源：http://uh.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yi.shtwfgs.cn

PHP:  public static function f() {}
来源：http://mq.bjjhwx.cn

JS:   static f() {}
来源：http://ap.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://ik.shxzskj.cn

Java: static void f() {}
来源：http://kb.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hr.nicolike.cn

Ruby: def self.f; end
来源：http://ef.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://xb.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://kr.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://ot.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ti.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cg.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://gi.521024.cn

Java: interface Shape { double area(); }
来源：http://cj.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://cd.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sj.521024.cn

C#:   interface IShape { double Area(); }
来源：http://cs.asd995.cn

[G10] 访问控制
来源：http://me.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://oq.9csxet.cn

PHP:  public / protected / private
来源：http://qc.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ws.wgjwhj.cn

TS:   public / protected / private
来源：http://ek.colortex.cn

Java: public / protected / private / 默认包级
来源：http://oq.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bi.muxihuayi.cn

Ruby: public / protected / private
来源：http://so.shxzukj.cn

C#:   public / protected / private / internal
来源：http://mg.hahajie.cn

[G11] getter / setter
来源：http://qa.huanxung.cn

Py:   @property 与 @x.setter
来源：http://ov.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://il.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://rm.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://oc.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rk.gzmigu.cn

Ruby: attr_accessor :name
来源：http://jm.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://xx.huanxung.cn

[G12] 对象转字符串
来源：http://ny.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://nk.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ps.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://yx.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://fd.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://cv.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rz.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://kd.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://dt.nicolike.cn

[G13] 判断对象类型
来源：http://jl.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://xy.shtwfgs.cn

PHP:  $u instanceof User
来源：http://xb.9csxet.cn

JS:   u instanceof User
来源：http://ux.newstarts.cn

TS:   u instanceof User
来源：http://su.shtwfgs.cn

Java: u instanceof User
来源：http://zm.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lf.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://aj.gzmigu.cn

C#:   u is User
来源：http://ps.newstarts.cn

[G14] 数据类 / record
来源：http://oy.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://do.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://oo.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bx.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://sq.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://lt.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://yg.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ik.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://sm.521024.cn

[G15] 枚举
来源：http://br.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zf.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kr.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wv.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xo.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://hv.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ng.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ma.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ww.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://mw.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bv.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://he.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://yl.colortex.cn

TS:   Object.entries(obj)
来源：http://ip.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uj.jctech888.com.cn


<!-- 参考信息 -->