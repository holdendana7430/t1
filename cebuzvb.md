代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ws.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dh.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yj.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lt.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ob.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ha.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nn.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://kd.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://of.521024.cn

Java: String.format("%03d", 7)
来源：http://so.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pi.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://de.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ks.chemitech.net.cn

[E11] 反转字符串
来源：http://sx.colortex.cn

Py:   s[::-1]
来源：http://ni.haigaiapp.cn

PHP:  strrev($s);
来源：http://fn.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://ud.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://do.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dt.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lh.bookmarksfly.cn

Ruby: s.reverse
来源：http://sg.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://es.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://oh.chemitech.net.cn

Py:   s.count("a")
来源：http://dw.asd995.cn

PHP:  substr_count($s, "a");
来源：http://vn.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ip.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://un.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pi.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://ec.chemitech.net.cn

Ruby: s.count("a")
来源：http://hx.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://vs.muxihuayi.cn

[E13] 逐字符遍历
来源：http://dy.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://aa.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yi.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lc.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kj.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ve.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yl.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hq.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mv.nszjky.cn

[E14] URL 编码与 Base64
来源：http://rw.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mg.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iv.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ag.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ri.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://et.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://il.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dc.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zg.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://mh.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bp.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://on.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://js.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lq.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ht.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://do.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ys.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jq.szsharing.cn

[E16] 数字千分位
来源：http://qj.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://kd.asd995.cn

PHP:  number_format(1234567);
来源：http://al.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ey.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://he.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ii.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://st.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://yy.chemitech.net.cn

[E17] 首字母大写
来源：http://af.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fu.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mu.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jk.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vz.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jg.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vx.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ey.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yi.nicolike.cn

[E18] 模板占位符替换
来源：http://eh.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rv.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ca.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jh.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zt.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gc.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wn.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vw.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://si.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://ni.wgjwhj.cn

Py:   s.splitlines()
来源：http://hm.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hq.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://cc.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://vv.colortex.cn

Java: s.lines().toList()
来源：http://xk.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://or.lnxyls.cn

Ruby: s.lines
来源：http://ru.nszjky.cn

C#:   s.Split('\n')
来源：http://uc.asd995.cn

[E20] 判断字符串是否为空
来源：http://my.bjjhwx.cn

Py:   if not s:
来源：http://cn.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pa.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://es.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ds.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://bg.szsharing.cn

Go:   if s == "" {}
来源：http://ks.hahajie.cn

Ruby: if s.empty?
来源：http://ct.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mt.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://ek.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jc.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tt.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fp.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ri.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cd.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://jh.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://im.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ya.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ru.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pk.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ai.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zi.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xr.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vc.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://an.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://ci.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://al.chemitech.net.cn

================================================================================
来源：http://wg.szsharing.cn

F. 文件与目录
来源：http://yh.9csxet.cn

================================================================================
来源：http://sz.shtwfgs.cn

[F01] 读取整个文件
来源：http://uq.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sc.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://li.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ph.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qx.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yr.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bm.szsharing.cn

Ruby: File.read("a.txt")
来源：http://on.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://qz.szsharing.cn

[F02] 逐行读取文件
来源：http://op.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vk.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eh.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ob.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kt.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://te.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yw.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jl.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mn.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://gf.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iv.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iy.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yy.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wc.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lz.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dl.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://lm.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://st.asd995.cn

[F04] 追加写入文件
来源：http://go.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ps.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gq.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mp.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zg.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://js.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://un.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kk.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://gz.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xe.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://kr.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://xp.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://dn.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pc.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fa.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://lz.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://nq.yuexingan06.cn

[F06] 删除文件
来源：http://lx.newstarts.cn

Py:   os.remove("a.txt")
来源：http://uc.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://db.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oa.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tj.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zz.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://bf.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://xn.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://uw.szsharing.cn

