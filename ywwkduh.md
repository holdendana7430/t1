代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gy.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nn.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ak.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nu.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://op.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://ia.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://np.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yn.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rl.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iv.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ys.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ua.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ag.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pt.bookmarksfly.cn

[E16] 数字千分位
来源：http://fg.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://fx.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ju.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ty.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wi.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://te.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oi.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://do.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://sf.huixiangedu.cn

[E17] 首字母大写
来源：http://lg.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dv.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iq.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ng.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uc.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lz.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qn.521024.cn

Ruby: s.capitalize
来源：http://jl.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xb.yuexingan06.cn

[E18] 模板占位符替换
来源：http://dm.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dz.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pc.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rp.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://my.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ld.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dq.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hi.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gm.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://nz.huanxung.cn

Py:   s.splitlines()
来源：http://jd.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ww.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://lz.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://cs.newstarts.cn

Java: s.lines().toList()
来源：http://za.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://fg.shxzskj.cn

Ruby: s.lines
来源：http://co.hnjuh.cn

C#:   s.Split('\n')
来源：http://qc.huanxung.cn

[E20] 判断字符串是否为空
来源：http://wh.szxytkj.cn

Py:   if not s:
来源：http://ty.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yb.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://no.9csxet.cn

TS:   if (s === "") {}
来源：http://gk.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://xb.huanxung.cn

Go:   if s == "" {}
来源：http://mv.asd995.cn

Ruby: if s.empty?
来源：http://rs.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vh.gzmigu.cn

[E21] 超长截断加省略号
来源：http://jm.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ne.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hg.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://za.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ni.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gc.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://db.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eo.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mv.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://go.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bn.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sz.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ms.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bz.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fy.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://gw.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uf.jctech888.com.cn

================================================================================
来源：http://oq.yuexingan06.cn

F. 文件与目录
来源：http://wv.chemitech.net.cn

================================================================================
来源：http://ds.521024.cn

[F01] 读取整个文件
来源：http://xz.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ps.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://nj.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hr.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fq.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gc.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sp.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://eq.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://ku.shtwfgs.cn

[F02] 逐行读取文件
来源：http://xn.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://in.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mk.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hg.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dq.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dw.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zj.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gq.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://la.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://zm.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ii.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hu.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ad.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ed.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qc.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://gm.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wf.szsharing.cn

[F04] 追加写入文件
来源：http://qe.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mh.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pu.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://we.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tg.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tf.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pj.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gh.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://fj.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yh.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://by.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://hi.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://tq.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zm.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wp.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://hf.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://wv.asd995.cn

[F06] 删除文件
来源：http://jo.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://po.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://ro.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://op.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lb.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ga.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://eo.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://xb.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://te.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://rk.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://al.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://os.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dh.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zh.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://el.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fd.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ky.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://no.huixiangedu.cn

[F08] 遍历目录
来源：http://ns.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wm.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mz.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://iz.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ln.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xs.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://je.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://dy.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://yr.szxytkj.cn

[F09] 获取文件大小
来源：http://gg.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://pi.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://th.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://xe.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://fj.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ev.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gx.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://de.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://wu.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ie.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wu.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://es.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uo.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://ga.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://il.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://za.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://do.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iq.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://hm.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bk.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ud.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bp.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cw.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fw.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ls.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iy.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lc.huixiangedu.cn

[F12] CSV 读写
来源：http://vo.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wq.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lf.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iu.panjiajie.cn

TS:   // 同上
来源：http://yf.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zl.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fi.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jl.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wj.szsharing.cn

================================================================================
来源：http://cp.huixiangedu.cn

G. 面向对象
来源：http://ga.szsharing.cn

================================================================================
来源：http://tl.huixiangedu.cn

[G01] 定义类
来源：http://yj.shxzukj.cn

Py:   class User: pass
来源：http://nt.szsharing.cn

PHP:  class User {}
来源：http://sy.szxytkj.cn

JS:   class User {}
来源：http://yu.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://dn.huixinmuqiang.cn

Java: class User {}
来源：http://qh.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://ru.521024.cn

Ruby: class User; end
来源：http://ob.bookmarksfly.cn

C#:   class User {}
来源：http://jk.hahajie.cn

[G02] 构造函数
来源：http://wg.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://hw.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://sw.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://fy.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://mt.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://yi.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://br.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://sj.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://kb.shxzukj.cn

[G03] 实例属性
来源：http://vv.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://eg.panjiajie.cn

PHP:  public string $name = "x";
来源：http://zo.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://rj.lnxyls.cn

TS:   name: string = "x";
来源：http://xi.shxzukj.cn

Java: private String name;
来源：http://gx.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ny.shxzskj.cn

Ruby: @name = "x"
来源：http://go.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://xu.lnxyls.cn

[G04] 定义方法
来源：http://oa.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://ho.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xo.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://nf.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://kt.newstarts.cn

Java: String greet() { return name; }
来源：http://rk.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mn.colortex.cn

Ruby: def greet; @name; end
来源：http://ph.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ut.huixinmuqiang.cn

[G05] 继承
来源：http://iy.newstarts.cn

Py:   class Admin(User): pass
来源：http://vu.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://ew.hahajie.cn

JS:   class Admin extends User {}
来源：http://bk.hnjuh.cn

TS:   class Admin extends User {}
来源：http://wj.lnxyls.cn

Java: class Admin extends User {}
来源：http://rc.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hm.szsharing.cn

Ruby: class Admin < User; end
来源：http://zs.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ak.jctech888.com.cn

[G06] 重写方法
来源：http://cc.colortex.cn

Py:   def greet(self): return "admin"
来源：http://us.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sn.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://yx.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ra.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://vh.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ha.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://cs.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://jq.asd995.cn

[G07] 调用父类方法
来源：http://bd.bjjhwx.cn

Py:   super().greet()
来源：http://be.muxihuayi.cn

PHP:  parent::greet();
来源：http://rc.shxzukj.cn

JS:   super.greet();
来源：http://nf.jianghongdianzi.cn

TS:   super.greet();
来源：http://xe.huixinmuqiang.cn

Java: super.greet();
来源：http://sw.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zq.521024.cn

Ruby: super
来源：http://ji.szxytkj.cn

C#:   base.Greet();
来源：http://wg.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://oa.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kx.shxzskj.cn

PHP:  public static function f() {}
来源：http://nf.haigaiapp.cn

JS:   static f() {}
来源：http://ie.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://yk.lnxyls.cn

Java: static void f() {}
来源：http://vx.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ih.newstarts.cn

Ruby: def self.f; end
来源：http://jr.lnxyls.cn

C#:   public static void F() {}
来源：http://oh.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://rd.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://im.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uo.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hf.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://nh.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://mh.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://gs.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ip.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://kq.huanxung.cn

[G10] 访问控制
来源：http://ob.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://cc.colortex.cn

PHP:  public / protected / private
来源：http://ha.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://ig.lnxyls.cn

TS:   public / protected / private
来源：http://sv.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ya.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zs.wgjwhj.cn

Ruby: public / protected / private
来源：http://do.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://ea.hnjuh.cn

[G11] getter / setter
来源：http://in.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://md.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kl.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://me.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ua.huanxung.cn

Java: public String getName() { return name; }
来源：http://ie.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://es.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://ta.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://hh.gzmigu.cn

[G12] 对象转字符串
来源：http://et.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://qx.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hl.newstarts.cn

JS:   toString() { return this.name; }
来源：http://ho.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://yg.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://tm.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nk.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://ls.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ph.wgjwhj.cn

[G13] 判断对象类型
来源：http://zm.muxihuayi.cn


<!-- 参考信息 -->