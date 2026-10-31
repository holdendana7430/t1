代发 wailian999

PHP:  substr_count($s, "a");
来源：http://df.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://rp.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://vh.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zr.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://kl.nicolike.cn

Ruby: s.count("a")
来源：http://xt.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://em.hnjuh.cn

[E13] 逐字符遍历
来源：http://iw.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://gf.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://os.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vm.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nd.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ag.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kp.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wk.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qe.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://yk.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mj.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mr.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yo.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ok.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pb.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ue.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qv.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cp.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://wv.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rg.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mv.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ip.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cq.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gk.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cf.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pb.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://up.wgjwhj.cn

[E16] 数字千分位
来源：http://uq.asd995.cn

Py:   f"{1234567:,}"
来源：http://yv.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ld.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ce.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vw.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cg.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kk.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ye.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ei.muxihuayi.cn

[E17] 首字母大写
来源：http://sg.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ei.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wu.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jv.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ef.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bs.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fm.chemitech.net.cn

Ruby: s.capitalize
来源：http://zc.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ts.chemitech.net.cn

[E18] 模板占位符替换
来源：http://di.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ag.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tg.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lc.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ke.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xi.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fa.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://em.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rz.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://kw.hnjuh.cn

Py:   s.splitlines()
来源：http://il.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iw.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://dr.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://vf.shtwfgs.cn

Java: s.lines().toList()
来源：http://pu.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://fu.muxihuayi.cn

Ruby: s.lines
来源：http://fr.gzmigu.cn

C#:   s.Split('\n')
来源：http://qz.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://jr.hahajie.cn

Py:   if not s:
来源：http://rn.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://us.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eg.wgjwhj.cn

TS:   if (s === "") {}
来源：http://xl.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://mr.nicolike.cn

Go:   if s == "" {}
来源：http://id.asd995.cn

Ruby: if s.empty?
来源：http://vl.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://om.szxytkj.cn

[E21] 超长截断加省略号
来源：http://je.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://th.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nx.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uh.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fy.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zj.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://hv.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yh.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://os.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://aw.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dq.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fl.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://um.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nx.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zm.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nm.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ql.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qe.haigaiapp.cn

================================================================================
来源：http://gn.shtwfgs.cn

F. 文件与目录
来源：http://mc.shtwfgs.cn

================================================================================
来源：http://tr.jctech888.com.cn

[F01] 读取整个文件
来源：http://ef.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mg.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ul.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ft.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bn.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://me.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ir.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://hj.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://jw.wgjwhj.cn

[F02] 逐行读取文件
来源：http://xs.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iu.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ja.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hx.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kv.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ss.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fp.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ge.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wi.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://wc.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lb.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tb.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://db.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xe.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ev.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ui.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://dm.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zb.9csxet.cn

[F04] 追加写入文件
来源：http://zp.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gw.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yc.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zk.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bt.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://al.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oy.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ox.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jp.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://wb.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oy.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://aj.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://lw.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://ch.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zg.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://im.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://fg.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://yc.yuntaijiaju.cn

[F06] 删除文件
来源：http://cj.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://yp.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://pi.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ln.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fh.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tu.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ad.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ic.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://pa.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://jk.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://er.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ys.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yw.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qn.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wz.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sw.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pg.jctech888.com.cn

[F08] 遍历目录
来源：http://dw.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://is.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ae.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://cv.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://gv.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://er.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ae.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://zf.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://ba.hnjuh.cn

[F09] 获取文件大小
来源：http://yo.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://tt.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://hz.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://kr.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://mt.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lq.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fh.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://mn.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://id.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://gx.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kq.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rc.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://df.asd995.cn

TS:   path.extname("a.txt")
来源：http://sw.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ak.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xh.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lw.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://by.szxytkj.cn

[F11] 复制与移动文件
来源：http://ue.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cs.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zi.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aa.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oe.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://st.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://so.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://di.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hd.muxihuayi.cn

[F12] CSV 读写
来源：http://rp.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ft.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bv.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vo.hahajie.cn

