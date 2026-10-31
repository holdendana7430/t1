代发 wailian999

Ruby: s.reverse
来源：http://wl.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ki.newstarts.cn

[E12] 统计某字符出现次数
来源：http://fl.bjjhwx.cn

Py:   s.count("a")
来源：http://pw.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://yq.hahajie.cn

JS:   s.split("a").length - 1
来源：http://pe.nszjky.cn

TS:   s.split("a").length - 1
来源：http://yu.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uz.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://ik.shxzskj.cn

Ruby: s.count("a")
来源：http://nb.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ai.bjjhwx.cn

[E13] 逐字符遍历
来源：http://yc.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://xh.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hb.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wm.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fm.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bg.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jx.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ff.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://al.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://zl.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uz.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lf.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://re.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yn.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bs.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sw.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xt.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://av.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://ep.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jw.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nf.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qw.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ay.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oj.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cx.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ql.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eh.muxihuayi.cn

[E16] 数字千分位
来源：http://jz.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://iq.szxytkj.cn

PHP:  number_format(1234567);
来源：http://li.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ym.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://am.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iu.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dl.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://al.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://mj.huixiangedu.cn

[E17] 首字母大写
来源：http://yb.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iv.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bu.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zf.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qv.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://om.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ik.9csxet.cn

Ruby: s.capitalize
来源：http://sw.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yy.nszjky.cn

[E18] 模板占位符替换
来源：http://aj.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xz.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xi.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yq.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qv.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yr.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kz.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ji.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cl.521024.cn

[E19] 多行文本按行拆分
来源：http://sz.asd995.cn

Py:   s.splitlines()
来源：http://di.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ar.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://ut.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://kr.wgjwhj.cn

Java: s.lines().toList()
来源：http://rb.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://af.chemitech.net.cn

Ruby: s.lines
来源：http://gz.521024.cn

C#:   s.Split('\n')
来源：http://mi.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ly.jianghongdianzi.cn

Py:   if not s:
来源：http://ze.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://an.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wj.panjiajie.cn

TS:   if (s === "") {}
来源：http://lu.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://sh.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://tw.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://yo.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ar.lnxyls.cn

[E21] 超长截断加省略号
来源：http://gq.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iw.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sa.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pf.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yu.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kq.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ho.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://um.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ht.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://rg.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wy.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fm.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hf.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xc.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zw.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ol.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://rv.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jo.muxihuayi.cn

================================================================================
来源：http://ng.bookmarksfly.cn

F. 文件与目录
来源：http://hr.haigaiapp.cn

================================================================================
来源：http://px.shxzukj.cn

[F01] 读取整个文件
来源：http://ka.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://no.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://fm.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ja.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ue.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ry.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dx.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://bs.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://zv.jctech888.com.cn

[F02] 逐行读取文件
来源：http://gl.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uu.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bu.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ur.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gs.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dm.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://it.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mu.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dn.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://po.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uv.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ja.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kh.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://go.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iy.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://ir.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vi.chemitech.net.cn

[F04] 追加写入文件
来源：http://jg.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lf.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qn.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zx.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uw.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ld.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hf.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xf.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ce.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://eu.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fh.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://gz.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://fp.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://ae.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wo.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jg.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://eg.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ly.yuexingan06.cn

[F06] 删除文件
来源：http://rp.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://mz.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://be.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cd.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jw.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://is.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://sd.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://kh.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://oc.huanxung.cn

[F07] 创建目录（含多级）
来源：http://hz.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lv.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gr.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ag.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bb.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lj.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ur.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fu.huanxung.cn

[F08] 遍历目录
来源：http://gc.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zc.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hs.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://ls.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://qj.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sq.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hp.9csxet.cn

Ruby: Dir.children("dir")
来源：http://sq.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ov.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://sf.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://mj.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://yc.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://hi.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://yn.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sg.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wf.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://sl.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://sc.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://dw.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ol.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zf.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bd.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://cr.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oa.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wf.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ts.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.shtwfgs.cn

