代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fv.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ou.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iw.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ri.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xp.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sh.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dn.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://is.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zc.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bj.lnxyls.cn

[E16] 数字千分位
来源：http://yk.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://nw.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ts.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sw.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rf.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nr.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cw.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kc.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://lt.shtwfgs.cn

[E17] 首字母大写
来源：http://gy.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cb.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ey.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ia.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uf.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ez.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rk.lnxyls.cn

Ruby: s.capitalize
来源：http://ce.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tp.521024.cn

[E18] 模板占位符替换
来源：http://jh.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lu.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uv.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://te.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qp.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://di.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bv.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sy.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xx.huanxung.cn

[E19] 多行文本按行拆分
来源：http://fy.hahajie.cn

Py:   s.splitlines()
来源：http://ek.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rz.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://jn.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://ix.9csxet.cn

Java: s.lines().toList()
来源：http://st.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ir.newstarts.cn

Ruby: s.lines
来源：http://oa.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://yw.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://df.nicolike.cn

Py:   if not s:
来源：http://rp.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fe.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mq.gzmigu.cn

TS:   if (s === "") {}
来源：http://aj.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://pq.yuexingan06.cn

Go:   if s == "" {}
来源：http://ar.nszjky.cn

Ruby: if s.empty?
来源：http://ct.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zx.nszjky.cn

[E21] 超长截断加省略号
来源：http://ww.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ea.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hk.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sp.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yp.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jx.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://bk.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://or.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ru.newstarts.cn

[E22] 字节长度与字符长度
来源：http://qx.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://li.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xc.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mk.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zk.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aj.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dq.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://pe.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://yd.shtwfgs.cn

F. 文件与目录
来源：http://jg.asd995.cn

================================================================================
来源：http://lp.muxihuayi.cn

[F01] 读取整个文件
来源：http://jy.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uh.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://lz.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dk.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gi.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vt.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ty.huanxung.cn

Ruby: File.read("a.txt")
来源：http://px.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://ib.nicolike.cn

[F02] 逐行读取文件
来源：http://un.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://on.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ja.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hw.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mk.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yg.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wf.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oi.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ae.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://xx.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jx.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hf.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ss.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ju.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://go.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ag.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://az.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ba.521024.cn

[F04] 追加写入文件
来源：http://nj.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://we.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mc.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sy.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ic.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pi.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dk.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mr.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pz.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://cp.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kt.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://lv.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://wl.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://ok.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ye.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ux.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://uk.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://jc.huanxung.cn

[F06] 删除文件
来源：http://en.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://lf.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ko.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ti.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zw.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eo.521024.cn

Go:   os.Remove("a.txt")
来源：http://aa.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://hl.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://rg.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://cm.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zv.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hx.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ov.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tl.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yc.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://na.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lz.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.nszjky.cn

[F08] 遍历目录
来源：http://ys.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tb.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tj.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ru.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://gg.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bi.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lj.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://vh.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://vl.hnjuh.cn

[F09] 获取文件大小
来源：http://on.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://ce.szsharing.cn

PHP:  filesize("a.txt");
来源：http://fo.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://cp.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://px.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ou.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://km.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://kg.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://qm.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://ih.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ls.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hb.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vk.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://gt.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fw.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tx.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zm.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ru.szsharing.cn

[F11] 复制与移动文件
来源：http://cm.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sa.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gd.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qr.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ni.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ue.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tf.yuntaijiaju.cn

[F12] CSV 读写
来源：http://gd.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tr.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hc.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vt.hnjuh.cn

TS:   // 同上
来源：http://it.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gu.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bk.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qv.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zb.lnxyls.cn

================================================================================
来源：http://ex.shxzukj.cn

G. 面向对象
来源：http://gk.panjiajie.cn

================================================================================
来源：http://fo.huixinmuqiang.cn

[G01] 定义类
来源：http://xe.9csxet.cn

Py:   class User: pass
来源：http://yf.521024.cn

PHP:  class User {}
来源：http://nj.huixinmuqiang.cn

JS:   class User {}
来源：http://zb.colortex.cn

TS:   class User { name: string = ""; }
来源：http://lx.9csxet.cn

Java: class User {}
来源：http://yo.gzmigu.cn

Go:   type User struct { Name string }
来源：http://wy.521024.cn

Ruby: class User; end
来源：http://ph.huixinmuqiang.cn

C#:   class User {}
来源：http://ao.huixinmuqiang.cn

