代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gd.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://bw.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wq.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hq.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://to.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ss.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://in.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://it.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wn.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qz.panjiajie.cn

[E16] 数字千分位
来源：http://wy.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://ky.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://vu.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lh.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ih.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dn.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eo.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bd.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://mw.yuntaijiaju.cn

[E17] 首字母大写
来源：http://hy.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ka.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jw.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zm.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dp.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dk.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fx.newstarts.cn

Ruby: s.capitalize
来源：http://zi.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bi.chemitech.net.cn

[E18] 模板占位符替换
来源：http://ou.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ex.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lb.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dv.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://br.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qf.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hs.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://or.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vp.9csxet.cn

[E19] 多行文本按行拆分
来源：http://lp.jctech888.com.cn

Py:   s.splitlines()
来源：http://vz.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://he.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://ur.521024.cn

TS:   s.split(/\r?\n/)
来源：http://bg.521024.cn

Java: s.lines().toList()
来源：http://zm.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://ws.colortex.cn

Ruby: s.lines
来源：http://rx.hahajie.cn

C#:   s.Split('\n')
来源：http://uw.hahajie.cn

[E20] 判断字符串是否为空
来源：http://wh.jctech888.com.cn

Py:   if not s:
来源：http://mx.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ru.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://es.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://da.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://hg.yuexingan06.cn

Go:   if s == "" {}
来源：http://de.muxihuayi.cn

Ruby: if s.empty?
来源：http://st.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ss.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://kn.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cz.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ev.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ov.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cd.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ur.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://yq.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ty.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ib.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://av.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fw.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ev.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dw.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zz.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zg.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://au.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sp.nszjky.cn

================================================================================
来源：http://ta.huanxung.cn

F. 文件与目录
来源：http://ot.huixinmuqiang.cn

================================================================================
来源：http://ds.yuexingan06.cn

[F01] 读取整个文件
来源：http://vh.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bp.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://sm.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ac.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xd.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tp.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uv.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://ks.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ez.chemitech.net.cn

[F02] 逐行读取文件
来源：http://va.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vc.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tj.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rt.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ci.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kf.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vi.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uj.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cg.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://gl.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vb.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ap.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gl.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ij.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ds.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://di.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://sn.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xb.nicolike.cn

[F04] 追加写入文件
来源：http://si.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://li.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://am.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ll.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ac.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yf.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cc.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dn.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kc.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://zh.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bd.colortex.cn

PHP:  file_exists("a.txt");
来源：http://gp.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://rb.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://kg.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cg.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xf.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://yj.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://rj.yuexingan06.cn

[F06] 删除文件
来源：http://vx.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://ze.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://nk.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lo.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lw.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://gd.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://nj.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://qi.nicolike.cn

[F07] 创建目录（含多级）
来源：http://ze.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://et.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pq.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ij.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pf.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ce.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gq.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vz.9csxet.cn

[F08] 遍历目录
来源：http://tu.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wn.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tf.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://uj.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ss.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uy.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bo.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://yx.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://wt.521024.cn

[F09] 获取文件大小
来源：http://rr.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://we.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wi.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://nu.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://hf.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ew.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://su.szsharing.cn

Ruby: File.size("a.txt")
来源：http://rt.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://qu.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://pi.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fj.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ym.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ik.9csxet.cn

TS:   path.extname("a.txt")
来源：http://xm.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oc.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cw.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zw.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ll.szsharing.cn

[F11] 复制与移动文件
来源：http://ui.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ln.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://an.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yl.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dk.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lg.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jz.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wg.haigaiapp.cn

[F12] CSV 读写
来源：http://ic.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://po.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pe.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sf.lnxyls.cn

TS:   // 同上
来源：http://lh.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bm.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://un.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ji.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ee.wgjwhj.cn

================================================================================
来源：http://tv.yuexingan06.cn

G. 面向对象
来源：http://hu.hnjuh.cn

================================================================================
来源：http://qn.huixiangedu.cn

[G01] 定义类
来源：http://gi.jianghongdianzi.cn

Py:   class User: pass
来源：http://ne.lnxyls.cn

PHP:  class User {}
来源：http://ui.lnxyls.cn

JS:   class User {}
来源：http://iu.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://nt.shxzskj.cn