[F11] 复制与移动文件
来源：http://qa.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qd.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qc.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sz.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hs.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ey.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ev.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oj.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pr.yuexingan06.cn

[F12] CSV 读写
来源：http://da.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://it.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lc.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mx.hahajie.cn

TS:   // 同上
来源：http://tt.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zj.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sv.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://si.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mt.hnjuh.cn

================================================================================
来源：http://gb.newstarts.cn

G. 面向对象
来源：http://ni.jianghongdianzi.cn

================================================================================
来源：http://ex.colortex.cn

[G01] 定义类
来源：http://qh.bjjhwx.cn

Py:   class User: pass
来源：http://ak.shtwfgs.cn

PHP:  class User {}
来源：http://mo.szsharing.cn

JS:   class User {}
来源：http://iy.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://sy.jianghongdianzi.cn

Java: class User {}
来源：http://vc.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://bi.jianghongdianzi.cn

Ruby: class User; end
来源：http://gj.bjjhwx.cn

C#:   class User {}
来源：http://mz.shtwfgs.cn

[G02] 构造函数
来源：http://py.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ys.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://pg.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://kf.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://px.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ee.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fm.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://cu.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://pt.szsharing.cn

[G03] 实例属性
来源：http://lj.yuexingan06.cn

Py:   self.name = "x"
来源：http://hf.hahajie.cn

PHP:  public string $name = "x";
来源：http://gn.gzmigu.cn

JS:   this.name = "x";
来源：http://ok.bookmarksfly.cn

TS:   name: string = "x";
来源：http://tg.yuntaijiaju.cn

Java: private String name;
来源：http://je.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cm.panjiajie.cn

Ruby: @name = "x"
来源：http://qt.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://jk.521024.cn

[G04] 定义方法
来源：http://yo.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vs.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gm.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://se.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://wp.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ij.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oq.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://fe.9csxet.cn

C#:   public string Greet() => Name;
来源：http://mc.shxzukj.cn

[G05] 继承
来源：http://xz.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://zp.nicolike.cn

PHP:  class Admin extends User {}
来源：http://tp.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://aw.521024.cn

TS:   class Admin extends User {}
来源：http://qt.colortex.cn

Java: class Admin extends User {}
来源：http://up.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uf.nicolike.cn

Ruby: class Admin < User; end
来源：http://sj.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ms.hahajie.cn

[G06] 重写方法
来源：http://mq.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://nc.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gl.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://hh.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ss.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://di.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ha.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://sj.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://ah.shxzskj.cn

[G07] 调用父类方法
来源：http://ki.shtwfgs.cn

Py:   super().greet()
来源：http://ev.shtwfgs.cn

PHP:  parent::greet();
来源：http://bm.szxytkj.cn

JS:   super.greet();
来源：http://th.shxzskj.cn

TS:   super.greet();
来源：http://te.nszjky.cn

Java: super.greet();
来源：http://ul.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mn.muxihuayi.cn

Ruby: super
来源：http://da.lnxyls.cn

C#:   base.Greet();
来源：http://lj.shxzskj.cn

[G08] 静态方法与属性
来源：http://jb.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://au.chemitech.net.cn

PHP:  public static function f() {}
来源：http://eu.huixinmuqiang.cn

JS:   static f() {}
来源：http://gj.shxzukj.cn

TS:   static f(): void {}
来源：http://fg.muxihuayi.cn

Java: static void f() {}
来源：http://ki.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ju.hnjuh.cn

Ruby: def self.f; end
来源：http://xf.gzmigu.cn

C#:   public static void F() {}
来源：http://yy.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://cc.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://lz.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mf.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yw.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://wc.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://vh.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wj.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://he.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://kn.shxzukj.cn

[G10] 访问控制
来源：http://xg.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://qp.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://es.nszjky.cn

JS:   #private 字段；其余公开
来源：http://pn.huixinmuqiang.cn


<!-- 参考信息 -->