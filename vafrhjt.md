代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://kn.asd995.cn

Java: String.format("%03d", 7)
来源：http://hu.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://io.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nc.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mg.nicolike.cn

[E11] 反转字符串
来源：http://wd.muxihuayi.cn

Py:   s[::-1]
来源：http://ue.szsharing.cn

PHP:  strrev($s);
来源：http://ve.asd995.cn

JS:   [...s].reverse().join("")
来源：http://el.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://ip.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://go.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vf.szxytkj.cn

Ruby: s.reverse
来源：http://rw.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ld.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://oa.shxzukj.cn

Py:   s.count("a")
来源：http://kr.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://ti.colortex.cn

JS:   s.split("a").length - 1
来源：http://ju.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://wj.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wx.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://rz.szxytkj.cn

Ruby: s.count("a")
来源：http://xl.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://mw.hnjuh.cn

[E13] 逐字符遍历
来源：http://ov.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://su.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mv.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xd.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://te.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://as.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://np.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://az.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cq.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://td.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cs.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ww.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xw.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sx.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ch.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jp.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ka.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fb.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://wt.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qv.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ie.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zw.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rd.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dy.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nm.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jj.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zi.9csxet.cn

[E16] 数字千分位
来源：http://zz.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ul.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://ni.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ja.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vr.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gv.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hp.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qo.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://uv.huixiangedu.cn

[E17] 首字母大写
来源：http://iw.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qm.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://is.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yb.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://my.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wc.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://el.nszjky.cn

Ruby: s.capitalize
来源：http://qo.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gu.hnjuh.cn

[E18] 模板占位符替换
来源：http://zs.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pe.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dd.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ha.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ql.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kf.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uu.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wm.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xl.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://up.shxzukj.cn

Py:   s.splitlines()
来源：http://pf.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ze.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://sx.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://za.szsharing.cn

Java: s.lines().toList()
来源：http://fk.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://hs.asd995.cn

Ruby: s.lines
来源：http://ul.huixiangedu.cn

C#:   s.Split('\n')
来源：http://pj.huanxung.cn

[E20] 判断字符串是否为空
来源：http://hu.jianghongdianzi.cn

Py:   if not s:
来源：http://kg.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jp.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://df.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://bn.521024.cn

Java: if (s.isEmpty()) {}
来源：http://wx.asd995.cn

Go:   if s == "" {}
来源：http://fc.shtwfgs.cn

Ruby: if s.empty?
来源：http://wy.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://br.hahajie.cn

[E21] 超长截断加省略号
来源：http://wx.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nj.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rr.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xm.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vy.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nq.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ah.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ey.szsharing.cn

[E22] 字节长度与字符长度
来源：http://hm.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vq.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rb.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ci.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bm.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dg.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ot.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://xk.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vk.colortex.cn

================================================================================
来源：http://bl.nicolike.cn

F. 文件与目录
来源：http://mo.bookmarksfly.cn

================================================================================
来源：http://vy.shxzskj.cn

[F01] 读取整个文件
来源：http://aa.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bj.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ui.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vw.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yv.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bi.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jz.asd995.cn

Ruby: File.read("a.txt")
来源：http://dd.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://rj.lnxyls.cn

[F02] 逐行读取文件
来源：http://lg.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://va.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dh.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ko.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tu.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vr.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mp.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://df.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://ro.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ty.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nz.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://am.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sp.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wo.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xp.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://pu.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xd.521024.cn

[F04] 追加写入文件
来源：http://ip.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zm.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jv.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ss.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sh.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qf.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jt.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ru.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xy.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://xf.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ou.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://ly.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://jh.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://el.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lg.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gr.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://mv.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://bv.huixinmuqiang.cn

[F06] 删除文件
来源：http://av.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://hg.colortex.cn

PHP:  unlink("a.txt");
来源：http://ak.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vj.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rf.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qr.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://cp.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://xy.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://qu.huanxung.cn

[F07] 创建目录（含多级）
来源：http://nd.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cj.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ta.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wn.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kw.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://md.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ui.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bz.bjjhwx.cn