[F07] 创建目录（含多级）
来源：http://sc.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sj.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://au.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cg.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ft.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gy.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zl.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pl.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qu.shtwfgs.cn

[F08] 遍历目录
来源：http://mr.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tj.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yi.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://re.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://la.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aq.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vt.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://cz.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://ue.yuexingan06.cn

[F09] 获取文件大小
来源：http://px.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://hr.nszjky.cn

PHP:  filesize("a.txt");
来源：http://sb.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://al.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ce.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://js.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://en.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://oa.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://ze.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://yt.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jv.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qr.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dx.asd995.cn

TS:   path.extname("a.txt")
来源：http://gx.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sj.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zo.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ie.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lo.panjiajie.cn

[F11] 复制与移动文件
来源：http://nq.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kp.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bz.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ip.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yh.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gf.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://je.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xk.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zw.muxihuayi.cn

[F12] CSV 读写
来源：http://jx.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ej.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xi.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jg.hnjuh.cn

TS:   // 同上
来源：http://sn.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://he.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nn.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sa.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qx.hnjuh.cn

================================================================================
来源：http://nb.haigaiapp.cn

G. 面向对象
来源：http://zq.yuexingan06.cn

================================================================================
来源：http://jr.bjjhwx.cn

[G01] 定义类
来源：http://yw.szsharing.cn

Py:   class User: pass
来源：http://hp.nicolike.cn

PHP:  class User {}
来源：http://br.shxzskj.cn

JS:   class User {}
来源：http://nc.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://he.chemitech.net.cn

Java: class User {}
来源：http://oj.szsharing.cn

Go:   type User struct { Name string }
来源：http://na.9csxet.cn

Ruby: class User; end
来源：http://yc.gzmigu.cn

C#:   class User {}
来源：http://er.yuntaijiaju.cn

[G02] 构造函数
来源：http://mg.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://up.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ge.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ya.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://yr.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ps.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rq.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ge.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://og.nszjky.cn

[G03] 实例属性
来源：http://nj.muxihuayi.cn

Py:   self.name = "x"
来源：http://yf.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://yk.bjjhwx.cn

JS:   this.name = "x";
来源：http://id.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://sf.colortex.cn

Java: private String name;
来源：http://be.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uu.chemitech.net.cn

Ruby: @name = "x"
来源：http://sq.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://fd.szsharing.cn

[G04] 定义方法
来源：http://km.huanxung.cn

Py:   def greet(self): return self.name
来源：http://uu.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zy.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://nw.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://cw.muxihuayi.cn

Java: String greet() { return name; }
来源：http://hb.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ye.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://vp.nicolike.cn

C#:   public string Greet() => Name;
来源：http://of.panjiajie.cn

[G05] 继承
来源：http://bz.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://bk.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://vy.huanxung.cn

JS:   class Admin extends User {}
来源：http://mx.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://nd.9csxet.cn

Java: class Admin extends User {}
来源：http://hy.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mt.newstarts.cn

Ruby: class Admin < User; end
来源：http://kf.bjjhwx.cn

C#:   class Admin : User {}
来源：http://fu.huixinmuqiang.cn

[G06] 重写方法
来源：http://pa.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://nk.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tj.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://xr.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://wx.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://wn.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xh.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://lb.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://nf.szxytkj.cn

[G07] 调用父类方法
来源：http://ka.panjiajie.cn

Py:   super().greet()
来源：http://ug.muxihuayi.cn

PHP:  parent::greet();
来源：http://as.huixiangedu.cn

JS:   super.greet();
来源：http://sa.hahajie.cn

TS:   super.greet();
来源：http://qs.bjjhwx.cn

Java: super.greet();
来源：http://pd.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ac.yuexingan06.cn

Ruby: super
来源：http://fp.yuexingan06.cn

C#:   base.Greet();
来源：http://ed.shtwfgs.cn

[G08] 静态方法与属性
来源：http://vb.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zq.szxytkj.cn


<!-- 参考信息 -->