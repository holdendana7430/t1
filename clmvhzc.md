代发 wailian999

Ruby: s.reverse
来源：http://pk.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gk.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://ud.shxzukj.cn

Py:   s.count("a")
来源：http://yo.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://zj.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://ba.nicolike.cn

TS:   s.split("a").length - 1
来源：http://cx.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yx.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://bv.muxihuayi.cn

Ruby: s.count("a")
来源：http://kl.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://mt.jctech888.com.cn

[E13] 逐字符遍历
来源：http://oc.colortex.cn

Py:   for ch in s: print(ch)
来源：http://ei.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dl.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sx.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fk.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kk.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ly.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lk.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://br.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://ob.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lw.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gw.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qr.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qb.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rb.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zx.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bc.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aq.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://pj.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wo.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gh.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xn.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nh.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yo.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bg.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kc.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ao.shxzukj.cn

[E16] 数字千分位
来源：http://xm.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://xt.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://an.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dm.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dj.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gn.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ze.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qg.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://jl.9csxet.cn

[E17] 首字母大写
来源：http://wm.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ri.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ps.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hn.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xv.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bm.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pj.asd995.cn

Ruby: s.capitalize
来源：http://rp.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nj.shxzukj.cn

[E18] 模板占位符替换
来源：http://bb.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ft.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rl.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ue.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lo.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xu.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xp.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jm.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sg.asd995.cn

[E19] 多行文本按行拆分
来源：http://gb.shxzskj.cn

Py:   s.splitlines()
来源：http://di.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gx.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://cg.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://bv.hahajie.cn

Java: s.lines().toList()
来源：http://zt.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://ap.huanxung.cn

Ruby: s.lines
来源：http://qb.huanxung.cn

C#:   s.Split('\n')
来源：http://ob.521024.cn

[E20] 判断字符串是否为空
来源：http://rl.521024.cn

Py:   if not s:
来源：http://xu.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pl.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wq.hahajie.cn

TS:   if (s === "") {}
来源：http://wf.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://zi.bjjhwx.cn

Go:   if s == "" {}
来源：http://me.hahajie.cn

Ruby: if s.empty?
来源：http://bf.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qg.nszjky.cn

[E21] 超长截断加省略号
来源：http://me.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vb.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oq.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zr.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zx.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wy.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://lh.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vd.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://py.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://zf.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xr.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vl.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rw.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wn.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yx.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://er.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oh.bjjhwx.cn

================================================================================
来源：http://iw.521024.cn

F. 文件与目录
来源：http://yv.hnjuh.cn

================================================================================
来源：http://ac.newstarts.cn

[F01] 读取整个文件
来源：http://me.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gx.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://qx.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tk.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wu.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tv.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bz.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://mi.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://fk.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://xm.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ay.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pg.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zk.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tu.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tm.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ni.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fe.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://pq.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jb.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dz.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vb.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rz.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zl.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wb.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fy.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://qa.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wl.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fr.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ea.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cu.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uq.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dr.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dc.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hs.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://cr.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dc.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://eo.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://xr.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://rs.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jb.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://en.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://lj.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ue.haigaiapp.cn

[F06] 删除文件
来源：http://rl.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://ho.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://rg.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uy.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eo.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lf.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://kt.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://tr.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://ei.nszjky.cn

[F07] 创建目录（含多级）
来源：http://vk.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://od.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yb.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dy.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hi.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://le.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hg.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iw.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rd.nszjky.cn

[F08] 遍历目录
来源：http://hi.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://co.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://di.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://fj.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://zy.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://il.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://da.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://ez.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://rr.nicolike.cn

[F09] 获取文件大小
来源：http://ib.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ha.nicolike.cn

PHP:  filesize("a.txt");
来源：http://pj.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://tk.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://dt.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lt.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sh.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://xq.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://yd.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://lw.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ml.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lc.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://co.9csxet.cn

TS:   path.extname("a.txt")
来源：http://ay.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://le.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fn.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bw.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ol.muxihuayi.cn