[F08] 遍历目录
来源：http://bp.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kb.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://js.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://wt.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://sn.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sp.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ek.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://hp.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://fa.hnjuh.cn

[F09] 获取文件大小
来源：http://au.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://om.9csxet.cn

PHP:  filesize("a.txt");
来源：http://ep.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://wx.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://vm.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lw.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nh.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://ij.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lk.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lj.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kv.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://es.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jw.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://dl.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cb.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://up.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iy.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ul.chemitech.net.cn

[F11] 复制与移动文件
来源：http://pz.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wk.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nm.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://op.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ji.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yc.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ev.9csxet.cn

[F12] CSV 读写
来源：http://pi.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ys.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qn.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ow.9csxet.cn

TS:   // 同上
来源：http://mi.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rh.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nq.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lc.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hd.shxzukj.cn

================================================================================
来源：http://tm.jctech888.com.cn

G. 面向对象
来源：http://oz.bookmarksfly.cn

================================================================================
来源：http://ft.muxihuayi.cn

[G01] 定义类
来源：http://qj.nicolike.cn

Py:   class User: pass
来源：http://tq.jianghongdianzi.cn

PHP:  class User {}
来源：http://kx.bjjhwx.cn

JS:   class User {}
来源：http://wh.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://mp.asd995.cn

Java: class User {}
来源：http://tp.shxzskj.cn

Go:   type User struct { Name string }
来源：http://fr.yuntaijiaju.cn

Ruby: class User; end
来源：http://io.szxytkj.cn

C#:   class User {}
来源：http://jr.panjiajie.cn

[G02] 构造函数
来源：http://fq.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://aq.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://ew.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ez.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://wf.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://mm.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dd.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://uu.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://ko.asd995.cn

[G03] 实例属性
来源：http://xk.yuexingan06.cn

Py:   self.name = "x"
来源：http://kc.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://nj.huixiangedu.cn

JS:   this.name = "x";
来源：http://tf.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://po.9csxet.cn

Java: private String name;
来源：http://ex.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nt.newstarts.cn

Ruby: @name = "x"
来源：http://tt.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cs.szsharing.cn

[G04] 定义方法
来源：http://lm.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://kg.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fn.szsharing.cn

JS:   greet() { return this.name; }
来源：http://og.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://tf.chemitech.net.cn

Java: String greet() { return name; }
来源：http://nb.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mp.nicolike.cn

Ruby: def greet; @name; end
来源：http://lf.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://ey.hnjuh.cn

[G05] 继承
来源：http://il.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://bv.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://kt.asd995.cn

JS:   class Admin extends User {}
来源：http://ko.panjiajie.cn

TS:   class Admin extends User {}
来源：http://le.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://mz.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gg.panjiajie.cn

Ruby: class Admin < User; end
来源：http://bt.lnxyls.cn

C#:   class Admin : User {}
来源：http://ms.newstarts.cn

[G06] 重写方法
来源：http://qy.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ee.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kt.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://hd.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://yc.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://jy.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gr.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://gp.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://oz.huanxung.cn

[G07] 调用父类方法
来源：http://kb.nszjky.cn

Py:   super().greet()
来源：http://uf.9csxet.cn

PHP:  parent::greet();
来源：http://pf.haigaiapp.cn

JS:   super.greet();
来源：http://ud.shxzskj.cn

TS:   super.greet();
来源：http://zo.panjiajie.cn

Java: super.greet();
来源：http://lc.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cp.gzmigu.cn

Ruby: super
来源：http://se.jianghongdianzi.cn

C#:   base.Greet();
来源：http://jz.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://yz.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kz.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://wf.lnxyls.cn

JS:   static f() {}
来源：http://uq.bookmarksfly.cn

TS:   static f(): void {}
来源：http://hi.huixiangedu.cn

Java: static void f() {}
来源：http://iu.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zr.jctech888.com.cn

Ruby: def self.f; end
来源：http://dj.panjiajie.cn

C#:   public static void F() {}
来源：http://ic.9csxet.cn

[G09] 接口 / 抽象类
来源：http://nf.yuexingan06.cn


<!-- 参考信息 -->