代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ff.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://mr.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vp.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ou.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ls.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pp.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ei.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fr.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zu.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jn.muxihuayi.cn

[E16] 数字千分位
来源：http://wt.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://fw.hnjuh.cn

PHP:  number_format(1234567);
来源：http://bb.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ag.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wy.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vq.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ua.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dq.asd995.cn

C#:   1234567.ToString("N0")
来源：http://zs.huixiangedu.cn

[E17] 首字母大写
来源：http://ed.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eb.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xq.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xd.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dy.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tm.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.szsharing.cn

Ruby: s.capitalize
来源：http://kv.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qm.hahajie.cn

[E18] 模板占位符替换
来源：http://xg.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://se.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jw.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ft.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yb.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qn.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://md.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ig.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sq.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://bh.shxzukj.cn

Py:   s.splitlines()
来源：http://dz.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kd.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://ly.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://rh.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://no.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://zd.szxytkj.cn

Ruby: s.lines
来源：http://zc.panjiajie.cn

C#:   s.Split('\n')
来源：http://gm.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://ke.bookmarksfly.cn

Py:   if not s:
来源：http://od.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xy.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hf.panjiajie.cn

TS:   if (s === "") {}
来源：http://ax.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://fv.521024.cn

Go:   if s == "" {}
来源：http://nn.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://as.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.panjiajie.cn

[E21] 超长截断加省略号
来源：http://la.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ur.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hf.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fn.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vc.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cr.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gq.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://ip.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qm.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://in.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uy.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ab.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hy.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cr.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://uz.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.wgjwhj.cn

================================================================================
来源：http://io.hnjuh.cn

F. 文件与目录
来源：http://cl.yuntaijiaju.cn

================================================================================
来源：http://ac.huixiangedu.cn

[F01] 读取整个文件
来源：http://uq.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qm.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://tn.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fc.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mj.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ma.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tr.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://fn.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://zy.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ul.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pj.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rj.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kx.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zi.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sd.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kg.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fs.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://xm.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ck.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pd.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jv.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ds.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rd.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iy.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://ak.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ji.newstarts.cn

[F04] 追加写入文件
来源：http://cy.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nc.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://md.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xz.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rj.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ka.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wo.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gl.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sb.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ar.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://na.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://qr.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://dh.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://yj.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dt.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://el.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://xc.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://xi.haigaiapp.cn

[F06] 删除文件
来源：http://kq.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://qi.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://mo.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wl.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zm.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rl.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ka.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ol.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://nz.nszjky.cn

[F07] 创建目录（含多级）
来源：http://dk.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wv.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ey.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nj.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ja.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jq.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aa.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lg.nicolike.cn

[F08] 遍历目录
来源：http://fz.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ts.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hh.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://gv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://pi.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://np.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ie.9csxet.cn

Ruby: Dir.children("dir")
来源：http://lq.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ti.muxihuayi.cn

[F09] 获取文件大小
来源：http://hp.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://mg.szsharing.cn

PHP:  filesize("a.txt");
来源：http://do.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://al.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://jx.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ai.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ma.szsharing.cn

Ruby: File.size("a.txt")
来源：http://ro.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kz.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://op.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zo.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ip.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://go.newstarts.cn

TS:   path.extname("a.txt")
来源：http://zh.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zo.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jw.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eu.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tk.lnxyls.cn

[F11] 复制与移动文件
来源：http://ec.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gi.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://se.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pq.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pp.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cb.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cr.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ts.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ft.bookmarksfly.cn

[F12] CSV 读写
来源：http://bc.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wu.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ee.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xb.szxytkj.cn

TS:   // 同上
来源：http://en.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gl.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pb.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ga.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yo.asd995.cn

================================================================================
来源：http://wc.huixiangedu.cn

G. 面向对象
来源：http://hq.huanxung.cn

================================================================================
来源：http://ld.wgjwhj.cn

[G01] 定义类
来源：http://iy.nszjky.cn

Py:   class User: pass
来源：http://bn.panjiajie.cn

PHP:  class User {}
来源：http://pw.nicolike.cn

JS:   class User {}
来源：http://kv.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://mm.lnxyls.cn

