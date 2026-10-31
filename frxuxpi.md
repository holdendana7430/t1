代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://rm.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://fu.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://za.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://le.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iw.jctech888.com.cn

[E11] 反转字符串
来源：http://va.nszjky.cn

Py:   s[::-1]
来源：http://qx.haigaiapp.cn

PHP:  strrev($s);
来源：http://ls.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ph.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://si.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://be.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sr.yuexingan06.cn

Ruby: s.reverse
来源：http://he.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eq.521024.cn

[E12] 统计某字符出现次数
来源：http://jo.huanxung.cn

Py:   s.count("a")
来源：http://fr.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://va.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://wd.huanxung.cn

TS:   s.split("a").length - 1
来源：http://oh.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nc.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://pz.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://rg.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://tm.lnxyls.cn

[E13] 逐字符遍历
来源：http://vm.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://iq.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lb.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tt.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vd.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pl.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dl.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yp.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ta.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://tx.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ff.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dk.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pd.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nr.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ef.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xy.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ng.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nj.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://pz.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ag.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xf.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xj.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cx.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qd.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oo.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rx.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ul.szsharing.cn

[E16] 数字千分位
来源：http://id.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://yo.shxzukj.cn

PHP:  number_format(1234567);
来源：http://cu.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lq.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eq.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jk.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sd.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mg.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://so.colortex.cn

[E17] 首字母大写
来源：http://ut.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nv.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kw.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ac.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vv.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ch.nszjky.cn

Ruby: s.capitalize
来源：http://or.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lw.panjiajie.cn

[E18] 模板占位符替换
来源：http://ne.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pi.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://or.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hq.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lk.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vb.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tr.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://az.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wa.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://db.haigaiapp.cn

Py:   s.splitlines()
来源：http://am.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ai.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://mu.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://mc.9csxet.cn

Java: s.lines().toList()
来源：http://fu.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://fk.nszjky.cn

Ruby: s.lines
来源：http://yx.newstarts.cn

C#:   s.Split('\n')
来源：http://nf.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://oi.huanxung.cn

Py:   if not s:
来源：http://sf.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hw.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://am.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://xr.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://fa.chemitech.net.cn

Go:   if s == "" {}
来源：http://ah.nicolike.cn

Ruby: if s.empty?
来源：http://mn.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rf.shxzukj.cn

[E21] 超长截断加省略号
来源：http://qb.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://so.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wv.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bq.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sn.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qs.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://cq.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vd.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hk.521024.cn

[E22] 字节长度与字符长度
来源：http://xw.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lf.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wy.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wj.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vv.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yr.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nc.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://le.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ww.9csxet.cn

================================================================================
来源：http://ky.chemitech.net.cn

F. 文件与目录
来源：http://rg.shtwfgs.cn

================================================================================
来源：http://vn.bjjhwx.cn

[F01] 读取整个文件
来源：http://le.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wo.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://uy.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://au.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ah.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jc.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mm.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://dz.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://pd.szsharing.cn

[F02] 逐行读取文件
来源：http://qt.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://br.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kj.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cf.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gj.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://js.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oz.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rm.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kd.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://hm.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wt.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eg.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hp.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://di.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hi.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://kw.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rz.bjjhwx.cn

[F04] 追加写入文件
来源：http://cu.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dj.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tx.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mq.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mv.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ux.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ek.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pj.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hi.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://qt.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zf.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://qn.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://oq.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://dy.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sk.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ia.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://vo.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://uw.yuntaijiaju.cn

[F06] 删除文件
来源：http://tf.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://yk.szsharing.cn

PHP:  unlink("a.txt");
来源：http://hu.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ax.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iy.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dg.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://en.521024.cn

Ruby: File.delete("a.txt")
来源：http://ub.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://fv.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://jl.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bd.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://po.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qu.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yc.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kn.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ve.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hv.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ar.newstarts.cn

[F08] 遍历目录
来源：http://hs.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nr.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rk.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://nk.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://ei.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qt.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bj.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://jc.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://er.9csxet.cn

[F09] 获取文件大小
来源：http://qe.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://to.asd995.cn

