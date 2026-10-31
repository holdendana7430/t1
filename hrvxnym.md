代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rc.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vl.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lc.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ij.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ve.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ar.jianghongdianzi.cn

[E16] 数字千分位
来源：http://ll.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://yc.panjiajie.cn

PHP:  number_format(1234567);
来源：http://js.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ug.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rb.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lo.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hg.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ci.asd995.cn

C#:   1234567.ToString("N0")
来源：http://ij.shxzskj.cn

[E17] 首字母大写
来源：http://lq.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ew.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://id.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://re.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kx.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rq.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://px.newstarts.cn

Ruby: s.capitalize
来源：http://mb.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://na.huanxung.cn

[E18] 模板占位符替换
来源：http://nb.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pa.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ae.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dw.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dm.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tl.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://em.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xf.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jk.newstarts.cn

[E19] 多行文本按行拆分
来源：http://yi.shxzskj.cn

Py:   s.splitlines()
来源：http://ig.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ug.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://la.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://im.szxytkj.cn

Java: s.lines().toList()
来源：http://ce.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://io.hnjuh.cn

Ruby: s.lines
来源：http://wb.huixiangedu.cn

C#:   s.Split('\n')
来源：http://mj.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://gk.9csxet.cn

Py:   if not s:
来源：http://iu.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ol.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jb.shtwfgs.cn

TS:   if (s === "") {}
来源：http://pr.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://ea.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://nn.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://qh.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://xk.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vp.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hd.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bf.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uk.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ip.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zr.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://or.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cy.nszjky.cn

[E22] 字节长度与字符长度
来源：http://ya.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zd.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ii.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bg.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bf.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://op.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bs.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://gz.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://et.bjjhwx.cn

================================================================================
来源：http://rm.colortex.cn

F. 文件与目录
来源：http://hm.nicolike.cn

================================================================================
来源：http://lb.szsharing.cn

[F01] 读取整个文件
来源：http://mo.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ux.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://ou.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lp.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zp.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pq.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://le.asd995.cn

Ruby: File.read("a.txt")
来源：http://lo.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://pz.hnjuh.cn

[F02] 逐行读取文件
来源：http://yq.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://km.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://he.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://en.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pt.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pb.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iw.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yj.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://np.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pt.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qj.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fk.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://my.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ht.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pn.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://tm.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dk.muxihuayi.cn

[F04] 追加写入文件
来源：http://ng.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bb.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bg.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://li.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nu.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ws.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wx.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vp.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vp.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://io.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ky.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://fl.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://dq.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://vh.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fs.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ss.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://uc.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://bk.gzmigu.cn

[F06] 删除文件
来源：http://qy.nicolike.cn

Py:   os.remove("a.txt")
来源：http://qj.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://ky.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tn.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qf.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://es.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://xz.colortex.cn

Ruby: File.delete("a.txt")
来源：http://ak.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://kb.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://zy.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mx.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rb.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ao.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sh.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gx.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ne.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://si.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hh.szsharing.cn

[F08] 遍历目录
来源：http://lr.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qa.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://km.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://db.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ub.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ri.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hw.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://qo.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://lm.nicolike.cn

[F09] 获取文件大小
来源：http://ov.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://jq.colortex.cn

PHP:  filesize("a.txt");
来源：http://hu.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://pf.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://vm.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://de.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ak.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ef.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://jx.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://qd.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://br.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hy.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jr.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://bl.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ac.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pw.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xo.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jp.521024.cn

[F11] 复制与移动文件
来源：http://oh.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tw.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ll.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oe.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rz.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zv.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cl.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fq.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vf.huanxung.cn

[F12] CSV 读写
来源：http://oc.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://on.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jg.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://db.hahajie.cn

TS:   // 同上
来源：http://ia.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hy.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hw.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tr.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://zb.colortex.cn

G. 面向对象
来源：http://xd.bookmarksfly.cn

================================================================================
来源：http://mw.shtwfgs.cn

[G01] 定义类
来源：http://zs.hnjuh.cn

Py:   class User: pass
来源：http://pd.hahajie.cn

PHP:  class User {}
来源：http://xx.panjiajie.cn

JS:   class User {}
来源：http://jh.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://ye.colortex.cn

