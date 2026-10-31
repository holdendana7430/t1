代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vt.shtwfgs.cn

[E11] 反转字符串
来源：http://lz.muxihuayi.cn

Py:   s[::-1]
来源：http://ny.huanxung.cn

PHP:  strrev($s);
来源：http://jp.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://dp.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://au.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yt.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xi.chemitech.net.cn

Ruby: s.reverse
来源：http://mk.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ao.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://be.jianghongdianzi.cn

Py:   s.count("a")
来源：http://zw.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://kb.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://zx.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://yy.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ye.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://ff.asd995.cn

Ruby: s.count("a")
来源：http://xv.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://np.huanxung.cn

[E13] 逐字符遍历
来源：http://hl.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://nb.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zw.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xi.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vx.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sc.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ez.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ss.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nw.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://nb.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ao.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aq.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bm.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yg.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yt.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kr.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ux.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kf.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://iq.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sq.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pb.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kr.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ex.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hg.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dd.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oh.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vc.haigaiapp.cn

[E16] 数字千分位
来源：http://wt.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://wr.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://js.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jh.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zr.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://il.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ki.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uw.521024.cn

C#:   1234567.ToString("N0")
来源：http://er.bjjhwx.cn

[E17] 首字母大写
来源：http://kw.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fr.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gk.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hw.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vo.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oq.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nq.shxzukj.cn

Ruby: s.capitalize
来源：http://hx.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://se.huanxung.cn

[E18] 模板占位符替换
来源：http://ww.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bf.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dg.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zo.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mu.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jy.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qv.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ph.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kr.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://fc.shxzukj.cn

Py:   s.splitlines()
来源：http://si.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mq.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://kg.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://kz.521024.cn

Java: s.lines().toList()
来源：http://dc.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://es.nicolike.cn

Ruby: s.lines
来源：http://lc.lnxyls.cn

C#:   s.Split('\n')
来源：http://vc.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://nf.lnxyls.cn

Py:   if not s:
来源：http://ur.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dr.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sz.jctech888.com.cn

TS:   if (s === "") {}
来源：http://gn.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://qd.huixiangedu.cn

Go:   if s == "" {}
来源：http://mu.shxzukj.cn

Ruby: if s.empty?
来源：http://vr.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ub.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://mq.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fs.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ef.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jx.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ge.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bm.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ng.colortex.cn

[E22] 字节长度与字符长度
来源：http://vj.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nc.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://or.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rb.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ho.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iu.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://fd.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jf.szxytkj.cn

================================================================================
来源：http://fo.muxihuayi.cn

F. 文件与目录
来源：http://cu.gzmigu.cn

================================================================================
来源：http://bp.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://th.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://li.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://tb.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cm.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hi.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rj.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://se.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ou.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://uw.shtwfgs.cn

[F02] 逐行读取文件
来源：http://yz.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://do.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jc.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bc.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gq.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ad.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sg.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xo.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qm.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://fy.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vr.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gz.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vr.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://je.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ny.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ed.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ag.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bb.asd995.cn

[F04] 追加写入文件
来源：http://jr.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ok.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vw.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bv.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lg.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fa.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hp.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wm.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qk.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://jf.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pc.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://qc.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://ie.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ch.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ap.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://js.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://ot.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://jw.huixinmuqiang.cn

[F06] 删除文件
来源：http://ku.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ts.nszjky.cn

PHP:  unlink("a.txt");
来源：http://wj.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ye.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ag.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pr.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://zt.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://sn.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://mb.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://mr.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kx.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hq.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sa.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nx.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://un.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oz.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mo.jianghongdianzi.cn

[F08] 遍历目录
来源：http://bb.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bb.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pm.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://xr.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://kp.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://un.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ws.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://zg.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://wi.shxzskj.cn

[F09] 获取文件大小
来源：http://lr.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ys.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://yh.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://mv.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://cq.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://so.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sc.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://iw.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://br.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ly.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ts.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ob.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ya.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://ta.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://um.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lv.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://os.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gi.szxytkj.cn

