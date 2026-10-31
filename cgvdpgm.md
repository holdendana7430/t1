代发 wailian999

PHP:  substr_count($s, "a");
来源：http://gj.asd995.cn

JS:   s.split("a").length - 1
来源：http://jv.hahajie.cn

TS:   s.split("a").length - 1
来源：http://au.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aq.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://ac.521024.cn

Ruby: s.count("a")
来源：http://rg.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://yw.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://gv.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://zm.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bx.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vs.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pf.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://po.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bb.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vc.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ef.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://no.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rc.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zn.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://py.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ef.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qe.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ew.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pt.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://el.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://fl.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gz.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dm.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ru.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cd.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rd.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jo.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zt.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qm.yuntaijiaju.cn

[E16] 数字千分位
来源：http://qt.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ip.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://sr.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gm.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pf.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uq.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ej.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nt.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://yi.szxytkj.cn

[E17] 首字母大写
来源：http://jo.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yp.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nl.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cn.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yb.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cd.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rs.asd995.cn

Ruby: s.capitalize
来源：http://bu.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qe.shtwfgs.cn

[E18] 模板占位符替换
来源：http://ec.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bt.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://am.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zy.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hg.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aa.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wy.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bv.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ru.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://op.haigaiapp.cn

Py:   s.splitlines()
来源：http://tq.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pi.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://yq.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://vm.haigaiapp.cn

Java: s.lines().toList()
来源：http://oz.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://wt.lnxyls.cn

Ruby: s.lines
来源：http://wy.haigaiapp.cn

C#:   s.Split('\n')
来源：http://fu.nszjky.cn

[E20] 判断字符串是否为空
来源：http://gc.muxihuayi.cn

Py:   if not s:
来源：http://jq.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rf.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://so.haigaiapp.cn

TS:   if (s === "") {}
来源：http://vz.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://jq.hahajie.cn

Go:   if s == "" {}
来源：http://mi.huixiangedu.cn

Ruby: if s.empty?
来源：http://uj.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cu.szxytkj.cn

[E21] 超长截断加省略号
来源：http://qr.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zl.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jq.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gw.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zf.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oy.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ad.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qg.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jr.newstarts.cn

[E22] 字节长度与字符长度
来源：http://bz.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kw.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ty.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dq.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jy.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bk.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pk.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ms.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vr.lnxyls.cn

================================================================================
来源：http://co.shtwfgs.cn

F. 文件与目录
来源：http://is.colortex.cn

================================================================================
来源：http://ri.haigaiapp.cn

[F01] 读取整个文件
来源：http://dz.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uk.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://js.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lr.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qd.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sx.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dq.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://af.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ax.colortex.cn

[F02] 逐行读取文件
来源：http://yg.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fs.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wf.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ng.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ae.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ov.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hu.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nv.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://fc.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rf.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ub.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zm.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nn.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hd.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aj.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://yu.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://os.szsharing.cn

[F04] 追加写入文件
来源：http://ap.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wu.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kv.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wd.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yx.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hl.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cn.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ay.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ii.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://xj.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ob.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ye.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://tq.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://by.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://en.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dw.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://tm.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://pp.wgjwhj.cn

[F06] 删除文件
来源：http://jc.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://mv.asd995.cn

PHP:  unlink("a.txt");
来源：http://sw.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vo.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://db.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fr.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://bm.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://ga.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://nb.szsharing.cn

[F07] 创建目录（含多级）
来源：http://gc.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cq.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ya.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zj.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mi.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://si.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mb.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mi.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qk.shtwfgs.cn

[F08] 遍历目录
来源：http://jw.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://td.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ru.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ej.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://be.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ux.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xh.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ys.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://cz.nszjky.cn

[F09] 获取文件大小
来源：http://vg.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ai.nszjky.cn

PHP:  filesize("a.txt");
来源：http://md.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://to.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://cd.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ic.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rd.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://pr.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://pe.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://jd.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bp.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yj.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yj.colortex.cn

