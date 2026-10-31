代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://mz.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://xy.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tr.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iv.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://km.yuntaijiaju.cn

[E11] 反转字符串
来源：http://md.521024.cn

Py:   s[::-1]
来源：http://bo.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://sg.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ii.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://vr.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bx.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hu.haigaiapp.cn

Ruby: s.reverse
来源：http://qh.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vr.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://nq.huanxung.cn

Py:   s.count("a")
来源：http://dp.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://kk.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://za.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ri.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gb.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://uo.huixiangedu.cn

Ruby: s.count("a")
来源：http://jq.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://qm.yuexingan06.cn

[E13] 逐字符遍历
来源：http://yf.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://gi.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ut.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jl.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mp.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fr.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kx.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ak.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tj.521024.cn

[E14] URL 编码与 Base64
来源：http://aw.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://he.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ts.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cf.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://by.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://la.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pk.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://go.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lg.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://gm.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bp.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oe.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sw.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ic.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://en.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xs.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qn.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://us.hahajie.cn

[E16] 数字千分位
来源：http://ki.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://cq.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ft.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sl.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jl.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://om.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jz.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qu.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://bl.nszjky.cn

[E17] 首字母大写
来源：http://tl.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hi.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gx.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pb.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cb.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zo.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xs.newstarts.cn

Ruby: s.capitalize
来源：http://tf.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vk.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://vs.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sc.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ow.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jk.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nd.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vh.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://by.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ih.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ug.newstarts.cn

[E19] 多行文本按行拆分
来源：http://tl.colortex.cn

Py:   s.splitlines()
来源：http://lz.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ki.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://fu.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://tz.lnxyls.cn

Java: s.lines().toList()
来源：http://ul.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://bj.nszjky.cn

Ruby: s.lines
来源：http://ax.nszjky.cn

C#:   s.Split('\n')
来源：http://pt.huanxung.cn

[E20] 判断字符串是否为空
来源：http://ue.nicolike.cn

Py:   if not s:
来源：http://th.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://va.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fv.shxzukj.cn

TS:   if (s === "") {}
来源：http://iu.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://cw.jctech888.com.cn

Go:   if s == "" {}
来源：http://ej.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://ay.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tz.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://yw.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sw.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fj.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ix.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hw.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pf.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://ep.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://is.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qg.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://uv.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zz.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jj.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bt.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lq.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://br.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://az.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://az.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vq.yuexingan06.cn

================================================================================
来源：http://rp.hnjuh.cn

F. 文件与目录
来源：http://lr.bookmarksfly.cn

================================================================================
来源：http://de.newstarts.cn

[F01] 读取整个文件
来源：http://ef.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ru.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://sz.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cm.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rr.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xn.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xh.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://we.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://xj.lnxyls.cn

[F02] 逐行读取文件
来源：http://yz.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pm.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qu.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ke.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pi.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ue.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hf.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tv.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xi.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ct.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://px.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://al.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bf.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uv.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wd.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ux.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://it.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vd.shxzukj.cn

[F04] 追加写入文件
来源：http://uv.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uw.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qc.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yf.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ew.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bg.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ed.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zy.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ev.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://tw.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wn.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://df.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://gu.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://io.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hs.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ch.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://hv.asd995.cn

C#:   File.Exists("a.txt")
来源：http://sv.9csxet.cn

[F06] 删除文件
来源：http://ph.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://ur.newstarts.cn

PHP:  unlink("a.txt");
来源：http://pn.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lg.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xy.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pp.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ny.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://zs.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://vs.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://qn.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sg.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jk.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nn.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tq.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mw.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://do.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bf.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://up.nszjky.cn

[F08] 遍历目录
来源：http://wk.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xz.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zy.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://wa.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://pt.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lg.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bn.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://kd.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://hc.yuexingan06.cn

[F09] 获取文件大小
来源：http://ny.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://zl.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ra.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ks.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://nc.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pp.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hx.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://nq.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lc.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://kr.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ic.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dw.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://td.nicolike.cn

