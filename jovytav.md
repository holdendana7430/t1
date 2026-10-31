代发 wailian999

Py:   for ch in s: print(ch)
来源：http://rw.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zb.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mf.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yt.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yv.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tf.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fr.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sn.nszjky.cn

[E14] URL 编码与 Base64
来源：http://qm.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yz.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ej.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ir.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ly.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fr.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ro.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yt.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ag.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://gk.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fv.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zh.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://su.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://id.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tf.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://do.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yq.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zt.yuexingan06.cn

[E16] 数字千分位
来源：http://xe.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://zs.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://bg.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fe.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://we.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iy.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hw.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xq.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://fm.chemitech.net.cn

[E17] 首字母大写
来源：http://ef.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gq.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://me.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wo.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xc.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ap.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tr.9csxet.cn

Ruby: s.capitalize
来源：http://ws.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qr.nszjky.cn

[E18] 模板占位符替换
来源：http://xg.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pv.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ki.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://js.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tj.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lc.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://co.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://na.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wg.huanxung.cn

[E19] 多行文本按行拆分
来源：http://va.chemitech.net.cn

Py:   s.splitlines()
来源：http://rq.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ms.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://hr.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://fi.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://lk.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://td.yuntaijiaju.cn

Ruby: s.lines
来源：http://rr.huanxung.cn

C#:   s.Split('\n')
来源：http://tm.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://yx.521024.cn

Py:   if not s:
来源：http://dl.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://an.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://su.shxzskj.cn

TS:   if (s === "") {}
来源：http://qv.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://qo.huanxung.cn

Go:   if s == "" {}
来源：http://gr.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://ev.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fl.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://jx.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vc.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dk.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eu.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yv.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lb.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://jy.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://um.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ez.hahajie.cn

[E22] 字节长度与字符长度
来源：http://rb.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://th.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://re.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://is.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zp.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fh.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fr.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://ib.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pq.huixinmuqiang.cn

================================================================================
来源：http://kt.chemitech.net.cn

F. 文件与目录
来源：http://ks.lnxyls.cn

================================================================================
来源：http://aq.muxihuayi.cn

[F01] 读取整个文件
来源：http://ew.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rm.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://im.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nx.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zg.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nl.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vw.nicolike.cn

Ruby: File.read("a.txt")
来源：http://kd.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://md.szxytkj.cn

[F02] 逐行读取文件
来源：http://fa.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ud.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mt.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zy.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tc.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ou.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ve.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kr.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cv.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://pm.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mr.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pv.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ix.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://za.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pq.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://fl.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wl.hahajie.cn

[F04] 追加写入文件
来源：http://wx.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wj.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xq.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fz.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ga.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lb.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wt.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mb.521024.cn

[F05] 判断文件或目录是否存在
来源：http://gl.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zu.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://na.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://cj.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://xf.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qf.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uz.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://uj.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ek.nicolike.cn

[F06] 删除文件
来源：http://ev.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://dk.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://ct.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gd.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fz.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dq.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://vq.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://nb.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://dt.521024.cn

[F07] 创建目录（含多级）
来源：http://we.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lb.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tx.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dw.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cs.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mw.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hj.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zo.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ae.panjiajie.cn

[F08] 遍历目录
来源：http://kv.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aq.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mu.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://bs.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://tq.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jo.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ak.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ll.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://cx.shxzukj.cn

[F09] 获取文件大小
来源：http://wl.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://ml.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://ue.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://lh.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://ba.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hk.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gy.nszjky.cn

Ruby: File.size("a.txt")
来源：http://ha.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lu.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://ny.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oc.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://es.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ue.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://xo.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fc.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sc.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vf.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fe.newstarts.cn

[F11] 复制与移动文件
来源：http://zs.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ft.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ta.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ka.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nh.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yf.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lb.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kt.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://py.szsharing.cn

[F12] CSV 读写
来源：http://vc.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kw.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jf.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ht.chemitech.net.cn

TS:   // 同上
来源：http://nx.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mt.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ph.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://az.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hb.colortex.cn

================================================================================
来源：http://iw.asd995.cn

G. 面向对象
来源：http://tl.nszjky.cn

================================================================================
来源：http://wu.hnjuh.cn

[G01] 定义类
来源：http://gm.9csxet.cn

