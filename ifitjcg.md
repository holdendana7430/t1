代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://jw.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yp.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ly.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://yi.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://js.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://da.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pc.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xy.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xh.521024.cn

[E11] 反转字符串
来源：http://qd.jctech888.com.cn

Py:   s[::-1]
来源：http://kc.hahajie.cn

PHP:  strrev($s);
来源：http://ai.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://fc.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://xo.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vz.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xt.gzmigu.cn

Ruby: s.reverse
来源：http://kx.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ja.szsharing.cn

[E12] 统计某字符出现次数
来源：http://zc.bookmarksfly.cn

Py:   s.count("a")
来源：http://ip.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://ps.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ka.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://rn.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ty.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://yk.521024.cn

Ruby: s.count("a")
来源：http://up.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://zy.chemitech.net.cn

[E13] 逐字符遍历
来源：http://kb.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://xn.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sb.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kt.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wn.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zj.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dq.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sx.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ck.szsharing.cn

[E14] URL 编码与 Base64
来源：http://kx.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ox.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ew.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fu.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oa.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sh.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wa.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gh.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fu.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://xt.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bi.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kb.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yd.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cx.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ho.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cb.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wy.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ja.yuexingan06.cn

[E16] 数字千分位
来源：http://ir.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://qm.shxzskj.cn

PHP:  number_format(1234567);
来源：http://ju.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sc.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ur.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gz.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cu.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nz.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://vn.hnjuh.cn

[E17] 首字母大写
来源：http://fw.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ir.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yo.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nq.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fu.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rn.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dk.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://pj.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rp.nszjky.cn

[E18] 模板占位符替换
来源：http://nw.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pv.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://au.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ah.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zi.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://na.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rl.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://as.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vu.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://it.szxytkj.cn

Py:   s.splitlines()
来源：http://cb.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://da.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://mc.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://jy.jctech888.com.cn

Java: s.lines().toList()
来源：http://yw.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://gn.newstarts.cn

Ruby: s.lines
来源：http://tu.panjiajie.cn

C#:   s.Split('\n')
来源：http://kz.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://nn.yuntaijiaju.cn

Py:   if not s:
来源：http://if.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iu.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hv.nszjky.cn

TS:   if (s === "") {}
来源：http://km.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://ep.muxihuayi.cn

Go:   if s == "" {}
来源：http://qq.521024.cn

Ruby: if s.empty?
来源：http://na.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vr.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://xm.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vn.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eg.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ix.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qn.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vc.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://rj.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nw.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pc.521024.cn

[E22] 字节长度与字符长度
来源：http://at.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://av.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qm.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rk.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wx.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ku.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fl.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://gt.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cy.huixinmuqiang.cn

================================================================================
来源：http://ys.jctech888.com.cn

F. 文件与目录
来源：http://vx.szsharing.cn

================================================================================
来源：http://ir.nszjky.cn

[F01] 读取整个文件
来源：http://lg.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hw.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://gf.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dh.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ew.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://me.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://db.huanxung.cn

Ruby: File.read("a.txt")
来源：http://om.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://mo.szsharing.cn

[F02] 逐行读取文件
来源：http://qe.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dv.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xa.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ez.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xq.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gv.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://al.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mj.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jb.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://sw.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sk.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ru.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sq.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://en.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://is.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nh.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://id.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ss.lnxyls.cn

[F04] 追加写入文件
来源：http://zb.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://de.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hv.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kv.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xx.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ki.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tm.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fm.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lt.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://lo.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bx.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://md.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://vs.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://sr.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mx.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mf.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://or.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://ke.haigaiapp.cn

[F06] 删除文件
来源：http://pw.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://bs.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://lx.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eg.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sh.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bq.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://sx.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://zc.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://cd.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://wn.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ln.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://je.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ad.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gz.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vr.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hm.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yj.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vt.huanxung.cn

[F08] 遍历目录
来源：http://sp.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ka.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sf.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://hp.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://lh.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ei.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fq.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://sp.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://ak.newstarts.cn

