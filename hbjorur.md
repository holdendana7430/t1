代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zt.newstarts.cn

[E11] 反转字符串
来源：http://gd.haigaiapp.cn

Py:   s[::-1]
来源：http://vu.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://sx.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://bw.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://lw.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zy.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wk.shtwfgs.cn

Ruby: s.reverse
来源：http://tu.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fz.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://vl.colortex.cn

Py:   s.count("a")
来源：http://pf.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://fp.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://gz.9csxet.cn

TS:   s.split("a").length - 1
来源：http://jj.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ly.colortex.cn

Go:   strings.Count(s, "a")
来源：http://ec.asd995.cn

Ruby: s.count("a")
来源：http://nt.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://yw.yuexingan06.cn

[E13] 逐字符遍历
来源：http://qu.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://hl.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://av.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xx.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kr.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sd.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nu.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gi.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://de.colortex.cn

[E14] URL 编码与 Base64
来源：http://rc.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bf.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fb.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pf.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ny.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qp.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://et.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zj.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hx.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://on.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hu.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mj.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lh.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zz.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wv.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sp.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://md.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qm.asd995.cn

[E16] 数字千分位
来源：http://nk.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://xz.gzmigu.cn

PHP:  number_format(1234567);
来源：http://eq.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kf.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qz.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://er.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yc.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mi.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://in.shxzskj.cn

[E17] 首字母大写
来源：http://hw.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://at.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://to.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://og.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fq.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ll.chemitech.net.cn

Ruby: s.capitalize
来源：http://bk.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nj.shxzskj.cn

[E18] 模板占位符替换
来源：http://om.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fe.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fj.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qd.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ak.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zn.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://un.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://df.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nm.9csxet.cn

[E19] 多行文本按行拆分
来源：http://bt.wgjwhj.cn

Py:   s.splitlines()
来源：http://zr.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bo.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ab.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ec.haigaiapp.cn

Java: s.lines().toList()
来源：http://xf.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://sl.jctech888.com.cn

Ruby: s.lines
来源：http://by.huixiangedu.cn

C#:   s.Split('\n')
来源：http://vy.hahajie.cn

[E20] 判断字符串是否为空
来源：http://al.huixiangedu.cn

Py:   if not s:
来源：http://kj.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eb.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nk.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://yh.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://qo.chemitech.net.cn

Go:   if s == "" {}
来源：http://fb.chemitech.net.cn

Ruby: if s.empty?
来源：http://cp.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kk.newstarts.cn

[E21] 超长截断加省略号
来源：http://hw.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vq.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dg.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wi.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jz.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lk.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://oz.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sr.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kk.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://xt.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hy.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vv.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ro.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ch.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tz.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://mn.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bs.huixinmuqiang.cn

================================================================================
来源：http://sc.shtwfgs.cn

F. 文件与目录
来源：http://uq.huixiangedu.cn

================================================================================
来源：http://zy.521024.cn

[F01] 读取整个文件
来源：http://xp.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gf.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://bq.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://it.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sh.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ts.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://sd.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wq.szsharing.cn

[F02] 逐行读取文件
来源：http://sl.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pz.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yq.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://re.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://an.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gv.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ga.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cu.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jm.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://pl.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://al.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ld.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hg.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://km.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tc.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ib.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ef.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eq.nszjky.cn

[F04] 追加写入文件
来源：http://mp.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sc.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fq.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zz.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zi.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rf.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zj.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gu.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sz.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://ns.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cq.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://zq.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://dy.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://da.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zr.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oa.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ey.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://qk.jctech888.com.cn

[F06] 删除文件
来源：http://cs.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://fq.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ge.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ij.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://my.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lw.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://tp.521024.cn

Ruby: File.delete("a.txt")
来源：http://ls.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://bq.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://ui.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://os.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hc.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mo.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jg.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vj.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lo.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vy.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ju.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ya.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mp.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xx.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://vt.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://xy.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jn.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hg.szsharing.cn

Ruby: Dir.children("dir")
来源：http://ig.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://dk.lnxyls.cn