TS:   path.extname("a.txt")
来源：http://ep.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lu.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://so.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xm.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lv.szxytkj.cn

[F11] 复制与移动文件
来源：http://uo.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://er.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zd.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hs.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jw.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://re.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ue.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://za.nicolike.cn

[F12] CSV 读写
来源：http://xj.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nh.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pb.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vv.lnxyls.cn

TS:   // 同上
来源：http://th.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xd.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xb.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://az.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nb.szsharing.cn

================================================================================
来源：http://sk.jctech888.com.cn

G. 面向对象
来源：http://id.haigaiapp.cn

================================================================================
来源：http://aj.szxytkj.cn

[G01] 定义类
来源：http://vo.muxihuayi.cn

Py:   class User: pass
来源：http://tf.gzmigu.cn

PHP:  class User {}
来源：http://es.jianghongdianzi.cn

JS:   class User {}
来源：http://vp.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://fd.colortex.cn

Java: class User {}
来源：http://df.shxzskj.cn

Go:   type User struct { Name string }
来源：http://np.chemitech.net.cn

Ruby: class User; end
来源：http://fl.haigaiapp.cn

C#:   class User {}
来源：http://uo.shtwfgs.cn

[G02] 构造函数
来源：http://hc.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://aq.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://nt.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jn.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://sf.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://oj.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ws.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://mk.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://on.asd995.cn

[G03] 实例属性
来源：http://vx.521024.cn

Py:   self.name = "x"
来源：http://kn.gzmigu.cn

PHP:  public string $name = "x";
来源：http://yy.yuexingan06.cn

JS:   this.name = "x";
来源：http://mw.shtwfgs.cn

TS:   name: string = "x";
来源：http://za.asd995.cn

Java: private String name;
来源：http://nl.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xs.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://cb.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://ah.panjiajie.cn

[G04] 定义方法
来源：http://lv.asd995.cn

Py:   def greet(self): return self.name
来源：http://hi.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tr.colortex.cn

JS:   greet() { return this.name; }
来源：http://rv.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://ny.jctech888.com.cn

Java: String greet() { return name; }
来源：http://nq.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zy.lnxyls.cn

Ruby: def greet; @name; end
来源：http://wv.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://xc.shxzskj.cn

[G05] 继承
来源：http://bu.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://zo.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://ky.shxzskj.cn

JS:   class Admin extends User {}
来源：http://nk.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://un.szxytkj.cn

Java: class Admin extends User {}
来源：http://yz.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bk.colortex.cn

Ruby: class Admin < User; end
来源：http://qe.shxzskj.cn

C#:   class Admin : User {}
来源：http://pq.bookmarksfly.cn

[G06] 重写方法
来源：http://jo.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://ow.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cg.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://di.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://nl.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://xe.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vg.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://yc.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://dn.huanxung.cn

[G07] 调用父类方法
来源：http://cv.9csxet.cn

Py:   super().greet()
来源：http://qr.huixiangedu.cn

PHP:  parent::greet();
来源：http://qb.lnxyls.cn

JS:   super.greet();
来源：http://bq.wgjwhj.cn

TS:   super.greet();
来源：http://ii.gzmigu.cn

Java: super.greet();
来源：http://vl.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://la.shxzskj.cn

Ruby: super
来源：http://vh.jctech888.com.cn

C#:   base.Greet();
来源：http://ur.huanxung.cn

[G08] 静态方法与属性
来源：http://yj.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://ny.chemitech.net.cn

JS:   static f() {}
来源：http://bz.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://hw.asd995.cn

Java: static void f() {}
来源：http://mi.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ok.9csxet.cn

Ruby: def self.f; end
来源：http://zb.bookmarksfly.cn

C#:   public static void F() {}
来源：http://kv.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://iy.shxzukj.cn


<!-- 参考信息 -->