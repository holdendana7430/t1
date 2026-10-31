代发 wailian999

Ruby: s.reverse
来源：http://ky.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jf.521024.cn

[E12] 统计某字符出现次数
来源：http://ou.nicolike.cn

Py:   s.count("a")
来源：http://uy.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://mf.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://gy.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://ip.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cc.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://tx.newstarts.cn

Ruby: s.count("a")
来源：http://ov.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://uy.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://gp.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://gh.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ds.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hh.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ao.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ib.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ur.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://so.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rj.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://vh.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ic.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ed.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dr.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://la.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qg.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eh.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://su.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hb.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://mq.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fd.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vb.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eq.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tc.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://za.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rm.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ep.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://to.asd995.cn

[E16] 数字千分位
来源：http://mn.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://wa.gzmigu.cn

PHP:  number_format(1234567);
来源：http://un.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ow.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uc.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hl.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rt.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vg.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://np.hnjuh.cn

[E17] 首字母大写
来源：http://xo.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uk.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yd.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xn.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fg.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zt.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dn.hnjuh.cn

Ruby: s.capitalize
来源：http://vv.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ux.haigaiapp.cn

[E18] 模板占位符替换
来源：http://fc.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ag.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iu.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vd.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ez.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tc.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wf.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fi.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zc.asd995.cn

[E19] 多行文本按行拆分
来源：http://vb.asd995.cn

Py:   s.splitlines()
来源：http://ik.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fd.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://qv.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://wf.jctech888.com.cn

Java: s.lines().toList()
来源：http://dp.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ev.9csxet.cn

Ruby: s.lines
来源：http://ma.shtwfgs.cn

C#:   s.Split('\n')
来源：http://wr.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://em.yuexingan06.cn

Py:   if not s:
来源：http://wh.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bc.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hg.shtwfgs.cn

TS:   if (s === "") {}
来源：http://vy.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://hn.nszjky.cn

Go:   if s == "" {}
来源：http://jo.shxzskj.cn

Ruby: if s.empty?
来源：http://mi.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vy.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://ti.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tc.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mp.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pq.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lj.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cl.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://zg.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ya.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fa.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://aj.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ts.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ie.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fu.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ln.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nc.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pk.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ov.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qn.bookmarksfly.cn

================================================================================
来源：http://sc.wgjwhj.cn

F. 文件与目录
来源：http://kq.huixinmuqiang.cn

================================================================================
来源：http://lr.gzmigu.cn

[F01] 读取整个文件
来源：http://eh.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rh.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://wg.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ng.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rw.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iq.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://bb.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ip.shtwfgs.cn

[F02] 逐行读取文件
来源：http://ll.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fa.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://my.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rv.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tp.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rd.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tl.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sl.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ux.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://lj.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cd.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gi.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zj.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://il.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sf.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ca.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://nl.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pa.asd995.cn

[F04] 追加写入文件
来源：http://mq.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dk.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nx.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dy.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://go.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xj.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xp.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ja.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dp.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://ud.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ew.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://ue.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://id.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://xu.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xr.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pk.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://kt.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://er.nszjky.cn

[F06] 删除文件
来源：http://ci.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://fe.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://bc.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pz.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wa.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lv.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://js.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://tg.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://ka.newstarts.cn

[F07] 创建目录（含多级）
来源：http://rm.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vg.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kl.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qm.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qk.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zr.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ot.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ka.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dp.lnxyls.cn

[F08] 遍历目录
来源：http://ql.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sv.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jh.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://zu.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://bw.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wr.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ty.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://xx.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://lg.szsharing.cn

[F09] 获取文件大小
来源：http://ag.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://ns.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ia.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://wh.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ii.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tb.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ij.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://td.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://zw.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ot.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ku.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jv.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vm.nicolike.cn

TS:   path.extname("a.txt")
来源：http://iw.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ne.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wi.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wl.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ld.szsharing.cn

[F11] 复制与移动文件
来源：http://ik.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yu.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aj.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kb.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kz.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://my.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ia.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://at.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mh.nszjky.cn

