代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://yp.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://in.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aa.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uy.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://lk.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vc.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oj.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://uf.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ti.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://ok.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yw.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wi.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lv.nicolike.cn

[E11] 反转字符串
来源：http://lz.hahajie.cn

Py:   s[::-1]
来源：http://zr.yuexingan06.cn

PHP:  strrev($s);
来源：http://re.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://vn.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://sp.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://td.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mb.yuntaijiaju.cn

Ruby: s.reverse
来源：http://iw.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kt.hahajie.cn

[E12] 统计某字符出现次数
来源：http://qk.newstarts.cn

Py:   s.count("a")
来源：http://ci.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://jk.nicolike.cn

JS:   s.split("a").length - 1
来源：http://ad.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ne.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jr.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://lr.hahajie.cn

Ruby: s.count("a")
来源：http://am.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://on.lnxyls.cn

[E13] 逐字符遍历
来源：http://xp.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://gm.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nx.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vh.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rc.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ov.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zr.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://md.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lw.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://dv.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nn.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kn.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://de.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ap.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vc.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pj.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iy.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ow.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://nc.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://et.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fm.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vn.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iu.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qh.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fm.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ca.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pf.lnxyls.cn

[E16] 数字千分位
来源：http://jb.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://dv.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://st.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mm.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kw.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ou.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uj.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xh.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://mn.shxzukj.cn

[E17] 首字母大写
来源：http://aq.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xg.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wd.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nb.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mz.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sg.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pl.lnxyls.cn

Ruby: s.capitalize
来源：http://zg.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dv.hnjuh.cn

[E18] 模板占位符替换
来源：http://dn.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xe.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ku.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://er.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ne.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gh.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wa.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mw.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zo.nicolike.cn

[E19] 多行文本按行拆分
来源：http://bp.muxihuayi.cn

Py:   s.splitlines()
来源：http://cg.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hk.521024.cn

JS:   s.split(/\r?\n/)
来源：http://rj.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://yn.colortex.cn

Java: s.lines().toList()
来源：http://jv.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://si.bookmarksfly.cn

Ruby: s.lines
来源：http://vm.newstarts.cn

C#:   s.Split('\n')
来源：http://wr.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://eg.yuexingan06.cn

Py:   if not s:
来源：http://kb.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qr.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uw.newstarts.cn

TS:   if (s === "") {}
来源：http://ki.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://bb.szxytkj.cn

Go:   if s == "" {}
来源：http://ng.asd995.cn

Ruby: if s.empty?
来源：http://lm.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ba.colortex.cn

[E21] 超长截断加省略号
来源：http://ol.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yb.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tc.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gx.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kq.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zq.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ao.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nz.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fx.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://lj.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kl.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iu.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ng.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ol.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qz.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kj.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ju.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yt.chemitech.net.cn

================================================================================
来源：http://uk.huixiangedu.cn

F. 文件与目录
来源：http://kg.szsharing.cn

================================================================================
来源：http://rp.hahajie.cn

[F01] 读取整个文件
来源：http://sk.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hi.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://qa.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aw.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sp.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oj.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lr.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://pr.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://md.wgjwhj.cn

[F02] 逐行读取文件
来源：http://td.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aa.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xv.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mw.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ta.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mu.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jg.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vd.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qz.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://pj.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pl.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cb.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://da.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://se.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ah.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ha.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xx.wgjwhj.cn

[F04] 追加写入文件
来源：http://bi.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dq.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vy.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zx.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sy.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://an.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dh.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hr.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kx.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://cn.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lp.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://jd.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://tm.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://zh.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ng.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wf.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://zu.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://rk.huixinmuqiang.cn

[F06] 删除文件
来源：http://ys.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://dk.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://mg.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cw.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fo.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://pr.asd995.cn

Ruby: File.delete("a.txt")
来源：http://rr.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://xv.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://ti.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vx.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ow.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qg.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jh.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lh.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mt.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yy.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ru.shtwfgs.cn

[F08] 遍历目录
来源：http://ev.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vw.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ck.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://fc.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://er.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cn.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qb.hahajie.cn

Ruby: Dir.children("dir")
来源：http://pw.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://bp.muxihuayi.cn

[F09] 获取文件大小
来源：http://wf.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://dg.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://uo.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://bk.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://zw.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fk.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zh.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ap.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://dt.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://xp.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ha.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cy.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pd.hahajie.cn

TS:   path.extname("a.txt")
来源：http://za.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://be.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xf.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hu.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nz.9csxet.cn

[F11] 复制与移动文件
来源：http://xg.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ph.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lm.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xi.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wi.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mt.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ch.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kn.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ur.haigaiapp.cn

[F12] CSV 读写
来源：http://mg.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bh.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lf.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lp.gzmigu.cn

TS:   // 同上
来源：http://ea.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bm.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gc.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lk.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gi.yuexingan06.cn

================================================================================
来源：http://hx.huixiangedu.cn

G. 面向对象
来源：http://em.huixiangedu.cn

================================================================================
来源：http://dq.huanxung.cn

[G01] 定义类
来源：http://yp.521024.cn

Py:   class User: pass
来源：http://tp.huanxung.cn

PHP:  class User {}
来源：http://us.jctech888.com.cn

JS:   class User {}
来源：http://cw.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://jk.lnxyls.cn

Java: class User {}
来源：http://az.panjiajie.cn

Go:   type User struct { Name string }
来源：http://eb.9csxet.cn

Ruby: class User; end
来源：http://zi.nszjky.cn

C#:   class User {}
来源：http://tz.huanxung.cn

[G02] 构造函数
来源：http://bm.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://pf.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://xf.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://zn.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://jq.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://oz.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uj.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://fj.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://iq.9csxet.cn

[G03] 实例属性
来源：http://ht.haigaiapp.cn

Py:   self.name = "x"
来源：http://qw.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://nj.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://li.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://tv.521024.cn

Java: private String name;
来源：http://xt.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://un.jctech888.com.cn

Ruby: @name = "x"
来源：http://kg.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://sa.jianghongdianzi.cn

[G04] 定义方法
来源：http://no.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://xj.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ee.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://zz.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://dz.shtwfgs.cn

Java: String greet() { return name; }
来源：http://iu.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pm.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ao.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ik.bookmarksfly.cn

[G05] 继承
来源：http://hp.shxzukj.cn

Py:   class Admin(User): pass
来源：http://sf.nicolike.cn

PHP:  class Admin extends User {}
来源：http://hy.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://yx.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://vs.szxytkj.cn

Java: class Admin extends User {}
来源：http://ac.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bt.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://qc.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://ck.chemitech.net.cn

[G06] 重写方法
来源：http://oz.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://uo.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ql.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://bv.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://pv.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ar.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sj.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://tc.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://gw.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ls.colortex.cn

Py:   super().greet()
来源：http://ui.shtwfgs.cn

PHP:  parent::greet();
来源：http://rq.jctech888.com.cn

JS:   super.greet();
来源：http://iu.chemitech.net.cn

TS:   super.greet();
来源：http://jn.asd995.cn

Java: super.greet();
来源：http://ie.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://so.bjjhwx.cn

Ruby: super
来源：http://zs.shxzukj.cn

C#:   base.Greet();
来源：http://ne.newstarts.cn

[G08] 静态方法与属性
来源：http://kh.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rm.chemitech.net.cn


<!-- 参考信息 -->