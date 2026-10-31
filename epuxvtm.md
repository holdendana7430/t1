代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wh.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://xw.asd995.cn

TS:   s.split("a").length - 1
来源：http://di.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rb.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://wv.colortex.cn

Ruby: s.count("a")
来源：http://rx.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://gi.panjiajie.cn

[E13] 逐字符遍历
来源：http://tr.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://cr.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ur.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ey.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sm.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zw.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://el.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vz.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dd.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://of.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xl.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cp.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://po.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qr.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qt.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nx.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ne.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kc.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://qz.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yj.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://je.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lj.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ux.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fn.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bv.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fh.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ds.gzmigu.cn

[E16] 数字千分位
来源：http://sl.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://ft.shxzskj.cn

PHP:  number_format(1234567);
来源：http://fg.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xt.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jz.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mt.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qz.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xo.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://bp.jctech888.com.cn

[E17] 首字母大写
来源：http://hw.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wj.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bk.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ng.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hs.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tf.shtwfgs.cn

Ruby: s.capitalize
来源：http://wc.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pc.9csxet.cn

[E18] 模板占位符替换
来源：http://sb.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nj.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pk.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gi.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ac.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ll.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ht.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hj.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xn.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://vu.gzmigu.cn

Py:   s.splitlines()
来源：http://wg.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xj.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://pb.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://tu.wgjwhj.cn

Java: s.lines().toList()
来源：http://rj.521024.cn

Go:   strings.Split(s, "\n")
来源：http://un.521024.cn

Ruby: s.lines
来源：http://if.shxzukj.cn

C#:   s.Split('\n')
来源：http://kv.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://yj.panjiajie.cn

Py:   if not s:
来源：http://mz.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lu.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ad.shxzskj.cn

TS:   if (s === "") {}
来源：http://fp.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://xd.newstarts.cn

Go:   if s == "" {}
来源：http://nb.colortex.cn

Ruby: if s.empty?
来源：http://xd.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ae.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://si.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nz.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nx.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ly.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ck.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://um.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://yh.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://np.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ia.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://lz.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mo.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gr.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qd.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ea.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mq.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://oa.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ia.huanxung.cn

================================================================================
来源：http://tn.hnjuh.cn

F. 文件与目录
来源：http://nw.szsharing.cn

================================================================================
来源：http://we.gzmigu.cn

[F01] 读取整个文件
来源：http://ju.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gm.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://fb.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ic.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qt.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://el.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nr.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://aj.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://tk.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://wa.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eq.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aq.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mi.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ki.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fz.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bo.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://by.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://cl.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fh.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jx.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yb.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gd.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vc.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lm.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://zh.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lk.bjjhwx.cn

[F04] 追加写入文件
来源：http://gf.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://di.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kf.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hy.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oc.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wf.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yg.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wo.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://th.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://fr.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iz.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://bx.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://zw.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://dc.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://af.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fj.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://bw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://nm.huixiangedu.cn

[F06] 删除文件
来源：http://sh.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://fp.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://rj.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bd.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vs.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gy.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://pk.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://hp.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://fc.9csxet.cn

[F07] 创建目录（含多级）
来源：http://mt.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lb.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yz.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sf.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://op.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qz.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uz.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kv.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dk.lnxyls.cn

[F08] 遍历目录
来源：http://eo.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bo.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://il.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://tg.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://tk.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yn.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ty.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://zp.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://nx.bjjhwx.cn

[F09] 获取文件大小
来源：http://yt.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://ey.szsharing.cn

PHP:  filesize("a.txt");
来源：http://tl.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://zp.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://qy.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nw.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cz.asd995.cn

Ruby: File.size("a.txt")
来源：http://in.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://dq.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fq.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ao.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qo.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://my.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://gy.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jt.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xb.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://in.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wi.9csxet.cn

[F11] 复制与移动文件
来源：http://vy.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lm.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fj.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jv.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://td.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kt.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://im.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xg.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cj.jianghongdianzi.cn

[F12] CSV 读写
来源：http://uc.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hr.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jx.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qq.haigaiapp.cn

TS:   // 同上
来源：http://vh.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://od.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mf.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pw.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wl.asd995.cn

================================================================================
来源：http://ep.hahajie.cn

G. 面向对象
来源：http://xc.bjjhwx.cn

================================================================================
来源：http://ey.yuntaijiaju.cn

[G01] 定义类
来源：http://po.gzmigu.cn

Py:   class User: pass
来源：http://os.gzmigu.cn

PHP:  class User {}
来源：http://fn.shxzukj.cn

JS:   class User {}
来源：http://wn.asd995.cn

TS:   class User { name: string = ""; }
来源：http://dq.9csxet.cn

Java: class User {}
来源：http://md.hahajie.cn

Go:   type User struct { Name string }
来源：http://rc.nicolike.cn

Ruby: class User; end
来源：http://ip.hahajie.cn

C#:   class User {}
来源：http://jb.hnjuh.cn

[G02] 构造函数
来源：http://nx.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://yg.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://to.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://bb.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://qb.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://wb.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zo.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://uv.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://xz.yuexingan06.cn

[G03] 实例属性
来源：http://jh.gzmigu.cn

Py:   self.name = "x"
来源：http://id.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://cb.szsharing.cn

JS:   this.name = "x";
来源：http://as.lnxyls.cn

TS:   name: string = "x";
来源：http://kc.yuntaijiaju.cn

Java: private String name;
来源：http://cs.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://js.nszjky.cn

Ruby: @name = "x"
来源：http://ho.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://xj.hahajie.cn

[G04] 定义方法
来源：http://mz.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://sl.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vd.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://my.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://ya.shtwfgs.cn

Java: String greet() { return name; }
来源：http://ye.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tc.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://lh.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://hb.jianghongdianzi.cn

[G05] 继承
来源：http://ty.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ip.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://xv.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ap.asd995.cn

TS:   class Admin extends User {}
来源：http://oy.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://cj.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aq.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ky.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://tn.panjiajie.cn

[G06] 重写方法
来源：http://qm.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://hp.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://am.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://uy.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://ou.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://no.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lo.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://pb.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://ca.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://wh.shtwfgs.cn

Py:   super().greet()
来源：http://gs.hahajie.cn

PHP:  parent::greet();
来源：http://pa.huixinmuqiang.cn

JS:   super.greet();
来源：http://ok.newstarts.cn

TS:   super.greet();
来源：http://dt.nszjky.cn

Java: super.greet();
来源：http://nu.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rw.szxytkj.cn

Ruby: super
来源：http://tw.gzmigu.cn

C#:   base.Greet();
来源：http://wi.muxihuayi.cn

[G08] 静态方法与属性
来源：http://pn.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bt.colortex.cn

PHP:  public static function f() {}
来源：http://ef.haigaiapp.cn

JS:   static f() {}
来源：http://wh.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://xs.huanxung.cn

Java: static void f() {}
来源：http://aq.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sp.asd995.cn

Ruby: def self.f; end
来源：http://qs.chemitech.net.cn

C#:   public static void F() {}
来源：http://rh.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://wg.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://id.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sp.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mx.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://hb.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://hx.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://sb.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://uy.huanxung.cn

[G10] 访问控制
来源：http://vh.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://ji.muxihuayi.cn

PHP:  public / protected / private
来源：http://sj.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ae.gzmigu.cn

TS:   public / protected / private
来源：http://ng.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://zo.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ol.haigaiapp.cn

Ruby: public / protected / private
来源：http://rt.yuexingan06.cn


<!-- 参考信息 -->