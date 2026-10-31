代发 wailian999

JS:   [...s].reverse().join("")
来源：http://gg.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://nn.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://at.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://el.huixinmuqiang.cn

Ruby: s.reverse
来源：http://pk.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://no.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ab.chemitech.net.cn

Py:   s.count("a")
来源：http://cx.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://rz.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://xp.9csxet.cn

TS:   s.split("a").length - 1
来源：http://dm.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jm.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://un.hnjuh.cn

Ruby: s.count("a")
来源：http://by.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://mj.shxzukj.cn

[E13] 逐字符遍历
来源：http://pm.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://rk.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dq.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ud.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://py.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sn.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ym.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xf.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eb.521024.cn

[E14] URL 编码与 Base64
来源：http://ha.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xu.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ns.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vl.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kw.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zc.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ly.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gc.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nq.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://zs.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sl.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tx.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ye.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kk.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://al.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nh.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ex.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cc.huixinmuqiang.cn

[E16] 数字千分位
来源：http://wg.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://ci.huanxung.cn

PHP:  number_format(1234567);
来源：http://xg.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pt.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qh.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lr.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jq.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qv.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://tu.hahajie.cn

[E17] 首字母大写
来源：http://qn.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nu.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ob.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ls.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tw.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ab.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yw.shxzskj.cn

Ruby: s.capitalize
来源：http://xi.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ux.521024.cn

[E18] 模板占位符替换
来源：http://fs.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uu.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jk.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ua.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ev.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qc.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qm.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yu.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ua.huanxung.cn

[E19] 多行文本按行拆分
来源：http://qp.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ry.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nm.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ub.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://cc.9csxet.cn

Java: s.lines().toList()
来源：http://jy.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://sg.panjiajie.cn

Ruby: s.lines
来源：http://ph.colortex.cn

C#:   s.Split('\n')
来源：http://nm.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://sa.yuntaijiaju.cn

Py:   if not s:
来源：http://hc.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jt.nszjky.cn

TS:   if (s === "") {}
来源：http://nk.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://bk.asd995.cn

Go:   if s == "" {}
来源：http://be.hahajie.cn

Ruby: if s.empty?
来源：http://ph.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ua.panjiajie.cn

[E21] 超长截断加省略号
来源：http://mq.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://un.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sv.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mr.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cl.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bm.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ei.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://se.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hg.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://yg.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uj.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ss.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sn.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mc.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yt.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://he.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://eu.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ep.bookmarksfly.cn

================================================================================
来源：http://qx.haigaiapp.cn

F. 文件与目录
来源：http://gv.jctech888.com.cn

================================================================================
来源：http://kc.gzmigu.cn

[F01] 读取整个文件
来源：http://rd.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yz.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://zg.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ue.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dm.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qm.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ys.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://vm.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://ii.muxihuayi.cn

[F02] 逐行读取文件
来源：http://bi.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dh.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uw.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sp.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aa.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ho.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mw.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pg.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gg.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://km.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oy.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tj.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yf.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nc.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zk.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://qy.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://it.yuexingan06.cn

[F04] 追加写入文件
来源：http://kp.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qw.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xr.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iw.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bn.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rg.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://un.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nc.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qt.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://ys.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tk.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://hl.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://mg.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://mv.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wl.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ws.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ot.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://ot.bookmarksfly.cn

[F06] 删除文件
来源：http://dl.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://iw.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://fq.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vu.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jb.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://of.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ab.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://lt.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://dd.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://qx.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rr.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wk.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qb.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lt.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ef.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jg.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zf.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xk.lnxyls.cn

[F08] 遍历目录
来源：http://vh.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ij.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://da.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://kp.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://nd.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wj.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ho.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://zb.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://qf.bjjhwx.cn

[F09] 获取文件大小
来源：http://hp.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://jr.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://dn.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://bw.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://yc.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zv.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mj.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://dd.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://wu.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://jd.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bu.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ns.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ky.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://wt.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ni.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jq.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pz.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qh.9csxet.cn