TS:   // 同上
来源：http://nl.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xi.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://an.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ei.shtwfgs.cn

================================================================================
来源：http://sr.yuntaijiaju.cn

G. 面向对象
来源：http://dh.chemitech.net.cn

================================================================================
来源：http://mg.wgjwhj.cn

[G01] 定义类
来源：http://cz.shtwfgs.cn

Py:   class User: pass
来源：http://ru.bjjhwx.cn

PHP:  class User {}
来源：http://nc.bjjhwx.cn

JS:   class User {}
来源：http://dq.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://kj.jctech888.com.cn

Java: class User {}
来源：http://ce.lnxyls.cn

Go:   type User struct { Name string }
来源：http://vi.colortex.cn

Ruby: class User; end
来源：http://ta.chemitech.net.cn

C#:   class User {}
来源：http://gh.haigaiapp.cn

[G02] 构造函数
来源：http://hq.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://dq.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://nd.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://eo.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://qk.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://sj.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ke.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://oz.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://gb.huixinmuqiang.cn

[G03] 实例属性
来源：http://ke.521024.cn

Py:   self.name = "x"
来源：http://nj.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ar.hahajie.cn

JS:   this.name = "x";
来源：http://am.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://ph.9csxet.cn

Java: private String name;
来源：http://ye.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vj.hnjuh.cn

Ruby: @name = "x"
来源：http://gu.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://lg.haigaiapp.cn

[G04] 定义方法
来源：http://aj.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://wh.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yj.huanxung.cn

JS:   greet() { return this.name; }
来源：http://gh.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://oc.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://la.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ef.newstarts.cn

Ruby: def greet; @name; end
来源：http://db.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://fq.newstarts.cn

[G05] 继承
来源：http://pr.hnjuh.cn

Py:   class Admin(User): pass
来源：http://nu.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://hd.newstarts.cn

JS:   class Admin extends User {}
来源：http://nj.asd995.cn

TS:   class Admin extends User {}
来源：http://mm.bjjhwx.cn

Java: class Admin extends User {}
来源：http://va.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hn.hahajie.cn

Ruby: class Admin < User; end
来源：http://wm.asd995.cn

C#:   class Admin : User {}
来源：http://rm.panjiajie.cn

[G06] 重写方法
来源：http://sz.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://sh.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cf.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://rg.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://mr.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://nk.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pd.colortex.cn

Ruby: def greet; "admin"; end
来源：http://da.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://zq.wgjwhj.cn

[G07] 调用父类方法
来源：http://iw.huanxung.cn

Py:   super().greet()
来源：http://ee.shxzukj.cn

PHP:  parent::greet();
来源：http://vg.yuntaijiaju.cn

JS:   super.greet();
来源：http://be.nszjky.cn

TS:   super.greet();
来源：http://je.shxzukj.cn

Java: super.greet();
来源：http://uj.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pc.yuexingan06.cn

Ruby: super
来源：http://ln.szsharing.cn

C#:   base.Greet();
来源：http://oa.shxzukj.cn

[G08] 静态方法与属性
来源：http://re.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://po.nicolike.cn

PHP:  public static function f() {}
来源：http://kd.nszjky.cn

JS:   static f() {}
来源：http://ph.bookmarksfly.cn

TS:   static f(): void {}
来源：http://rd.chemitech.net.cn

Java: static void f() {}
来源：http://ml.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uh.szsharing.cn

Ruby: def self.f; end
来源：http://it.hahajie.cn

C#:   public static void F() {}
来源：http://hr.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://rd.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://fe.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xg.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mv.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://vg.huanxung.cn

Java: interface Shape { double area(); }
来源：http://uj.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://ne.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ok.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://xp.nszjky.cn

[G10] 访问控制
来源：http://yd.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vn.521024.cn

PHP:  public / protected / private
来源：http://pi.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://ov.521024.cn

TS:   public / protected / private
来源：http://kd.521024.cn

Java: public / protected / private / 默认包级
来源：http://vw.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://em.hnjuh.cn

Ruby: public / protected / private
来源：http://qd.bookmarksfly.cn


<!-- 参考信息 -->