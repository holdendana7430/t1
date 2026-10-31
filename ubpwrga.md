代发 wailian999

PHP:  substr_count($s, "a");
来源：http://zg.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ae.9csxet.cn

TS:   s.split("a").length - 1
来源：http://ij.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rf.colortex.cn

Go:   strings.Count(s, "a")
来源：http://vs.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://ea.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://zz.shxzukj.cn

[E13] 逐字符遍历
来源：http://pw.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://lt.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dy.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ts.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oy.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rr.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://in.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qd.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ga.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://fq.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ft.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://io.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hi.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zx.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nk.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lt.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://is.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zl.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://dz.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jt.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ud.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aq.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sv.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ev.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jf.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ll.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cl.newstarts.cn

[E16] 数字千分位
来源：http://bv.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://uu.shxzskj.cn

PHP:  number_format(1234567);
来源：http://ur.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ll.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oj.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qg.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uo.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://tr.szsharing.cn

[E17] 首字母大写
来源：http://or.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yq.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cv.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kj.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yv.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ls.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wg.shxzukj.cn

Ruby: s.capitalize
来源：http://xw.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xn.jctech888.com.cn

[E18] 模板占位符替换
来源：http://ac.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ju.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ud.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fe.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qt.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xb.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://py.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zt.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sv.nicolike.cn

[E19] 多行文本按行拆分
来源：http://mn.jctech888.com.cn

Py:   s.splitlines()
来源：http://yd.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ks.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://pt.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://xm.hahajie.cn

Java: s.lines().toList()
来源：http://ns.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://ae.521024.cn

Ruby: s.lines
来源：http://xr.nicolike.cn

C#:   s.Split('\n')
来源：http://na.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://cf.huixiangedu.cn

Py:   if not s:
来源：http://yi.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zj.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hj.9csxet.cn

TS:   if (s === "") {}
来源：http://vv.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://bt.panjiajie.cn

Go:   if s == "" {}
来源：http://jg.lnxyls.cn

Ruby: if s.empty?
来源：http://es.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pp.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://ub.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hu.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ci.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://il.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vo.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ug.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://ao.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://no.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yu.521024.cn

[E22] 字节长度与字符长度
来源：http://fc.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ei.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://za.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://np.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fr.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rd.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://es.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://na.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://od.9csxet.cn

================================================================================
来源：http://pv.lnxyls.cn

F. 文件与目录
来源：http://us.hahajie.cn

================================================================================
来源：http://uk.bjjhwx.cn

[F01] 读取整个文件
来源：http://gl.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tz.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ej.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mg.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://es.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oa.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://io.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://tp.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://xo.wgjwhj.cn

[F02] 逐行读取文件
来源：http://fy.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hi.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kg.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wb.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://do.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://la.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qe.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gr.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ce.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://tq.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mq.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xf.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hd.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jt.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fu.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zs.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://md.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bt.newstarts.cn

[F04] 追加写入文件
来源：http://oo.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rt.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sh.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://py.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fo.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://su.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://je.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://er.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ul.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://nq.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rp.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://rn.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://na.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://nw.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hn.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vw.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://la.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://dr.lnxyls.cn

[F06] 删除文件
来源：http://wi.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://kz.nicolike.cn

PHP:  unlink("a.txt");
来源：http://yr.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ur.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ma.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vx.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://fk.asd995.cn

Ruby: File.delete("a.txt")
来源：http://pf.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://hl.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://be.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wi.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uv.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mr.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ix.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://av.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://in.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cy.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ki.colortex.cn

[F08] 遍历目录
来源：http://hy.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qk.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hs.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://xb.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://gt.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mb.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ay.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://aj.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://od.shtwfgs.cn

[F09] 获取文件大小
来源：http://dh.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://ua.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://nk.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://un.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://hi.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lp.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ou.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://xt.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://cx.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ao.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yb.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bt.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mh.nicolike.cn

