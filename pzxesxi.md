代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gm.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://as.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gb.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nk.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://no.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tf.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://md.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qa.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yf.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zc.yuexingan06.cn

[E16] 数字千分位
来源：http://os.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://pg.szsharing.cn

PHP:  number_format(1234567);
来源：http://ik.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ka.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pz.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xw.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zf.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://ew.hnjuh.cn

[E17] 首字母大写
来源：http://wm.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qh.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://so.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qg.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://if.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ks.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vn.muxihuayi.cn

Ruby: s.capitalize
来源：http://qy.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hw.shxzukj.cn

[E18] 模板占位符替换
来源：http://xn.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kc.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://np.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://km.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ym.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hs.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ly.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cz.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qx.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ky.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://bp.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cl.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://qd.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://vt.shxzskj.cn

Java: s.lines().toList()
来源：http://ij.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://hx.nszjky.cn

Ruby: s.lines
来源：http://lh.muxihuayi.cn

C#:   s.Split('\n')
来源：http://vy.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://du.nszjky.cn

Py:   if not s:
来源：http://jc.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ga.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vr.nszjky.cn

TS:   if (s === "") {}
来源：http://zl.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://zj.gzmigu.cn

Go:   if s == "" {}
来源：http://pw.yuexingan06.cn

Ruby: if s.empty?
来源：http://ch.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://xv.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cw.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mi.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ov.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jv.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ue.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://tp.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wx.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rz.nicolike.cn

[E22] 字节长度与字符长度
来源：http://zs.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kb.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lb.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vh.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ns.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tb.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://th.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://cs.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ry.panjiajie.cn

================================================================================
来源：http://gy.hnjuh.cn

F. 文件与目录
来源：http://bz.yuexingan06.cn

================================================================================
来源：http://ay.szxytkj.cn

[F01] 读取整个文件
来源：http://hg.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vd.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://fm.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kf.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vi.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vb.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xm.9csxet.cn

Ruby: File.read("a.txt")
来源：http://qf.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://vp.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ew.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dw.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jv.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ax.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hh.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ah.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kh.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jz.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ko.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://sm.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yl.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xh.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://md.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ns.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yo.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lu.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zm.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ka.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ot.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://by.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fj.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://av.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cn.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sa.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nm.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xu.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hs.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ch.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aq.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ac.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://oy.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://wd.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://as.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://il.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://dj.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ro.asd995.cn

[F06] 删除文件
来源：http://fo.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://sj.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://rs.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pl.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xt.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ir.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ij.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://xt.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://ma.nicolike.cn

[F07] 创建目录（含多级）
来源：http://qz.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lf.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wx.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cn.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lm.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fx.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cf.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://os.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gc.521024.cn

[F08] 遍历目录
来源：http://un.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://re.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nj.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://tw.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ni.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iv.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oi.szsharing.cn

Ruby: Dir.children("dir")
来源：http://za.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://zo.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://no.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://sq.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://wu.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://pf.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://zp.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ja.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jp.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://vg.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://cb.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://bd.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bf.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vj.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ke.9csxet.cn

TS:   path.extname("a.txt")
来源：http://ew.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gn.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fd.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cq.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qc.bjjhwx.cn

[F11] 复制与移动文件
来源：http://xu.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ak.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://de.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jc.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qb.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dx.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nu.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vu.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iq.shxzukj.cn

[F12] CSV 读写
来源：http://zu.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ax.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wx.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rt.hnjuh.cn

TS:   // 同上
来源：http://oe.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bt.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tr.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iv.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fb.521024.cn

================================================================================
来源：http://vc.huanxung.cn

G. 面向对象
来源：http://hf.nicolike.cn

================================================================================
来源：http://bo.muxihuayi.cn

[G01] 定义类
来源：http://py.nicolike.cn

Py:   class User: pass
来源：http://yh.panjiajie.cn

PHP:  class User {}
来源：http://wb.hahajie.cn

JS:   class User {}
来源：http://jm.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://zw.haigaiapp.cn

Java: class User {}
来源：http://fn.asd995.cn

Go:   type User struct { Name string }
来源：http://kj.haigaiapp.cn

Ruby: class User; end
来源：http://ta.bookmarksfly.cn

