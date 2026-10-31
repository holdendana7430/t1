代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://vg.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dm.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xr.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://af.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://mm.huanxung.cn

Java: String.format("%03d", 7)
来源：http://dn.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nr.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ax.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yw.panjiajie.cn

[E11] 反转字符串
来源：http://zg.hahajie.cn

Py:   s[::-1]
来源：http://qf.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://it.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ie.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://oz.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gp.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nu.huanxung.cn

Ruby: s.reverse
来源：http://rw.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ap.colortex.cn

[E12] 统计某字符出现次数
来源：http://sw.wgjwhj.cn

Py:   s.count("a")
来源：http://ga.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://ed.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://jv.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ik.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bx.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://aa.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://pl.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://hf.muxihuayi.cn

[E13] 逐字符遍历
来源：http://hd.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://bt.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rz.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jf.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://op.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sg.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ku.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wq.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jo.9csxet.cn

[E14] URL 编码与 Base64
来源：http://og.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zx.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ws.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uk.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oy.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vd.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fw.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uu.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gr.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ad.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ij.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qm.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://as.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ex.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mf.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bn.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qg.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kt.szxytkj.cn

[E16] 数字千分位
来源：http://of.9csxet.cn

Py:   f"{1234567:,}"
来源：http://yc.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://fr.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ne.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yg.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kq.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kt.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xx.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://fz.haigaiapp.cn

[E17] 首字母大写
来源：http://df.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ym.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bk.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ly.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kh.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ay.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nn.colortex.cn

Ruby: s.capitalize
来源：http://yy.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gy.lnxyls.cn

[E18] 模板占位符替换
来源：http://js.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://se.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://np.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yl.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://os.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://av.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zc.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dh.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://cz.szxytkj.cn

Py:   s.splitlines()
来源：http://zg.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ua.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://zx.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://hx.shxzskj.cn

Java: s.lines().toList()
来源：http://wi.521024.cn

Go:   strings.Split(s, "\n")
来源：http://oa.asd995.cn

Ruby: s.lines
来源：http://yi.huixiangedu.cn

C#:   s.Split('\n')
来源：http://bc.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://sb.hahajie.cn

Py:   if not s:
来源：http://bj.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wj.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wm.huanxung.cn

TS:   if (s === "") {}
来源：http://ru.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://lo.szsharing.cn

Go:   if s == "" {}
来源：http://sc.wgjwhj.cn

Ruby: if s.empty?
来源：http://um.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ga.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://vu.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hv.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://at.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://km.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kl.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://nw.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ts.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ov.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://ux.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sn.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lr.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lt.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://di.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ry.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sl.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://zp.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hx.panjiajie.cn

================================================================================
来源：http://zt.shtwfgs.cn

F. 文件与目录
来源：http://rr.bookmarksfly.cn

================================================================================
来源：http://ep.huanxung.cn

[F01] 读取整个文件
来源：http://jc.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fh.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://lx.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hq.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pg.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://no.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oq.hahajie.cn

Ruby: File.read("a.txt")
来源：http://zi.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://sj.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ar.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ft.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://po.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dp.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cv.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vg.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ox.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ph.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tg.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://dm.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kk.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pd.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uw.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vu.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yl.haigaiapp.cn

[F04] 追加写入文件
来源：http://xd.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yj.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dt.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ue.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sv.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ko.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zb.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oh.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jp.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://et.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jt.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://tv.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://tx.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://wf.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pv.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rd.521024.cn

Ruby: File.exist?("a.txt")
来源：http://cd.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://yq.jctech888.com.cn

[F06] 删除文件
来源：http://zb.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://jo.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://gk.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nr.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fz.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ik.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://on.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ni.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://vi.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://wc.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qi.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vw.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jt.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vl.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://om.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mx.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yl.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ev.wgjwhj.cn

[F08] 遍历目录
来源：http://tu.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zv.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ft.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://jn.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://ek.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sc.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gg.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://mi.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://qw.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://ts.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://pz.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://rg.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://wk.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ez.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://js.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ff.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ez.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://tt.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ry.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bs.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sm.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iv.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://nx.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bg.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uo.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oa.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ew.gzmigu.cn

[F11] 复制与移动文件
来源：http://ae.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wq.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tl.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vh.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fc.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dd.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ki.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fp.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qs.szsharing.cn

[F12] CSV 读写
来源：http://jp.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gz.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vr.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jl.colortex.cn

TS:   // 同上
来源：http://ze.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gk.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dn.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ek.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ap.yuntaijiaju.cn

================================================================================
来源：http://qo.jianghongdianzi.cn

G. 面向对象
来源：http://hm.chemitech.net.cn

================================================================================
来源：http://ul.haigaiapp.cn

[G01] 定义类
来源：http://ui.shxzukj.cn

Py:   class User: pass
来源：http://wm.jctech888.com.cn

PHP:  class User {}
来源：http://so.huixinmuqiang.cn

JS:   class User {}
来源：http://dk.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://tm.jianghongdianzi.cn

Java: class User {}
来源：http://ii.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://nt.muxihuayi.cn

Ruby: class User; end
来源：http://lp.muxihuayi.cn

C#:   class User {}
来源：http://yr.shtwfgs.cn

[G02] 构造函数
来源：http://jq.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://fk.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://bu.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ki.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://gn.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://ip.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ht.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://lz.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://qn.szxytkj.cn

[G03] 实例属性
来源：http://rt.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://hx.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://id.shxzukj.cn

JS:   this.name = "x";
来源：http://kh.asd995.cn

TS:   name: string = "x";
来源：http://ij.yuexingan06.cn

Java: private String name;
来源：http://xo.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xp.asd995.cn

Ruby: @name = "x"
来源：http://lw.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://qq.szxytkj.cn

[G04] 定义方法
来源：http://yc.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://mv.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xm.9csxet.cn

JS:   greet() { return this.name; }
来源：http://ei.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://rg.lnxyls.cn

Java: String greet() { return name; }
来源：http://bc.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sy.newstarts.cn

Ruby: def greet; @name; end
来源：http://gb.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://pi.hnjuh.cn

[G05] 继承
来源：http://mg.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://in.nicolike.cn

PHP:  class Admin extends User {}
来源：http://gi.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://sg.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://em.hnjuh.cn

Java: class Admin extends User {}
来源：http://ew.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ul.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://gy.muxihuayi.cn

C#:   class Admin : User {}
来源：http://tz.haigaiapp.cn

[G06] 重写方法
来源：http://lw.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ov.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nc.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://pt.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://am.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ru.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oq.521024.cn

Ruby: def greet; "admin"; end
来源：http://im.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ve.haigaiapp.cn

[G07] 调用父类方法
来源：http://sm.huixiangedu.cn

Py:   super().greet()
来源：http://zq.yuexingan06.cn

PHP:  parent::greet();
来源：http://uu.panjiajie.cn

JS:   super.greet();
来源：http://jp.shtwfgs.cn

TS:   super.greet();
来源：http://mj.521024.cn

Java: super.greet();
来源：http://bo.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bd.colortex.cn

Ruby: super
来源：http://kt.hahajie.cn

C#:   base.Greet();
来源：http://bm.nszjky.cn

[G08] 静态方法与属性
来源：http://qw.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jh.hahajie.cn

PHP:  public static function f() {}
来源：http://cn.wgjwhj.cn

JS:   static f() {}
来源：http://it.asd995.cn

TS:   static f(): void {}
来源：http://ro.jctech888.com.cn

Java: static void f() {}
来源：http://ji.yuntaijiaju.cn


<!-- 参考信息 -->