Java: class User {}
来源：http://ld.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://eu.colortex.cn

Ruby: class User; end
来源：http://bn.shxzskj.cn

C#:   class User {}
来源：http://er.haigaiapp.cn

[G02] 构造函数
来源：http://cz.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wk.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://vq.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://px.521024.cn

TS:   constructor(public name: string) {}
来源：http://qv.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://yk.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eh.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://gp.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://je.asd995.cn

[G03] 实例属性
来源：http://lg.huixiangedu.cn

Py:   self.name = "x"
来源：http://uc.lnxyls.cn

PHP:  public string $name = "x";
来源：http://dv.nicolike.cn

JS:   this.name = "x";
来源：http://wg.shxzskj.cn

TS:   name: string = "x";
来源：http://ww.jianghongdianzi.cn

Java: private String name;
来源：http://fs.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ve.gzmigu.cn

Ruby: @name = "x"
来源：http://pu.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://hl.shtwfgs.cn

[G04] 定义方法
来源：http://xq.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://ix.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://od.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://zv.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://zi.szsharing.cn

Java: String greet() { return name; }
来源：http://fy.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pw.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://wf.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://eb.jianghongdianzi.cn

[G05] 继承
来源：http://rp.colortex.cn

Py:   class Admin(User): pass
来源：http://bv.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://ja.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://rb.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://dd.yuexingan06.cn

Java: class Admin extends User {}
来源：http://xd.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mc.521024.cn

Ruby: class Admin < User; end
来源：http://rg.jctech888.com.cn

C#:   class Admin : User {}
来源：http://rp.yuntaijiaju.cn

[G06] 重写方法
来源：http://wo.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://sa.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vr.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://gk.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://kq.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://kq.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uy.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://vk.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://id.chemitech.net.cn

[G07] 调用父类方法
来源：http://ob.shxzskj.cn

Py:   super().greet()
来源：http://pm.huixiangedu.cn

PHP:  parent::greet();
来源：http://pu.huixinmuqiang.cn

JS:   super.greet();
来源：http://vy.lnxyls.cn

TS:   super.greet();
来源：http://xz.newstarts.cn

Java: super.greet();
来源：http://gn.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rc.hnjuh.cn

Ruby: super
来源：http://gj.newstarts.cn

C#:   base.Greet();
来源：http://bt.asd995.cn

[G08] 静态方法与属性
来源：http://re.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wn.lnxyls.cn

PHP:  public static function f() {}
来源：http://jx.bookmarksfly.cn

JS:   static f() {}
来源：http://yg.muxihuayi.cn

TS:   static f(): void {}
来源：http://wv.shxzukj.cn

Java: static void f() {}
来源：http://rl.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lj.huixiangedu.cn

Ruby: def self.f; end
来源：http://bv.nicolike.cn

C#:   public static void F() {}
来源：http://da.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://rc.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://pt.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://le.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ol.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://rh.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://qs.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://fo.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xr.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://wz.newstarts.cn

[G10] 访问控制
来源：http://xh.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://kb.szsharing.cn

PHP:  public / protected / private
来源：http://wf.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://be.yuntaijiaju.cn

TS:   public / protected / private
来源：http://iq.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://qi.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xr.521024.cn

Ruby: public / protected / private
来源：http://hp.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://zg.9csxet.cn

[G11] getter / setter
来源：http://qk.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://xi.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pn.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ry.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://ty.hahajie.cn

Java: public String getName() { return name; }
来源：http://jw.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fi.hahajie.cn

Ruby: attr_accessor :name
来源：http://pj.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://cy.huixiangedu.cn

[G12] 对象转字符串
来源：http://qi.asd995.cn

Py:   def __str__(self): return self.name
来源：http://it.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wl.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://cp.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://ul.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://oq.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dw.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ot.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://mn.asd995.cn

[G13] 判断对象类型
来源：http://xy.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://hx.hahajie.cn

PHP:  $u instanceof User
来源：http://xu.hnjuh.cn

JS:   u instanceof User
来源：http://hc.huanxung.cn

TS:   u instanceof User
来源：http://ro.newstarts.cn


<!-- 参考信息 -->