TS:   path.extname("a.txt")
来源：http://jp.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ev.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uk.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xc.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://os.huixiangedu.cn

[F11] 复制与移动文件
来源：http://qc.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lf.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pf.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gq.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sm.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mb.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kv.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ri.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://se.muxihuayi.cn

[F12] CSV 读写
来源：http://xy.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yx.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zk.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yt.muxihuayi.cn

TS:   // 同上
来源：http://by.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ov.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ev.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tq.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tt.bookmarksfly.cn

================================================================================
来源：http://fs.hnjuh.cn

G. 面向对象
来源：http://ma.gzmigu.cn

================================================================================
来源：http://lq.521024.cn

[G01] 定义类
来源：http://af.shtwfgs.cn

Py:   class User: pass
来源：http://dv.colortex.cn

PHP:  class User {}
来源：http://ir.nszjky.cn

JS:   class User {}
来源：http://rc.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://er.bjjhwx.cn

Java: class User {}
来源：http://od.521024.cn

Go:   type User struct { Name string }
来源：http://up.lnxyls.cn

Ruby: class User; end
来源：http://ty.wgjwhj.cn

C#:   class User {}
来源：http://wx.chemitech.net.cn

[G02] 构造函数
来源：http://wm.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://sf.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://dg.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://dr.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://mc.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://ie.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pu.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ao.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://mo.chemitech.net.cn

[G03] 实例属性
来源：http://de.shxzukj.cn

Py:   self.name = "x"
来源：http://mk.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://uf.huanxung.cn

JS:   this.name = "x";
来源：http://pc.shxzukj.cn

TS:   name: string = "x";
来源：http://dm.haigaiapp.cn

Java: private String name;
来源：http://mf.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ez.nszjky.cn

Ruby: @name = "x"
来源：http://dp.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://sq.hahajie.cn

[G04] 定义方法
来源：http://ok.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://qp.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://om.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://ub.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://sv.szxytkj.cn

Java: String greet() { return name; }
来源：http://uh.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mf.9csxet.cn

Ruby: def greet; @name; end
来源：http://bg.colortex.cn

C#:   public string Greet() => Name;
来源：http://ie.chemitech.net.cn

[G05] 继承
来源：http://vp.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://mx.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://zf.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://tl.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://bv.gzmigu.cn

Java: class Admin extends User {}
来源：http://em.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iv.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://cx.colortex.cn

C#:   class Admin : User {}
来源：http://zz.yuexingan06.cn

[G06] 重写方法
来源：http://qy.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ct.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gz.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://xk.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hc.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ek.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tw.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://dw.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://qr.wgjwhj.cn

[G07] 调用父类方法
来源：http://wt.chemitech.net.cn

Py:   super().greet()
来源：http://xd.bjjhwx.cn

PHP:  parent::greet();
来源：http://dv.chemitech.net.cn

JS:   super.greet();
来源：http://tt.gzmigu.cn

TS:   super.greet();
来源：http://gk.szxytkj.cn

Java: super.greet();
来源：http://gx.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ri.bjjhwx.cn

Ruby: super
来源：http://is.newstarts.cn

C#:   base.Greet();
来源：http://ja.lnxyls.cn

[G08] 静态方法与属性
来源：http://cz.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dr.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://yv.wgjwhj.cn

JS:   static f() {}
来源：http://fr.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ua.muxihuayi.cn

Java: static void f() {}
来源：http://am.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uk.hnjuh.cn

Ruby: def self.f; end
来源：http://cq.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://xk.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://zh.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://id.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tf.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ii.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://ys.newstarts.cn

Java: interface Shape { double area(); }
来源：http://be.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://xx.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ih.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://vh.newstarts.cn

[G10] 访问控制
来源：http://on.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://xb.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://no.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://bq.hnjuh.cn

TS:   public / protected / private
来源：http://mx.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://cg.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ha.szsharing.cn

Ruby: public / protected / private
来源：http://gr.chemitech.net.cn


<!-- 参考信息 -->