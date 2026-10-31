代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wp.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ts.yuntaijiaju.cn

[E16] 数字千分位
来源：http://ve.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://kk.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://vo.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yu.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gr.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yl.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sc.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yn.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://vy.bookmarksfly.cn

[E17] 首字母大写
来源：http://nt.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tp.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://om.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sh.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dg.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yj.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jc.szxytkj.cn

Ruby: s.capitalize
来源：http://gw.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hd.haigaiapp.cn

[E18] 模板占位符替换
来源：http://jh.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qk.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lq.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ic.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pf.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vz.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eq.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kr.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jv.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://sj.bookmarksfly.cn

Py:   s.splitlines()
来源：http://uw.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jn.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://zx.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://et.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://iy.521024.cn

Go:   strings.Split(s, "\n")
来源：http://ty.hnjuh.cn

Ruby: s.lines
来源：http://oq.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://sf.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://pk.yuexingan06.cn

Py:   if not s:
来源：http://ru.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mp.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dm.colortex.cn

TS:   if (s === "") {}
来源：http://uh.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://jo.wgjwhj.cn

Go:   if s == "" {}
来源：http://uh.shxzskj.cn

Ruby: if s.empty?
来源：http://in.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jf.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://hd.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xe.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jc.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ot.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zi.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://jt.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ic.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vz.huanxung.cn

[E22] 字节长度与字符长度
来源：http://uf.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cz.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uf.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iq.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ag.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sy.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tt.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://iz.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yt.wgjwhj.cn

================================================================================
来源：http://mo.szxytkj.cn

F. 文件与目录
来源：http://fy.colortex.cn

================================================================================
来源：http://rb.asd995.cn

[F01] 读取整个文件
来源：http://im.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lz.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://tu.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://th.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zi.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zn.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hx.huanxung.cn

Ruby: File.read("a.txt")
来源：http://zr.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://wk.shxzukj.cn

[F02] 逐行读取文件
来源：http://ix.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qy.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bw.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oy.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lh.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dq.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qy.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wm.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ok.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://bb.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ky.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nf.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ci.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mu.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ho.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rb.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://el.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cj.yuexingan06.cn

[F04] 追加写入文件
来源：http://fv.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ia.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oy.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ms.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://el.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vo.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vq.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://re.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://id.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://zw.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://po.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://mx.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://ww.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://cu.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uu.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pf.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://qw.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://lj.chemitech.net.cn

[F06] 删除文件
来源：http://zu.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://of.nszjky.cn

PHP:  unlink("a.txt");
来源：http://uy.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ql.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tl.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nj.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://cm.colortex.cn

Ruby: File.delete("a.txt")
来源：http://sq.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ek.9csxet.cn

[F07] 创建目录（含多级）
来源：http://hj.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nv.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yw.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fd.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ve.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ar.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mm.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sq.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dx.yuexingan06.cn

[F08] 遍历目录
来源：http://kt.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tr.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pw.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://tj.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://lt.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://le.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ts.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://pu.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://ue.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://mg.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://jj.nicolike.cn

PHP:  filesize("a.txt");
来源：http://re.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://sn.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://ho.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wp.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mo.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://jw.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://ja.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://vy.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xq.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ne.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jn.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://gi.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://we.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hy.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mh.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zk.panjiajie.cn

[F11] 复制与移动文件
来源：http://fr.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mj.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mx.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wa.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ig.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://or.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yl.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qw.bookmarksfly.cn

[F12] CSV 读写
来源：http://eg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sh.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lk.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bz.huixinmuqiang.cn

TS:   // 同上
来源：http://cv.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ft.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://je.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kl.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kt.521024.cn

================================================================================
来源：http://ej.asd995.cn

G. 面向对象
来源：http://yh.chemitech.net.cn

================================================================================
来源：http://pu.huixiangedu.cn

[G01] 定义类
来源：http://bl.nicolike.cn

Py:   class User: pass
来源：http://tk.gzmigu.cn

PHP:  class User {}
来源：http://pt.jianghongdianzi.cn

JS:   class User {}
来源：http://kj.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://dd.521024.cn

Java: class User {}
来源：http://qy.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://dm.hnjuh.cn

Ruby: class User; end
来源：http://xo.panjiajie.cn