Java: class User {}
来源：http://js.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://jf.nicolike.cn

Ruby: class User; end
来源：http://xw.newstarts.cn

C#:   class User {}
来源：http://ht.newstarts.cn

[G02] 构造函数
来源：http://iq.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://ga.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://bg.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://fy.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://zq.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://oq.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xx.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://hw.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://nv.shxzskj.cn

[G03] 实例属性
来源：http://wn.panjiajie.cn

Py:   self.name = "x"
来源：http://rx.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://rm.haigaiapp.cn

JS:   this.name = "x";
来源：http://ny.chemitech.net.cn

TS:   name: string = "x";
来源：http://xd.asd995.cn

Java: private String name;
来源：http://pj.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ew.gzmigu.cn

Ruby: @name = "x"
来源：http://tw.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://tf.yuexingan06.cn

[G04] 定义方法
来源：http://jo.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://ff.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lr.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://bs.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://np.szxytkj.cn

Java: String greet() { return name; }
来源：http://qp.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jg.newstarts.cn

Ruby: def greet; @name; end
来源：http://lx.huanxung.cn

C#:   public string Greet() => Name;
来源：http://oi.yuntaijiaju.cn

[G05] 继承
来源：http://eo.nicolike.cn

Py:   class Admin(User): pass
来源：http://wf.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://jy.shxzukj.cn

JS:   class Admin extends User {}
来源：http://uh.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://rj.szsharing.cn

Java: class Admin extends User {}
来源：http://tb.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pr.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://pt.panjiajie.cn

C#:   class Admin : User {}
来源：http://dj.jctech888.com.cn

[G06] 重写方法
来源：http://nj.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://sp.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jx.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://kd.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://au.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ow.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ta.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://by.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://lr.521024.cn

[G07] 调用父类方法
来源：http://lr.huanxung.cn

Py:   super().greet()
来源：http://wp.muxihuayi.cn

PHP:  parent::greet();
来源：http://rp.szsharing.cn

JS:   super.greet();
来源：http://sw.szxytkj.cn

TS:   super.greet();
来源：http://gv.shxzukj.cn

Java: super.greet();
来源：http://pt.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://an.shxzukj.cn

Ruby: super
来源：http://da.jctech888.com.cn

C#:   base.Greet();
来源：http://ui.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://my.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://np.chemitech.net.cn

PHP:  public static function f() {}
来源：http://ya.panjiajie.cn

JS:   static f() {}
来源：http://sq.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://vu.huanxung.cn

Java: static void f() {}
来源：http://ux.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lw.colortex.cn

Ruby: def self.f; end
来源：http://dw.lnxyls.cn

C#:   public static void F() {}
来源：http://ax.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://zs.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://ej.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nr.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ad.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://ad.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://yt.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://dh.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lk.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ms.gzmigu.cn

[G10] 访问控制
来源：http://oc.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://lk.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://nj.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://tw.szsharing.cn

TS:   public / protected / private
来源：http://lo.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://bt.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rv.nszjky.cn

Ruby: public / protected / private
来源：http://hf.hahajie.cn

C#:   public / protected / private / internal
来源：http://uj.wgjwhj.cn

[G11] getter / setter
来源：http://py.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://nz.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://au.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://tv.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://gh.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://lm.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hn.szsharing.cn

Ruby: attr_accessor :name
来源：http://ay.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://tl.asd995.cn

[G12] 对象转字符串
来源：http://al.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://tr.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lq.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://cq.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://pv.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://kw.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xe.asd995.cn

Ruby: def to_s; @name; end
来源：http://nu.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://pl.huanxung.cn

[G13] 判断对象类型
来源：http://kr.asd995.cn

Py:   isinstance(u, User)
来源：http://zq.shtwfgs.cn

PHP:  $u instanceof User
来源：http://rd.9csxet.cn

JS:   u instanceof User
来源：http://ln.shxzskj.cn

TS:   u instanceof User
来源：http://mv.bookmarksfly.cn

Java: u instanceof User
来源：http://tb.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://od.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://fq.gzmigu.cn

C#:   u is User
来源：http://bu.hahajie.cn


<!-- 参考信息 -->