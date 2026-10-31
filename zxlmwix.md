代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ku.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://eg.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://se.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ko.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rj.yuntaijiaju.cn

[E11] 反转字符串
来源：http://kt.bjjhwx.cn

Py:   s[::-1]
来源：http://mc.nicolike.cn

PHP:  strrev($s);
来源：http://ch.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://uw.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://dt.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mb.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hp.shxzskj.cn

Ruby: s.reverse
来源：http://ez.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zi.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://lt.asd995.cn

Py:   s.count("a")
来源：http://yb.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://qq.szsharing.cn

JS:   s.split("a").length - 1
来源：http://cu.huanxung.cn

TS:   s.split("a").length - 1
来源：http://li.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jh.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://gd.shxzukj.cn

Ruby: s.count("a")
来源：http://aj.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://pw.jctech888.com.cn

[E13] 逐字符遍历
来源：http://dm.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://bg.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dk.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://to.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ru.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oq.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sm.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://il.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ki.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://sw.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cl.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nm.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://co.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lr.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fc.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cr.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ww.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://ph.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kz.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lx.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ee.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mp.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ee.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://id.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lj.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xt.newstarts.cn

[E16] 数字千分位
来源：http://du.nszjky.cn

Py:   f"{1234567:,}"
来源：http://mp.hahajie.cn

PHP:  number_format(1234567);
来源：http://je.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mz.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kr.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wc.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vv.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vt.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://wa.wgjwhj.cn

[E17] 首字母大写
来源：http://sk.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ze.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ji.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yw.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kg.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ya.muxihuayi.cn

Ruby: s.capitalize
来源：http://lt.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://au.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://iw.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xo.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tq.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ag.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rx.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yz.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vy.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://et.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hx.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://yj.haigaiapp.cn

Py:   s.splitlines()
来源：http://rq.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rr.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ht.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://am.asd995.cn

Java: s.lines().toList()
来源：http://my.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://nv.bookmarksfly.cn

Ruby: s.lines
来源：http://ti.chemitech.net.cn

C#:   s.Split('\n')
来源：http://wd.nszjky.cn

[E20] 判断字符串是否为空
来源：http://sb.521024.cn

Py:   if not s:
来源：http://hn.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zt.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ts.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://li.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://eh.huixiangedu.cn

Go:   if s == "" {}
来源：http://ps.chemitech.net.cn

Ruby: if s.empty?
来源：http://fr.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oc.gzmigu.cn

[E21] 超长截断加省略号
来源：http://yn.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kd.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://da.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dr.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tx.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://za.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://mu.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bj.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zz.asd995.cn

[E22] 字节长度与字符长度
来源：http://gx.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pt.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ql.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://go.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cm.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rv.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ek.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://ey.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bn.jianghongdianzi.cn

================================================================================
来源：http://ku.bookmarksfly.cn

F. 文件与目录
来源：http://ch.asd995.cn

================================================================================
来源：http://ao.bjjhwx.cn

[F01] 读取整个文件
来源：http://mk.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sw.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ix.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qe.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yx.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lp.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zu.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://na.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ih.szxytkj.cn

[F02] 逐行读取文件
来源：http://of.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yq.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ww.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qw.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cn.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ko.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eh.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pw.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eg.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ha.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bf.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ob.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ig.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mm.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zx.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ri.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://bh.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wj.lnxyls.cn

[F04] 追加写入文件
来源：http://yc.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pr.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dx.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ri.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ee.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://is.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gz.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pm.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sj.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://ah.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eg.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://pp.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://iv.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ik.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fa.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xq.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://iq.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://xn.shtwfgs.cn

[F06] 删除文件
来源：http://ws.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://qs.huanxung.cn

PHP:  unlink("a.txt");
来源：http://va.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gg.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mc.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yq.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://rm.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://pb.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ay.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://jf.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bz.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ah.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gs.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fk.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ck.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://po.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://el.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ux.nicolike.cn

[F08] 遍历目录
来源：http://fy.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://at.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bn.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://xg.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://wf.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jk.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://he.colortex.cn

