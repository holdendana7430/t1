代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://al.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xs.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fr.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qq.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://is.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wj.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ll.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://cz.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://aw.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ck.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pj.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zq.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ja.521024.cn

[E11] 反转字符串
来源：http://bn.newstarts.cn

Py:   s[::-1]
来源：http://gq.asd995.cn

PHP:  strrev($s);
来源：http://rq.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://cp.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://qc.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qq.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://so.wgjwhj.cn

Ruby: s.reverse
来源：http://dk.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xi.hahajie.cn

[E12] 统计某字符出现次数
来源：http://ma.shxzskj.cn

Py:   s.count("a")
来源：http://yo.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://ut.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://aa.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://zc.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vj.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://ru.lnxyls.cn

Ruby: s.count("a")
来源：http://xk.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://xr.jctech888.com.cn

[E13] 逐字符遍历
来源：http://we.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://up.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xq.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ot.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nj.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pu.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jc.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bs.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kk.521024.cn

[E14] URL 编码与 Base64
来源：http://ma.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hj.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dr.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vt.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://on.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://el.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tz.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yc.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eh.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://lj.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vl.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qd.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hb.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vj.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kj.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jt.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uk.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yo.jctech888.com.cn

[E16] 数字千分位
来源：http://fx.521024.cn

Py:   f"{1234567:,}"
来源：http://wk.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://fl.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vo.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ha.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mv.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ck.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ec.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://gq.gzmigu.cn

[E17] 首字母大写
来源：http://gf.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nv.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pg.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oa.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dx.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cm.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qo.yuexingan06.cn

Ruby: s.capitalize
来源：http://fq.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ux.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://pk.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lz.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ps.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tn.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yj.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vf.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ta.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vw.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mv.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://qc.bookmarksfly.cn

Py:   s.splitlines()
来源：http://vs.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mk.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://hj.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ja.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ff.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://xo.shxzskj.cn

Ruby: s.lines
来源：http://wd.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ea.huanxung.cn

[E20] 判断字符串是否为空
来源：http://xe.jianghongdianzi.cn

Py:   if not s:
来源：http://qp.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ec.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rk.gzmigu.cn

TS:   if (s === "") {}
来源：http://qn.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://sb.haigaiapp.cn

Go:   if s == "" {}
来源：http://pz.jctech888.com.cn

Ruby: if s.empty?
来源：http://jp.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://af.asd995.cn

[E21] 超长截断加省略号
来源：http://pl.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ln.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yr.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oc.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zz.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bs.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://ib.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hg.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jh.hahajie.cn

[E22] 字节长度与字符长度
来源：http://fs.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://um.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cw.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://js.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cn.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tm.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://jf.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zg.521024.cn

================================================================================
来源：http://gr.bookmarksfly.cn

F. 文件与目录
来源：http://bt.asd995.cn

================================================================================
来源：http://bl.521024.cn

[F01] 读取整个文件
来源：http://qu.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bp.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://hn.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hn.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ih.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://am.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://bw.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ne.asd995.cn

[F02] 逐行读取文件
来源：http://hk.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fo.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nc.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sr.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yx.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fz.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mm.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wr.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qt.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://qn.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jv.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gv.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iy.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ld.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ah.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://dw.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ud.szxytkj.cn

[F04] 追加写入文件
来源：http://tj.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sc.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jh.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qy.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rq.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ke.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sh.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yw.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zd.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://gt.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cz.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://ak.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://na.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://ov.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ai.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wr.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://ti.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://gn.yuntaijiaju.cn

[F06] 删除文件
来源：http://uk.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://fv.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://yo.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cw.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nt.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kh.521024.cn

Go:   os.Remove("a.txt")
来源：http://cw.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://dq.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://xp.521024.cn

[F07] 创建目录（含多级）
来源：http://nx.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zj.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aj.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fi.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ww.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vw.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rr.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sd.shtwfgs.cn

