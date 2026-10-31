代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vi.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xy.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dr.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ej.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ij.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://bx.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zh.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uf.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://me.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nz.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tv.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cf.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nx.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ez.haigaiapp.cn

[E16] 数字千分位
来源：http://ip.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://bo.nszjky.cn

PHP:  number_format(1234567);
来源：http://wo.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hh.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zy.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vs.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yz.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ri.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://be.hnjuh.cn

[E17] 首字母大写
来源：http://cd.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vg.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xh.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zl.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jq.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nh.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://je.521024.cn

Ruby: s.capitalize
来源：http://pu.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yp.haigaiapp.cn

[E18] 模板占位符替换
来源：http://xe.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sa.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hs.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ul.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://te.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mn.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://an.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sp.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tl.asd995.cn

[E19] 多行文本按行拆分
来源：http://dt.jctech888.com.cn

Py:   s.splitlines()
来源：http://dc.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tw.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://wh.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://ua.colortex.cn

Java: s.lines().toList()
来源：http://lz.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://oi.nicolike.cn

Ruby: s.lines
来源：http://jr.shxzukj.cn

C#:   s.Split('\n')
来源：http://so.newstarts.cn

[E20] 判断字符串是否为空
来源：http://eu.hnjuh.cn

Py:   if not s:
来源：http://qa.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dv.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fj.9csxet.cn

TS:   if (s === "") {}
来源：http://xm.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://rh.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://kc.colortex.cn

Ruby: if s.empty?
来源：http://os.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cl.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://dz.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nz.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nj.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sh.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jx.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pq.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://lm.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ao.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eo.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://ot.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yz.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hv.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jj.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://di.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oa.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://wq.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ke.haigaiapp.cn

================================================================================
来源：http://ps.newstarts.cn

F. 文件与目录
来源：http://yx.hahajie.cn

================================================================================
来源：http://sp.shxzukj.cn

[F01] 读取整个文件
来源：http://mn.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ti.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://br.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://im.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nf.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sz.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ta.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://jo.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://iw.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://vw.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bb.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bz.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mn.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wm.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bt.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yr.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tu.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gv.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://xz.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hf.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://en.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pm.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ch.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bw.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vf.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ht.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ig.gzmigu.cn

[F04] 追加写入文件
来源：http://nr.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mf.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ph.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ch.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rv.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aw.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zm.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hw.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fi.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://nh.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://se.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ae.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://cr.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://rg.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tu.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ac.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://yg.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://fo.yuntaijiaju.cn

[F06] 删除文件
来源：http://rl.asd995.cn

Py:   os.remove("a.txt")
来源：http://rx.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://op.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jf.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kg.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ia.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://hd.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://cx.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://mw.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://mj.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dw.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ix.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cp.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jw.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ev.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://il.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qe.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ya.wgjwhj.cn

[F08] 遍历目录
来源：http://at.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fp.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://er.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://sz.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://io.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fs.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cm.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://gf.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://wl.huanxung.cn

[F09] 获取文件大小
来源：http://zp.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://lt.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://nq.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://ng.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://mt.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://si.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kd.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://iq.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://bi.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://qm.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://on.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wq.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qw.9csxet.cn

TS:   path.extname("a.txt")
来源：http://iw.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zt.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dp.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aw.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ke.hnjuh.cn

[F11] 复制与移动文件
来源：http://xy.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://so.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hw.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hx.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aw.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fr.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tz.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uz.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lw.jctech888.com.cn

[F12] CSV 读写
来源：http://dp.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ge.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oq.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ok.shxzukj.cn

TS:   // 同上
来源：http://kj.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mr.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tr.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xo.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gf.lnxyls.cn

================================================================================
来源：http://ov.asd995.cn

G. 面向对象
来源：http://yl.hnjuh.cn

================================================================================
来源：http://fz.shtwfgs.cn

[G01] 定义类
来源：http://tu.lnxyls.cn

