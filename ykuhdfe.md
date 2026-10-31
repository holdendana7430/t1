代发 wailian999

JS:   [...s].reverse().join("")
来源：http://pj.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://gb.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wd.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bs.asd995.cn

Ruby: s.reverse
来源：http://gb.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ke.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://xy.szxytkj.cn

Py:   s.count("a")
来源：http://of.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ss.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://nt.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://ed.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cb.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://rp.haigaiapp.cn

Ruby: s.count("a")
来源：http://ef.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://xw.9csxet.cn

[E13] 逐字符遍历
来源：http://kg.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://nv.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zk.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zs.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://om.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lz.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jq.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rt.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bz.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://wc.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bq.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://go.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cz.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gv.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pw.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ts.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ga.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xi.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ow.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ib.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xm.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://or.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vb.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pn.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fv.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://re.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pj.jianghongdianzi.cn

[E16] 数字千分位
来源：http://mr.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://bt.shxzukj.cn

PHP:  number_format(1234567);
来源：http://dv.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ne.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yc.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bp.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qa.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mi.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://lf.panjiajie.cn

[E17] 首字母大写
来源：http://ti.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pe.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ek.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qa.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vj.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ga.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lb.bjjhwx.cn

Ruby: s.capitalize
来源：http://ef.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ys.muxihuayi.cn

[E18] 模板占位符替换
来源：http://bg.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ea.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zj.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ts.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rp.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dn.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fv.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wv.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rp.huanxung.cn

[E19] 多行文本按行拆分
来源：http://mo.muxihuayi.cn

Py:   s.splitlines()
来源：http://ur.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ti.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ou.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ag.nszjky.cn

Java: s.lines().toList()
来源：http://dx.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://hj.521024.cn

Ruby: s.lines
来源：http://br.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ds.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://yo.huixiangedu.cn

Py:   if not s:
来源：http://me.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://au.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zg.haigaiapp.cn

TS:   if (s === "") {}
来源：http://yo.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://zr.gzmigu.cn

Go:   if s == "" {}
来源：http://mi.bjjhwx.cn

Ruby: if s.empty?
来源：http://oz.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sv.colortex.cn

[E21] 超长截断加省略号
来源：http://gw.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gg.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gn.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lc.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gq.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fw.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://wa.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hy.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qi.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://aj.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tw.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ej.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gr.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ww.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wi.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://iw.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://br.yuntaijiaju.cn

================================================================================
来源：http://xh.lnxyls.cn

F. 文件与目录
来源：http://oa.jianghongdianzi.cn

================================================================================
来源：http://zw.chemitech.net.cn

[F01] 读取整个文件
来源：http://zp.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tt.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://gq.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xz.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fr.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hs.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://it.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://gh.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://jg.bjjhwx.cn

[F02] 逐行读取文件
来源：http://tw.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nw.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fv.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ha.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ox.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dc.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fn.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vc.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fx.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ye.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gm.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sd.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ot.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hn.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rz.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pf.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://mk.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jo.521024.cn

[F04] 追加写入文件
来源：http://bu.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yn.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ts.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hc.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kt.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qx.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://me.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vc.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://mv.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jh.colortex.cn

PHP:  file_exists("a.txt");
来源：http://pi.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://tf.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://uy.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zp.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://op.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://vv.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://pe.shxzskj.cn

[F06] 删除文件
来源：http://yp.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://rg.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://qy.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ir.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xm.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kj.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://kk.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://sk.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://eq.colortex.cn

[F07] 创建目录（含多级）
来源：http://eo.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rg.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xl.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dv.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://px.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ih.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wq.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uo.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jj.jctech888.com.cn

[F08] 遍历目录
来源：http://xd.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jc.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mh.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://qn.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://ao.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bs.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://up.521024.cn

Ruby: Dir.children("dir")
来源：http://tv.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://fk.bjjhwx.cn

