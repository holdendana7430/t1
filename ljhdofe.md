代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jl.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wc.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yu.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ze.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qs.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://ci.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kp.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pa.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gg.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fz.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yy.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ki.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://me.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mb.bjjhwx.cn

[E16] 数字千分位
来源：http://jv.newstarts.cn

Py:   f"{1234567:,}"
来源：http://pw.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://bq.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ys.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://me.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pi.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ju.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yo.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://dk.jctech888.com.cn

[E17] 首字母大写
来源：http://ah.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xv.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oz.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ra.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ev.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uy.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hj.9csxet.cn

Ruby: s.capitalize
来源：http://od.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://js.shxzskj.cn

[E18] 模板占位符替换
来源：http://eu.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yh.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cr.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zo.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ia.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nv.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mv.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sh.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dh.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://ny.huixiangedu.cn

Py:   s.splitlines()
来源：http://mi.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uj.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://qy.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://zz.gzmigu.cn

Java: s.lines().toList()
来源：http://jt.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://tz.jianghongdianzi.cn

Ruby: s.lines
来源：http://hd.nszjky.cn

C#:   s.Split('\n')
来源：http://fc.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://pu.shtwfgs.cn

Py:   if not s:
来源：http://lu.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://us.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mn.nszjky.cn

TS:   if (s === "") {}
来源：http://yx.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ia.shtwfgs.cn

Go:   if s == "" {}
来源：http://ap.jctech888.com.cn

Ruby: if s.empty?
来源：http://ok.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jb.hahajie.cn

[E21] 超长截断加省略号
来源：http://ud.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bi.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ob.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lx.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tt.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dr.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://xp.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zh.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ks.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://sd.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iy.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zg.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ds.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://me.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gb.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://ts.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yc.nicolike.cn

================================================================================
来源：http://co.nszjky.cn

F. 文件与目录
来源：http://wi.szxytkj.cn

================================================================================
来源：http://il.muxihuayi.cn

[F01] 读取整个文件
来源：http://kg.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dz.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://rj.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sb.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pl.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sm.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eb.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ul.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://pf.szsharing.cn

[F02] 逐行读取文件
来源：http://qh.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oz.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ov.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xh.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yq.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nv.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xa.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qc.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qs.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://ke.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rl.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ey.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://om.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hy.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xs.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ko.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://rd.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zg.521024.cn

[F04] 追加写入文件
来源：http://zq.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rn.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qh.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mb.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qq.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tu.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gj.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bx.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://zi.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ow.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://nx.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://gj.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://jc.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://il.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://st.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://vg.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://mw.muxihuayi.cn

[F06] 删除文件
来源：http://ya.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://fp.newstarts.cn

PHP:  unlink("a.txt");
来源：http://xn.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://od.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pw.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mm.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://ms.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://jv.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://qv.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://cv.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cn.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jc.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tm.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mq.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cf.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ar.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ch.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://og.shxzukj.cn

[F08] 遍历目录
来源：http://ik.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pu.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ua.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://hs.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://st.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ld.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ve.9csxet.cn

Ruby: Dir.children("dir")
来源：http://ji.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://xl.hahajie.cn

[F09] 获取文件大小
来源：http://mf.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ma.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://hi.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://bp.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://ka.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ya.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wx.colortex.cn

Ruby: File.size("a.txt")
来源：http://ux.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://pc.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ad.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zy.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kt.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ci.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://jv.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rz.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bl.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ga.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tn.shxzskj.cn

[F11] 复制与移动文件
来源：http://ar.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://do.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://js.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qj.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zg.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lr.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nv.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://re.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zu.szxytkj.cn

[F12] CSV 读写
来源：http://yi.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pd.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sn.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ym.szsharing.cn

TS:   // 同上
来源：http://wq.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qg.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wd.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uw.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ur.bjjhwx.cn

================================================================================
来源：http://vv.nicolike.cn

G. 面向对象
来源：http://rx.panjiajie.cn

================================================================================
来源：http://uo.jctech888.com.cn

[G01] 定义类
来源：http://yi.newstarts.cn