C#:   class User {}
来源：http://fc.nszjky.cn

[G02] 构造函数
来源：http://wg.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://bs.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://je.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://qv.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://qd.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://fj.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fs.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://ae.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://eo.yuntaijiaju.cn

[G03] 实例属性
来源：http://ga.muxihuayi.cn

Py:   self.name = "x"
来源：http://tx.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://cv.newstarts.cn

JS:   this.name = "x";
来源：http://hq.colortex.cn

TS:   name: string = "x";
来源：http://mk.yuntaijiaju.cn

Java: private String name;
来源：http://wt.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ls.panjiajie.cn

Ruby: @name = "x"
来源：http://xj.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://qk.gzmigu.cn

[G04] 定义方法
来源：http://vv.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://uw.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wr.asd995.cn

JS:   greet() { return this.name; }
来源：http://cz.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://jx.shxzskj.cn

Java: String greet() { return name; }
来源：http://ux.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mn.colortex.cn

Ruby: def greet; @name; end
来源：http://ud.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://yd.shxzukj.cn

[G05] 继承
来源：http://yx.lnxyls.cn

Py:   class Admin(User): pass
来源：http://rp.szsharing.cn

PHP:  class Admin extends User {}
来源：http://im.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://lw.hahajie.cn

TS:   class Admin extends User {}
来源：http://pi.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://ls.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zq.asd995.cn

Ruby: class Admin < User; end
来源：http://xc.shxzukj.cn

C#:   class Admin : User {}
来源：http://xu.hahajie.cn

[G06] 重写方法
来源：http://pq.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://lb.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nx.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://ce.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://qs.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://nl.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://em.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://pr.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://rj.bookmarksfly.cn

[G07] 调用父类方法
来源：http://rv.newstarts.cn

Py:   super().greet()
来源：http://jp.chemitech.net.cn

PHP:  parent::greet();
来源：http://mo.yuexingan06.cn

JS:   super.greet();
来源：http://fo.nszjky.cn

TS:   super.greet();
来源：http://jw.huanxung.cn

Java: super.greet();
来源：http://ez.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fq.bjjhwx.cn

Ruby: super
来源：http://hs.huanxung.cn

C#:   base.Greet();
来源：http://xi.nszjky.cn

[G08] 静态方法与属性
来源：http://ed.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nq.jctech888.com.cn

PHP:  public static function f() {}
来源：http://yf.asd995.cn

JS:   static f() {}
来源：http://gw.yuexingan06.cn

TS:   static f(): void {}
来源：http://dt.gzmigu.cn

Java: static void f() {}
来源：http://zq.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ms.shtwfgs.cn

Ruby: def self.f; end
来源：http://cz.bjjhwx.cn

C#:   public static void F() {}
来源：http://cu.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://yq.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://vs.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zv.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://if.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://mx.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://dn.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ci.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://my.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://pe.521024.cn

[G10] 访问控制
来源：http://dr.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://tz.521024.cn

PHP:  public / protected / private
来源：http://fq.nicolike.cn

JS:   #private 字段；其余公开
来源：http://xo.yuntaijiaju.cn

TS:   public / protected / private
来源：http://ba.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://om.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ly.muxihuayi.cn

Ruby: public / protected / private
来源：http://cl.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://md.muxihuayi.cn

[G11] getter / setter
来源：http://zz.huanxung.cn

Py:   @property 与 @x.setter
来源：http://sz.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ez.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://fn.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://zq.hnjuh.cn

Java: public String getName() { return name; }
来源：http://gg.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jn.lnxyls.cn

Ruby: attr_accessor :name
来源：http://am.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://md.bookmarksfly.cn

[G12] 对象转字符串
来源：http://az.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://yx.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dl.521024.cn

JS:   toString() { return this.name; }
来源：http://sa.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://zi.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://or.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jt.colortex.cn

Ruby: def to_s; @name; end
来源：http://kb.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://xl.panjiajie.cn

[G13] 判断对象类型
来源：http://in.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://xo.bjjhwx.cn

PHP:  $u instanceof User
来源：http://zu.jctech888.com.cn

JS:   u instanceof User
来源：http://av.jctech888.com.cn

TS:   u instanceof User
来源：http://ry.panjiajie.cn


<!-- 参考信息 -->