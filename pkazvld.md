代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://md.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ye.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xa.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zl.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qd.newstarts.cn

[E11] 反转字符串
来源：http://tz.shxzskj.cn

Py:   s[::-1]
来源：http://im.chemitech.net.cn

PHP:  strrev($s);
来源：http://ni.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://cs.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://wh.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hb.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qg.jianghongdianzi.cn

Ruby: s.reverse
来源：http://yn.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ed.asd995.cn

[E12] 统计某字符出现次数
来源：http://tx.shtwfgs.cn

Py:   s.count("a")
来源：http://gx.colortex.cn

PHP:  substr_count($s, "a");
来源：http://iq.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://tl.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://aq.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dh.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://yt.haigaiapp.cn

Ruby: s.count("a")
来源：http://ff.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://cq.chemitech.net.cn

[E13] 逐字符遍历
来源：http://af.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://wv.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zw.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ek.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bg.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kw.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xa.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://me.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zp.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://qv.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pv.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sc.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://no.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kb.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ta.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ks.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gk.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vi.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://oj.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fp.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lp.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rq.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ee.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fv.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ff.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sd.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bg.521024.cn

[E16] 数字千分位
来源：http://lf.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://sh.9csxet.cn

PHP:  number_format(1234567);
来源：http://nr.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mm.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hd.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xs.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ob.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tw.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://lb.huanxung.cn

[E17] 首字母大写
来源：http://ey.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cl.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://de.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://md.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ls.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zm.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bo.bookmarksfly.cn

Ruby: s.capitalize
来源：http://oj.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sm.szsharing.cn

[E18] 模板占位符替换
来源：http://xg.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pu.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hm.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rq.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zs.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tl.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yx.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://am.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://up.newstarts.cn

[E19] 多行文本按行拆分
来源：http://gu.bjjhwx.cn

Py:   s.splitlines()
来源：http://kw.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://na.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://yd.521024.cn

TS:   s.split(/\r?\n/)
来源：http://gl.chemitech.net.cn

Java: s.lines().toList()
来源：http://cn.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://bx.nszjky.cn

Ruby: s.lines
来源：http://ic.panjiajie.cn

C#:   s.Split('\n')
来源：http://uy.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://ie.yuntaijiaju.cn

Py:   if not s:
来源：http://wq.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jt.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ly.newstarts.cn

TS:   if (s === "") {}
来源：http://vn.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://uy.shtwfgs.cn

Go:   if s == "" {}
来源：http://mw.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://jq.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vy.hnjuh.cn

[E21] 超长截断加省略号
来源：http://bi.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bq.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rh.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xi.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ig.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sk.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ok.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rr.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fh.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://ln.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://di.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uk.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zd.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eh.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sn.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://os.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://za.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qy.jianghongdianzi.cn

================================================================================
来源：http://jj.muxihuayi.cn

F. 文件与目录
来源：http://vu.yuntaijiaju.cn

================================================================================
来源：http://dw.nszjky.cn

[F01] 读取整个文件
来源：http://ao.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://br.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://yb.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hj.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nf.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vz.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ej.asd995.cn

Ruby: File.read("a.txt")
来源：http://go.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://nd.shxzskj.cn

[F02] 逐行读取文件
来源：http://il.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zu.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sw.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wu.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xq.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xw.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://py.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qa.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mz.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://dz.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://of.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oq.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pb.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ib.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://po.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://nm.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nn.shxzukj.cn

[F04] 追加写入文件
来源：http://rj.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kp.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://us.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ry.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rx.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zt.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rf.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fl.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cv.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://hi.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dw.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://sz.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://fw.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://tv.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pf.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qj.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://xp.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://bo.yuntaijiaju.cn

[F06] 删除文件
来源：http://tv.asd995.cn

Py:   os.remove("a.txt")
来源：http://nb.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://lj.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rb.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zd.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wx.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://ko.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ga.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://de.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://zy.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gv.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jv.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wa.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bu.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sm.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://js.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qz.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ab.nicolike.cn