[F11] 复制与移动文件
来源：http://gf.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zz.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://se.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://do.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wi.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qk.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xp.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qd.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mo.panjiajie.cn

[F12] CSV 读写
来源：http://nx.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mn.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yz.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ry.asd995.cn

TS:   // 同上
来源：http://pq.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xg.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cm.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xv.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dm.yuexingan06.cn

================================================================================
来源：http://rj.bookmarksfly.cn

G. 面向对象
来源：http://yc.yuexingan06.cn

================================================================================
来源：http://og.nszjky.cn

[G01] 定义类
来源：http://pj.haigaiapp.cn

Py:   class User: pass
来源：http://rw.colortex.cn

PHP:  class User {}
来源：http://qj.colortex.cn

JS:   class User {}
来源：http://ds.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://vy.nszjky.cn

Java: class User {}
来源：http://th.szsharing.cn

Go:   type User struct { Name string }
来源：http://gf.colortex.cn

Ruby: class User; end
来源：http://nx.gzmigu.cn

C#:   class User {}
来源：http://al.huixiangedu.cn

[G02] 构造函数
来源：http://pj.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://uh.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://za.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://jp.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://zu.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://pz.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zf.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://go.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://ev.nszjky.cn

[G03] 实例属性
来源：http://gt.jctech888.com.cn

Py:   self.name = "x"
来源：http://iy.gzmigu.cn

PHP:  public string $name = "x";
来源：http://zn.hahajie.cn

JS:   this.name = "x";
来源：http://hv.haigaiapp.cn

TS:   name: string = "x";
来源：http://sp.shtwfgs.cn

Java: private String name;
来源：http://gx.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ab.haigaiapp.cn

Ruby: @name = "x"
来源：http://bn.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://ea.chemitech.net.cn

[G04] 定义方法
来源：http://sy.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://zg.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ob.asd995.cn

JS:   greet() { return this.name; }
来源：http://dx.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://mn.shxzskj.cn

Java: String greet() { return name; }
来源：http://bo.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ay.huanxung.cn

Ruby: def greet; @name; end
来源：http://at.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://cu.panjiajie.cn

[G05] 继承
来源：http://ka.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://ec.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://xt.colortex.cn

JS:   class Admin extends User {}
来源：http://mc.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://oq.haigaiapp.cn

Java: class Admin extends User {}
来源：http://gp.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tu.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://rj.newstarts.cn

C#:   class Admin : User {}
来源：http://bp.colortex.cn

[G06] 重写方法
来源：http://pc.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://pp.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mb.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://nt.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://bt.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://yx.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ke.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://xt.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://iv.shtwfgs.cn

[G07] 调用父类方法
来源：http://rd.szxytkj.cn

Py:   super().greet()
来源：http://vi.szsharing.cn

PHP:  parent::greet();
来源：http://pv.szsharing.cn

JS:   super.greet();
来源：http://do.hnjuh.cn

TS:   super.greet();
来源：http://kt.gzmigu.cn

Java: super.greet();
来源：http://po.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ue.bjjhwx.cn

Ruby: super
来源：http://py.bjjhwx.cn

C#:   base.Greet();
来源：http://in.hnjuh.cn

[G08] 静态方法与属性
来源：http://iw.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jp.lnxyls.cn

PHP:  public static function f() {}
来源：http://gy.chemitech.net.cn

JS:   static f() {}
来源：http://ur.asd995.cn

TS:   static f(): void {}
来源：http://bh.colortex.cn

Java: static void f() {}
来源：http://jc.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tp.shxzukj.cn

Ruby: def self.f; end
来源：http://np.wgjwhj.cn

C#:   public static void F() {}
来源：http://wc.nszjky.cn

[G09] 接口 / 抽象类
来源：http://pn.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://lw.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tn.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qx.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://lv.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://bu.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://ov.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sg.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://wz.yuexingan06.cn

[G10] 访问控制
来源：http://bp.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://jq.panjiajie.cn

PHP:  public / protected / private
来源：http://hn.nszjky.cn

JS:   #private 字段；其余公开
来源：http://uk.bjjhwx.cn


<!-- 参考信息 -->