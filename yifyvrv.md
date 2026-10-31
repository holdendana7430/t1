代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://po.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://ac.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ad.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pt.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lu.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ud.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ib.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://su.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yz.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rt.bookmarksfly.cn

[E16] 数字千分位
来源：http://wj.nicolike.cn

Py:   f"{1234567:,}"
来源：http://rm.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://rr.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bp.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://op.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yi.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vr.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hm.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://jy.hahajie.cn

[E17] 首字母大写
来源：http://vq.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tn.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://my.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aq.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ut.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kq.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lr.bjjhwx.cn

Ruby: s.capitalize
来源：http://gt.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lu.bjjhwx.cn

[E18] 模板占位符替换
来源：http://pf.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xn.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mm.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ch.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qy.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dv.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mk.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://to.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://kp.haigaiapp.cn

Py:   s.splitlines()
来源：http://wc.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jw.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://sm.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://yk.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://wp.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://ei.gzmigu.cn

Ruby: s.lines
来源：http://ku.shxzskj.cn

C#:   s.Split('\n')
来源：http://rr.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://be.bjjhwx.cn

Py:   if not s:
来源：http://yw.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ag.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yk.shtwfgs.cn

TS:   if (s === "") {}
来源：http://yj.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://gh.haigaiapp.cn

Go:   if s == "" {}
来源：http://tx.haigaiapp.cn

Ruby: if s.empty?
来源：http://lo.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zq.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://cc.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oz.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ci.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rd.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ad.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rb.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ka.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ew.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kn.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://pj.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://em.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zt.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pa.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dq.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wi.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oi.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ud.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cp.newstarts.cn

================================================================================
来源：http://bn.lnxyls.cn

F. 文件与目录
来源：http://dz.muxihuayi.cn

================================================================================
来源：http://rs.chemitech.net.cn

[F01] 读取整个文件
来源：http://bd.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zh.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://tn.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bw.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hf.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cp.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rw.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://vr.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://io.chemitech.net.cn

[F02] 逐行读取文件
来源：http://im.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yw.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lz.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hl.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://en.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fi.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cp.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ut.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://da.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://yl.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fq.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://de.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ol.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://le.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xy.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lm.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://lb.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nj.panjiajie.cn

[F04] 追加写入文件
来源：http://sd.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ut.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qo.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ie.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fv.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rw.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qw.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aj.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qb.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://cw.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ad.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ng.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://gb.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://hx.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dh.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dt.521024.cn

Ruby: File.exist?("a.txt")
来源：http://lc.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://rx.9csxet.cn

[F06] 删除文件
来源：http://dd.newstarts.cn

Py:   os.remove("a.txt")
来源：http://se.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://js.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jr.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://of.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dn.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://lp.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://ui.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://fo.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ib.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yz.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ht.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bh.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qr.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rx.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pc.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sv.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ep.chemitech.net.cn

[F08] 遍历目录
来源：http://ou.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ew.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kq.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://lm.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://um.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vv.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sm.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://fw.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://nf.yuexingan06.cn

[F09] 获取文件大小
来源：http://kl.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://ob.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://tl.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://jx.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://kp.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fs.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cu.nicolike.cn

Ruby: File.size("a.txt")
来源：http://ml.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://zo.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://pj.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://co.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dw.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fk.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://kx.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lr.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zf.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wy.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cc.muxihuayi.cn

[F11] 复制与移动文件
来源：http://hy.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ya.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pl.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xg.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://td.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aw.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rl.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ns.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tb.jctech888.com.cn

[F12] CSV 读写
来源：http://dz.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nq.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qm.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kx.hnjuh.cn

TS:   // 同上
来源：http://ji.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zc.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kp.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vu.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ym.colortex.cn

================================================================================
来源：http://af.bjjhwx.cn

G. 面向对象
来源：http://ik.gzmigu.cn

================================================================================
来源：http://gd.huanxung.cn

[G01] 定义类
来源：http://qh.huanxung.cn

Py:   class User: pass
来源：http://kd.wgjwhj.cn

PHP:  class User {}
来源：http://uy.huanxung.cn

JS:   class User {}
来源：http://hm.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ox.shxzukj.cn