[F08] 遍历目录
来源：http://hj.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://de.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fb.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://va.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://uf.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ry.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bg.9csxet.cn

Ruby: Dir.children("dir")
来源：http://gz.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://sf.hnjuh.cn

[F09] 获取文件大小
来源：http://qa.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://gh.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://fd.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ol.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://qm.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fw.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uh.9csxet.cn

Ruby: File.size("a.txt")
来源：http://po.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://pf.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://eh.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jv.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yv.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jo.newstarts.cn

TS:   path.extname("a.txt")
来源：http://zs.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ev.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iu.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ir.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mu.nszjky.cn

[F11] 复制与移动文件
来源：http://gj.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bt.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gs.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ov.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sz.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bq.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oz.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bo.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fb.shxzukj.cn

[F12] CSV 读写
来源：http://tg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hd.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xf.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bs.9csxet.cn

TS:   // 同上
来源：http://zd.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wv.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sk.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nm.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xi.newstarts.cn

================================================================================
来源：http://yz.nicolike.cn

G. 面向对象
来源：http://ph.jianghongdianzi.cn

================================================================================
来源：http://vy.szxytkj.cn

[G01] 定义类
来源：http://ry.jianghongdianzi.cn

Py:   class User: pass
来源：http://oq.jctech888.com.cn

PHP:  class User {}
来源：http://jk.shxzukj.cn

JS:   class User {}
来源：http://fo.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://ef.muxihuayi.cn

Java: class User {}
来源：http://gd.shxzskj.cn

Go:   type User struct { Name string }
来源：http://si.asd995.cn

Ruby: class User; end
来源：http://mz.gzmigu.cn

C#:   class User {}
来源：http://fi.yuexingan06.cn

[G02] 构造函数
来源：http://ij.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://su.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://pe.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://cy.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://vn.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://rt.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ap.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://de.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://eb.shxzukj.cn

[G03] 实例属性
来源：http://qx.521024.cn

Py:   self.name = "x"
来源：http://au.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://yo.colortex.cn

JS:   this.name = "x";
来源：http://ne.huanxung.cn

TS:   name: string = "x";
来源：http://gn.lnxyls.cn

Java: private String name;
来源：http://uw.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sh.huixiangedu.cn

Ruby: @name = "x"
来源：http://gb.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://gw.521024.cn

[G04] 定义方法
来源：http://ly.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://pr.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qb.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ip.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://ax.szxytkj.cn

Java: String greet() { return name; }
来源：http://kz.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xp.asd995.cn

Ruby: def greet; @name; end
来源：http://ny.nicolike.cn

C#:   public string Greet() => Name;
来源：http://sn.huixinmuqiang.cn

[G05] 继承
来源：http://fb.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ne.9csxet.cn

PHP:  class Admin extends User {}
来源：http://kp.panjiajie.cn

JS:   class Admin extends User {}
来源：http://jc.szsharing.cn

TS:   class Admin extends User {}
来源：http://ha.nszjky.cn

Java: class Admin extends User {}
来源：http://zf.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tq.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://rc.colortex.cn

C#:   class Admin : User {}
来源：http://om.bookmarksfly.cn

[G06] 重写方法
来源：http://nm.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://jr.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kg.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://zl.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://vl.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://if.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vl.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://cb.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://gk.hnjuh.cn

[G07] 调用父类方法
来源：http://yf.521024.cn

Py:   super().greet()
来源：http://uc.asd995.cn

PHP:  parent::greet();
来源：http://cp.gzmigu.cn

JS:   super.greet();
来源：http://jt.huixinmuqiang.cn

TS:   super.greet();
来源：http://ds.shxzukj.cn

Java: super.greet();
来源：http://jq.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gw.gzmigu.cn

Ruby: super
来源：http://po.panjiajie.cn

C#:   base.Greet();
来源：http://wx.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://eq.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tc.hahajie.cn


<!-- 参考信息 -->