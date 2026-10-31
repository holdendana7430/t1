代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vx.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wb.bookmarksfly.cn

[E16] 数字千分位
来源：http://fz.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://eh.nszjky.cn

PHP:  number_format(1234567);
来源：http://ij.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jy.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cp.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zi.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ao.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://lq.yuexingan06.cn

[E17] 首字母大写
来源：http://ug.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dm.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rl.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sp.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eb.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://il.521024.cn

Ruby: s.capitalize
来源：http://qb.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://im.gzmigu.cn

[E18] 模板占位符替换
来源：http://pv.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fa.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ag.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ux.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hp.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ty.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gr.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ej.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ot.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://vi.huanxung.cn

Py:   s.splitlines()
来源：http://ux.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ka.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://vi.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://yd.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://qr.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://oh.bjjhwx.cn

Ruby: s.lines
来源：http://bn.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ry.colortex.cn

[E20] 判断字符串是否为空
来源：http://nf.nszjky.cn

Py:   if not s:
来源：http://gz.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ec.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zx.yuexingan06.cn

TS:   if (s === "") {}
来源：http://mu.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://gt.nszjky.cn

Go:   if s == "" {}
来源：http://nk.nszjky.cn

Ruby: if s.empty?
来源：http://vo.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ba.newstarts.cn

[E21] 超长截断加省略号
来源：http://ps.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ba.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ju.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dj.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bz.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://bm.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pf.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ld.colortex.cn

[E22] 字节长度与字符长度
来源：http://bu.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wc.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nb.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pp.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xk.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rt.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pq.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://rx.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oz.yuexingan06.cn

================================================================================
来源：http://dc.wgjwhj.cn

F. 文件与目录
来源：http://ik.nicolike.cn

================================================================================
来源：http://tx.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://kf.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wa.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://lu.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xd.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ev.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hj.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wb.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://bz.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://lp.hahajie.cn

[F02] 逐行读取文件
来源：http://ey.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ff.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qq.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pf.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gj.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lc.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wc.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kk.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ef.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://pw.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cz.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nc.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ef.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tp.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xh.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://es.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://pa.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sm.gzmigu.cn

[F04] 追加写入文件
来源：http://uc.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dy.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dy.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://km.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ul.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ta.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qu.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://et.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ux.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://hh.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://et.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://kh.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://gp.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://zc.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ft.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pc.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://pd.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://qs.newstarts.cn

[F06] 删除文件
来源：http://gt.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://wj.9csxet.cn

PHP:  unlink("a.txt");
来源：http://ms.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ds.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://js.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ip.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://uh.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://uv.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://hx.colortex.cn

[F07] 创建目录（含多级）
来源：http://gv.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ws.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mu.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lp.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mj.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sl.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ih.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fx.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fb.521024.cn

[F08] 遍历目录
来源：http://qj.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gs.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wi.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://nr.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://gz.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ht.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rq.colortex.cn

Ruby: Dir.children("dir")
来源：http://tx.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://ma.szsharing.cn

[F09] 获取文件大小
来源：http://jg.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://jh.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://qc.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://lx.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://zw.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ih.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ax.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://be.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://zj.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://pm.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fv.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nf.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vk.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://rg.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ov.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zs.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iy.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ws.szxytkj.cn

[F11] 复制与移动文件
来源：http://xr.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bz.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vo.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pd.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ri.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pa.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://as.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vf.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://di.yuexingan06.cn

[F12] CSV 读写
来源：http://ao.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ap.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uo.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ko.asd995.cn

TS:   // 同上
来源：http://wa.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dk.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cv.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sh.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jt.gzmigu.cn

================================================================================
来源：http://nd.wgjwhj.cn

G. 面向对象
来源：http://gx.hahajie.cn

================================================================================
来源：http://th.chemitech.net.cn

[G01] 定义类
来源：http://be.muxihuayi.cn

Py:   class User: pass
来源：http://lv.jctech888.com.cn

PHP:  class User {}
来源：http://rr.bjjhwx.cn

JS:   class User {}
来源：http://ms.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ly.yuntaijiaju.cn

Java: class User {}
来源：http://xo.521024.cn

Go:   type User struct { Name string }
来源：http://sj.521024.cn