Py:   class User: pass
来源：http://bo.jianghongdianzi.cn

PHP:  class User {}
来源：http://wg.hahajie.cn

JS:   class User {}
来源：http://kv.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://gl.nicolike.cn

Java: class User {}
来源：http://ku.panjiajie.cn

Go:   type User struct { Name string }
来源：http://za.nicolike.cn

Ruby: class User; end
来源：http://lc.szxytkj.cn

C#:   class User {}
来源：http://xt.huixinmuqiang.cn

[G02] 构造函数
来源：http://vi.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://eo.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://vn.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://md.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://lo.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://rn.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lu.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://ln.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ey.521024.cn

[G03] 实例属性
来源：http://sp.haigaiapp.cn

Py:   self.name = "x"
来源：http://qe.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://xf.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://dt.hnjuh.cn

TS:   name: string = "x";
来源：http://is.huanxung.cn

Java: private String name;
来源：http://ch.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tt.jctech888.com.cn

Ruby: @name = "x"
来源：http://km.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://gd.shtwfgs.cn

[G04] 定义方法
来源：http://ce.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://iu.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://db.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://xq.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://mg.nszjky.cn

Java: String greet() { return name; }
来源：http://hh.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ep.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://yk.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://bd.newstarts.cn

[G05] 继承
来源：http://bs.colortex.cn

Py:   class Admin(User): pass
来源：http://dr.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://th.szsharing.cn

JS:   class Admin extends User {}
来源：http://lj.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://nt.shxzukj.cn

Java: class Admin extends User {}
来源：http://ud.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wg.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://oi.521024.cn

C#:   class Admin : User {}
来源：http://nt.huixinmuqiang.cn

[G06] 重写方法
来源：http://lm.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://cb.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rq.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://vo.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://gn.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://by.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yc.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://zc.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://li.shxzukj.cn

[G07] 调用父类方法
来源：http://zi.nicolike.cn

Py:   super().greet()
来源：http://ye.bjjhwx.cn

PHP:  parent::greet();
来源：http://my.gzmigu.cn

JS:   super.greet();
来源：http://et.yuntaijiaju.cn

TS:   super.greet();
来源：http://tu.panjiajie.cn

Java: super.greet();
来源：http://xl.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rj.szsharing.cn

Ruby: super
来源：http://qk.panjiajie.cn

C#:   base.Greet();
来源：http://yz.shxzukj.cn

[G08] 静态方法与属性
来源：http://qm.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ka.newstarts.cn

PHP:  public static function f() {}
来源：http://dk.lnxyls.cn

JS:   static f() {}
来源：http://et.lnxyls.cn

TS:   static f(): void {}
来源：http://zq.huixiangedu.cn

Java: static void f() {}
来源：http://jw.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xr.hnjuh.cn

Ruby: def self.f; end
来源：http://ar.521024.cn

C#:   public static void F() {}
来源：http://fy.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://mv.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://xe.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ly.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hu.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://cx.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://un.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://am.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xw.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://no.gzmigu.cn

[G10] 访问控制
来源：http://yj.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://si.jctech888.com.cn

PHP:  public / protected / private
来源：http://xu.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://bi.muxihuayi.cn

TS:   public / protected / private
来源：http://mz.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://uo.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yz.bjjhwx.cn

Ruby: public / protected / private
来源：http://wz.szsharing.cn

C#:   public / protected / private / internal
来源：http://so.9csxet.cn

[G11] getter / setter
来源：http://po.huanxung.cn

Py:   @property 与 @x.setter
来源：http://vn.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fa.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://io.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://fx.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ui.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xw.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ck.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://xm.szxytkj.cn

[G12] 对象转字符串
来源：http://lx.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://oi.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yo.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://qs.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://fn.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ay.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xx.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ru.521024.cn

C#:   public override string ToString() => Name;
来源：http://ek.521024.cn

[G13] 判断对象类型
来源：http://ul.bookmarksfly.cn


<!-- 参考信息 -->