C#:   class User {}
来源：http://yb.huanxung.cn

[G02] 构造函数
来源：http://rr.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://kh.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ej.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://dt.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://ko.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://no.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oe.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://am.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://mb.szsharing.cn

[G03] 实例属性
来源：http://hj.muxihuayi.cn

Py:   self.name = "x"
来源：http://yf.shxzskj.cn

PHP:  public string $name = "x";
来源：http://sb.jctech888.com.cn

JS:   this.name = "x";
来源：http://ah.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://nk.nszjky.cn

Java: private String name;
来源：http://uf.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mk.hnjuh.cn

Ruby: @name = "x"
来源：http://em.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://sv.lnxyls.cn

[G04] 定义方法
来源：http://ms.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://ap.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nc.nicolike.cn

JS:   greet() { return this.name; }
来源：http://rz.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://ln.haigaiapp.cn

Java: String greet() { return name; }
来源：http://vh.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bp.asd995.cn

Ruby: def greet; @name; end
来源：http://sr.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://mi.nicolike.cn

[G05] 继承
来源：http://gp.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://cx.nicolike.cn

PHP:  class Admin extends User {}
来源：http://rw.asd995.cn

JS:   class Admin extends User {}
来源：http://uo.521024.cn

TS:   class Admin extends User {}
来源：http://qe.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://sh.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gp.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://mk.gzmigu.cn

C#:   class Admin : User {}
来源：http://fx.hahajie.cn

[G06] 重写方法
来源：http://yu.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://sl.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ml.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://gk.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://vn.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://kn.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://av.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://fn.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://lc.yuexingan06.cn

[G07] 调用父类方法
来源：http://vc.nicolike.cn

Py:   super().greet()
来源：http://pw.nszjky.cn

PHP:  parent::greet();
来源：http://dx.asd995.cn

JS:   super.greet();
来源：http://vp.huixinmuqiang.cn

TS:   super.greet();
来源：http://zk.shtwfgs.cn

Java: super.greet();
来源：http://ml.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ge.521024.cn

Ruby: super
来源：http://mc.panjiajie.cn

C#:   base.Greet();
来源：http://kk.shtwfgs.cn

[G08] 静态方法与属性
来源：http://gw.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ux.szxytkj.cn

PHP:  public static function f() {}
来源：http://mi.hahajie.cn

JS:   static f() {}
来源：http://ty.nicolike.cn

TS:   static f(): void {}
来源：http://lv.bookmarksfly.cn

Java: static void f() {}
来源：http://ya.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aw.szxytkj.cn

Ruby: def self.f; end
来源：http://bk.nicolike.cn

C#:   public static void F() {}
来源：http://cp.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://in.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://ox.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tc.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://af.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://ju.nicolike.cn

Java: interface Shape { double area(); }
来源：http://dt.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://ip.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ne.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://tf.szxytkj.cn

[G10] 访问控制
来源：http://id.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xh.nicolike.cn

PHP:  public / protected / private
来源：http://rt.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://ms.haigaiapp.cn

TS:   public / protected / private
来源：http://ey.521024.cn

Java: public / protected / private / 默认包级
来源：http://gg.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jq.muxihuayi.cn

Ruby: public / protected / private
来源：http://es.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ns.szxytkj.cn

[G11] getter / setter
来源：http://vm.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://cb.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sk.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://br.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://wv.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://sg.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uz.lnxyls.cn

Ruby: attr_accessor :name
来源：http://tm.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ix.szxytkj.cn

[G12] 对象转字符串
来源：http://cl.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://dh.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ae.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://on.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://iw.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://bt.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ic.nszjky.cn

Ruby: def to_s; @name; end
来源：http://qx.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://ax.shxzskj.cn

[G13] 判断对象类型
来源：http://lz.hnjuh.cn

Py:   isinstance(u, User)
来源：http://my.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://pz.szsharing.cn

JS:   u instanceof User
来源：http://ql.shtwfgs.cn

TS:   u instanceof User
来源：http://yf.yuexingan06.cn

Java: u instanceof User
来源：http://sj.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fa.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://da.szxytkj.cn

C#:   u is User
来源：http://pr.huixiangedu.cn

[G14] 数据类 / record
来源：http://np.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sz.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://zr.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wx.huixiangedu.cn


<!-- 参考信息 -->