[F09] 获取文件大小
来源：http://zm.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://ok.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://aj.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ca.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://li.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ob.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dr.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ym.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://mn.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://py.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mc.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sh.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kh.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://vi.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ms.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://em.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hj.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yi.hnjuh.cn

[F11] 复制与移动文件
来源：http://gb.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sm.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ze.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ug.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ti.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zn.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ed.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tt.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://al.nicolike.cn

[F12] CSV 读写
来源：http://uj.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://th.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fb.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ky.szsharing.cn

TS:   // 同上
来源：http://me.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hp.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ty.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wj.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://um.9csxet.cn

================================================================================
来源：http://iv.521024.cn

G. 面向对象
来源：http://yg.hnjuh.cn

================================================================================
来源：http://lx.huixinmuqiang.cn

[G01] 定义类
来源：http://zh.nszjky.cn

Py:   class User: pass
来源：http://yq.colortex.cn

PHP:  class User {}
来源：http://kd.yuexingan06.cn

JS:   class User {}
来源：http://cj.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://du.huixiangedu.cn

Java: class User {}
来源：http://tc.panjiajie.cn

Go:   type User struct { Name string }
来源：http://ww.muxihuayi.cn

Ruby: class User; end
来源：http://rl.newstarts.cn

C#:   class User {}
来源：http://yd.jianghongdianzi.cn

[G02] 构造函数
来源：http://gj.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ae.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://aq.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://th.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://as.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://yp.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ha.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://in.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://wi.chemitech.net.cn

[G03] 实例属性
来源：http://tc.9csxet.cn

Py:   self.name = "x"
来源：http://et.hahajie.cn

PHP:  public string $name = "x";
来源：http://vr.nicolike.cn

JS:   this.name = "x";
来源：http://yv.hahajie.cn

TS:   name: string = "x";
来源：http://wn.szsharing.cn

Java: private String name;
来源：http://ov.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oo.lnxyls.cn

Ruby: @name = "x"
来源：http://xq.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://hv.wgjwhj.cn

[G04] 定义方法
来源：http://xx.newstarts.cn

Py:   def greet(self): return self.name
来源：http://og.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rc.szsharing.cn

JS:   greet() { return this.name; }
来源：http://gl.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://mr.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://ra.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wc.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://ou.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://av.huixinmuqiang.cn

[G05] 继承
来源：http://hk.521024.cn

Py:   class Admin(User): pass
来源：http://li.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://jo.nszjky.cn

JS:   class Admin extends User {}
来源：http://ln.lnxyls.cn

TS:   class Admin extends User {}
来源：http://jm.szxytkj.cn

Java: class Admin extends User {}
来源：http://ng.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rj.colortex.cn

Ruby: class Admin < User; end
来源：http://og.wgjwhj.cn

C#:   class Admin : User {}
来源：http://zo.yuntaijiaju.cn

[G06] 重写方法
来源：http://ib.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://aq.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vy.colortex.cn

JS:   greet() { return "admin"; }
来源：http://vv.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://xk.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://wx.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ow.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://ak.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://jc.colortex.cn

[G07] 调用父类方法
来源：http://cx.9csxet.cn

Py:   super().greet()
来源：http://za.hahajie.cn

PHP:  parent::greet();
来源：http://ra.huanxung.cn

JS:   super.greet();
来源：http://pa.chemitech.net.cn

TS:   super.greet();
来源：http://ez.nicolike.cn

Java: super.greet();
来源：http://xk.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kv.szsharing.cn

Ruby: super
来源：http://zp.huanxung.cn

C#:   base.Greet();
来源：http://tp.wgjwhj.cn

[G08] 静态方法与属性
来源：http://zz.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xp.yuexingan06.cn

PHP:  public static function f() {}
来源：http://ge.newstarts.cn

JS:   static f() {}
来源：http://am.hahajie.cn

TS:   static f(): void {}
来源：http://yr.haigaiapp.cn

Java: static void f() {}
来源：http://aq.muxihuayi.cn


<!-- 参考信息 -->