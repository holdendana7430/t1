代发 wailian999

Go:   strings.Count(s, "a")
来源：http://aq.muxihuayi.cn

Ruby: s.count("a")
来源：http://nm.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://rm.jctech888.com.cn

[E13] 逐字符遍历
来源：http://pr.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ng.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qw.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wd.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fz.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yy.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zv.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jv.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dw.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://wk.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ym.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yy.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gx.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rg.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ia.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jj.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fr.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ox.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://xb.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zf.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gb.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vc.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fm.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iy.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yz.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vh.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ll.jctech888.com.cn

[E16] 数字千分位
来源：http://cq.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://jp.asd995.cn

PHP:  number_format(1234567);
来源：http://vc.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jz.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hc.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bg.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vs.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fd.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://fp.bjjhwx.cn

[E17] 首字母大写
来源：http://rf.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kg.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gw.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xr.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qt.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kq.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pr.huixiangedu.cn

Ruby: s.capitalize
来源：http://ed.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ev.nszjky.cn

[E18] 模板占位符替换
来源：http://pv.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ds.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hp.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yk.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uz.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://is.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ti.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qp.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://tl.jctech888.com.cn

Py:   s.splitlines()
来源：http://tk.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xs.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://pp.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://nd.shxzukj.cn

Java: s.lines().toList()
来源：http://hc.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://fm.bjjhwx.cn

Ruby: s.lines
来源：http://es.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://lm.9csxet.cn

[E20] 判断字符串是否为空
来源：http://yn.9csxet.cn

Py:   if not s:
来源：http://vv.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rj.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hs.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ql.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://ww.nszjky.cn

Go:   if s == "" {}
来源：http://lv.huixiangedu.cn

Ruby: if s.empty?
来源：http://nq.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yx.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ng.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xa.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sv.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://va.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vb.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kl.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://az.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zk.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pl.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://ea.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ln.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tl.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rv.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nx.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zi.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ft.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://uh.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://df.shxzukj.cn

================================================================================
来源：http://tj.szxytkj.cn

F. 文件与目录
来源：http://yw.nicolike.cn

================================================================================
来源：http://ok.chemitech.net.cn

[F01] 读取整个文件
来源：http://hn.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qq.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://tw.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vl.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nm.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yl.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nu.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://ps.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://oa.wgjwhj.cn

[F02] 逐行读取文件
来源：http://st.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oo.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://to.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://go.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xw.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nq.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xb.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://be.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xj.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://yj.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oo.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jh.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cf.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ue.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://im.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wb.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://lg.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aq.wgjwhj.cn

[F04] 追加写入文件
来源：http://hn.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jn.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nh.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ci.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nz.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ww.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://io.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ub.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://za.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cs.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ko.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://ex.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://sb.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ts.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rj.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://hw.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://kj.bjjhwx.cn

[F06] 删除文件
来源：http://br.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://pb.nicolike.cn

PHP:  unlink("a.txt");
来源：http://el.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rm.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vu.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ja.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ro.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://os.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://sd.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://cs.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://va.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qc.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://su.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cc.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ph.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oe.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wg.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kj.colortex.cn

[F08] 遍历目录
来源：http://ga.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qc.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jo.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://sb.521024.cn

TS:   fs.readdirSync("dir")
来源：http://fs.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pq.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://ho.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://zw.521024.cn

[F09] 获取文件大小
来源：http://oz.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://ad.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://ec.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://qu.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://ag.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xe.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://su.newstarts.cn

Ruby: File.size("a.txt")
来源：http://nu.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://mz.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://vj.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ur.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tb.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sw.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://dv.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jv.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ou.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eu.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kr.szsharing.cn

[F11] 复制与移动文件
来源：http://wd.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ut.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zs.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dk.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rx.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gf.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sx.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gs.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lb.hnjuh.cn

[F12] CSV 读写
来源：http://pr.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ga.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aj.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hh.huixinmuqiang.cn

TS:   // 同上
来源：http://gl.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://si.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aw.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qk.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ne.asd995.cn

================================================================================
来源：http://vd.shxzskj.cn

