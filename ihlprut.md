代发 wailian999

Ruby: s.reverse
来源：http://hg.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oo.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://tw.hnjuh.cn

Py:   s.count("a")
来源：http://hz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://sl.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://bw.szsharing.cn

TS:   s.split("a").length - 1
来源：http://vx.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lm.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://jg.521024.cn

Ruby: s.count("a")
来源：http://wr.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://oi.huixiangedu.cn

[E13] 逐字符遍历
来源：http://kx.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ht.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mh.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oc.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://da.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zl.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://az.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oy.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bi.nszjky.cn

[E14] URL 编码与 Base64
来源：http://yl.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dr.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eb.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://my.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tc.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cg.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://su.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tn.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hl.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://qq.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fx.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gt.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nh.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fb.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kf.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tl.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xu.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lr.hahajie.cn

[E16] 数字千分位
来源：http://bj.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ce.nszjky.cn

PHP:  number_format(1234567);
来源：http://ck.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hj.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fg.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cg.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://us.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://un.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://er.lnxyls.cn

[E17] 首字母大写
来源：http://mi.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rp.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ma.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ov.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zo.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cv.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://rx.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ro.nicolike.cn

[E18] 模板占位符替换
来源：http://ls.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qf.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cf.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ge.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://na.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ax.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://he.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sm.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ml.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://de.521024.cn

Py:   s.splitlines()
来源：http://ex.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bm.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ax.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://dk.chemitech.net.cn

Java: s.lines().toList()
来源：http://xh.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://oj.521024.cn

Ruby: s.lines
来源：http://px.colortex.cn

C#:   s.Split('\n')
来源：http://he.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://kv.hnjuh.cn

Py:   if not s:
来源：http://zj.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eo.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hj.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://an.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ra.bjjhwx.cn

Go:   if s == "" {}
来源：http://je.colortex.cn

Ruby: if s.empty?
来源：http://xm.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qb.szxytkj.cn

[E21] 超长截断加省略号
来源：http://nr.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cv.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gj.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ke.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hi.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cf.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://bo.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bm.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vt.nicolike.cn

[E22] 字节长度与字符长度
来源：http://wc.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://md.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pb.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dw.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://al.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zo.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ah.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://wm.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vr.szxytkj.cn

================================================================================
来源：http://ba.yuntaijiaju.cn

F. 文件与目录
来源：http://jq.bjjhwx.cn

================================================================================
来源：http://sn.szxytkj.cn

[F01] 读取整个文件
来源：http://mt.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xd.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://wz.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ud.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://or.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uq.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ba.hahajie.cn

Ruby: File.read("a.txt")
来源：http://vp.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://le.wgjwhj.cn

[F02] 逐行读取文件
来源：http://in.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://li.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://og.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jz.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rc.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xh.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nm.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vk.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nd.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://yu.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ly.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://js.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ym.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uh.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zl.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zw.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://qb.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.yuexingan06.cn

[F04] 追加写入文件
来源：http://sm.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tc.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sf.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mf.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yf.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ul.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xa.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mu.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://bo.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cv.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://ji.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://fx.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://xw.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qe.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xt.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://cm.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://wz.gzmigu.cn

[F06] 删除文件
来源：http://rd.szsharing.cn

Py:   os.remove("a.txt")
来源：http://yt.nicolike.cn

PHP:  unlink("a.txt");
来源：http://az.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ju.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sg.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uc.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://br.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://lq.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://lq.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://hc.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dm.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jx.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mj.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yr.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uj.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vn.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://na.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pe.huanxung.cn

[F08] 遍历目录
来源：http://hq.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ne.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dd.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://xx.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://pu.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dz.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tu.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://tc.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://ob.shtwfgs.cn

[F09] 获取文件大小
来源：http://qs.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://ag.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://hi.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://hk.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://nq.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sq.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ra.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://of.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://cs.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://rt.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://md.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hq.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lw.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://fz.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oz.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wh.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lw.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lt.newstarts.cn

