代发 wailian999

Go:   strings.Count(s, "a")
来源：http://kw.yuexingan06.cn

Ruby: s.count("a")
来源：http://ev.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://zz.nszjky.cn

[E13] 逐字符遍历
来源：http://cp.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://si.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ds.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yb.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nx.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uz.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hh.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nv.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://og.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ns.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://td.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dj.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jq.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sj.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dt.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gd.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lv.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qe.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://sc.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ar.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nb.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mt.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bd.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ge.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iy.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hi.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wo.521024.cn

[E16] 数字千分位
来源：http://lo.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ev.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ur.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hv.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rk.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://be.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ve.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nw.521024.cn

C#:   1234567.ToString("N0")
来源：http://wj.huixinmuqiang.cn

[E17] 首字母大写
来源：http://xs.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mc.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eo.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vn.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qs.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dn.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ef.jctech888.com.cn

Ruby: s.capitalize
来源：http://fi.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mt.szxytkj.cn

[E18] 模板占位符替换
来源：http://hf.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hn.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nw.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ee.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fm.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yb.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aq.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ri.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ra.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://yo.bjjhwx.cn

Py:   s.splitlines()
来源：http://bf.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vf.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://wm.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://uc.hnjuh.cn

Java: s.lines().toList()
来源：http://bj.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://lg.jctech888.com.cn

Ruby: s.lines
来源：http://aj.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://my.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://rj.panjiajie.cn

Py:   if not s:
来源：http://gh.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gg.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sl.newstarts.cn

TS:   if (s === "") {}
来源：http://aj.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ya.jctech888.com.cn

Go:   if s == "" {}
来源：http://io.panjiajie.cn

Ruby: if s.empty?
来源：http://vn.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ay.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://lo.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uv.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qa.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nt.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ox.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://se.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ox.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bl.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gr.szsharing.cn

[E22] 字节长度与字符长度
来源：http://ok.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bs.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wn.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yz.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xj.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dw.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gz.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://cj.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rb.huixinmuqiang.cn

================================================================================
来源：http://ep.yuntaijiaju.cn

F. 文件与目录
来源：http://le.nicolike.cn

================================================================================
来源：http://za.chemitech.net.cn

[F01] 读取整个文件
来源：http://am.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://id.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://un.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://na.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ld.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jc.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gz.nszjky.cn

Ruby: File.read("a.txt")
来源：http://sl.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://rl.hahajie.cn

[F02] 逐行读取文件
来源：http://hq.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iw.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bw.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bl.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vl.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oc.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bm.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ql.521024.cn

[F03] 写入文件（覆盖）
来源：http://kc.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dl.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fs.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ok.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aj.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kx.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jy.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://iw.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://af.9csxet.cn

[F04] 追加写入文件
来源：http://ku.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kc.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jk.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uv.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xl.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pr.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rp.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ax.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zs.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://co.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bq.asd995.cn

PHP:  file_exists("a.txt");
来源：http://nu.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://yv.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://ae.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://os.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iw.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://zo.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://al.bjjhwx.cn

[F06] 删除文件
来源：http://kz.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://lh.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://zy.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wo.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kd.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qt.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://yu.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://uu.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://le.nicolike.cn

[F07] 创建目录（含多级）
来源：http://qi.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ff.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sf.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lu.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eh.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kn.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ys.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ms.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qb.huixiangedu.cn

[F08] 遍历目录
来源：http://go.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bv.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ed.521024.cn

JS:   fs.readdirSync("dir")
来源：http://qg.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://zs.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nr.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qa.colortex.cn

Ruby: Dir.children("dir")
来源：http://yk.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://ot.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://wk.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://bd.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://bb.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://cn.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://nb.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ar.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://is.newstarts.cn

Ruby: File.size("a.txt")
来源：http://eo.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://ey.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://qq.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ft.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ut.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ml.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://zc.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vd.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zj.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tp.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bc.wgjwhj.cn

[F11] 复制与移动文件
来源：http://vm.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xk.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hi.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tl.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wx.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://co.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ck.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fu.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ko.shtwfgs.cn

[F12] CSV 读写
来源：http://ee.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fk.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wp.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ck.szxytkj.cn