G. 面向对象
来源：http://ca.bjjhwx.cn

================================================================================
来源：http://bz.muxihuayi.cn

[G01] 定义类
来源：http://kw.shxzukj.cn

Py:   class User: pass
来源：http://xf.9csxet.cn

PHP:  class User {}
来源：http://ei.colortex.cn

JS:   class User {}
来源：http://pn.colortex.cn

TS:   class User { name: string = ""; }
来源：http://rg.muxihuayi.cn

Java: class User {}
来源：http://ej.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://ag.jctech888.com.cn

Ruby: class User; end
来源：http://av.nszjky.cn

C#:   class User {}
来源：http://ef.szsharing.cn

[G02] 构造函数
来源：http://un.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://sg.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://dp.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://la.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://gu.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://jd.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qh.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://jy.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://fy.colortex.cn

[G03] 实例属性
来源：http://kn.haigaiapp.cn

Py:   self.name = "x"
来源：http://sh.asd995.cn

PHP:  public string $name = "x";
来源：http://in.lnxyls.cn

JS:   this.name = "x";
来源：http://mk.muxihuayi.cn

TS:   name: string = "x";
来源：http://kr.jianghongdianzi.cn

Java: private String name;
来源：http://rc.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iz.shtwfgs.cn

Ruby: @name = "x"
来源：http://yc.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://kh.lnxyls.cn

[G04] 定义方法
来源：http://vz.nszjky.cn

Py:   def greet(self): return self.name
来源：http://vp.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mj.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://rq.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://cl.huixiangedu.cn

Java: String greet() { return name; }
来源：http://az.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hb.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://iq.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://cl.shxzskj.cn

[G05] 继承
来源：http://fa.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://sk.szsharing.cn

PHP:  class Admin extends User {}
来源：http://fv.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://fq.hahajie.cn

TS:   class Admin extends User {}
来源：http://eq.muxihuayi.cn

Java: class Admin extends User {}
来源：http://bq.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://di.panjiajie.cn

Ruby: class Admin < User; end
来源：http://st.wgjwhj.cn

C#:   class Admin : User {}
来源：http://la.bjjhwx.cn

[G06] 重写方法
来源：http://pl.521024.cn

Py:   def greet(self): return "admin"
来源：http://ay.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gk.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://pv.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://uh.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://uu.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://su.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://nx.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://vw.lnxyls.cn

[G07] 调用父类方法
来源：http://fa.yuntaijiaju.cn

Py:   super().greet()
来源：http://ro.muxihuayi.cn

PHP:  parent::greet();
来源：http://ft.gzmigu.cn

JS:   super.greet();
来源：http://lt.lnxyls.cn

TS:   super.greet();
来源：http://vp.yuntaijiaju.cn

Java: super.greet();
来源：http://yz.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fx.szxytkj.cn

Ruby: super
来源：http://ij.huanxung.cn

C#:   base.Greet();
来源：http://ih.jctech888.com.cn

[G08] 静态方法与属性
来源：http://ae.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mv.hahajie.cn

PHP:  public static function f() {}
来源：http://co.521024.cn

JS:   static f() {}
来源：http://rg.colortex.cn

TS:   static f(): void {}
来源：http://ez.huixiangedu.cn

Java: static void f() {}
来源：http://bv.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nc.hahajie.cn

Ruby: def self.f; end
来源：http://eo.szsharing.cn

C#:   public static void F() {}
来源：http://nb.hahajie.cn

[G09] 接口 / 抽象类
来源：http://pm.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://hg.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yd.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ic.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://uc.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://ha.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://vl.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tb.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://er.nszjky.cn

[G10] 访问控制
来源：http://gx.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://vu.yuexingan06.cn

PHP:  public / protected / private
来源：http://ws.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://nf.colortex.cn

TS:   public / protected / private
来源：http://dm.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://by.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ox.colortex.cn

Ruby: public / protected / private
来源：http://pt.gzmigu.cn

C#:   public / protected / private / internal
来源：http://dt.colortex.cn

[G11] getter / setter
来源：http://ot.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://bq.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tw.huixinmuqiang.cn


<!-- 参考信息 -->