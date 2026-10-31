代发 wailian999

Ruby: s.reverse
来源：http://au.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tz.521024.cn

[E12] 统计某字符出现次数
来源：http://vg.nszjky.cn

Py:   s.count("a")
来源：http://vp.521024.cn

PHP:  substr_count($s, "a");
来源：http://qs.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://me.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://mb.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xf.521024.cn

Go:   strings.Count(s, "a")
来源：http://tn.yuexingan06.cn

Ruby: s.count("a")
来源：http://en.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://rz.521024.cn

[E13] 逐字符遍历
来源：http://wh.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://vp.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zk.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tj.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uf.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dr.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pd.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mu.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ug.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://ce.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ak.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bg.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tr.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wk.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qx.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://da.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jk.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hc.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://vb.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uq.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fw.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dr.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nr.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vy.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xi.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pa.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fg.chemitech.net.cn

[E16] 数字千分位
来源：http://wd.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://wr.shxzskj.cn

PHP:  number_format(1234567);
来源：http://ts.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yo.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lj.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gz.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wv.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tr.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://cc.shxzskj.cn

[E17] 首字母大写
来源：http://bw.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vu.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zv.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fg.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://az.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xc.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iw.bjjhwx.cn

Ruby: s.capitalize
来源：http://wa.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://td.gzmigu.cn

[E18] 模板占位符替换
来源：http://qv.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lb.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bj.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zt.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jw.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oy.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yh.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gr.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kj.9csxet.cn

[E19] 多行文本按行拆分
来源：http://vb.jctech888.com.cn

Py:   s.splitlines()
来源：http://sj.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kf.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://bj.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ei.haigaiapp.cn

Java: s.lines().toList()
来源：http://cy.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ie.chemitech.net.cn

Ruby: s.lines
来源：http://ih.lnxyls.cn

C#:   s.Split('\n')
来源：http://gl.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ot.nszjky.cn

Py:   if not s:
来源：http://by.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tg.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sj.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ae.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://wm.gzmigu.cn

Go:   if s == "" {}
来源：http://oe.panjiajie.cn

Ruby: if s.empty?
来源：http://wh.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wk.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://au.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yo.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wc.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lk.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ka.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://gi.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cu.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ct.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://kf.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sz.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lz.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ul.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://zu.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hq.nszjky.cn

================================================================================
来源：http://yz.shtwfgs.cn

F. 文件与目录
来源：http://nb.colortex.cn

================================================================================
来源：http://fd.shxzskj.cn

[F01] 读取整个文件
来源：http://hb.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://di.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://bh.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://af.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://od.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ow.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ly.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://wj.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://yy.nicolike.cn

[F02] 逐行读取文件
来源：http://ay.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sk.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zh.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pu.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sc.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hg.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vi.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qa.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://mo.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vl.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qy.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pc.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fh.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jv.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fo.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ka.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dg.shxzskj.cn

[F04] 追加写入文件
来源：http://vj.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ad.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sp.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bu.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fp.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fz.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://je.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jf.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://nl.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bh.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://pc.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://lb.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://wa.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hp.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pa.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://yh.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://kl.yuexingan06.cn

[F06] 删除文件
来源：http://xc.nicolike.cn

Py:   os.remove("a.txt")
来源：http://ir.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://fq.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yf.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ag.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wj.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://vf.521024.cn

Ruby: File.delete("a.txt")
来源：http://ze.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://tt.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://ay.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://os.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yi.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://et.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fz.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kt.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ep.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wo.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rl.yuntaijiaju.cn

[F08] 遍历目录
来源：http://jv.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fr.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fz.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://gt.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://pn.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tn.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ko.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://gf.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://yq.szsharing.cn

[F09] 获取文件大小
来源：http://lf.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://vw.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://vi.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://fh.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://ud.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://al.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bv.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://hz.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://pn.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://kg.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ir.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cd.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tm.521024.cn

TS:   path.extname("a.txt")
来源：http://gd.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ih.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gy.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xs.gzmigu.cn