[F12] CSV 读写
来源：http://vc.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ir.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pq.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fd.panjiajie.cn

TS:   // 同上
来源：http://tz.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uq.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jb.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ze.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dw.shtwfgs.cn

================================================================================
来源：http://jq.panjiajie.cn

G. 面向对象
来源：http://jv.nszjky.cn

================================================================================
来源：http://ke.hnjuh.cn

[G01] 定义类
来源：http://mj.hnjuh.cn

Py:   class User: pass
来源：http://gj.newstarts.cn

PHP:  class User {}
来源：http://zb.lnxyls.cn

JS:   class User {}
来源：http://mi.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://ww.huixinmuqiang.cn

Java: class User {}
来源：http://vr.shxzskj.cn

Go:   type User struct { Name string }
来源：http://cg.chemitech.net.cn

Ruby: class User; end
来源：http://rz.lnxyls.cn

C#:   class User {}
来源：http://qc.jianghongdianzi.cn

[G02] 构造函数
来源：http://sq.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://rl.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://sz.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://jq.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://tz.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://br.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jf.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://hk.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://zo.muxihuayi.cn

[G03] 实例属性
来源：http://wg.shxzukj.cn

Py:   self.name = "x"
来源：http://fc.nszjky.cn

PHP:  public string $name = "x";
来源：http://mx.shxzukj.cn

JS:   this.name = "x";
来源：http://ad.shxzskj.cn

TS:   name: string = "x";
来源：http://fg.huanxung.cn

Java: private String name;
来源：http://vl.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nm.shtwfgs.cn

Ruby: @name = "x"
来源：http://gf.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://mz.chemitech.net.cn

[G04] 定义方法
来源：http://bx.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://pd.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gt.huanxung.cn

JS:   greet() { return this.name; }
来源：http://kx.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://dw.huanxung.cn

Java: String greet() { return name; }
来源：http://wx.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lj.shxzskj.cn

Ruby: def greet; @name; end
来源：http://pg.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ib.jianghongdianzi.cn

[G05] 继承
来源：http://yh.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://mh.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://yq.szxytkj.cn

JS:   class Admin extends User {}
来源：http://kb.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://yk.jctech888.com.cn

Java: class Admin extends User {}
来源：http://az.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vf.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://xg.panjiajie.cn

C#:   class Admin : User {}
来源：http://hy.nszjky.cn

[G06] 重写方法
来源：http://fi.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://cw.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ji.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://pr.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://nt.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://fl.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ev.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ou.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://jf.shtwfgs.cn

[G07] 调用父类方法
来源：http://df.jctech888.com.cn

Py:   super().greet()
来源：http://by.lnxyls.cn

PHP:  parent::greet();
来源：http://rb.muxihuayi.cn

JS:   super.greet();
来源：http://nt.szxytkj.cn

TS:   super.greet();
来源：http://kw.gzmigu.cn

Java: super.greet();
来源：http://gy.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dd.szxytkj.cn

Ruby: super
来源：http://gw.chemitech.net.cn

C#:   base.Greet();
来源：http://wr.gzmigu.cn

[G08] 静态方法与属性
来源：http://hu.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nq.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://oe.shxzskj.cn

JS:   static f() {}
来源：http://kc.hnjuh.cn

TS:   static f(): void {}
来源：http://na.yuexingan06.cn

Java: static void f() {}
来源：http://ti.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xs.newstarts.cn

Ruby: def self.f; end
来源：http://ga.haigaiapp.cn

C#:   public static void F() {}
来源：http://cj.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://xx.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://kw.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oa.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://da.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://it.hahajie.cn

Java: interface Shape { double area(); }
来源：http://lq.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://vf.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://go.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://nn.panjiajie.cn

[G10] 访问控制
来源：http://ax.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://iu.haigaiapp.cn

PHP:  public / protected / private
来源：http://gs.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://ta.colortex.cn


<!-- 参考信息 -->