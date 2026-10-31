代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yc.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ll.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ec.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tw.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mh.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://dd.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xf.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rv.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://em.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://in.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ai.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qz.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dg.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cw.nszjky.cn

[E16] 数字千分位
来源：http://is.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://og.colortex.cn

PHP:  number_format(1234567);
来源：http://dm.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pp.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://si.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hn.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gp.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ff.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://jx.panjiajie.cn

[E17] 首字母大写
来源：http://io.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gi.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zj.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fv.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rl.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nf.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wp.muxihuayi.cn

Ruby: s.capitalize
来源：http://uq.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://as.szsharing.cn

[E18] 模板占位符替换
来源：http://uz.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ys.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://up.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ow.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vr.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gt.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aq.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zz.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://co.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://gl.9csxet.cn

Py:   s.splitlines()
来源：http://us.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fz.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://hw.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://mb.colortex.cn

Java: s.lines().toList()
来源：http://aa.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://eq.jctech888.com.cn

Ruby: s.lines
来源：http://gh.hnjuh.cn

C#:   s.Split('\n')
来源：http://cq.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://kc.asd995.cn

Py:   if not s:
来源：http://ng.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ch.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rm.panjiajie.cn

TS:   if (s === "") {}
来源：http://xs.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ga.bjjhwx.cn

Go:   if s == "" {}
来源：http://ts.szxytkj.cn

Ruby: if s.empty?
来源：http://ez.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gn.shxzukj.cn

[E21] 超长截断加省略号
来源：http://xt.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xk.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fd.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iu.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kc.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://tm.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hv.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kh.nszjky.cn

[E22] 字节长度与字符长度
来源：http://qg.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://be.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rm.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iu.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gf.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jk.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fr.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://jk.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kh.newstarts.cn

================================================================================
来源：http://gi.bookmarksfly.cn

F. 文件与目录
来源：http://rl.asd995.cn

================================================================================
来源：http://hz.huanxung.cn

[F01] 读取整个文件
来源：http://rw.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lq.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://si.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ty.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://br.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://be.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zv.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://iv.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://wz.9csxet.cn

[F02] 逐行读取文件
来源：http://ek.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://od.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zf.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xb.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qs.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jo.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xf.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lg.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hw.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://sl.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vu.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yx.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ze.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sx.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cw.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://tb.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cx.colortex.cn

[F04] 追加写入文件
来源：http://ja.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jh.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ar.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xj.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kw.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ky.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lp.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ov.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ku.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://ic.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jz.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://lj.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://mu.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://dc.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xv.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kp.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://mq.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://vu.jctech888.com.cn

[F06] 删除文件
来源：http://zd.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://nh.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://du.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kr.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ic.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hw.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://pe.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://pk.521024.cn

C#:   File.Delete("a.txt");
来源：http://qc.hahajie.cn

[F07] 创建目录（含多级）
来源：http://vl.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bn.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fr.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vv.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ux.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xj.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://db.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qo.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vo.newstarts.cn

[F08] 遍历目录
来源：http://st.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zm.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xi.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://zy.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://iz.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wz.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gg.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://nm.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://yb.shxzukj.cn

[F09] 获取文件大小
来源：http://fj.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://wz.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://pp.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://kv.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://pa.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wo.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tl.nszjky.cn

Ruby: File.size("a.txt")
来源：http://lv.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ol.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fi.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nk.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hj.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gd.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ie.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fc.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ad.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pe.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zs.bjjhwx.cn

[F11] 复制与移动文件
来源：http://nu.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hk.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vs.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jf.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yk.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ra.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bm.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kq.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xb.panjiajie.cn

[F12] CSV 读写
来源：http://wv.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sa.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mb.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qm.huixiangedu.cn

TS:   // 同上
来源：http://vg.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fj.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ex.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qx.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://is.shxzskj.cn

================================================================================
来源：http://ia.panjiajie.cn

G. 面向对象
来源：http://ch.huanxung.cn

================================================================================
来源：http://bw.jianghongdianzi.cn

[G01] 定义类
来源：http://pq.hahajie.cn

Py:   class User: pass
来源：http://fq.jctech888.com.cn

PHP:  class User {}
来源：http://bm.9csxet.cn