[F09] 获取文件大小
来源：http://in.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://bt.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://yl.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://yd.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://wz.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tl.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://ef.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ij.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://zw.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zv.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bp.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://do.9csxet.cn

TS:   path.extname("a.txt")
来源：http://ew.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mu.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lo.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fq.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bx.huanxung.cn

[F11] 复制与移动文件
来源：http://dl.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ub.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wf.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tr.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ah.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hk.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mt.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jd.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lu.shxzskj.cn

[F12] CSV 读写
来源：http://gt.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lu.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ac.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zn.lnxyls.cn

TS:   // 同上
来源：http://ul.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ci.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zb.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sz.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xs.nicolike.cn

================================================================================
来源：http://yj.521024.cn

G. 面向对象
来源：http://uq.wgjwhj.cn

================================================================================
来源：http://kv.shtwfgs.cn

[G01] 定义类
来源：http://ii.haigaiapp.cn

Py:   class User: pass
来源：http://rj.szxytkj.cn

PHP:  class User {}
来源：http://yb.bookmarksfly.cn

JS:   class User {}
来源：http://zh.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://vq.bjjhwx.cn

Java: class User {}
来源：http://ve.shxzskj.cn

Go:   type User struct { Name string }
来源：http://la.jctech888.com.cn

Ruby: class User; end
来源：http://fi.muxihuayi.cn

C#:   class User {}
来源：http://on.colortex.cn

[G02] 构造函数
来源：http://go.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://xa.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://zh.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://at.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://fp.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://yr.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rx.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://ql.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://io.nicolike.cn

[G03] 实例属性
来源：http://ih.hnjuh.cn

Py:   self.name = "x"
来源：http://th.newstarts.cn

PHP:  public string $name = "x";
来源：http://qb.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ue.szsharing.cn

TS:   name: string = "x";
来源：http://bq.9csxet.cn

Java: private String name;
来源：http://tn.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ri.panjiajie.cn

Ruby: @name = "x"
来源：http://qn.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://os.chemitech.net.cn

[G04] 定义方法
来源：http://sr.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://ys.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://en.nicolike.cn

JS:   greet() { return this.name; }
来源：http://wo.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://vb.9csxet.cn

Java: String greet() { return name; }
来源：http://cf.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nk.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ac.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://zl.jianghongdianzi.cn

[G05] 继承
来源：http://co.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://pl.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://vb.huanxung.cn

JS:   class Admin extends User {}
来源：http://by.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://je.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://qs.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kx.521024.cn

Ruby: class Admin < User; end
来源：http://ea.szxytkj.cn

C#:   class Admin : User {}
来源：http://hw.chemitech.net.cn

[G06] 重写方法
来源：http://gg.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://tr.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hn.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://eb.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://ex.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://qm.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lx.521024.cn

Ruby: def greet; "admin"; end
来源：http://am.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://di.lnxyls.cn

[G07] 调用父类方法
来源：http://nm.jianghongdianzi.cn

Py:   super().greet()
来源：http://vk.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://pd.newstarts.cn

JS:   super.greet();
来源：http://vh.shxzskj.cn

TS:   super.greet();
来源：http://ta.muxihuayi.cn

Java: super.greet();
来源：http://aj.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ig.shxzukj.cn

Ruby: super
来源：http://kk.lnxyls.cn

C#:   base.Greet();
来源：http://fr.shxzukj.cn

[G08] 静态方法与属性
来源：http://dp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qa.szsharing.cn

PHP:  public static function f() {}
来源：http://ia.yuexingan06.cn

JS:   static f() {}
来源：http://pu.shxzskj.cn

TS:   static f(): void {}
来源：http://mz.jctech888.com.cn

Java: static void f() {}
来源：http://lm.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ht.shxzskj.cn

Ruby: def self.f; end
来源：http://ln.9csxet.cn

C#:   public static void F() {}
来源：http://qt.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://kc.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://yn.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://he.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kh.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://qj.shxzskj.cn


<!-- 参考信息 -->