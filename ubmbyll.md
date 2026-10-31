代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hv.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hg.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nc.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ju.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ed.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xw.nszjky.cn

[E16] 数字千分位
来源：http://zl.newstarts.cn

Py:   f"{1234567:,}"
来源：http://sh.lnxyls.cn

PHP:  number_format(1234567);
来源：http://pl.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uy.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dr.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gh.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sd.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qc.521024.cn

C#:   1234567.ToString("N0")
来源：http://ee.shxzukj.cn

[E17] 首字母大写
来源：http://rf.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gn.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ee.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fa.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://og.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ls.nszjky.cn

Ruby: s.capitalize
来源：http://vg.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qk.hahajie.cn

[E18] 模板占位符替换
来源：http://bp.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ri.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ib.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://da.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jp.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xu.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ja.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ks.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.asd995.cn

[E19] 多行文本按行拆分
来源：http://vc.gzmigu.cn

Py:   s.splitlines()
来源：http://ml.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oz.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ru.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://ci.asd995.cn

Java: s.lines().toList()
来源：http://av.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://wh.colortex.cn

Ruby: s.lines
来源：http://uu.chemitech.net.cn

C#:   s.Split('\n')
来源：http://jt.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://bp.shtwfgs.cn

Py:   if not s:
来源：http://ht.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gk.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zf.521024.cn

TS:   if (s === "") {}
来源：http://uc.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://ye.huanxung.cn

Go:   if s == "" {}
来源：http://mt.shxzskj.cn

Ruby: if s.empty?
来源：http://za.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ap.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://bw.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ts.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vw.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bi.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ms.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hw.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://hg.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jv.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nf.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://hz.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mq.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://et.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cy.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rj.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zw.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sg.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://fh.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qj.newstarts.cn

================================================================================
来源：http://jy.shxzskj.cn

F. 文件与目录
来源：http://eg.gzmigu.cn

================================================================================
来源：http://fw.szxytkj.cn

[F01] 读取整个文件
来源：http://uo.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qh.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://jy.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ll.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nb.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wa.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://er.colortex.cn

Ruby: File.read("a.txt")
来源：http://ha.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://xw.gzmigu.cn

[F02] 逐行读取文件
来源：http://gl.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bq.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bc.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hr.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cq.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dv.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xp.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hy.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fx.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://nk.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lb.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xx.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sz.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://he.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rk.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jx.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://tm.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://or.szxytkj.cn

[F04] 追加写入文件
来源：http://wu.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qv.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wz.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://me.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://od.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vy.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://an.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cx.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qn.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://lm.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qn.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://wc.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://vs.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://vi.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dc.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://us.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://to.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://gr.panjiajie.cn

[F06] 删除文件
来源：http://ab.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://db.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://sp.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dk.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ts.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fi.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://wy.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://ga.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://ax.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://pj.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qh.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xv.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ar.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://li.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cd.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://of.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zl.wgjwhj.cn

[F08] 遍历目录
来源：http://rw.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tf.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ca.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://dp.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://os.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jt.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://em.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://xk.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://ya.asd995.cn

[F09] 获取文件大小
来源：http://lh.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://sw.asd995.cn

PHP:  filesize("a.txt");
来源：http://lz.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://bp.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://fn.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mn.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oz.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://sn.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://kg.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://vf.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pj.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lx.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://im.9csxet.cn

TS:   path.extname("a.txt")
来源：http://we.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pd.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wr.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qb.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://py.hahajie.cn

[F11] 复制与移动文件
来源：http://ol.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ct.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bn.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wm.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mp.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qu.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xz.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vv.bjjhwx.cn

[F12] CSV 读写
来源：http://mr.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fm.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://no.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lg.asd995.cn

TS:   // 同上
来源：http://vg.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yk.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tl.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ft.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lh.shxzskj.cn

================================================================================
来源：http://ks.nszjky.cn

G. 面向对象
来源：http://jb.asd995.cn

================================================================================
来源：http://wd.jctech888.com.cn

[G01] 定义类
来源：http://kr.hnjuh.cn

Py:   class User: pass
来源：http://xw.nicolike.cn

PHP:  class User {}
来源：http://dv.bookmarksfly.cn

JS:   class User {}
来源：http://uw.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://db.huixinmuqiang.cn