[F11] 复制与移动文件
来源：http://fb.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ct.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xs.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wd.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fs.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jw.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fj.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hp.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dx.nszjky.cn

[F12] CSV 读写
来源：http://yb.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hk.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ww.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zh.panjiajie.cn

TS:   // 同上
来源：http://iu.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yz.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vf.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://em.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ak.yuexingan06.cn

================================================================================
来源：http://jx.gzmigu.cn

G. 面向对象
来源：http://lt.bookmarksfly.cn

================================================================================
来源：http://dv.muxihuayi.cn

[G01] 定义类
来源：http://fc.nszjky.cn

Py:   class User: pass
来源：http://ds.9csxet.cn

PHP:  class User {}
来源：http://si.newstarts.cn

JS:   class User {}
来源：http://zp.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://vj.shxzukj.cn

Java: class User {}
来源：http://yl.521024.cn

Go:   type User struct { Name string }
来源：http://hw.huixiangedu.cn

Ruby: class User; end
来源：http://ct.lnxyls.cn

C#:   class User {}
来源：http://cs.haigaiapp.cn

[G02] 构造函数
来源：http://qf.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://zj.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ok.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://zy.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://cv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://of.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nt.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://wx.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://if.jianghongdianzi.cn

[G03] 实例属性
来源：http://qz.bjjhwx.cn

Py:   self.name = "x"
来源：http://fg.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://dv.hahajie.cn

JS:   this.name = "x";
来源：http://ml.hnjuh.cn

TS:   name: string = "x";
来源：http://zo.bookmarksfly.cn

Java: private String name;
来源：http://hq.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qz.muxihuayi.cn

Ruby: @name = "x"
来源：http://nx.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://cb.bjjhwx.cn

[G04] 定义方法
来源：http://sy.huanxung.cn

Py:   def greet(self): return self.name
来源：http://xo.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jj.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://jr.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://mm.szxytkj.cn

Java: String greet() { return name; }
来源：http://ux.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qb.gzmigu.cn

Ruby: def greet; @name; end
来源：http://gn.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://gl.nszjky.cn

[G05] 继承
来源：http://yx.shxzskj.cn

Py:   class Admin(User): pass
来源：http://hh.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://wr.nszjky.cn

JS:   class Admin extends User {}
来源：http://zt.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://qf.szsharing.cn

Java: class Admin extends User {}
来源：http://cd.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vm.asd995.cn

Ruby: class Admin < User; end
来源：http://sz.gzmigu.cn

C#:   class Admin : User {}
来源：http://eu.521024.cn

[G06] 重写方法
来源：http://bz.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://qm.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://is.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://jr.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://zl.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://cl.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rs.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ge.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://gv.gzmigu.cn

[G07] 调用父类方法
来源：http://wn.521024.cn

Py:   super().greet()
来源：http://mj.haigaiapp.cn

PHP:  parent::greet();
来源：http://lm.shtwfgs.cn

JS:   super.greet();
来源：http://dg.nszjky.cn

TS:   super.greet();
来源：http://xb.szxytkj.cn

Java: super.greet();
来源：http://pk.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://he.muxihuayi.cn

Ruby: super
来源：http://qi.jianghongdianzi.cn

C#:   base.Greet();
来源：http://ht.shxzskj.cn

[G08] 静态方法与属性
来源：http://zp.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xl.gzmigu.cn

PHP:  public static function f() {}
来源：http://rm.huixinmuqiang.cn

JS:   static f() {}
来源：http://uo.jctech888.com.cn

TS:   static f(): void {}
来源：http://tg.shxzskj.cn

Java: static void f() {}
来源：http://dl.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://li.huixiangedu.cn

Ruby: def self.f; end
来源：http://uh.9csxet.cn

C#:   public static void F() {}
来源：http://oq.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mv.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://og.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pe.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://up.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://sm.szsharing.cn

Java: interface Shape { double area(); }
来源：http://eu.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ch.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pq.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ga.bjjhwx.cn


<!-- 参考信息 -->