JS:   class User {}
来源：http://fm.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://pw.huixinmuqiang.cn

Java: class User {}
来源：http://tl.hahajie.cn

Go:   type User struct { Name string }
来源：http://bl.shtwfgs.cn

Ruby: class User; end
来源：http://tl.chemitech.net.cn

C#:   class User {}
来源：http://ap.521024.cn

[G02] 构造函数
来源：http://qb.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ql.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ia.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://hn.colortex.cn

TS:   constructor(public name: string) {}
来源：http://hc.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://mr.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uo.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://kt.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://xd.bjjhwx.cn

[G03] 实例属性
来源：http://qm.shtwfgs.cn

Py:   self.name = "x"
来源：http://sh.huanxung.cn

PHP:  public string $name = "x";
来源：http://av.asd995.cn

JS:   this.name = "x";
来源：http://dr.bookmarksfly.cn

TS:   name: string = "x";
来源：http://oa.lnxyls.cn

Java: private String name;
来源：http://zy.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://to.szxytkj.cn

Ruby: @name = "x"
来源：http://zg.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://fr.huixinmuqiang.cn

[G04] 定义方法
来源：http://sp.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://ti.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rc.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://rn.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://ir.panjiajie.cn

Java: String greet() { return name; }
来源：http://xc.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://no.nszjky.cn

Ruby: def greet; @name; end
来源：http://vw.asd995.cn

C#:   public string Greet() => Name;
来源：http://ta.bjjhwx.cn

[G05] 继承
来源：http://yk.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://dh.9csxet.cn

PHP:  class Admin extends User {}
来源：http://qc.9csxet.cn

JS:   class Admin extends User {}
来源：http://bw.huanxung.cn

TS:   class Admin extends User {}
来源：http://il.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://uh.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://se.gzmigu.cn

Ruby: class Admin < User; end
来源：http://dp.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://fe.huixinmuqiang.cn

[G06] 重写方法
来源：http://gw.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://vl.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wk.colortex.cn

JS:   greet() { return "admin"; }
来源：http://pr.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://pu.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vo.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qo.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://gw.521024.cn

C#:   public override string Greet() => "admin";
来源：http://yx.huanxung.cn

[G07] 调用父类方法
来源：http://rg.gzmigu.cn

Py:   super().greet()
来源：http://gs.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://id.huanxung.cn

JS:   super.greet();
来源：http://sg.wgjwhj.cn

TS:   super.greet();
来源：http://kq.yuexingan06.cn

Java: super.greet();
来源：http://ar.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://re.newstarts.cn

Ruby: super
来源：http://ai.haigaiapp.cn

C#:   base.Greet();
来源：http://gf.shxzukj.cn

[G08] 静态方法与属性
来源：http://hn.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hk.szxytkj.cn

PHP:  public static function f() {}
来源：http://mx.newstarts.cn

JS:   static f() {}
来源：http://bh.521024.cn

TS:   static f(): void {}
来源：http://bf.panjiajie.cn

Java: static void f() {}
来源：http://eb.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sn.huixiangedu.cn

Ruby: def self.f; end
来源：http://et.bookmarksfly.cn

C#:   public static void F() {}
来源：http://to.szsharing.cn

[G09] 接口 / 抽象类
来源：http://nl.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://le.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rp.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wo.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://gf.newstarts.cn

Java: interface Shape { double area(); }
来源：http://au.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://ny.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ud.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://wi.nszjky.cn

[G10] 访问控制
来源：http://jv.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://rj.szsharing.cn

PHP:  public / protected / private
来源：http://nw.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://pn.shxzskj.cn

TS:   public / protected / private
来源：http://wg.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://wb.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://po.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://dr.asd995.cn

C#:   public / protected / private / internal
来源：http://ku.yuntaijiaju.cn

[G11] getter / setter
来源：http://je.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://xg.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xj.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://ci.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://pf.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://je.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mu.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ou.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://pe.szxytkj.cn

[G12] 对象转字符串
来源：http://wd.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://sy.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qx.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://qp.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://vx.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://mf.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hq.nszjky.cn

Ruby: def to_s; @name; end
来源：http://kd.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://zu.shtwfgs.cn

[G13] 判断对象类型
来源：http://yx.szxytkj.cn


<!-- 参考信息 -->