Java: class User {}
来源：http://cl.shxzskj.cn

Go:   type User struct { Name string }
来源：http://or.jianghongdianzi.cn

Ruby: class User; end
来源：http://zv.muxihuayi.cn

C#:   class User {}
来源：http://gm.yuexingan06.cn

[G02] 构造函数
来源：http://hr.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://uo.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://rv.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://lw.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://bt.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://vi.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ts.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://hk.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://ae.huixinmuqiang.cn

[G03] 实例属性
来源：http://cx.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://eq.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://wz.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://vr.newstarts.cn

TS:   name: string = "x";
来源：http://cd.newstarts.cn

Java: private String name;
来源：http://fk.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yx.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://rc.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://oy.gzmigu.cn

[G04] 定义方法
来源：http://ch.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://eg.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sj.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://zj.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://wl.nicolike.cn

Java: String greet() { return name; }
来源：http://wd.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mi.hnjuh.cn

Ruby: def greet; @name; end
来源：http://pi.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://um.lnxyls.cn

[G05] 继承
来源：http://ly.colortex.cn

Py:   class Admin(User): pass
来源：http://sy.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://rz.hnjuh.cn

JS:   class Admin extends User {}
来源：http://pz.gzmigu.cn

TS:   class Admin extends User {}
来源：http://mr.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://qv.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yf.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://xq.shxzskj.cn

C#:   class Admin : User {}
来源：http://lv.9csxet.cn

[G06] 重写方法
来源：http://lj.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://dl.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://to.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://gb.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://wy.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ku.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hw.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://yq.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://dr.muxihuayi.cn

[G07] 调用父类方法
来源：http://yu.panjiajie.cn

Py:   super().greet()
来源：http://mm.colortex.cn

PHP:  parent::greet();
来源：http://mh.yuexingan06.cn

JS:   super.greet();
来源：http://qy.wgjwhj.cn

TS:   super.greet();
来源：http://uq.asd995.cn

Java: super.greet();
来源：http://ht.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kc.gzmigu.cn

Ruby: super
来源：http://ux.bjjhwx.cn

C#:   base.Greet();
来源：http://fn.hahajie.cn

[G08] 静态方法与属性
来源：http://ad.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://as.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://dq.yuntaijiaju.cn

JS:   static f() {}
来源：http://hp.haigaiapp.cn

TS:   static f(): void {}
来源：http://xz.bookmarksfly.cn

Java: static void f() {}
来源：http://fi.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rz.lnxyls.cn

Ruby: def self.f; end
来源：http://ue.huanxung.cn

C#:   public static void F() {}
来源：http://wi.9csxet.cn

[G09] 接口 / 抽象类
来源：http://vq.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://mn.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hs.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uk.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://we.newstarts.cn

Java: interface Shape { double area(); }
来源：http://ps.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://ad.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xi.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://br.gzmigu.cn

[G10] 访问控制
来源：http://cn.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://py.521024.cn

PHP:  public / protected / private
来源：http://ez.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://rp.colortex.cn

TS:   public / protected / private
来源：http://kt.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://rg.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yf.wgjwhj.cn

Ruby: public / protected / private
来源：http://td.hahajie.cn

C#:   public / protected / private / internal
来源：http://ir.szxytkj.cn

[G11] getter / setter
来源：http://mx.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://yf.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tg.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://wk.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://nt.panjiajie.cn

Java: public String getName() { return name; }
来源：http://yd.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://br.hahajie.cn

Ruby: attr_accessor :name
来源：http://fe.huanxung.cn

C#:   public string Name { get; set; }
来源：http://pb.hahajie.cn

[G12] 对象转字符串
来源：http://ja.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://pl.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://io.hahajie.cn

JS:   toString() { return this.name; }
来源：http://xb.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://av.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://pn.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://md.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://vz.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://ik.panjiajie.cn

[G13] 判断对象类型
来源：http://vb.9csxet.cn

Py:   isinstance(u, User)
来源：http://cx.asd995.cn

PHP:  $u instanceof User
来源：http://kf.gzmigu.cn

JS:   u instanceof User
来源：http://ce.panjiajie.cn

TS:   u instanceof User
来源：http://rn.9csxet.cn


<!-- 参考信息 -->