[G02] 构造函数
来源：http://kv.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://ar.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ou.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://iu.521024.cn

TS:   constructor(public name: string) {}
来源：http://ql.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://zb.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nj.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://lm.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://uh.gzmigu.cn

[G03] 实例属性
来源：http://tt.huanxung.cn

Py:   self.name = "x"
来源：http://ez.9csxet.cn

PHP:  public string $name = "x";
来源：http://ur.chemitech.net.cn

JS:   this.name = "x";
来源：http://dr.huanxung.cn

TS:   name: string = "x";
来源：http://vq.gzmigu.cn

Java: private String name;
来源：http://dg.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dd.nszjky.cn

Ruby: @name = "x"
来源：http://la.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://rq.bookmarksfly.cn

[G04] 定义方法
来源：http://on.huanxung.cn

Py:   def greet(self): return self.name
来源：http://xa.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xp.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://nn.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://ex.huanxung.cn

Java: String greet() { return name; }
来源：http://am.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yz.szsharing.cn

Ruby: def greet; @name; end
来源：http://ov.nszjky.cn

C#:   public string Greet() => Name;
来源：http://fs.haigaiapp.cn

[G05] 继承
来源：http://ak.szxytkj.cn

Py:   class Admin(User): pass
来源：http://nl.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://fh.nszjky.cn

JS:   class Admin extends User {}
来源：http://zy.newstarts.cn

TS:   class Admin extends User {}
来源：http://yi.hahajie.cn

Java: class Admin extends User {}
来源：http://xk.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xm.szxytkj.cn

Ruby: class Admin < User; end
来源：http://lk.jctech888.com.cn

C#:   class Admin : User {}
来源：http://rj.shxzskj.cn

[G06] 重写方法
来源：http://cp.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://gs.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://px.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://er.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://hz.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ig.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://co.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://wg.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://wl.huixiangedu.cn

[G07] 调用父类方法
来源：http://wu.jctech888.com.cn

Py:   super().greet()
来源：http://sz.shxzskj.cn

PHP:  parent::greet();
来源：http://an.chemitech.net.cn

JS:   super.greet();
来源：http://dh.szxytkj.cn

TS:   super.greet();
来源：http://go.haigaiapp.cn

Java: super.greet();
来源：http://wd.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fw.bjjhwx.cn

Ruby: super
来源：http://tl.bjjhwx.cn

C#:   base.Greet();
来源：http://fp.asd995.cn

[G08] 静态方法与属性
来源：http://ib.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zz.szsharing.cn

PHP:  public static function f() {}
来源：http://or.gzmigu.cn

JS:   static f() {}
来源：http://pk.521024.cn

TS:   static f(): void {}
来源：http://bv.huixinmuqiang.cn

Java: static void f() {}
来源：http://dc.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eo.lnxyls.cn

Ruby: def self.f; end
来源：http://hv.9csxet.cn

C#:   public static void F() {}
来源：http://id.newstarts.cn

[G09] 接口 / 抽象类
来源：http://xh.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://dc.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hk.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mc.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://yt.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://yu.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://pz.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vo.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://rg.shtwfgs.cn

[G10] 访问控制
来源：http://mg.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://mp.nicolike.cn

PHP:  public / protected / private
来源：http://fx.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://lk.shxzukj.cn

TS:   public / protected / private
来源：http://tx.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://go.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gz.hahajie.cn

Ruby: public / protected / private
来源：http://ki.9csxet.cn

C#:   public / protected / private / internal
来源：http://jx.gzmigu.cn

[G11] getter / setter
来源：http://xy.nszjky.cn

Py:   @property 与 @x.setter
来源：http://ds.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bm.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://mr.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://zp.9csxet.cn

Java: public String getName() { return name; }
来源：http://kp.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tv.9csxet.cn

Ruby: attr_accessor :name
来源：http://vs.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://rk.huixiangedu.cn

[G12] 对象转字符串
来源：http://jg.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://fa.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nm.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://yb.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://li.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://jd.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hj.hahajie.cn

Ruby: def to_s; @name; end
来源：http://uh.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://pc.bookmarksfly.cn

[G13] 判断对象类型
来源：http://eh.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://wf.huanxung.cn

PHP:  $u instanceof User
来源：http://ms.jianghongdianzi.cn

JS:   u instanceof User
来源：http://pe.gzmigu.cn

TS:   u instanceof User
来源：http://zh.gzmigu.cn


<!-- 参考信息 -->