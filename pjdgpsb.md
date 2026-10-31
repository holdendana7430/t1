代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vm.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uf.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cr.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uo.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dc.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://es.shxzskj.cn

[E16] 数字千分位
来源：http://sz.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://zw.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://lw.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mj.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gf.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tx.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jj.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ym.asd995.cn

C#:   1234567.ToString("N0")
来源：http://kh.hahajie.cn

[E17] 首字母大写
来源：http://db.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lb.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xh.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kq.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pt.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kb.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hf.shxzukj.cn

Ruby: s.capitalize
来源：http://ry.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ff.hahajie.cn

[E18] 模板占位符替换
来源：http://so.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ir.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ig.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zk.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xm.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ut.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eo.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uk.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://ry.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://jl.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://et.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://rg.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://mh.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://rm.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://qf.haigaiapp.cn

Ruby: s.lines
来源：http://dx.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://ec.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://hk.nszjky.cn

Py:   if not s:
来源：http://pw.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nr.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ba.huixiangedu.cn

TS:   if (s === "") {}
来源：http://ri.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://tq.shtwfgs.cn

Go:   if s == "" {}
来源：http://df.huixiangedu.cn

Ruby: if s.empty?
来源：http://ap.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vn.9csxet.cn

[E21] 超长截断加省略号
来源：http://id.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gg.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vg.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vn.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cw.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://rg.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uu.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ba.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ey.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rq.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ex.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kx.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hs.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sr.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sp.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://if.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tp.bookmarksfly.cn

================================================================================
来源：http://cg.colortex.cn

F. 文件与目录
来源：http://jh.bjjhwx.cn

================================================================================
来源：http://wb.hahajie.cn

[F01] 读取整个文件
来源：http://ag.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vu.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://ma.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://td.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://re.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kh.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wb.nszjky.cn

Ruby: File.read("a.txt")
来源：http://jp.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://tn.lnxyls.cn

[F02] 逐行读取文件
来源：http://mb.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qn.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sl.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://be.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bg.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fb.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vl.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gh.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dm.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://hm.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oo.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rj.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ql.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lx.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ia.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bt.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://od.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ne.521024.cn

[F04] 追加写入文件
来源：http://tp.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lh.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://st.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oc.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oc.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kr.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://so.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ph.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://av.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://cc.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ex.colortex.cn

PHP:  file_exists("a.txt");
来源：http://rh.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://ci.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://wv.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ym.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yo.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://yr.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://bq.shtwfgs.cn

[F06] 删除文件
来源：http://ir.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://aj.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://br.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cp.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rh.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cc.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://rt.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://xd.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ke.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://uf.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gh.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ms.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cc.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sc.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dl.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zw.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ib.hahajie.cn

[F08] 遍历目录
来源：http://gr.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fh.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iv.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://up.521024.cn

TS:   fs.readdirSync("dir")
来源：http://wd.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zh.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oa.9csxet.cn

Ruby: Dir.children("dir")
来源：http://he.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://hw.nicolike.cn

[F09] 获取文件大小
来源：http://ru.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://wo.huanxung.cn

PHP:  filesize("a.txt");
来源：http://vr.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://vg.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://lz.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qd.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tg.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://ah.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://aj.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ol.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jq.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vk.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://to.huanxung.cn

TS:   path.extname("a.txt")
来源：http://qm.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qx.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dk.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kn.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jv.9csxet.cn

[F11] 复制与移动文件
来源：http://bi.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xa.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yn.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aj.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://na.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ph.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nl.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gl.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nc.huixiangedu.cn

[F12] CSV 读写
来源：http://kk.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://if.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ny.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ow.colortex.cn

TS:   // 同上
来源：http://mh.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ig.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ty.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zj.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qr.wgjwhj.cn

================================================================================
来源：http://rf.yuexingan06.cn

G. 面向对象
来源：http://er.asd995.cn

================================================================================
来源：http://pq.9csxet.cn

[G01] 定义类
来源：http://sz.nicolike.cn

Py:   class User: pass
来源：http://ow.huixiangedu.cn

PHP:  class User {}
来源：http://no.chemitech.net.cn

JS:   class User {}
来源：http://nz.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://ya.shxzukj.cn

Java: class User {}
来源：http://gz.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://ih.bjjhwx.cn

