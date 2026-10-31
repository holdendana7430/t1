代发 wailian999

PHP:  substr_count($s, "a");
来源：http://gu.huanxung.cn

JS:   s.split("a").length - 1
来源：http://wl.asd995.cn

TS:   s.split("a").length - 1
来源：http://ya.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ax.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ua.huixiangedu.cn

Ruby: s.count("a")
来源：http://rn.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://xt.muxihuayi.cn

[E13] 逐字符遍历
来源：http://so.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://cu.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vi.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xg.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fd.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gp.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nu.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nj.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ti.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://sg.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fy.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sg.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pd.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mg.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://og.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gp.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yy.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://up.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://ho.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bw.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qp.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pe.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uh.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kq.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cu.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://on.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://io.szxytkj.cn

[E16] 数字千分位
来源：http://gm.hahajie.cn

Py:   f"{1234567:,}"
来源：http://dq.colortex.cn

PHP:  number_format(1234567);
来源：http://me.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mm.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ln.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ob.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eh.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qb.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://ru.huixiangedu.cn

[E17] 首字母大写
来源：http://cb.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://re.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vt.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pm.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ts.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ds.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qc.hnjuh.cn

Ruby: s.capitalize
来源：http://mb.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bl.9csxet.cn

[E18] 模板占位符替换
来源：http://nw.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rl.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uc.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wo.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lm.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ix.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://st.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gc.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dq.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://zh.hahajie.cn

Py:   s.splitlines()
来源：http://ni.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pq.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://tw.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://pm.shtwfgs.cn

Java: s.lines().toList()
来源：http://hk.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://zx.wgjwhj.cn

Ruby: s.lines
来源：http://ol.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://df.szsharing.cn

[E20] 判断字符串是否为空
来源：http://qf.huixiangedu.cn

Py:   if not s:
来源：http://vo.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lm.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ng.huixiangedu.cn

TS:   if (s === "") {}
来源：http://gk.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://ht.wgjwhj.cn

Go:   if s == "" {}
来源：http://jy.newstarts.cn

Ruby: if s.empty?
来源：http://qx.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ib.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ha.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://if.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qj.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sa.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rv.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dt.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://wc.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mu.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hd.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://hk.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://af.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vp.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bf.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dl.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qg.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wp.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ma.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://if.521024.cn

================================================================================
来源：http://iv.huixiangedu.cn

F. 文件与目录
来源：http://nf.nszjky.cn

================================================================================
来源：http://sm.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://wr.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yn.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://xd.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zn.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ka.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fb.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oo.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://nd.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://xf.hahajie.cn

[F02] 逐行读取文件
来源：http://pn.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pz.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dj.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ce.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eg.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kh.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xe.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pn.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nc.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://oi.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mj.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hv.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ai.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://va.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mh.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ug.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ea.bjjhwx.cn

[F04] 追加写入文件
来源：http://ua.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uw.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mz.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://an.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jj.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ym.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bt.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ai.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://gy.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wa.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://ew.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://xd.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://tm.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mt.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hy.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ze.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://gd.lnxyls.cn

[F06] 删除文件
来源：http://ir.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://cg.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://pj.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ei.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uq.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vs.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://le.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://ch.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://wa.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ot.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mf.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://it.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qj.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sb.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://is.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bq.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vp.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kh.hahajie.cn

[F08] 遍历目录
来源：http://ex.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://td.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sd.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://un.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ol.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yo.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fi.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://cr.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://iw.muxihuayi.cn

[F09] 获取文件大小
来源：http://ri.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://dv.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://yn.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://vl.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://yf.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jf.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ln.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://tw.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://kt.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://te.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qv.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nu.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dd.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://va.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ds.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lo.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rh.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sd.shxzukj.cn

[F11] 复制与移动文件
来源：http://cg.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ic.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://es.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oa.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xl.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ez.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vm.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ro.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ko.szsharing.cn

[F12] CSV 读写
来源：http://yu.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gd.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dr.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vd.colortex.cn

TS:   // 同上
来源：http://mg.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zn.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ds.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iy.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rf.chemitech.net.cn

================================================================================
来源：http://jg.bookmarksfly.cn

G. 面向对象
来源：http://xv.521024.cn

================================================================================
来源：http://qi.haigaiapp.cn

[G01] 定义类
来源：http://fz.colortex.cn

Py:   class User: pass
来源：http://fj.newstarts.cn

PHP:  class User {}
来源：http://we.jianghongdianzi.cn

JS:   class User {}
来源：http://zh.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ii.asd995.cn

Java: class User {}
来源：http://sq.nicolike.cn

Go:   type User struct { Name string }
来源：http://hc.shxzskj.cn

Ruby: class User; end
来源：http://yp.lnxyls.cn

C#:   class User {}
来源：http://ce.yuexingan06.cn

[G02] 构造函数
来源：http://cx.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://mi.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://zn.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://ka.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://kh.521024.cn

Java: User(String name) { this.name = name; }
来源：http://fd.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ko.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://no.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://jq.bjjhwx.cn

[G03] 实例属性
来源：http://iw.bjjhwx.cn

Py:   self.name = "x"
来源：http://br.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://wn.szsharing.cn

JS:   this.name = "x";
来源：http://kf.wgjwhj.cn

TS:   name: string = "x";
来源：http://ff.huixinmuqiang.cn

Java: private String name;
来源：http://so.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://be.shxzukj.cn

Ruby: @name = "x"
来源：http://lz.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://ty.shxzukj.cn

[G04] 定义方法
来源：http://hl.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://hd.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nw.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://cf.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://du.panjiajie.cn

Java: String greet() { return name; }
来源：http://gb.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dw.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://rw.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://vj.bjjhwx.cn

[G05] 继承
来源：http://lc.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://lz.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://tt.panjiajie.cn

JS:   class Admin extends User {}
来源：http://pv.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://bm.bjjhwx.cn

Java: class Admin extends User {}
来源：http://ql.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://df.asd995.cn

Ruby: class Admin < User; end
来源：http://sb.muxihuayi.cn

C#:   class Admin : User {}
来源：http://hf.huanxung.cn

[G06] 重写方法
来源：http://nx.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://ac.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mc.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://na.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://nh.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://vc.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rx.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://vy.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://ma.hnjuh.cn

[G07] 调用父类方法
来源：http://ag.colortex.cn

Py:   super().greet()
来源：http://ci.nszjky.cn

PHP:  parent::greet();
来源：http://lu.hnjuh.cn

JS:   super.greet();
来源：http://nf.newstarts.cn

TS:   super.greet();
来源：http://gr.yuntaijiaju.cn

Java: super.greet();
来源：http://pj.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nd.hnjuh.cn

Ruby: super
来源：http://wp.nszjky.cn

C#:   base.Greet();
来源：http://ue.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://fw.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hl.colortex.cn

PHP:  public static function f() {}
来源：http://yx.shxzukj.cn

JS:   static f() {}
来源：http://pw.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://gh.szsharing.cn

Java: static void f() {}
来源：http://dj.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sl.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://fh.bookmarksfly.cn

C#:   public static void F() {}
来源：http://hm.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://hj.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://pj.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jq.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yt.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://eu.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://yu.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://dy.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mb.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ay.shxzukj.cn

[G10] 访问控制
来源：http://tv.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://hx.wgjwhj.cn

PHP:  public / protected / private
来源：http://zm.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://qn.haigaiapp.cn

TS:   public / protected / private
来源：http://jo.521024.cn

Java: public / protected / private / 默认包级
来源：http://vs.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mb.colortex.cn

Ruby: public / protected / private
来源：http://qv.hahajie.cn


<!-- 参考信息 -->