Ruby: class User; end
来源：http://re.huixiangedu.cn

C#:   class User {}
来源：http://ri.huixinmuqiang.cn

[G02] 构造函数
来源：http://ij.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://hk.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://xr.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://fh.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://dz.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://ii.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lc.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://iu.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://sk.jctech888.com.cn

[G03] 实例属性
来源：http://gf.shxzukj.cn

Py:   self.name = "x"
来源：http://cj.panjiajie.cn

PHP:  public string $name = "x";
来源：http://vu.asd995.cn

JS:   this.name = "x";
来源：http://dp.nszjky.cn

TS:   name: string = "x";
来源：http://yh.gzmigu.cn

Java: private String name;
来源：http://cy.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qw.jctech888.com.cn

Ruby: @name = "x"
来源：http://nd.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://to.huixiangedu.cn

[G04] 定义方法
来源：http://by.9csxet.cn

Py:   def greet(self): return self.name
来源：http://tl.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gu.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://kq.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://qr.newstarts.cn

Java: String greet() { return name; }
来源：http://qh.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qa.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://cd.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ve.9csxet.cn

[G05] 继承
来源：http://hn.gzmigu.cn

Py:   class Admin(User): pass
来源：http://pk.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://uk.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://mb.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://fp.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://rj.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bs.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://jr.shxzskj.cn

C#:   class Admin : User {}
来源：http://bv.shtwfgs.cn

[G06] 重写方法
来源：http://ln.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://ge.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hu.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://fo.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://vo.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://dg.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gy.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://an.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://en.hnjuh.cn

[G07] 调用父类方法
来源：http://zg.wgjwhj.cn

Py:   super().greet()
来源：http://zg.muxihuayi.cn

PHP:  parent::greet();
来源：http://ww.newstarts.cn

JS:   super.greet();
来源：http://cz.nicolike.cn

TS:   super.greet();
来源：http://dc.bookmarksfly.cn

Java: super.greet();
来源：http://os.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ld.colortex.cn

Ruby: super
来源：http://do.shxzukj.cn

C#:   base.Greet();
来源：http://cq.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://zx.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hv.521024.cn

PHP:  public static function f() {}
来源：http://fd.jianghongdianzi.cn

JS:   static f() {}
来源：http://ms.szsharing.cn

TS:   static f(): void {}
来源：http://hy.yuntaijiaju.cn

Java: static void f() {}
来源：http://xz.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ju.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://dg.haigaiapp.cn

C#:   public static void F() {}
来源：http://kw.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://ed.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://jp.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uw.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zz.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://ud.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://md.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ea.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rf.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://um.jianghongdianzi.cn

[G10] 访问控制
来源：http://sl.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://nl.szsharing.cn

PHP:  public / protected / private
来源：http://qn.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://aq.szxytkj.cn

TS:   public / protected / private
来源：http://uv.colortex.cn

Java: public / protected / private / 默认包级
来源：http://kh.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kq.newstarts.cn

Ruby: public / protected / private
来源：http://os.nicolike.cn

C#:   public / protected / private / internal
来源：http://rb.shtwfgs.cn

[G11] getter / setter
来源：http://td.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://dz.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lm.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://hd.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://ft.521024.cn

Java: public String getName() { return name; }
来源：http://pr.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://op.asd995.cn

Ruby: attr_accessor :name
来源：http://km.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ma.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://uu.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://lq.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sd.521024.cn

JS:   toString() { return this.name; }
来源：http://jy.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://yy.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://zg.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dd.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://nk.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://ps.shxzskj.cn

[G13] 判断对象类型
来源：http://hs.asd995.cn

Py:   isinstance(u, User)
来源：http://ef.shtwfgs.cn

PHP:  $u instanceof User
来源：http://dk.szsharing.cn

JS:   u instanceof User
来源：http://hn.colortex.cn

TS:   u instanceof User
来源：http://cf.hahajie.cn

Java: u instanceof User
来源：http://om.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kq.nicolike.cn

Ruby: u.is_a?(User)
来源：http://fu.panjiajie.cn

C#:   u is User
来源：http://ku.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://lm.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mb.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://cq.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tn.hnjuh.cn


<!-- 参考信息 -->