Ruby: Dir.children("dir")
来源：http://xb.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://es.colortex.cn

[F09] 获取文件大小
来源：http://bc.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://eq.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://hd.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://hn.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://gj.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ay.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jb.szsharing.cn

Ruby: File.size("a.txt")
来源：http://fa.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://jn.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://bs.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nb.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://my.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yu.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://ur.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dr.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kn.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mj.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bi.huixiangedu.cn

[F11] 复制与移动文件
来源：http://mr.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hx.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hw.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fq.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cl.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://as.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sw.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bk.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fq.shtwfgs.cn

[F12] CSV 读写
来源：http://rb.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://st.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pz.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ir.gzmigu.cn

TS:   // 同上
来源：http://if.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iz.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oj.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ri.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iu.newstarts.cn

================================================================================
来源：http://kn.huanxung.cn

G. 面向对象
来源：http://if.shxzukj.cn

================================================================================
来源：http://hb.yuexingan06.cn

[G01] 定义类
来源：http://vc.colortex.cn

Py:   class User: pass
来源：http://fv.nszjky.cn

PHP:  class User {}
来源：http://rw.muxihuayi.cn

JS:   class User {}
来源：http://nb.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://ve.lnxyls.cn

Java: class User {}
来源：http://rk.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://cs.yuexingan06.cn

Ruby: class User; end
来源：http://bd.muxihuayi.cn

C#:   class User {}
来源：http://wu.newstarts.cn

[G02] 构造函数
来源：http://qg.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://ak.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://su.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://fp.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://mq.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://bj.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zj.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://xq.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://vl.muxihuayi.cn

[G03] 实例属性
来源：http://az.521024.cn

Py:   self.name = "x"
来源：http://lk.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://cz.muxihuayi.cn

JS:   this.name = "x";
来源：http://ag.jctech888.com.cn

TS:   name: string = "x";
来源：http://pc.yuexingan06.cn

Java: private String name;
来源：http://ue.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ha.nszjky.cn

Ruby: @name = "x"
来源：http://il.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://jo.521024.cn

[G04] 定义方法
来源：http://bk.hahajie.cn

Py:   def greet(self): return self.name
来源：http://jo.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://io.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://vv.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://mq.chemitech.net.cn

Java: String greet() { return name; }
来源：http://op.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gw.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://fd.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://vj.muxihuayi.cn

[G05] 继承
来源：http://zx.asd995.cn

Py:   class Admin(User): pass
来源：http://fc.szsharing.cn

PHP:  class Admin extends User {}
来源：http://me.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://mf.lnxyls.cn

TS:   class Admin extends User {}
来源：http://ne.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ej.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fw.szxytkj.cn

Ruby: class Admin < User; end
来源：http://ln.gzmigu.cn

C#:   class Admin : User {}
来源：http://kt.bjjhwx.cn

[G06] 重写方法
来源：http://dz.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://uf.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://op.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://xc.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://un.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://fd.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gv.521024.cn

Ruby: def greet; "admin"; end
来源：http://ax.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://cj.wgjwhj.cn

[G07] 调用父类方法
来源：http://lf.521024.cn

Py:   super().greet()
来源：http://rd.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://kk.jianghongdianzi.cn

JS:   super.greet();
来源：http://ar.hnjuh.cn

TS:   super.greet();
来源：http://br.shtwfgs.cn

Java: super.greet();
来源：http://iu.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gf.bookmarksfly.cn

Ruby: super
来源：http://wa.panjiajie.cn

C#:   base.Greet();
来源：http://et.muxihuayi.cn

[G08] 静态方法与属性
来源：http://jh.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kq.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://yw.szxytkj.cn

JS:   static f() {}
来源：http://xj.asd995.cn

TS:   static f(): void {}
来源：http://bn.haigaiapp.cn

Java: static void f() {}
来源：http://cy.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vm.colortex.cn

Ruby: def self.f; end
来源：http://sa.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://fp.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://mg.521024.cn


<!-- 参考信息 -->