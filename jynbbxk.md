代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vo.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tc.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://td.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://df.nszjky.cn

[E14] URL 编码与 Base64
来源：http://mg.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zy.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ck.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aj.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nq.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yz.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pf.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fh.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gx.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://zd.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ga.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ux.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ms.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://di.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://al.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bw.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yg.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ai.hnjuh.cn

[E16] 数字千分位
来源：http://ly.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://io.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://qf.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fu.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rh.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sj.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rs.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ss.colortex.cn

C#:   1234567.ToString("N0")
来源：http://xf.9csxet.cn

[E17] 首字母大写
来源：http://rg.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://el.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://de.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hi.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pm.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rc.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qg.bookmarksfly.cn

Ruby: s.capitalize
来源：http://oy.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zu.hahajie.cn

[E18] 模板占位符替换
来源：http://us.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://it.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kk.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zv.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aj.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fo.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wz.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yk.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://th.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://gx.shxzskj.cn

Py:   s.splitlines()
来源：http://jm.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dh.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://qb.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://tw.yuexingan06.cn

Java: s.lines().toList()
来源：http://ck.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://iw.huixinmuqiang.cn

Ruby: s.lines
来源：http://pm.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://es.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://qo.szsharing.cn

Py:   if not s:
来源：http://if.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mq.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kd.chemitech.net.cn

TS:   if (s === "") {}
来源：http://ru.521024.cn

Java: if (s.isEmpty()) {}
来源：http://oo.shtwfgs.cn

Go:   if s == "" {}
来源：http://ug.gzmigu.cn

Ruby: if s.empty?
来源：http://ub.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mn.gzmigu.cn

[E21] 超长截断加省略号
来源：http://rs.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ka.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ww.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rl.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://un.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jb.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://uk.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xd.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nn.9csxet.cn

[E22] 字节长度与字符长度
来源：http://sg.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wx.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ao.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bu.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ff.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bu.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nz.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://uk.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ra.nicolike.cn

================================================================================
来源：http://cr.nszjky.cn

F. 文件与目录
来源：http://rd.nicolike.cn

================================================================================
来源：http://cy.chemitech.net.cn

[F01] 读取整个文件
来源：http://xe.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uj.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://xt.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ua.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tq.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wj.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://db.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://yh.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://iy.yuexingan06.cn

[F02] 逐行读取文件
来源：http://we.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vt.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wm.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nl.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://av.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://no.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pt.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://no.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aw.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ul.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kp.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kv.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mt.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xo.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://em.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yv.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ak.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ie.jctech888.com.cn

[F04] 追加写入文件
来源：http://lb.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uz.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iv.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wm.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iw.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zw.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sk.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ev.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qm.521024.cn

[F05] 判断文件或目录是否存在
来源：http://ro.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iy.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://zk.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://sv.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://st.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xl.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kx.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://zl.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://qo.colortex.cn

[F06] 删除文件
来源：http://hf.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://bz.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://nq.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pl.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ds.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kc.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://jb.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://zy.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://cw.nicolike.cn

[F07] 创建目录（含多级）
来源：http://oo.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vk.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qs.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ud.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kq.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://an.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gl.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://az.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ou.panjiajie.cn

[F08] 遍历目录
来源：http://bw.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://do.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zb.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://qx.521024.cn

TS:   fs.readdirSync("dir")
来源：http://yn.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ai.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ys.colortex.cn

Ruby: Dir.children("dir")
来源：http://th.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://gl.szxytkj.cn

[F09] 获取文件大小
来源：http://ro.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://lc.huanxung.cn

PHP:  filesize("a.txt");
来源：http://eg.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://vo.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://ij.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qs.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://of.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://bj.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ew.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://pa.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xq.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jk.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xd.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://kk.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pz.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qm.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://le.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zl.nicolike.cn

[F11] 复制与移动文件
来源：http://jh.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sl.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cv.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://em.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ey.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nd.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://br.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yr.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ni.shtwfgs.cn

[F12] CSV 读写
来源：http://hg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gj.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xn.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ew.hahajie.cn

TS:   // 同上
来源：http://ag.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yt.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wp.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ot.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wc.muxihuayi.cn

================================================================================
来源：http://av.521024.cn

