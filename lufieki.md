代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vd.bjjhwx.cn

[E11] 反转字符串
来源：http://jn.wgjwhj.cn

Py:   s[::-1]
来源：http://vi.bookmarksfly.cn

PHP:  strrev($s);
来源：http://vp.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://qb.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://kx.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sp.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nk.shtwfgs.cn

Ruby: s.reverse
来源：http://sm.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ws.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://xp.huanxung.cn

Py:   s.count("a")
来源：http://ie.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://rc.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ib.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://td.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://us.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://kf.wgjwhj.cn

Ruby: s.count("a")
来源：http://gs.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://tm.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ae.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://zg.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rc.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gn.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xs.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://le.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yo.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qt.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mh.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ob.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pf.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lq.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jp.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ug.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vd.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qf.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nm.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lz.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://gu.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vm.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ld.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qf.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ag.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nz.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xh.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kn.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hj.huixiangedu.cn

[E16] 数字千分位
来源：http://pc.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://as.gzmigu.cn

PHP:  number_format(1234567);
来源：http://kv.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://af.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vo.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yk.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ap.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ga.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://xe.hahajie.cn

[E17] 首字母大写
来源：http://ns.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ws.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iq.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ub.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ek.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ru.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sj.panjiajie.cn

Ruby: s.capitalize
来源：http://xw.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xo.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://yz.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://el.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hu.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kj.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qs.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fs.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://it.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zc.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hh.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://zu.muxihuayi.cn

Py:   s.splitlines()
来源：http://cn.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sw.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://xj.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://yj.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://su.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://wf.nszjky.cn

Ruby: s.lines
来源：http://nn.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://cw.nszjky.cn

[E20] 判断字符串是否为空
来源：http://hm.bjjhwx.cn

Py:   if not s:
来源：http://io.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hf.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gh.shxzskj.cn

TS:   if (s === "") {}
来源：http://lr.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://gb.jctech888.com.cn

Go:   if s == "" {}
来源：http://xc.lnxyls.cn

Ruby: if s.empty?
来源：http://cn.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ki.521024.cn

[E21] 超长截断加省略号
来源：http://xn.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wj.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cv.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jo.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jf.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ry.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://rm.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://na.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kj.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://jv.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wq.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rn.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nl.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aw.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lx.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gq.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://gj.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vb.szxytkj.cn

================================================================================
来源：http://cq.haigaiapp.cn

F. 文件与目录
来源：http://ke.jianghongdianzi.cn

================================================================================
来源：http://jg.wgjwhj.cn

[F01] 读取整个文件
来源：http://xq.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uc.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ak.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://av.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://df.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zr.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://ap.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://qr.muxihuayi.cn

[F02] 逐行读取文件
来源：http://bw.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cx.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jo.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://or.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bx.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ey.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iu.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gm.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://zc.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nr.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cb.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yp.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dr.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gi.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sk.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://tn.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hh.chemitech.net.cn

[F04] 追加写入文件
来源：http://tf.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dq.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gf.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fp.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vl.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uk.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mk.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pa.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qi.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://mm.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ct.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://rp.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://dx.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://iu.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jf.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hv.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://nt.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ee.shxzukj.cn

[F06] 删除文件
来源：http://sh.szsharing.cn

Py:   os.remove("a.txt")
来源：http://sx.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://zt.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jr.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oo.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ak.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://rb.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://ug.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://mv.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://jl.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lt.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eo.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lk.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xs.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xe.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qd.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jt.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cc.huixiangedu.cn

[F08] 遍历目录
来源：http://ju.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pt.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hw.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://wg.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://mv.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lf.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uc.nszjky.cn

Ruby: Dir.children("dir")
来源：http://si.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://vw.colortex.cn

[F09] 获取文件大小
来源：http://hy.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://ha.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://hi.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://rb.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://pz.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oe.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yt.asd995.cn

Ruby: File.size("a.txt")
来源：http://qq.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://qp.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://or.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ld.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ag.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jr.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://uw.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mp.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://re.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kj.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qd.yuexingan06.cn