[F11] 复制与移动文件
来源：http://bx.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qi.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zk.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ga.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lj.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cl.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://md.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cp.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jz.gzmigu.cn

[F12] CSV 读写
来源：http://qj.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xv.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://we.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qt.szxytkj.cn

TS:   // 同上
来源：http://cl.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ah.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sv.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fr.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ul.szsharing.cn

================================================================================
来源：http://un.shtwfgs.cn

G. 面向对象
来源：http://cb.nszjky.cn

================================================================================
来源：http://gw.shtwfgs.cn

[G01] 定义类
来源：http://wv.shxzukj.cn

Py:   class User: pass
来源：http://ea.chemitech.net.cn

PHP:  class User {}
来源：http://om.yuexingan06.cn

JS:   class User {}
来源：http://qx.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://co.nszjky.cn

Java: class User {}
来源：http://fb.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://qh.jianghongdianzi.cn

Ruby: class User; end
来源：http://fl.shtwfgs.cn

C#:   class User {}
来源：http://pv.huanxung.cn

[G02] 构造函数
来源：http://ql.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://wt.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://mz.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://vf.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://pt.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://vk.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pa.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://sr.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://bb.hnjuh.cn

[G03] 实例属性
来源：http://zo.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://yo.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://oi.shxzskj.cn

JS:   this.name = "x";
来源：http://vf.bookmarksfly.cn

TS:   name: string = "x";
来源：http://sv.shtwfgs.cn

Java: private String name;
来源：http://cm.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tq.haigaiapp.cn

Ruby: @name = "x"
来源：http://hf.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://bx.colortex.cn

[G04] 定义方法
来源：http://gz.szsharing.cn

Py:   def greet(self): return self.name
来源：http://hi.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vp.nszjky.cn

JS:   greet() { return this.name; }
来源：http://sv.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://qy.colortex.cn

Java: String greet() { return name; }
来源：http://rw.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mz.lnxyls.cn

Ruby: def greet; @name; end
来源：http://fk.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://tn.521024.cn

[G05] 继承
来源：http://nb.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://bi.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://vy.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://vn.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://dk.newstarts.cn

Java: class Admin extends User {}
来源：http://jk.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pb.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://of.hahajie.cn

C#:   class Admin : User {}
来源：http://db.huixiangedu.cn

[G06] 重写方法
来源：http://kn.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://js.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gz.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ie.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://jx.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://dd.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qt.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://dk.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://cu.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://hd.jianghongdianzi.cn

Py:   super().greet()
来源：http://sc.asd995.cn

PHP:  parent::greet();
来源：http://iz.colortex.cn

JS:   super.greet();
来源：http://sn.gzmigu.cn

TS:   super.greet();
来源：http://xb.muxihuayi.cn

Java: super.greet();
来源：http://gf.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kf.panjiajie.cn

Ruby: super
来源：http://bh.huanxung.cn

C#:   base.Greet();
来源：http://gt.huixiangedu.cn

[G08] 静态方法与属性
来源：http://iq.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jt.szsharing.cn

PHP:  public static function f() {}
来源：http://su.szsharing.cn

JS:   static f() {}
来源：http://im.shxzskj.cn

TS:   static f(): void {}
来源：http://fu.colortex.cn

Java: static void f() {}
来源：http://gf.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fh.shtwfgs.cn

Ruby: def self.f; end
来源：http://ma.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://po.newstarts.cn

[G09] 接口 / 抽象类
来源：http://mo.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://ps.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nz.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kc.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ny.colortex.cn

Java: interface Shape { double area(); }
来源：http://pr.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://io.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ff.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://lj.jctech888.com.cn

[G10] 访问控制
来源：http://bm.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://gd.hahajie.cn

PHP:  public / protected / private
来源：http://xd.hahajie.cn

JS:   #private 字段；其余公开
来源：http://se.bookmarksfly.cn


<!-- 参考信息 -->