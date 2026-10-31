代发 wailian999

[E14] URL 编码与 Base64
来源：http://gp.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://af.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ti.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vc.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://va.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lv.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://we.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://an.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sd.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://ds.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ho.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sx.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nb.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nr.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://js.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pm.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nz.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lh.asd995.cn

[E16] 数字千分位
来源：http://qx.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://oy.nszjky.cn

PHP:  number_format(1234567);
来源：http://pn.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ew.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ts.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xm.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://km.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nd.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://zr.wgjwhj.cn

[E17] 首字母大写
来源：http://qt.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gh.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bs.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ek.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qm.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.haigaiapp.cn

Ruby: s.capitalize
来源：http://ak.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hh.colortex.cn

[E18] 模板占位符替换
来源：http://zs.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zl.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wo.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ut.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zl.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ej.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pt.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vu.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ov.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://op.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://tg.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qq.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://sl.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://zm.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://qp.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://it.521024.cn

Ruby: s.lines
来源：http://wb.lnxyls.cn

C#:   s.Split('\n')
来源：http://oy.9csxet.cn

[E20] 判断字符串是否为空
来源：http://lv.panjiajie.cn

Py:   if not s:
来源：http://tm.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yy.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nz.szxytkj.cn

TS:   if (s === "") {}
来源：http://mw.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://yl.shxzskj.cn

Go:   if s == "" {}
来源：http://gq.shxzskj.cn

Ruby: if s.empty?
来源：http://aa.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bp.hahajie.cn

[E21] 超长截断加省略号
来源：http://zl.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ym.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nw.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kr.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dn.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lg.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ry.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gf.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ab.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://gi.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://az.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cd.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wi.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zh.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://as.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gk.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://gh.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gi.nszjky.cn

================================================================================
来源：http://sl.shxzukj.cn

F. 文件与目录
来源：http://il.shxzskj.cn

================================================================================
来源：http://gt.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://dx.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xd.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ob.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zd.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vm.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yz.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rw.521024.cn

Ruby: File.read("a.txt")
来源：http://qk.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://bc.bjjhwx.cn

[F02] 逐行读取文件
来源：http://wl.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ka.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ly.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ov.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dt.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ce.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tu.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mp.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://id.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ug.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cr.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vm.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ua.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ju.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nj.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://dz.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gk.521024.cn

[F04] 追加写入文件
来源：http://si.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lt.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dv.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fe.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nl.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ao.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dl.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ma.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://xu.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xw.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://iq.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://tc.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://un.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fi.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kx.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://fn.asd995.cn

C#:   File.Exists("a.txt")
来源：http://jj.lnxyls.cn

[F06] 删除文件
来源：http://yi.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://no.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://hp.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://el.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xt.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://af.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://vm.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://ez.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://dw.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://nc.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dm.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ko.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wv.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://le.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uh.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vd.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jw.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dp.jctech888.com.cn

[F08] 遍历目录
来源：http://yl.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ay.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bp.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ll.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://ix.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ny.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ud.szsharing.cn

Ruby: Dir.children("dir")
来源：http://wv.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://jl.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://ue.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://xa.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://rx.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://vy.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://fu.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ou.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ce.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://uk.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ll.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://bf.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ql.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zm.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cw.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://yg.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://og.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vs.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yf.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mn.huanxung.cn

[F11] 复制与移动文件
来源：http://zr.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hu.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mo.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sw.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hw.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cb.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fa.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yk.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ey.shxzukj.cn

[F12] CSV 读写
来源：http://xu.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kf.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qc.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mn.muxihuayi.cn

TS:   // 同上
来源：http://sb.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zc.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hd.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eh.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sg.huanxung.cn

================================================================================
来源：http://gv.huixinmuqiang.cn

G. 面向对象
来源：http://nl.shxzukj.cn

================================================================================
来源：http://dp.panjiajie.cn

[G01] 定义类
来源：http://il.newstarts.cn

Py:   class User: pass
来源：http://om.haigaiapp.cn

PHP:  class User {}
来源：http://ur.bjjhwx.cn

