代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://nu.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nt.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ra.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fs.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://fn.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://en.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fh.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://vh.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://pk.hahajie.cn

Java: String.format("%03d", 7)
来源：http://jo.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ab.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ri.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mz.wgjwhj.cn

[E11] 反转字符串
来源：http://tm.hnjuh.cn

Py:   s[::-1]
来源：http://zm.panjiajie.cn

PHP:  strrev($s);
来源：http://wq.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://mp.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://rs.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://px.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://um.huixiangedu.cn

Ruby: s.reverse
来源：http://ij.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gn.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://sh.huixinmuqiang.cn

Py:   s.count("a")
来源：http://um.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://cq.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://fg.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://qz.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dt.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://kj.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://cv.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://oz.shxzskj.cn

[E13] 逐字符遍历
来源：http://nf.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://gx.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tj.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pc.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wi.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ay.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oi.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gj.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gr.asd995.cn

[E14] URL 编码与 Base64
来源：http://ep.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oq.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rb.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sy.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yz.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tr.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ye.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tt.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zk.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://cj.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nq.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yn.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yx.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cp.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kk.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aa.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nh.lnxyls.cn

[E16] 数字千分位
来源：http://xe.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://bd.hahajie.cn

PHP:  number_format(1234567);
来源：http://sk.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gr.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ti.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ee.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://px.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ri.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://kd.haigaiapp.cn

[E17] 首字母大写
来源：http://uk.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://an.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ov.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hx.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ht.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sv.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xt.shxzskj.cn

Ruby: s.capitalize
来源：http://sj.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mi.521024.cn

[E18] 模板占位符替换
来源：http://ju.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://op.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nx.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ef.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ku.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nl.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rj.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bb.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zp.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://pj.haigaiapp.cn

Py:   s.splitlines()
来源：http://pz.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zq.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://se.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://zp.hahajie.cn

Java: s.lines().toList()
来源：http://sl.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://nl.szsharing.cn

Ruby: s.lines
来源：http://od.asd995.cn

C#:   s.Split('\n')
来源：http://fn.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://uv.hnjuh.cn

Py:   if not s:
来源：http://ow.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rm.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bg.jctech888.com.cn

TS:   if (s === "") {}
来源：http://mw.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://bb.wgjwhj.cn

Go:   if s == "" {}
来源：http://ek.szsharing.cn

Ruby: if s.empty?
来源：http://wp.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zh.521024.cn

[E21] 超长截断加省略号
来源：http://ll.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xe.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vn.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rf.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wd.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ug.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://wj.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://si.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eh.huanxung.cn

[E22] 字节长度与字符长度
来源：http://lf.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sx.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hk.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qr.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jt.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iz.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xn.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://jc.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lt.huanxung.cn

================================================================================
来源：http://rc.shxzukj.cn

F. 文件与目录
来源：http://bg.newstarts.cn

================================================================================
来源：http://ql.9csxet.cn

[F01] 读取整个文件
来源：http://jf.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vd.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://si.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xh.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yx.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xp.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://an.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://uw.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://am.hnjuh.cn

[F02] 逐行读取文件
来源：http://qb.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ce.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://su.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pt.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pb.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ys.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ur.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fu.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bc.521024.cn

[F03] 写入文件（覆盖）
来源：http://se.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bp.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://go.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hw.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qh.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mu.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ix.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://vm.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xy.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://ip.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pt.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xq.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dg.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fz.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rt.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zx.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fd.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wv.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://qy.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xv.521024.cn

PHP:  file_exists("a.txt");
来源：http://pz.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://rb.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://nl.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bn.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iv.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://rx.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://wo.huixiangedu.cn

[F06] 删除文件
来源：http://mh.szsharing.cn

Py:   os.remove("a.txt")
来源：http://yn.asd995.cn

PHP:  unlink("a.txt");
来源：http://da.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ed.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dt.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ez.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://hq.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://od.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://lo.newstarts.cn