Py:   class User: pass
来源：http://xd.muxihuayi.cn

PHP:  class User {}
来源：http://ic.huixinmuqiang.cn

JS:   class User {}
来源：http://ay.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://aa.asd995.cn

Java: class User {}
来源：http://yt.szsharing.cn

Go:   type User struct { Name string }
来源：http://oj.jctech888.com.cn

Ruby: class User; end
来源：http://ai.bjjhwx.cn

C#:   class User {}
来源：http://ai.jctech888.com.cn

[G02] 构造函数
来源：http://lg.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://pp.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://wz.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://wb.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://qa.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://hg.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gm.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://rr.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://tp.hahajie.cn

[G03] 实例属性
来源：http://fz.shxzukj.cn

Py:   self.name = "x"
来源：http://sf.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://fj.hahajie.cn

JS:   this.name = "x";
来源：http://ur.shxzukj.cn

TS:   name: string = "x";
来源：http://vp.wgjwhj.cn

Java: private String name;
来源：http://xy.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lt.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://oo.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://yr.shxzskj.cn

[G04] 定义方法
来源：http://rz.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://ak.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rv.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://ex.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://ru.colortex.cn

Java: String greet() { return name; }
来源：http://ir.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lq.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://bh.nszjky.cn

C#:   public string Greet() => Name;
来源：http://or.szxytkj.cn

[G05] 继承
来源：http://kg.hnjuh.cn

Py:   class Admin(User): pass
来源：http://sd.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://mq.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://jf.newstarts.cn

TS:   class Admin extends User {}
来源：http://bq.muxihuayi.cn

Java: class Admin extends User {}
来源：http://mg.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wy.colortex.cn

Ruby: class Admin < User; end
来源：http://bi.lnxyls.cn

C#:   class Admin : User {}
来源：http://oc.yuntaijiaju.cn

[G06] 重写方法
来源：http://ip.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://zj.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fv.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://zw.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://gt.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://xi.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rf.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ig.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://jo.nicolike.cn

[G07] 调用父类方法
来源：http://hf.colortex.cn

Py:   super().greet()
来源：http://tx.chemitech.net.cn

PHP:  parent::greet();
来源：http://un.hahajie.cn

JS:   super.greet();
来源：http://ub.huixinmuqiang.cn

TS:   super.greet();
来源：http://iz.huanxung.cn

Java: super.greet();
来源：http://ko.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://di.shxzukj.cn

Ruby: super
来源：http://pi.lnxyls.cn

C#:   base.Greet();
来源：http://kf.hnjuh.cn

[G08] 静态方法与属性
来源：http://dh.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://be.nszjky.cn

PHP:  public static function f() {}
来源：http://sb.521024.cn

JS:   static f() {}
来源：http://lx.bjjhwx.cn

TS:   static f(): void {}
来源：http://ql.nicolike.cn

Java: static void f() {}
来源：http://vv.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rl.szsharing.cn

Ruby: def self.f; end
来源：http://ct.521024.cn

C#:   public static void F() {}
来源：http://em.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://hr.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://eo.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oo.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gj.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://uh.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://jm.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://qv.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://it.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://wo.shtwfgs.cn

[G10] 访问控制
来源：http://yo.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://ru.asd995.cn

PHP:  public / protected / private
来源：http://ex.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://wo.huanxung.cn

TS:   public / protected / private
来源：http://gg.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://oh.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vv.521024.cn

Ruby: public / protected / private
来源：http://pb.szxytkj.cn

C#:   public / protected / private / internal
来源：http://vd.521024.cn

[G11] getter / setter
来源：http://qc.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://dm.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ss.szsharing.cn

JS:   get name() { return this._name; }
来源：http://em.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://lw.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://fa.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xn.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://sm.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://us.szxytkj.cn

[G12] 对象转字符串
来源：http://vt.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://qw.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dy.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://kt.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://ov.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://bw.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bu.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://nq.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://lk.haigaiapp.cn

[G13] 判断对象类型
来源：http://zh.9csxet.cn


<!-- 参考信息 -->