[F11] 复制与移动文件
来源：http://pw.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jm.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zk.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nx.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ha.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://du.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://so.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gn.haigaiapp.cn

[F12] CSV 读写
来源：http://nq.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kh.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eb.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ic.shtwfgs.cn

TS:   // 同上
来源：http://jt.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ud.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ea.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pd.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hh.chemitech.net.cn

================================================================================
来源：http://kp.shxzskj.cn

G. 面向对象
来源：http://zu.huanxung.cn

================================================================================
来源：http://rj.9csxet.cn

[G01] 定义类
来源：http://gg.muxihuayi.cn

Py:   class User: pass
来源：http://og.hnjuh.cn

PHP:  class User {}
来源：http://gx.szsharing.cn

JS:   class User {}
来源：http://tf.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://my.szxytkj.cn

Java: class User {}
来源：http://ph.panjiajie.cn

Go:   type User struct { Name string }
来源：http://qf.huixiangedu.cn

Ruby: class User; end
来源：http://dg.jctech888.com.cn

C#:   class User {}
来源：http://fl.yuntaijiaju.cn

[G02] 构造函数
来源：http://vs.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://qi.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://ub.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://an.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://of.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://ey.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fj.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://mb.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://hd.nicolike.cn

[G03] 实例属性
来源：http://eo.chemitech.net.cn

Py:   self.name = "x"
来源：http://sj.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://gr.szxytkj.cn

JS:   this.name = "x";
来源：http://tl.szxytkj.cn

TS:   name: string = "x";
来源：http://xi.521024.cn

Java: private String name;
来源：http://nr.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uc.521024.cn

Ruby: @name = "x"
来源：http://dl.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oc.bjjhwx.cn

[G04] 定义方法
来源：http://wd.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://zn.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xb.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://vw.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://mu.521024.cn

Java: String greet() { return name; }
来源：http://cj.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nw.newstarts.cn

Ruby: def greet; @name; end
来源：http://wg.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://pz.szsharing.cn

[G05] 继承
来源：http://am.hahajie.cn

Py:   class Admin(User): pass
来源：http://ps.huanxung.cn

PHP:  class Admin extends User {}
来源：http://cd.shxzskj.cn

JS:   class Admin extends User {}
来源：http://zl.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://cj.yuexingan06.cn

Java: class Admin extends User {}
来源：http://kp.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://by.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://pc.szsharing.cn

C#:   class Admin : User {}
来源：http://gw.nszjky.cn

[G06] 重写方法
来源：http://fi.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://sx.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://el.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://ok.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://et.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://kt.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ep.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://xr.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://fa.shtwfgs.cn

[G07] 调用父类方法
来源：http://kq.panjiajie.cn

Py:   super().greet()
来源：http://hf.wgjwhj.cn

PHP:  parent::greet();
来源：http://ue.szsharing.cn

JS:   super.greet();
来源：http://jw.shxzukj.cn

TS:   super.greet();
来源：http://ze.jctech888.com.cn

Java: super.greet();
来源：http://vk.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zm.szxytkj.cn

Ruby: super
来源：http://ke.huixiangedu.cn

C#:   base.Greet();
来源：http://fl.521024.cn

[G08] 静态方法与属性
来源：http://md.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dj.szxytkj.cn

PHP:  public static function f() {}
来源：http://rp.szxytkj.cn

JS:   static f() {}
来源：http://am.gzmigu.cn

TS:   static f(): void {}
来源：http://kw.9csxet.cn

Java: static void f() {}
来源：http://om.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://py.nicolike.cn

Ruby: def self.f; end
来源：http://pv.lnxyls.cn

C#:   public static void F() {}
来源：http://vj.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://vy.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://so.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sb.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jk.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://sj.521024.cn


<!-- 参考信息 -->