PHP:  filesize("a.txt");
来源：http://zh.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://ot.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://tu.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aw.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qy.521024.cn

Ruby: File.size("a.txt")
来源：http://ql.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://sa.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://fm.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rx.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jl.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kb.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://un.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jw.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pr.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vs.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xq.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://xg.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dz.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://th.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xm.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cm.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sh.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eo.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tb.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dh.haigaiapp.cn

[F12] CSV 读写
来源：http://av.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gj.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uc.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rt.nszjky.cn

TS:   // 同上
来源：http://sq.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oy.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bo.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xn.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gz.bjjhwx.cn

================================================================================
来源：http://ri.jianghongdianzi.cn

G. 面向对象
来源：http://yk.colortex.cn

================================================================================
来源：http://jt.szxytkj.cn

[G01] 定义类
来源：http://vy.shxzskj.cn

Py:   class User: pass
来源：http://zo.9csxet.cn

PHP:  class User {}
来源：http://tq.shxzskj.cn

JS:   class User {}
来源：http://ap.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://kp.bookmarksfly.cn

Java: class User {}
来源：http://qv.nicolike.cn

Go:   type User struct { Name string }
来源：http://pp.asd995.cn

Ruby: class User; end
来源：http://rc.wgjwhj.cn

C#:   class User {}
来源：http://xx.bookmarksfly.cn

[G02] 构造函数
来源：http://ae.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ta.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://py.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://dv.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://wl.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://jj.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xi.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://yn.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://en.asd995.cn

[G03] 实例属性
来源：http://ne.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://bw.nszjky.cn

PHP:  public string $name = "x";
来源：http://nb.panjiajie.cn

JS:   this.name = "x";
来源：http://iq.huanxung.cn

TS:   name: string = "x";
来源：http://uy.wgjwhj.cn

Java: private String name;
来源：http://yo.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ck.gzmigu.cn

Ruby: @name = "x"
来源：http://ud.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://zn.bjjhwx.cn

[G04] 定义方法
来源：http://qr.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://wx.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jz.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://vo.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ab.shxzukj.cn

Java: String greet() { return name; }
来源：http://oo.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lk.gzmigu.cn

Ruby: def greet; @name; end
来源：http://np.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://pv.yuexingan06.cn

[G05] 继承
来源：http://nk.hahajie.cn

Py:   class Admin(User): pass
来源：http://py.9csxet.cn

PHP:  class Admin extends User {}
来源：http://qp.huanxung.cn

JS:   class Admin extends User {}
来源：http://gq.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://oe.szxytkj.cn

Java: class Admin extends User {}
来源：http://be.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rf.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ph.bjjhwx.cn

C#:   class Admin : User {}
来源：http://cs.shxzskj.cn

[G06] 重写方法
来源：http://rg.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://io.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mz.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://qy.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://im.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://rs.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jx.521024.cn

Ruby: def greet; "admin"; end
来源：http://hx.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ux.muxihuayi.cn

[G07] 调用父类方法
来源：http://um.haigaiapp.cn

Py:   super().greet()
来源：http://cw.asd995.cn

PHP:  parent::greet();
来源：http://cf.haigaiapp.cn

JS:   super.greet();
来源：http://vm.nicolike.cn

TS:   super.greet();
来源：http://ci.chemitech.net.cn

Java: super.greet();
来源：http://zc.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bg.jianghongdianzi.cn

Ruby: super
来源：http://dx.asd995.cn

C#:   base.Greet();
来源：http://hq.panjiajie.cn

[G08] 静态方法与属性
来源：http://wf.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ch.shxzukj.cn

PHP:  public static function f() {}
来源：http://rv.newstarts.cn

JS:   static f() {}
来源：http://vw.shxzskj.cn

TS:   static f(): void {}
来源：http://ir.nszjky.cn

Java: static void f() {}
来源：http://pb.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xq.szxytkj.cn

Ruby: def self.f; end
来源：http://sj.panjiajie.cn

C#:   public static void F() {}
来源：http://gk.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://mk.bookmarksfly.cn


<!-- 参考信息 -->