Py:   class User: pass
来源：http://yc.szsharing.cn

PHP:  class User {}
来源：http://vc.szsharing.cn

JS:   class User {}
来源：http://jf.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://nb.hnjuh.cn

Java: class User {}
来源：http://lu.gzmigu.cn

Go:   type User struct { Name string }
来源：http://fm.asd995.cn

Ruby: class User; end
来源：http://zh.panjiajie.cn

C#:   class User {}
来源：http://qk.hahajie.cn

[G02] 构造函数
来源：http://ct.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://xb.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://og.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://vc.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://sc.521024.cn

Java: User(String name) { this.name = name; }
来源：http://lo.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://on.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ar.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://kb.haigaiapp.cn

[G03] 实例属性
来源：http://mf.chemitech.net.cn

Py:   self.name = "x"
来源：http://dj.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ho.hnjuh.cn

JS:   this.name = "x";
来源：http://on.nszjky.cn

TS:   name: string = "x";
来源：http://lu.hnjuh.cn

Java: private String name;
来源：http://tz.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aj.haigaiapp.cn

Ruby: @name = "x"
来源：http://qy.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://ib.gzmigu.cn

[G04] 定义方法
来源：http://yl.newstarts.cn

Py:   def greet(self): return self.name
来源：http://ac.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://da.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://yb.521024.cn

TS:   greet(): string { return this.name; }
来源：http://fq.nszjky.cn

Java: String greet() { return name; }
来源：http://zn.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vz.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ft.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://xc.shxzskj.cn

[G05] 继承
来源：http://jo.521024.cn

Py:   class Admin(User): pass
来源：http://cn.hahajie.cn

PHP:  class Admin extends User {}
来源：http://zz.nszjky.cn

JS:   class Admin extends User {}
来源：http://jh.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://xo.jctech888.com.cn

Java: class Admin extends User {}
来源：http://hd.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tw.9csxet.cn

Ruby: class Admin < User; end
来源：http://ys.shtwfgs.cn

C#:   class Admin : User {}
来源：http://sc.lnxyls.cn

[G06] 重写方法
来源：http://qy.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://fv.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ui.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://or.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://ya.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://sq.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ky.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://mc.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://ra.yuexingan06.cn

[G07] 调用父类方法
来源：http://fl.huanxung.cn

Py:   super().greet()
来源：http://ai.huixiangedu.cn

PHP:  parent::greet();
来源：http://pl.huixiangedu.cn

JS:   super.greet();
来源：http://yd.hnjuh.cn

TS:   super.greet();
来源：http://vd.bookmarksfly.cn

Java: super.greet();
来源：http://sa.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ij.szxytkj.cn

Ruby: super
来源：http://zs.jctech888.com.cn

C#:   base.Greet();
来源：http://ay.wgjwhj.cn

[G08] 静态方法与属性
来源：http://jm.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fa.huanxung.cn

PHP:  public static function f() {}
来源：http://cr.hahajie.cn

JS:   static f() {}
来源：http://lj.jctech888.com.cn

TS:   static f(): void {}
来源：http://pd.shxzukj.cn

Java: static void f() {}
来源：http://ms.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ri.szsharing.cn

Ruby: def self.f; end
来源：http://jp.nszjky.cn

C#:   public static void F() {}
来源：http://od.521024.cn

[G09] 接口 / 抽象类
来源：http://jv.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zd.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bn.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bj.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://iv.colortex.cn

Java: interface Shape { double area(); }
来源：http://ri.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://nc.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mc.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://qt.yuntaijiaju.cn

[G10] 访问控制
来源：http://ry.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://io.asd995.cn

PHP:  public / protected / private
来源：http://or.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://mi.szxytkj.cn

TS:   public / protected / private
来源：http://mf.colortex.cn

Java: public / protected / private / 默认包级
来源：http://wk.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pf.colortex.cn

Ruby: public / protected / private
来源：http://ck.szxytkj.cn

C#:   public / protected / private / internal
来源：http://fl.wgjwhj.cn

[G11] getter / setter
来源：http://hq.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://ae.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uo.szsharing.cn

JS:   get name() { return this._name; }
来源：http://eb.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://wi.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://qo.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ad.bjjhwx.cn


<!-- 参考信息 -->