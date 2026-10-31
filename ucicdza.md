代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fn.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rl.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fw.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gc.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ko.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://wc.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://id.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gu.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xu.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kw.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ct.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fl.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vp.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qf.nszjky.cn

[E16] 数字千分位
来源：http://sp.asd995.cn

Py:   f"{1234567:,}"
来源：http://uf.nszjky.cn

PHP:  number_format(1234567);
来源：http://ty.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vz.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tf.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rd.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sa.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nm.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://sy.shtwfgs.cn

[E17] 首字母大写
来源：http://pd.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ic.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jd.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fg.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xp.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jy.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lm.bookmarksfly.cn

Ruby: s.capitalize
来源：http://pj.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vt.szxytkj.cn

[E18] 模板占位符替换
来源：http://ul.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ll.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sg.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://od.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dj.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://je.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xv.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bv.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gh.asd995.cn

[E19] 多行文本按行拆分
来源：http://ru.lnxyls.cn

Py:   s.splitlines()
来源：http://cf.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ls.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://cc.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://dk.yuexingan06.cn

Java: s.lines().toList()
来源：http://ww.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://gn.bookmarksfly.cn

Ruby: s.lines
来源：http://ju.bjjhwx.cn

C#:   s.Split('\n')
来源：http://lv.szsharing.cn

[E20] 判断字符串是否为空
来源：http://kj.jianghongdianzi.cn

Py:   if not s:
来源：http://pa.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ct.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wj.shxzukj.cn

TS:   if (s === "") {}
来源：http://po.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://up.wgjwhj.cn

Go:   if s == "" {}
来源：http://fv.szsharing.cn

Ruby: if s.empty?
来源：http://nu.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jf.newstarts.cn

[E21] 超长截断加省略号
来源：http://vx.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kp.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rc.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lz.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xg.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rt.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://qi.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ou.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mc.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://en.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vb.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mn.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ae.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yi.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://td.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qv.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://zy.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ox.hahajie.cn

================================================================================
来源：http://wa.szxytkj.cn

F. 文件与目录
来源：http://jo.bjjhwx.cn

================================================================================
来源：http://ha.shxzskj.cn

[F01] 读取整个文件
来源：http://sq.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jo.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://oq.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://om.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sd.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wg.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mo.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://gw.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://yq.nicolike.cn

[F02] 逐行读取文件
来源：http://kc.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://au.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bk.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xl.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jb.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rr.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ec.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ti.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vs.asd995.cn

[F03] 写入文件（覆盖）
来源：http://gh.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xu.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yi.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ei.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gu.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zm.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ri.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://lk.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.panjiajie.cn

[F04] 追加写入文件
来源：http://ca.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://td.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qj.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hp.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ua.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lx.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dn.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vu.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xo.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://nv.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qq.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://gn.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://vx.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://ps.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ha.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tl.521024.cn

Ruby: File.exist?("a.txt")
来源：http://mu.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://fd.wgjwhj.cn

[F06] 删除文件
来源：http://hi.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://fg.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://ua.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://by.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sd.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ul.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://rj.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://bi.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://tt.nszjky.cn

[F07] 创建目录（含多级）
来源：http://wg.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xo.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uj.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bm.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ta.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nm.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gr.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xx.hnjuh.cn

[F08] 遍历目录
来源：http://kx.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fq.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hx.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://sq.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://nq.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yl.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hf.nszjky.cn

Ruby: Dir.children("dir")
来源：http://jx.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://ha.9csxet.cn

[F09] 获取文件大小
来源：http://bt.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://as.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://lx.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://zz.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://gs.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oi.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ar.hahajie.cn

Ruby: File.size("a.txt")
来源：http://rn.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://xo.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://qp.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wo.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ha.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qa.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://do.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tg.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bs.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ru.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lz.9csxet.cn

[F11] 复制与移动文件
来源：http://hu.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ag.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jf.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ip.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ur.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wc.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cf.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bo.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lg.chemitech.net.cn

[F12] CSV 读写
来源：http://mj.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ul.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tg.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mq.nszjky.cn

TS:   // 同上
来源：http://pm.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://be.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fh.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jd.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nn.panjiajie.cn

================================================================================
来源：http://dr.newstarts.cn