TS:   path.extname("a.txt")
来源：http://xu.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cc.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lz.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lu.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://he.colortex.cn

[F11] 复制与移动文件
来源：http://lb.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cw.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ri.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ij.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lj.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mk.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mi.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ta.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pt.chemitech.net.cn

[F12] CSV 读写
来源：http://kv.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rg.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gc.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mb.yuntaijiaju.cn

TS:   // 同上
来源：http://ee.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kh.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zq.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dn.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eb.asd995.cn

================================================================================
来源：http://tv.huanxung.cn

G. 面向对象
来源：http://uj.huixiangedu.cn

================================================================================
来源：http://vy.shtwfgs.cn

[G01] 定义类
来源：http://nf.nszjky.cn

Py:   class User: pass
来源：http://qi.hnjuh.cn

PHP:  class User {}
来源：http://ir.lnxyls.cn

JS:   class User {}
来源：http://wi.asd995.cn

TS:   class User { name: string = ""; }
来源：http://wm.huixiangedu.cn

Java: class User {}
来源：http://rd.szsharing.cn

Go:   type User struct { Name string }
来源：http://pr.hahajie.cn

Ruby: class User; end
来源：http://at.gzmigu.cn

C#:   class User {}
来源：http://nx.wgjwhj.cn

[G02] 构造函数
来源：http://oe.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://kv.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://fr.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://az.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://ev.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ee.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ku.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://hm.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://yb.wgjwhj.cn

[G03] 实例属性
来源：http://bn.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://qm.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://nx.shxzukj.cn

JS:   this.name = "x";
来源：http://nk.9csxet.cn

TS:   name: string = "x";
来源：http://jt.jianghongdianzi.cn

Java: private String name;
来源：http://fm.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zg.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://zo.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://qf.yuntaijiaju.cn

[G04] 定义方法
来源：http://zm.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://fi.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://av.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://oq.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://fe.asd995.cn

Java: String greet() { return name; }
来源：http://iy.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gr.huanxung.cn

Ruby: def greet; @name; end
来源：http://oe.asd995.cn

C#:   public string Greet() => Name;
来源：http://dw.asd995.cn

[G05] 继承
来源：http://lv.shxzukj.cn

Py:   class Admin(User): pass
来源：http://yn.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://kx.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://qz.gzmigu.cn

TS:   class Admin extends User {}
来源：http://it.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://mn.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ok.lnxyls.cn

Ruby: class Admin < User; end
来源：http://tm.lnxyls.cn

C#:   class Admin : User {}
来源：http://nn.asd995.cn

[G06] 重写方法
来源：http://vs.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://el.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yp.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://fk.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://io.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://lh.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oo.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ps.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://jp.haigaiapp.cn

[G07] 调用父类方法
来源：http://oq.asd995.cn

Py:   super().greet()
来源：http://qi.bookmarksfly.cn

PHP:  parent::greet();
来源：http://db.yuexingan06.cn

JS:   super.greet();
来源：http://cv.muxihuayi.cn

TS:   super.greet();
来源：http://hw.haigaiapp.cn

Java: super.greet();
来源：http://kp.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uq.asd995.cn

Ruby: super
来源：http://ze.shxzskj.cn

C#:   base.Greet();
来源：http://eg.hahajie.cn

[G08] 静态方法与属性
来源：http://wn.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vf.yuexingan06.cn

PHP:  public static function f() {}
来源：http://mp.shtwfgs.cn

JS:   static f() {}
来源：http://hg.muxihuayi.cn

TS:   static f(): void {}
来源：http://di.yuexingan06.cn

Java: static void f() {}
来源：http://sr.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bx.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://gg.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://ym.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://be.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://yn.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vs.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ji.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://pc.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://eo.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://go.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hc.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://ro.szxytkj.cn

[G10] 访问控制
来源：http://nv.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ay.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://hu.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://uj.521024.cn

TS:   public / protected / private
来源：http://wy.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://nq.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vi.muxihuayi.cn

Ruby: public / protected / private
来源：http://qv.muxihuayi.cn


<!-- 参考信息 -->