TS:   // 同上
来源：http://yk.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ga.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rj.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pq.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vj.bjjhwx.cn

================================================================================
来源：http://rj.shxzskj.cn

G. 面向对象
来源：http://vp.yuntaijiaju.cn

================================================================================
来源：http://ys.newstarts.cn

[G01] 定义类
来源：http://vq.shxzukj.cn

Py:   class User: pass
来源：http://oe.9csxet.cn

PHP:  class User {}
来源：http://ny.chemitech.net.cn

JS:   class User {}
来源：http://xu.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://tu.nicolike.cn

Java: class User {}
来源：http://wy.asd995.cn

Go:   type User struct { Name string }
来源：http://vj.nszjky.cn

Ruby: class User; end
来源：http://sp.nszjky.cn

C#:   class User {}
来源：http://sz.yuexingan06.cn

[G02] 构造函数
来源：http://zn.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://we.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://se.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ll.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://vw.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://xl.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://cl.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ml.lnxyls.cn

[G03] 实例属性
来源：http://so.wgjwhj.cn

Py:   self.name = "x"
来源：http://cl.nszjky.cn

PHP:  public string $name = "x";
来源：http://hv.newstarts.cn

JS:   this.name = "x";
来源：http://ws.shxzukj.cn

TS:   name: string = "x";
来源：http://gq.gzmigu.cn

Java: private String name;
来源：http://ez.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yn.haigaiapp.cn

Ruby: @name = "x"
来源：http://ju.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://pw.bjjhwx.cn

[G04] 定义方法
来源：http://fd.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://zm.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yg.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://im.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://al.jctech888.com.cn

Java: String greet() { return name; }
来源：http://jk.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://se.shxzukj.cn

Ruby: def greet; @name; end
来源：http://gb.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://fp.gzmigu.cn

[G05] 继承
来源：http://io.nicolike.cn

Py:   class Admin(User): pass
来源：http://hq.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://ex.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://ce.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://rd.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ax.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yq.shxzskj.cn

Ruby: class Admin < User; end
来源：http://pq.huixiangedu.cn

C#:   class Admin : User {}
来源：http://np.chemitech.net.cn

[G06] 重写方法
来源：http://is.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://bi.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qe.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://vq.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://dx.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://md.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wf.colortex.cn

Ruby: def greet; "admin"; end
来源：http://rl.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://ok.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://mx.panjiajie.cn

Py:   super().greet()
来源：http://sw.shxzukj.cn

PHP:  parent::greet();
来源：http://in.hnjuh.cn

JS:   super.greet();
来源：http://bc.huanxung.cn

TS:   super.greet();
来源：http://ju.9csxet.cn

Java: super.greet();
来源：http://zl.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://te.hnjuh.cn

Ruby: super
来源：http://yx.szsharing.cn

C#:   base.Greet();
来源：http://zr.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://vq.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zj.bjjhwx.cn

PHP:  public static function f() {}
来源：http://qp.gzmigu.cn

JS:   static f() {}
来源：http://rv.shxzukj.cn

TS:   static f(): void {}
来源：http://bq.asd995.cn

Java: static void f() {}
来源：http://hg.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rv.nszjky.cn

Ruby: def self.f; end
来源：http://bv.gzmigu.cn

C#:   public static void F() {}
来源：http://zf.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://iy.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://ps.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://es.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dp.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://yq.szsharing.cn

Java: interface Shape { double area(); }
来源：http://ri.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://dm.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ik.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://bz.huixiangedu.cn

[G10] 访问控制
来源：http://qc.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://lg.yuexingan06.cn

PHP:  public / protected / private
来源：http://hi.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ha.hnjuh.cn

TS:   public / protected / private
来源：http://hu.asd995.cn

Java: public / protected / private / 默认包级
来源：http://qw.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pf.yuexingan06.cn

Ruby: public / protected / private
来源：http://xs.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://tz.huixinmuqiang.cn

[G11] getter / setter
来源：http://bj.nszjky.cn

Py:   @property 与 @x.setter
来源：http://zm.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ea.jianghongdianzi.cn


<!-- 参考信息 -->