[F08] 遍历目录
来源：http://yn.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zc.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ui.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ml.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://rv.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ug.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bs.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://ne.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://yz.huixiangedu.cn

[F09] 获取文件大小
来源：http://fc.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://dj.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://cu.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://gk.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://gl.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tm.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eg.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ph.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://cj.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ln.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://if.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oz.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pi.hahajie.cn

TS:   path.extname("a.txt")
来源：http://oc.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jl.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dv.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lb.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ff.asd995.cn

[F11] 复制与移动文件
来源：http://kv.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://in.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ax.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tn.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vw.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ua.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jc.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jk.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pa.bookmarksfly.cn

[F12] CSV 读写
来源：http://pa.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rx.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zz.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bl.shxzskj.cn

TS:   // 同上
来源：http://jx.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uh.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dj.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wo.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wj.szxytkj.cn

================================================================================
来源：http://eh.szxytkj.cn

G. 面向对象
来源：http://ds.newstarts.cn

================================================================================
来源：http://vc.shxzukj.cn

[G01] 定义类
来源：http://tu.gzmigu.cn

Py:   class User: pass
来源：http://dp.panjiajie.cn

PHP:  class User {}
来源：http://ug.szxytkj.cn

JS:   class User {}
来源：http://cs.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://zy.nicolike.cn

Java: class User {}
来源：http://zy.hnjuh.cn

Go:   type User struct { Name string }
来源：http://rz.muxihuayi.cn

Ruby: class User; end
来源：http://vu.yuntaijiaju.cn

C#:   class User {}
来源：http://cl.colortex.cn

[G02] 构造函数
来源：http://op.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://il.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ye.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://lk.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://ms.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://kv.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eb.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://bg.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://tx.wgjwhj.cn

[G03] 实例属性
来源：http://yj.bookmarksfly.cn

Py:   self.name = "x"
来源：http://iy.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://so.haigaiapp.cn

JS:   this.name = "x";
来源：http://bz.muxihuayi.cn

TS:   name: string = "x";
来源：http://rv.huixiangedu.cn

Java: private String name;
来源：http://he.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jq.haigaiapp.cn

Ruby: @name = "x"
来源：http://yt.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://se.shtwfgs.cn

[G04] 定义方法
来源：http://vi.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://yj.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eq.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://tx.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://lc.asd995.cn

Java: String greet() { return name; }
来源：http://fh.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sw.9csxet.cn

Ruby: def greet; @name; end
来源：http://gx.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://gm.haigaiapp.cn

[G05] 继承
来源：http://or.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ph.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://qf.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://nc.nicolike.cn

TS:   class Admin extends User {}
来源：http://ay.lnxyls.cn

Java: class Admin extends User {}
来源：http://nc.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://or.521024.cn

Ruby: class Admin < User; end
来源：http://rq.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://sh.panjiajie.cn

[G06] 重写方法
来源：http://jp.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://gm.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ro.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://rl.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://wx.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://ct.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ri.asd995.cn

Ruby: def greet; "admin"; end
来源：http://eh.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://ki.nszjky.cn

[G07] 调用父类方法
来源：http://vb.huixiangedu.cn

Py:   super().greet()
来源：http://aj.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://yf.hahajie.cn

JS:   super.greet();
来源：http://af.nszjky.cn

TS:   super.greet();
来源：http://ph.chemitech.net.cn

Java: super.greet();
来源：http://rz.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ew.haigaiapp.cn

Ruby: super
来源：http://cs.huanxung.cn

C#:   base.Greet();
来源：http://tw.hnjuh.cn

[G08] 静态方法与属性
来源：http://qz.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wo.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://nt.gzmigu.cn

JS:   static f() {}
来源：http://rm.shxzskj.cn

TS:   static f(): void {}
来源：http://ym.haigaiapp.cn

Java: static void f() {}
来源：http://cd.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zj.chemitech.net.cn

Ruby: def self.f; end
来源：http://td.muxihuayi.cn

C#:   public static void F() {}
来源：http://yo.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://lt.hahajie.cn


<!-- 参考信息 -->