[F11] 复制与移动文件
来源：http://tt.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lo.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sz.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xs.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://me.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dz.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yw.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ya.yuntaijiaju.cn

[F12] CSV 读写
来源：http://fl.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pa.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mc.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xj.shtwfgs.cn

TS:   // 同上
来源：http://nz.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tu.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aa.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ml.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ur.nicolike.cn

================================================================================
来源：http://ag.lnxyls.cn

G. 面向对象
来源：http://uu.colortex.cn

================================================================================
来源：http://uz.huanxung.cn

[G01] 定义类
来源：http://wu.hnjuh.cn

Py:   class User: pass
来源：http://je.shtwfgs.cn

PHP:  class User {}
来源：http://hu.lnxyls.cn

JS:   class User {}
来源：http://yg.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://vu.hahajie.cn

Java: class User {}
来源：http://bz.9csxet.cn

Go:   type User struct { Name string }
来源：http://pl.huanxung.cn

Ruby: class User; end
来源：http://lh.521024.cn

C#:   class User {}
来源：http://rb.huixiangedu.cn

[G02] 构造函数
来源：http://xg.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://yf.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://jz.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://nq.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://kp.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://gl.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bx.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://ja.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://fy.yuexingan06.cn

[G03] 实例属性
来源：http://dl.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://sy.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://mx.bjjhwx.cn

JS:   this.name = "x";
来源：http://ip.muxihuayi.cn

TS:   name: string = "x";
来源：http://pp.shtwfgs.cn

Java: private String name;
来源：http://pn.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wf.muxihuayi.cn

Ruby: @name = "x"
来源：http://jd.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://tt.bookmarksfly.cn

[G04] 定义方法
来源：http://tl.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://wr.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bx.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://ed.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://nl.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://gs.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zi.colortex.cn

Ruby: def greet; @name; end
来源：http://jr.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ua.lnxyls.cn

[G05] 继承
来源：http://kf.huanxung.cn

Py:   class Admin(User): pass
来源：http://za.nszjky.cn

PHP:  class Admin extends User {}
来源：http://ig.lnxyls.cn

JS:   class Admin extends User {}
来源：http://uo.hahajie.cn

TS:   class Admin extends User {}
来源：http://gw.haigaiapp.cn

Java: class Admin extends User {}
来源：http://yz.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yn.newstarts.cn

Ruby: class Admin < User; end
来源：http://xa.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://wy.lnxyls.cn

[G06] 重写方法
来源：http://ax.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://vd.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hu.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://hk.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://qm.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://uk.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hs.asd995.cn

Ruby: def greet; "admin"; end
来源：http://vm.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://dq.gzmigu.cn

[G07] 调用父类方法
来源：http://qy.asd995.cn

Py:   super().greet()
来源：http://sp.shxzskj.cn

PHP:  parent::greet();
来源：http://dm.bookmarksfly.cn

JS:   super.greet();
来源：http://lh.gzmigu.cn

TS:   super.greet();
来源：http://kz.wgjwhj.cn

Java: super.greet();
来源：http://fk.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ua.shtwfgs.cn

Ruby: super
来源：http://hr.hnjuh.cn

C#:   base.Greet();
来源：http://lw.chemitech.net.cn

[G08] 静态方法与属性
来源：http://dg.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tr.szsharing.cn

PHP:  public static function f() {}
来源：http://sr.shxzskj.cn

JS:   static f() {}
来源：http://dp.wgjwhj.cn

TS:   static f(): void {}
来源：http://hb.newstarts.cn

Java: static void f() {}
来源：http://ef.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bq.jctech888.com.cn

Ruby: def self.f; end
来源：http://or.muxihuayi.cn

C#:   public static void F() {}
来源：http://hc.colortex.cn

[G09] 接口 / 抽象类
来源：http://po.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://xg.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jm.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wc.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ev.muxihuayi.cn


<!-- 参考信息 -->