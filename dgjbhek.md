代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://aw.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ig.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gq.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vl.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://ve.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nz.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ba.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://is.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://dd.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://xh.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ca.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bm.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tj.huixinmuqiang.cn

[E11] 反转字符串
来源：http://vv.newstarts.cn

Py:   s[::-1]
来源：http://qr.bookmarksfly.cn

PHP:  strrev($s);
来源：http://is.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://fs.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://zd.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ya.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ow.haigaiapp.cn

Ruby: s.reverse
来源：http://ql.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nm.huanxung.cn

[E12] 统计某字符出现次数
来源：http://so.yuntaijiaju.cn

Py:   s.count("a")
来源：http://nr.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://hl.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://sf.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://be.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iq.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://yy.szsharing.cn

Ruby: s.count("a")
来源：http://xa.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://bx.haigaiapp.cn

[E13] 逐字符遍历
来源：http://fa.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://pl.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ma.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dr.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://da.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fd.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sk.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rh.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zg.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://nm.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lf.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dy.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ts.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yu.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jg.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lj.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ys.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ht.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://rx.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rb.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ih.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sx.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pd.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xw.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wr.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tx.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mk.huanxung.cn

[E16] 数字千分位
来源：http://st.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://ul.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://xh.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xt.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fm.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gp.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zy.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oe.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://hg.huanxung.cn

[E17] 首字母大写
来源：http://qz.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gy.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cs.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fw.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lm.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zz.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://za.chemitech.net.cn

Ruby: s.capitalize
来源：http://vp.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://em.chemitech.net.cn

[E18] 模板占位符替换
来源：http://nl.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nn.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tg.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://is.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vz.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qn.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dg.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kn.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ce.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://of.521024.cn

Py:   s.splitlines()
来源：http://ra.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xk.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://ca.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://ve.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://fi.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://gg.haigaiapp.cn

Ruby: s.lines
来源：http://va.9csxet.cn

C#:   s.Split('\n')
来源：http://vf.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ig.jctech888.com.cn

Py:   if not s:
来源：http://hz.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mc.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://so.shtwfgs.cn

TS:   if (s === "") {}
来源：http://db.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ex.hnjuh.cn

Go:   if s == "" {}
来源：http://ty.9csxet.cn

Ruby: if s.empty?
来源：http://zs.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://du.asd995.cn

[E21] 超长截断加省略号
来源：http://pn.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wp.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://za.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kb.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hd.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://co.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://kt.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xl.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yb.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://xu.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ie.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vn.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ce.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ye.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mn.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ik.521024.cn

Ruby: s.bytesize;  s.length
来源：http://zd.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pm.shxzukj.cn

================================================================================
来源：http://hf.huixiangedu.cn

F. 文件与目录
来源：http://ad.bjjhwx.cn

================================================================================
来源：http://yr.hahajie.cn

[F01] 读取整个文件
来源：http://nj.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ff.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://mf.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ew.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gn.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mu.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ya.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://uq.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://np.muxihuayi.cn

[F02] 逐行读取文件
来源：http://nx.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vo.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wu.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hn.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dc.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ol.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yd.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wb.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mo.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://gi.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ql.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xl.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mj.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sk.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hg.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gl.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://jz.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zt.shxzskj.cn

[F04] 追加写入文件
来源：http://rg.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ja.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rq.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mp.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pt.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lj.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://st.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ub.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tm.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://ru.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gz.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://sr.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://mq.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://sv.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zi.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nw.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://ip.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://bb.asd995.cn

[F06] 删除文件
来源：http://lg.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://zm.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://ib.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mk.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ql.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ek.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://fz.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://pr.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://cq.colortex.cn

[F07] 创建目录（含多级）
来源：http://ze.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://le.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pu.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ts.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cj.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ku.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qw.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fz.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nc.shxzskj.cn

[F08] 遍历目录
来源：http://ds.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tg.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://up.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://co.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://is.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ea.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ls.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://zx.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://bu.shxzskj.cn

[F09] 获取文件大小
来源：http://nw.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://jq.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ba.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://ue.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://hq.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vu.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mn.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://de.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ou.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://jo.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uc.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pk.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gi.hahajie.cn

TS:   path.extname("a.txt")
来源：http://yj.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zm.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oq.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://om.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nf.asd995.cn

[F11] 复制与移动文件
来源：http://yj.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qm.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vv.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lq.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oh.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://er.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ql.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bw.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gp.shtwfgs.cn

[F12] CSV 读写
来源：http://bg.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ue.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qk.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://la.newstarts.cn

TS:   // 同上
来源：http://ak.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sf.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wp.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://so.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ir.bookmarksfly.cn

================================================================================
来源：http://uo.haigaiapp.cn

G. 面向对象
来源：http://dm.hahajie.cn

================================================================================
来源：http://lc.newstarts.cn

[G01] 定义类
来源：http://gf.wgjwhj.cn

Py:   class User: pass
来源：http://lr.jctech888.com.cn

PHP:  class User {}
来源：http://br.chemitech.net.cn

JS:   class User {}
来源：http://vs.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ps.bjjhwx.cn

Java: class User {}
来源：http://gd.shxzskj.cn

Go:   type User struct { Name string }
来源：http://qw.yuntaijiaju.cn

Ruby: class User; end
来源：http://zb.newstarts.cn

C#:   class User {}
来源：http://vn.gzmigu.cn

[G02] 构造函数
来源：http://jk.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ba.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hp.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://pq.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://qp.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://cq.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jm.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://th.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://ft.huanxung.cn

[G03] 实例属性
来源：http://fh.521024.cn

Py:   self.name = "x"
来源：http://gk.asd995.cn

PHP:  public string $name = "x";
来源：http://um.szsharing.cn

JS:   this.name = "x";
来源：http://ek.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://ft.newstarts.cn

Java: private String name;
来源：http://gw.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ql.newstarts.cn

Ruby: @name = "x"
来源：http://yr.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://lv.asd995.cn

[G04] 定义方法
来源：http://um.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://my.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://il.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://nt.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://vc.nszjky.cn

Java: String greet() { return name; }
来源：http://kb.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mx.nicolike.cn

Ruby: def greet; @name; end
来源：http://bh.asd995.cn

C#:   public string Greet() => Name;
来源：http://py.szxytkj.cn

[G05] 继承
来源：http://ef.nszjky.cn

Py:   class Admin(User): pass
来源：http://me.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://hh.shxzskj.cn

JS:   class Admin extends User {}
来源：http://ql.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ek.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://er.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://su.asd995.cn

Ruby: class Admin < User; end
来源：http://um.lnxyls.cn

C#:   class Admin : User {}
来源：http://fg.jianghongdianzi.cn

[G06] 重写方法
来源：http://ko.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://qn.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zg.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://if.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://qi.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://iz.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wc.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://hn.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ua.huixiangedu.cn

[G07] 调用父类方法
来源：http://xu.521024.cn

Py:   super().greet()
来源：http://hd.newstarts.cn

PHP:  parent::greet();
来源：http://bh.szsharing.cn

JS:   super.greet();
来源：http://cb.nszjky.cn

TS:   super.greet();
来源：http://wi.bookmarksfly.cn

Java: super.greet();
来源：http://gs.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yx.colortex.cn

Ruby: super
来源：http://qf.chemitech.net.cn

C#:   base.Greet();
来源：http://ot.gzmigu.cn

[G08] 静态方法与属性
来源：http://eb.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eg.haigaiapp.cn


<!-- 参考信息 -->