Ruby: class User; end
来源：http://zg.shxzskj.cn

C#:   class User {}
来源：http://od.huanxung.cn

[G02] 构造函数
来源：http://cv.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://iw.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://mk.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://fa.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://mf.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://kl.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ip.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://lq.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://vd.yuntaijiaju.cn

[G03] 实例属性
来源：http://in.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://sp.colortex.cn

PHP:  public string $name = "x";
来源：http://jb.jctech888.com.cn

JS:   this.name = "x";
来源：http://ko.shtwfgs.cn

TS:   name: string = "x";
来源：http://qc.nicolike.cn

Java: private String name;
来源：http://jd.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://bs.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cp.muxihuayi.cn

[G04] 定义方法
来源：http://jh.szsharing.cn

Py:   def greet(self): return self.name
来源：http://ib.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cg.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://yq.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://zr.shtwfgs.cn

Java: String greet() { return name; }
来源：http://rc.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aj.gzmigu.cn

Ruby: def greet; @name; end
来源：http://cz.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://xq.hahajie.cn

[G05] 继承
来源：http://sq.newstarts.cn

Py:   class Admin(User): pass
来源：http://lr.nszjky.cn

PHP:  class Admin extends User {}
来源：http://zw.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://jn.hnjuh.cn

TS:   class Admin extends User {}
来源：http://pu.gzmigu.cn

Java: class Admin extends User {}
来源：http://lr.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vb.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://bi.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://qg.nszjky.cn

[G06] 重写方法
来源：http://pi.521024.cn

Py:   def greet(self): return "admin"
来源：http://iv.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ck.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://oy.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://fi.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://qk.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rr.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://mc.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://zi.bjjhwx.cn

[G07] 调用父类方法
来源：http://ho.shxzukj.cn

Py:   super().greet()
来源：http://xm.colortex.cn

PHP:  parent::greet();
来源：http://jq.wgjwhj.cn

JS:   super.greet();
来源：http://fi.jianghongdianzi.cn

TS:   super.greet();
来源：http://do.521024.cn

Java: super.greet();
来源：http://hz.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nk.521024.cn

Ruby: super
来源：http://hb.panjiajie.cn

C#:   base.Greet();
来源：http://ys.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://rf.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ub.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://jg.nicolike.cn

JS:   static f() {}
来源：http://rh.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ig.chemitech.net.cn

Java: static void f() {}
来源：http://ds.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ca.huixiangedu.cn

Ruby: def self.f; end
来源：http://lm.9csxet.cn

C#:   public static void F() {}
来源：http://jy.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://qs.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://kx.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zo.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ar.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://lm.hahajie.cn

Java: interface Shape { double area(); }
来源：http://qc.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://kj.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://za.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://bg.asd995.cn

[G10] 访问控制
来源：http://ej.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://tw.jctech888.com.cn

PHP:  public / protected / private
来源：http://yn.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://dn.huanxung.cn

TS:   public / protected / private
来源：http://ok.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://iz.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bx.shtwfgs.cn

Ruby: public / protected / private
来源：http://cp.panjiajie.cn

C#:   public / protected / private / internal
来源：http://in.jctech888.com.cn

[G11] getter / setter
来源：http://ql.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://xg.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pj.huanxung.cn

JS:   get name() { return this._name; }
来源：http://vq.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ja.nicolike.cn

Java: public String getName() { return name; }
来源：http://jy.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fp.521024.cn

Ruby: attr_accessor :name
来源：http://co.9csxet.cn

C#:   public string Name { get; set; }
来源：http://ph.yuexingan06.cn

[G12] 对象转字符串
来源：http://bk.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://op.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qt.521024.cn

JS:   toString() { return this.name; }
来源：http://di.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://vn.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://yi.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yk.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://gi.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://le.wgjwhj.cn

[G13] 判断对象类型
来源：http://xr.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://km.nszjky.cn

PHP:  $u instanceof User
来源：http://ec.huanxung.cn

JS:   u instanceof User
来源：http://wa.chemitech.net.cn

TS:   u instanceof User
来源：http://fl.yuntaijiaju.cn

Java: u instanceof User
来源：http://wz.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dr.521024.cn

Ruby: u.is_a?(User)
来源：http://qy.bjjhwx.cn

C#:   u is User
来源：http://vp.szxytkj.cn


<!-- 参考信息 -->