Java: class User {}
来源：http://eh.panjiajie.cn

Go:   type User struct { Name string }
来源：http://rd.yuntaijiaju.cn

Ruby: class User; end
来源：http://wi.shxzskj.cn

C#:   class User {}
来源：http://im.shxzukj.cn

[G02] 构造函数
来源：http://wy.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://zv.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://io.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ie.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://gs.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://he.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cv.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://gm.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://lm.shtwfgs.cn

[G03] 实例属性
来源：http://ar.521024.cn

Py:   self.name = "x"
来源：http://uc.szsharing.cn

PHP:  public string $name = "x";
来源：http://fp.hahajie.cn

JS:   this.name = "x";
来源：http://fl.asd995.cn

TS:   name: string = "x";
来源：http://uj.szsharing.cn

Java: private String name;
来源：http://mz.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cb.szxytkj.cn

Ruby: @name = "x"
来源：http://yi.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://fn.bjjhwx.cn

[G04] 定义方法
来源：http://qx.asd995.cn

Py:   def greet(self): return self.name
来源：http://ls.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://px.9csxet.cn

JS:   greet() { return this.name; }
来源：http://yz.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://un.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://no.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bb.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://dg.newstarts.cn

C#:   public string Greet() => Name;
来源：http://vr.jianghongdianzi.cn

[G05] 继承
来源：http://oi.panjiajie.cn

Py:   class Admin(User): pass
来源：http://zd.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://sj.szxytkj.cn

JS:   class Admin extends User {}
来源：http://sx.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://md.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://hk.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ti.hahajie.cn

Ruby: class Admin < User; end
来源：http://ke.huanxung.cn

C#:   class Admin : User {}
来源：http://kz.huanxung.cn

[G06] 重写方法
来源：http://hx.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://sa.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sm.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://zl.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://lg.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://da.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ar.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://al.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://rm.shtwfgs.cn

[G07] 调用父类方法
来源：http://wm.shxzskj.cn

Py:   super().greet()
来源：http://az.521024.cn

PHP:  parent::greet();
来源：http://lj.colortex.cn

JS:   super.greet();
来源：http://wd.jianghongdianzi.cn

TS:   super.greet();
来源：http://yu.shxzukj.cn

Java: super.greet();
来源：http://om.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gf.shxzskj.cn

Ruby: super
来源：http://lj.hahajie.cn

C#:   base.Greet();
来源：http://dt.shtwfgs.cn

[G08] 静态方法与属性
来源：http://bw.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gr.hnjuh.cn

PHP:  public static function f() {}
来源：http://gp.521024.cn

JS:   static f() {}
来源：http://nu.haigaiapp.cn

TS:   static f(): void {}
来源：http://qx.9csxet.cn

Java: static void f() {}
来源：http://vx.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fn.panjiajie.cn

Ruby: def self.f; end
来源：http://jk.huixiangedu.cn

C#:   public static void F() {}
来源：http://lc.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ud.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://ib.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vi.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aj.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://vz.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://fj.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://js.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ja.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://mh.szsharing.cn

[G10] 访问控制
来源：http://tz.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://vy.nicolike.cn

PHP:  public / protected / private
来源：http://mo.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://tv.huixinmuqiang.cn

TS:   public / protected / private
来源：http://au.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://ju.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ej.shxzukj.cn

Ruby: public / protected / private
来源：http://wn.nszjky.cn

C#:   public / protected / private / internal
来源：http://ob.jctech888.com.cn

[G11] getter / setter
来源：http://nh.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://fe.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ud.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://vf.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://mp.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://rt.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ny.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://cn.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://cd.hnjuh.cn

[G12] 对象转字符串
来源：http://ba.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://zm.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://th.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://rd.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://nf.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://yw.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eh.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://ou.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://we.panjiajie.cn

[G13] 判断对象类型
来源：http://el.szsharing.cn

Py:   isinstance(u, User)
来源：http://vb.shtwfgs.cn

PHP:  $u instanceof User
来源：http://zi.muxihuayi.cn

JS:   u instanceof User
来源：http://qc.szsharing.cn

TS:   u instanceof User
来源：http://yh.jctech888.com.cn


<!-- 参考信息 -->