[F09] 获取文件大小
来源：http://sz.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://rv.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://fo.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://ix.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://so.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ae.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cs.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://ts.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qr.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://vm.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ig.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mb.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cg.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://mk.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ha.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zg.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eu.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fd.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://wi.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vk.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://is.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rf.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xc.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bz.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pq.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bx.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xx.521024.cn

[F12] CSV 读写
来源：http://tz.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fq.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kh.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tk.shxzukj.cn

TS:   // 同上
来源：http://un.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ih.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ln.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://co.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zo.haigaiapp.cn

================================================================================
来源：http://vi.hnjuh.cn

G. 面向对象
来源：http://al.newstarts.cn

================================================================================
来源：http://su.huixiangedu.cn

[G01] 定义类
来源：http://oq.yuexingan06.cn

Py:   class User: pass
来源：http://fy.asd995.cn

PHP:  class User {}
来源：http://lf.hahajie.cn

JS:   class User {}
来源：http://zb.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://vm.muxihuayi.cn

Java: class User {}
来源：http://ay.colortex.cn

Go:   type User struct { Name string }
来源：http://wh.lnxyls.cn

Ruby: class User; end
来源：http://ru.521024.cn

C#:   class User {}
来源：http://ck.bookmarksfly.cn

[G02] 构造函数
来源：http://rq.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://pr.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ib.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://uz.521024.cn

TS:   constructor(public name: string) {}
来源：http://wc.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://tz.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jg.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://od.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://de.521024.cn

[G03] 实例属性
来源：http://tr.jctech888.com.cn

Py:   self.name = "x"
来源：http://sb.nicolike.cn

PHP:  public string $name = "x";
来源：http://ld.hnjuh.cn

JS:   this.name = "x";
来源：http://hm.yuexingan06.cn

TS:   name: string = "x";
来源：http://ij.bjjhwx.cn

Java: private String name;
来源：http://xw.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dw.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://on.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://mt.muxihuayi.cn

[G04] 定义方法
来源：http://os.asd995.cn

Py:   def greet(self): return self.name
来源：http://la.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bn.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://sc.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://xr.wgjwhj.cn

Java: String greet() { return name; }
来源：http://nt.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gl.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://wv.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://zd.521024.cn

[G05] 继承
来源：http://vc.huanxung.cn

Py:   class Admin(User): pass
来源：http://cm.nicolike.cn

PHP:  class Admin extends User {}
来源：http://mq.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://ot.szxytkj.cn

TS:   class Admin extends User {}
来源：http://gk.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ny.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pp.shxzskj.cn

Ruby: class Admin < User; end
来源：http://br.newstarts.cn

C#:   class Admin : User {}
来源：http://qr.shxzukj.cn

[G06] 重写方法
来源：http://zf.asd995.cn

Py:   def greet(self): return "admin"
来源：http://gc.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ro.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://dw.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://rw.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://yb.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ui.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://qx.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://iq.shtwfgs.cn

[G07] 调用父类方法
来源：http://vx.shxzskj.cn

Py:   super().greet()
来源：http://no.asd995.cn

PHP:  parent::greet();
来源：http://ej.huanxung.cn

JS:   super.greet();
来源：http://fm.lnxyls.cn

TS:   super.greet();
来源：http://li.jctech888.com.cn

Java: super.greet();
来源：http://pg.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://em.panjiajie.cn

Ruby: super
来源：http://rs.jianghongdianzi.cn

C#:   base.Greet();
来源：http://jj.jctech888.com.cn

[G08] 静态方法与属性
来源：http://jm.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gm.gzmigu.cn

PHP:  public static function f() {}
来源：http://hq.yuntaijiaju.cn

JS:   static f() {}
来源：http://mi.haigaiapp.cn

TS:   static f(): void {}
来源：http://ns.asd995.cn

Java: static void f() {}
来源：http://br.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yt.haigaiapp.cn

Ruby: def self.f; end
来源：http://kr.nszjky.cn

C#:   public static void F() {}
来源：http://vk.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ln.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://zd.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yo.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eq.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://hk.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://py.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://bf.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bp.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://ms.nicolike.cn


<!-- 参考信息 -->