[F11] 复制与移动文件
来源：http://lj.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://am.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ec.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jt.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zq.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://km.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yy.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zf.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://be.chemitech.net.cn

[F12] CSV 读写
来源：http://kb.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://br.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wc.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hl.nszjky.cn

TS:   // 同上
来源：http://ej.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vj.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qj.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iw.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ib.jianghongdianzi.cn

================================================================================
来源：http://hj.chemitech.net.cn

G. 面向对象
来源：http://sq.gzmigu.cn

================================================================================
来源：http://sg.newstarts.cn

[G01] 定义类
来源：http://ry.szxytkj.cn

Py:   class User: pass
来源：http://ca.newstarts.cn

PHP:  class User {}
来源：http://na.huixinmuqiang.cn

JS:   class User {}
来源：http://lg.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://kt.colortex.cn

Java: class User {}
来源：http://fo.huanxung.cn

Go:   type User struct { Name string }
来源：http://pv.bookmarksfly.cn

Ruby: class User; end
来源：http://xw.panjiajie.cn

C#:   class User {}
来源：http://wi.jianghongdianzi.cn

[G02] 构造函数
来源：http://fh.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://rc.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://ej.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://lq.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ks.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://px.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ab.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://sh.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://zg.lnxyls.cn

[G03] 实例属性
来源：http://dy.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://dv.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://ur.szxytkj.cn

JS:   this.name = "x";
来源：http://qx.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://vh.nszjky.cn

Java: private String name;
来源：http://go.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ho.jctech888.com.cn

Ruby: @name = "x"
来源：http://dk.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://tt.jianghongdianzi.cn

[G04] 定义方法
来源：http://yi.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ra.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sc.huanxung.cn

JS:   greet() { return this.name; }
来源：http://zk.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://tt.9csxet.cn

Java: String greet() { return name; }
来源：http://wk.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vr.panjiajie.cn

Ruby: def greet; @name; end
来源：http://ge.nszjky.cn

C#:   public string Greet() => Name;
来源：http://yn.jctech888.com.cn

[G05] 继承
来源：http://ai.colortex.cn

Py:   class Admin(User): pass
来源：http://ru.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://mw.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://tk.szsharing.cn

TS:   class Admin extends User {}
来源：http://hl.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://tb.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ej.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ao.gzmigu.cn

C#:   class Admin : User {}
来源：http://cu.bjjhwx.cn

[G06] 重写方法
来源：http://bp.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://jc.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yb.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://lf.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://gn.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://wi.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tf.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://uc.521024.cn

C#:   public override string Greet() => "admin";
来源：http://qi.wgjwhj.cn

[G07] 调用父类方法
来源：http://tm.shxzukj.cn

Py:   super().greet()
来源：http://mg.shxzukj.cn

PHP:  parent::greet();
来源：http://ny.shxzskj.cn

JS:   super.greet();
来源：http://dy.hahajie.cn

TS:   super.greet();
来源：http://bx.colortex.cn

Java: super.greet();
来源：http://bi.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qg.szxytkj.cn

Ruby: super
来源：http://ui.lnxyls.cn

C#:   base.Greet();
来源：http://ak.colortex.cn

[G08] 静态方法与属性
来源：http://ev.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ru.hnjuh.cn

PHP:  public static function f() {}
来源：http://qb.bjjhwx.cn

JS:   static f() {}
来源：http://dw.muxihuayi.cn

TS:   static f(): void {}
来源：http://mq.szxytkj.cn

Java: static void f() {}
来源：http://bf.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iz.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://xc.nicolike.cn

C#:   public static void F() {}
来源：http://kp.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://to.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://xt.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ps.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wl.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://yl.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://vp.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sc.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cm.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://fe.yuntaijiaju.cn

[G10] 访问控制
来源：http://bv.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://po.gzmigu.cn

PHP:  public / protected / private
来源：http://pg.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ra.yuexingan06.cn


<!-- 参考信息 -->