G. 面向对象
来源：http://lq.muxihuayi.cn

================================================================================
来源：http://iw.wgjwhj.cn

[G01] 定义类
来源：http://ca.chemitech.net.cn

Py:   class User: pass
来源：http://gz.haigaiapp.cn

PHP:  class User {}
来源：http://dr.szsharing.cn

JS:   class User {}
来源：http://oe.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://lg.szsharing.cn

Java: class User {}
来源：http://ac.9csxet.cn

Go:   type User struct { Name string }
来源：http://mn.chemitech.net.cn

Ruby: class User; end
来源：http://le.colortex.cn

C#:   class User {}
来源：http://vt.jianghongdianzi.cn

[G02] 构造函数
来源：http://jd.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://rv.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://qx.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://gs.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://ot.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://gr.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iy.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://ct.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://mh.szxytkj.cn

[G03] 实例属性
来源：http://da.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://me.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://lm.wgjwhj.cn

JS:   this.name = "x";
来源：http://ny.huanxung.cn

TS:   name: string = "x";
来源：http://pf.hnjuh.cn

Java: private String name;
来源：http://rn.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fh.panjiajie.cn

Ruby: @name = "x"
来源：http://rf.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://qq.szsharing.cn

[G04] 定义方法
来源：http://ls.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://sy.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nc.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://pt.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://rc.jctech888.com.cn

Java: String greet() { return name; }
来源：http://sy.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nl.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://rn.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://zv.jianghongdianzi.cn

[G05] 继承
来源：http://jj.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://hx.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://cp.gzmigu.cn

JS:   class Admin extends User {}
来源：http://hs.hnjuh.cn

TS:   class Admin extends User {}
来源：http://jh.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://he.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kg.nicolike.cn

Ruby: class Admin < User; end
来源：http://cq.muxihuayi.cn

C#:   class Admin : User {}
来源：http://he.muxihuayi.cn

[G06] 重写方法
来源：http://fw.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://rj.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ok.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://gg.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://gt.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://xf.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ym.colortex.cn

Ruby: def greet; "admin"; end
来源：http://qk.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://xk.shxzskj.cn

[G07] 调用父类方法
来源：http://gu.jianghongdianzi.cn

Py:   super().greet()
来源：http://jp.nicolike.cn

PHP:  parent::greet();
来源：http://tk.bookmarksfly.cn

JS:   super.greet();
来源：http://gc.asd995.cn

TS:   super.greet();
来源：http://rx.gzmigu.cn

Java: super.greet();
来源：http://at.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://le.panjiajie.cn

Ruby: super
来源：http://yi.muxihuayi.cn

C#:   base.Greet();
来源：http://no.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://lw.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ec.lnxyls.cn

PHP:  public static function f() {}
来源：http://ey.panjiajie.cn

JS:   static f() {}
来源：http://ja.lnxyls.cn

TS:   static f(): void {}
来源：http://cn.szxytkj.cn

Java: static void f() {}
来源：http://pb.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ch.huixiangedu.cn

Ruby: def self.f; end
来源：http://uk.colortex.cn

C#:   public static void F() {}
来源：http://zb.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://fm.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ds.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oa.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fy.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://ca.nszjky.cn

Java: interface Shape { double area(); }
来源：http://cb.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://jm.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ie.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://qx.colortex.cn

[G10] 访问控制
来源：http://rs.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://vg.shtwfgs.cn

PHP:  public / protected / private
来源：http://rc.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://ep.jianghongdianzi.cn

TS:   public / protected / private
来源：http://ia.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://pr.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gm.bookmarksfly.cn

Ruby: public / protected / private
来源：http://we.huanxung.cn

C#:   public / protected / private / internal
来源：http://ka.jianghongdianzi.cn

[G11] getter / setter
来源：http://kq.nicolike.cn

Py:   @property 与 @x.setter
来源：http://zu.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ig.nszjky.cn

JS:   get name() { return this._name; }
来源：http://eb.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://qh.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://tr.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://au.lnxyls.cn

Ruby: attr_accessor :name
来源：http://hw.hahajie.cn

C#:   public string Name { get; set; }
来源：http://qf.nicolike.cn

[G12] 对象转字符串
来源：http://ty.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://wd.lnxyls.cn


<!-- 参考信息 -->