[F07] 创建目录（含多级）
来源：http://mk.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sj.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ay.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xt.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nq.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pp.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gb.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nx.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gg.bookmarksfly.cn

[F08] 遍历目录
来源：http://ub.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tb.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uu.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://qh.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://zf.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ya.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://oy.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://xg.gzmigu.cn

[F09] 获取文件大小
来源：http://dk.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://ql.hahajie.cn

PHP:  filesize("a.txt");
来源：http://vv.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://kq.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://ew.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zm.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wv.newstarts.cn

Ruby: File.size("a.txt")
来源：http://xp.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ub.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://xe.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://za.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xi.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zv.huanxung.cn

TS:   path.extname("a.txt")
来源：http://ux.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xg.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ea.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cj.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rz.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://lm.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fe.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nd.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lk.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ur.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wk.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://el.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ke.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wg.lnxyls.cn

[F12] CSV 读写
来源：http://zn.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fm.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kw.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ne.nszjky.cn

TS:   // 同上
来源：http://mv.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oq.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mz.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ar.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ik.hnjuh.cn

================================================================================
来源：http://xh.szxytkj.cn

G. 面向对象
来源：http://oz.muxihuayi.cn

================================================================================
来源：http://jg.gzmigu.cn

[G01] 定义类
来源：http://xq.bookmarksfly.cn

Py:   class User: pass
来源：http://wh.hnjuh.cn

PHP:  class User {}
来源：http://iw.jctech888.com.cn

JS:   class User {}
来源：http://mx.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://zj.lnxyls.cn

Java: class User {}
来源：http://ea.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ht.gzmigu.cn

Ruby: class User; end
来源：http://mw.newstarts.cn

C#:   class User {}
来源：http://vo.nicolike.cn

[G02] 构造函数
来源：http://jj.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://xz.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://js.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://eu.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://jq.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ec.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bp.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://gi.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://qb.9csxet.cn

[G03] 实例属性
来源：http://ib.hahajie.cn

Py:   self.name = "x"
来源：http://oa.asd995.cn

PHP:  public string $name = "x";
来源：http://sr.szsharing.cn

JS:   this.name = "x";
来源：http://uh.asd995.cn

TS:   name: string = "x";
来源：http://aa.huanxung.cn

Java: private String name;
来源：http://hp.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rw.hnjuh.cn

Ruby: @name = "x"
来源：http://sx.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ta.9csxet.cn

[G04] 定义方法
来源：http://fm.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://un.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yo.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://nw.521024.cn

TS:   greet(): string { return this.name; }
来源：http://cc.lnxyls.cn

Java: String greet() { return name; }
来源：http://sv.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://im.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://sh.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://re.521024.cn

[G05] 继承
来源：http://uw.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://wz.nicolike.cn

PHP:  class Admin extends User {}
来源：http://hv.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://av.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://wl.newstarts.cn

Java: class Admin extends User {}
来源：http://sc.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dn.colortex.cn

Ruby: class Admin < User; end
来源：http://fq.chemitech.net.cn

C#:   class Admin : User {}
来源：http://yp.huixiangedu.cn

[G06] 重写方法
来源：http://xo.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://hb.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nc.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ws.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://fv.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://qo.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yf.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://tz.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ts.jctech888.com.cn

[G07] 调用父类方法
来源：http://ny.521024.cn

Py:   super().greet()
来源：http://kt.chemitech.net.cn

PHP:  parent::greet();
来源：http://wh.yuntaijiaju.cn

JS:   super.greet();
来源：http://nz.hnjuh.cn

TS:   super.greet();
来源：http://tn.muxihuayi.cn

Java: super.greet();
来源：http://db.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xk.huanxung.cn

Ruby: super
来源：http://nx.huixiangedu.cn

C#:   base.Greet();
来源：http://xe.hnjuh.cn

[G08] 静态方法与属性
来源：http://us.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://um.huixinmuqiang.cn


<!-- 参考信息 -->