JS:   class User {}
来源：http://dj.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://wr.nicolike.cn

Java: class User {}
来源：http://vz.lnxyls.cn

Go:   type User struct { Name string }
来源：http://ae.colortex.cn

Ruby: class User; end
来源：http://md.hnjuh.cn

C#:   class User {}
来源：http://kt.muxihuayi.cn

[G02] 构造函数
来源：http://oz.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://an.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://qd.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://zf.asd995.cn

TS:   constructor(public name: string) {}
来源：http://jr.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://ix.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mt.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://nz.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://gw.szxytkj.cn

[G03] 实例属性
来源：http://dp.shxzskj.cn

Py:   self.name = "x"
来源：http://nb.nszjky.cn

PHP:  public string $name = "x";
来源：http://ba.shxzskj.cn

JS:   this.name = "x";
来源：http://na.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://we.panjiajie.cn

Java: private String name;
来源：http://qq.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://br.shxzskj.cn

Ruby: @name = "x"
来源：http://di.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://st.szsharing.cn

[G04] 定义方法
来源：http://tm.nszjky.cn

Py:   def greet(self): return self.name
来源：http://tt.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xy.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://jz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://az.hahajie.cn

Java: String greet() { return name; }
来源：http://rb.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mz.shxzskj.cn

Ruby: def greet; @name; end
来源：http://tr.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://bf.szxytkj.cn

[G05] 继承
来源：http://mq.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ek.hahajie.cn

PHP:  class Admin extends User {}
来源：http://bo.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://an.hahajie.cn

TS:   class Admin extends User {}
来源：http://gh.jctech888.com.cn

Java: class Admin extends User {}
来源：http://lg.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://of.colortex.cn

Ruby: class Admin < User; end
来源：http://fj.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://oj.huixinmuqiang.cn

[G06] 重写方法
来源：http://ru.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://sa.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qv.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://gr.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ok.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://bs.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ql.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://va.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://cf.wgjwhj.cn

[G07] 调用父类方法
来源：http://ga.hnjuh.cn

Py:   super().greet()
来源：http://bo.9csxet.cn

PHP:  parent::greet();
来源：http://jv.jianghongdianzi.cn

JS:   super.greet();
来源：http://yu.shtwfgs.cn

TS:   super.greet();
来源：http://tk.nszjky.cn

Java: super.greet();
来源：http://vv.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ec.chemitech.net.cn

Ruby: super
来源：http://qm.huixiangedu.cn

C#:   base.Greet();
来源：http://qf.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://tm.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ue.9csxet.cn

PHP:  public static function f() {}
来源：http://oj.9csxet.cn

JS:   static f() {}
来源：http://mm.szxytkj.cn

TS:   static f(): void {}
来源：http://pc.haigaiapp.cn

Java: static void f() {}
来源：http://nx.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zy.panjiajie.cn

Ruby: def self.f; end
来源：http://ft.shxzskj.cn

C#:   public static void F() {}
来源：http://qw.9csxet.cn

[G09] 接口 / 抽象类
来源：http://fg.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://we.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zn.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ev.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://uc.9csxet.cn

Java: interface Shape { double area(); }
来源：http://qd.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://sh.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pz.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://lm.hnjuh.cn

[G10] 访问控制
来源：http://vx.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://tg.colortex.cn

PHP:  public / protected / private
来源：http://ss.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://pb.huixinmuqiang.cn

TS:   public / protected / private
来源：http://ze.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://bn.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mq.shxzukj.cn

Ruby: public / protected / private
来源：http://ej.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://dh.muxihuayi.cn

[G11] getter / setter
来源：http://up.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://tt.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zr.szsharing.cn

JS:   get name() { return this._name; }
来源：http://fh.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://pj.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ax.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gd.nszjky.cn

Ruby: attr_accessor :name
来源：http://kd.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://lb.bjjhwx.cn

[G12] 对象转字符串
来源：http://ff.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://sp.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://go.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://lp.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://kw.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://la.chemitech.net.cn


<!-- 参考信息 -->