Java: class User {}
来源：http://jc.szsharing.cn

Go:   type User struct { Name string }
来源：http://zb.huixiangedu.cn

Ruby: class User; end
来源：http://xq.lnxyls.cn

C#:   class User {}
来源：http://cv.521024.cn

[G02] 构造函数
来源：http://cn.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ch.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://tm.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://mz.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://jc.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://jq.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ci.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://wz.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://fg.hnjuh.cn

[G03] 实例属性
来源：http://ta.nszjky.cn

Py:   self.name = "x"
来源：http://in.shxzskj.cn

PHP:  public string $name = "x";
来源：http://ji.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://tf.shtwfgs.cn

TS:   name: string = "x";
来源：http://nt.szsharing.cn

Java: private String name;
来源：http://sd.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bt.asd995.cn

Ruby: @name = "x"
来源：http://nj.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://jm.huanxung.cn

[G04] 定义方法
来源：http://ng.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://kc.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zg.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://yh.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://sk.hahajie.cn

Java: String greet() { return name; }
来源：http://ri.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fb.panjiajie.cn

Ruby: def greet; @name; end
来源：http://dy.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://gv.huanxung.cn

[G05] 继承
来源：http://oz.nicolike.cn

Py:   class Admin(User): pass
来源：http://jg.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://ko.lnxyls.cn

JS:   class Admin extends User {}
来源：http://sh.huanxung.cn

TS:   class Admin extends User {}
来源：http://kr.colortex.cn

Java: class Admin extends User {}
来源：http://tx.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jg.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ki.bjjhwx.cn

C#:   class Admin : User {}
来源：http://xt.jianghongdianzi.cn

[G06] 重写方法
来源：http://pp.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://un.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tx.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://il.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://kb.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://tb.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eb.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://pk.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://sj.szsharing.cn

[G07] 调用父类方法
来源：http://ww.chemitech.net.cn

Py:   super().greet()
来源：http://kk.bookmarksfly.cn

PHP:  parent::greet();
来源：http://ox.newstarts.cn

JS:   super.greet();
来源：http://ki.szsharing.cn

TS:   super.greet();
来源：http://hj.bjjhwx.cn

Java: super.greet();
来源：http://ib.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://im.lnxyls.cn

Ruby: super
来源：http://xj.yuntaijiaju.cn

C#:   base.Greet();
来源：http://zx.hnjuh.cn

[G08] 静态方法与属性
来源：http://vn.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yu.yuexingan06.cn

PHP:  public static function f() {}
来源：http://mk.lnxyls.cn

JS:   static f() {}
来源：http://qy.huanxung.cn

TS:   static f(): void {}
来源：http://rq.gzmigu.cn

Java: static void f() {}
来源：http://mw.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qf.shxzukj.cn

Ruby: def self.f; end
来源：http://cc.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://wa.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://af.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ih.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uq.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mo.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://xn.nicolike.cn

Java: interface Shape { double area(); }
来源：http://yx.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://rd.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://um.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://we.shtwfgs.cn

[G10] 访问控制
来源：http://kt.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://uf.panjiajie.cn

PHP:  public / protected / private
来源：http://cq.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://ce.9csxet.cn

TS:   public / protected / private
来源：http://mz.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://jk.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://re.hahajie.cn

Ruby: public / protected / private
来源：http://oo.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://wf.jianghongdianzi.cn

[G11] getter / setter
来源：http://vx.521024.cn

Py:   @property 与 @x.setter
来源：http://um.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://he.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://cf.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://ca.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://uk.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kr.szsharing.cn

Ruby: attr_accessor :name
来源：http://xl.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://uy.huanxung.cn

[G12] 对象转字符串
来源：http://ua.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://sb.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ip.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://ub.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://da.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://am.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mk.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://cf.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://ku.haigaiapp.cn

[G13] 判断对象类型
来源：http://se.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://se.jctech888.com.cn

PHP:  $u instanceof User
来源：http://mr.szxytkj.cn

JS:   u instanceof User
来源：http://vn.521024.cn

TS:   u instanceof User
来源：http://rh.yuexingan06.cn

Java: u instanceof User
来源：http://ba.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cf.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://wf.newstarts.cn

C#:   u is User
来源：http://ej.jctech888.com.cn


<!-- 参考信息 -->