G. 面向对象
来源：http://zm.huanxung.cn

================================================================================
来源：http://bg.hnjuh.cn

[G01] 定义类
来源：http://sx.panjiajie.cn

Py:   class User: pass
来源：http://qt.bjjhwx.cn

PHP:  class User {}
来源：http://rt.9csxet.cn

JS:   class User {}
来源：http://py.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://jl.shxzukj.cn

Java: class User {}
来源：http://ei.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ib.yuntaijiaju.cn

Ruby: class User; end
来源：http://fs.newstarts.cn

C#:   class User {}
来源：http://rh.chemitech.net.cn

[G02] 构造函数
来源：http://wz.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://tq.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://sn.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://lb.521024.cn

TS:   constructor(public name: string) {}
来源：http://qb.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://dh.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mi.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://rd.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://ui.shxzskj.cn

[G03] 实例属性
来源：http://qr.9csxet.cn

Py:   self.name = "x"
来源：http://yg.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://wg.muxihuayi.cn

JS:   this.name = "x";
来源：http://yx.chemitech.net.cn

TS:   name: string = "x";
来源：http://kj.9csxet.cn

Java: private String name;
来源：http://hq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vn.colortex.cn

Ruby: @name = "x"
来源：http://vb.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://di.muxihuayi.cn

[G04] 定义方法
来源：http://rk.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://hr.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jn.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://tq.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://gi.szsharing.cn

Java: String greet() { return name; }
来源：http://vv.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rs.colortex.cn

Ruby: def greet; @name; end
来源：http://ae.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://sa.chemitech.net.cn

[G05] 继承
来源：http://ta.panjiajie.cn

Py:   class Admin(User): pass
来源：http://uc.szsharing.cn

PHP:  class Admin extends User {}
来源：http://bc.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://hs.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://xq.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://mv.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lx.huanxung.cn

Ruby: class Admin < User; end
来源：http://jt.hahajie.cn

C#:   class Admin : User {}
来源：http://zt.jianghongdianzi.cn

[G06] 重写方法
来源：http://vh.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://mo.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pt.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://wg.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://dt.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://kv.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lh.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://cl.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://ok.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://qv.nicolike.cn

Py:   super().greet()
来源：http://su.yuexingan06.cn

PHP:  parent::greet();
来源：http://fm.szsharing.cn

JS:   super.greet();
来源：http://ne.szsharing.cn

TS:   super.greet();
来源：http://hs.bjjhwx.cn

Java: super.greet();
来源：http://bq.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hd.panjiajie.cn

Ruby: super
来源：http://ux.nszjky.cn

C#:   base.Greet();
来源：http://us.chemitech.net.cn

[G08] 静态方法与属性
来源：http://az.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sq.panjiajie.cn

PHP:  public static function f() {}
来源：http://wg.nicolike.cn

JS:   static f() {}
来源：http://zq.nicolike.cn

TS:   static f(): void {}
来源：http://so.yuexingan06.cn

Java: static void f() {}
来源：http://sp.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wf.huanxung.cn

Ruby: def self.f; end
来源：http://gb.asd995.cn

C#:   public static void F() {}
来源：http://gp.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://fm.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://ds.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hm.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qo.521024.cn

TS:   interface Shape { area(): number; }
来源：http://ex.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://lg.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://fe.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eo.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://ru.hahajie.cn

[G10] 访问控制
来源：http://qe.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://sb.hnjuh.cn

PHP:  public / protected / private
来源：http://dq.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://ub.chemitech.net.cn

TS:   public / protected / private
来源：http://vz.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://mt.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lo.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://js.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ab.jianghongdianzi.cn

[G11] getter / setter
来源：http://bp.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://en.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ga.nicolike.cn

JS:   get name() { return this._name; }
来源：http://nx.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://cp.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://fk.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ak.lnxyls.cn

Ruby: attr_accessor :name
来源：http://tu.szsharing.cn

C#:   public string Name { get; set; }
来源：http://kw.nicolike.cn

[G12] 对象转字符串
来源：http://og.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://px.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gk.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://bt.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://up.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://yl.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wu.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://iw.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://gl.nicolike.cn

[G13] 判断对象类型
来源：http://eu.szxytkj.cn


<!-- 参考信息 -->