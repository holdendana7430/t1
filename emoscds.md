代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nd.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://el.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ah.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ra.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://of.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ji.haigaiapp.cn

[E16] 数字千分位
来源：http://eq.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://gq.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://jx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cc.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sp.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sl.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ec.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kz.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://gv.newstarts.cn

[E17] 首字母大写
来源：http://ge.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yt.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ld.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tt.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vo.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vr.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://et.shxzukj.cn

Ruby: s.capitalize
来源：http://ys.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iv.hahajie.cn

[E18] 模板占位符替换
来源：http://gk.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ar.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tl.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uo.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vq.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nc.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qj.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ge.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ty.521024.cn

[E19] 多行文本按行拆分
来源：http://av.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://gr.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://to.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ex.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://ra.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://iv.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://on.panjiajie.cn

Ruby: s.lines
来源：http://mw.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://rd.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://je.bjjhwx.cn

Py:   if not s:
来源：http://qk.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hy.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oc.haigaiapp.cn

TS:   if (s === "") {}
来源：http://jp.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://lx.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://ev.bjjhwx.cn

Ruby: if s.empty?
来源：http://ll.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zy.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://kp.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ks.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ld.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pj.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iw.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://br.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://mc.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://co.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hl.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://it.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iw.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://js.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ov.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dm.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zf.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jt.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://yc.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xy.nicolike.cn

================================================================================
来源：http://pg.muxihuayi.cn

F. 文件与目录
来源：http://rh.chemitech.net.cn

================================================================================
来源：http://uo.bookmarksfly.cn

[F01] 读取整个文件
来源：http://re.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xm.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://qy.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bk.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vv.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vf.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fk.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://xm.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://qu.nicolike.cn

[F02] 逐行读取文件
来源：http://vb.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ik.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jp.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mp.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fj.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ud.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gn.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dt.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://uj.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gt.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://un.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qv.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ga.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rb.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xi.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://oz.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ro.shxzskj.cn

[F04] 追加写入文件
来源：http://mn.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cx.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hm.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cn.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kp.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jg.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lf.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ch.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ce.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://qd.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ua.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://gu.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ij.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://rx.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xm.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jx.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://qp.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://fv.bookmarksfly.cn

[F06] 删除文件
来源：http://dn.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://px.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://cq.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xs.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sz.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rj.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://jj.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ox.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://iv.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://wo.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://et.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://br.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fc.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zg.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://if.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qt.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wl.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nz.shxzukj.cn

[F08] 遍历目录
来源：http://ot.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nz.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nj.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://sz.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ra.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rf.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ku.521024.cn

Ruby: Dir.children("dir")
来源：http://ky.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://bj.shxzukj.cn

[F09] 获取文件大小
来源：http://qj.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://iv.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://zn.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://os.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://xf.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ku.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lx.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://zk.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://bc.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://yr.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ka.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hw.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jq.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://rr.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ha.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nm.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vp.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yd.panjiajie.cn

[F11] 复制与移动文件
来源：http://sq.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ga.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xw.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ja.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fn.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qy.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iy.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yp.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fu.haigaiapp.cn

[F12] CSV 读写
来源：http://tv.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cc.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yx.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tn.9csxet.cn

TS:   // 同上
来源：http://ai.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jn.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wo.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uv.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.521024.cn

================================================================================
来源：http://wd.gzmigu.cn

G. 面向对象
来源：http://ls.9csxet.cn

================================================================================
来源：http://ig.haigaiapp.cn

[G01] 定义类
来源：http://iv.huixinmuqiang.cn

Py:   class User: pass
来源：http://sv.szxytkj.cn

PHP:  class User {}
来源：http://vj.521024.cn

JS:   class User {}
来源：http://mz.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://vr.521024.cn

Java: class User {}
来源：http://nd.hahajie.cn

Go:   type User struct { Name string }
来源：http://hf.huanxung.cn

Ruby: class User; end
来源：http://ur.chemitech.net.cn

C#:   class User {}
来源：http://rb.lnxyls.cn

[G02] 构造函数
来源：http://yv.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://yb.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ey.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ml.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://xp.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://si.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rd.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://uc.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://mx.wgjwhj.cn

[G03] 实例属性
来源：http://ve.colortex.cn

Py:   self.name = "x"
来源：http://gu.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://yi.gzmigu.cn

JS:   this.name = "x";
来源：http://vb.muxihuayi.cn

TS:   name: string = "x";
来源：http://yq.bjjhwx.cn

Java: private String name;
来源：http://bm.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oe.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://kx.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://qv.yuntaijiaju.cn

[G04] 定义方法
来源：http://oa.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ze.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ju.nicolike.cn

JS:   greet() { return this.name; }
来源：http://xg.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://ws.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ru.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cu.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://qm.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://rs.shxzskj.cn

[G05] 继承
来源：http://ac.shxzukj.cn

Py:   class Admin(User): pass
来源：http://bh.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://qm.hnjuh.cn

JS:   class Admin extends User {}
来源：http://fl.szxytkj.cn

TS:   class Admin extends User {}
来源：http://ug.jctech888.com.cn

Java: class Admin extends User {}
来源：http://if.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pe.newstarts.cn

Ruby: class Admin < User; end
来源：http://lz.newstarts.cn

C#:   class Admin : User {}
来源：http://nr.haigaiapp.cn

[G06] 重写方法
来源：http://mb.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ty.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oq.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://hu.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://os.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://cj.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wi.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://je.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://am.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://mk.huixiangedu.cn

Py:   super().greet()
来源：http://aj.hnjuh.cn

PHP:  parent::greet();
来源：http://es.yuntaijiaju.cn

JS:   super.greet();
来源：http://sl.jctech888.com.cn

TS:   super.greet();
来源：http://mp.wgjwhj.cn

Java: super.greet();
来源：http://dw.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ar.9csxet.cn

Ruby: super
来源：http://vl.asd995.cn

C#:   base.Greet();
来源：http://ur.shxzukj.cn

[G08] 静态方法与属性
来源：http://hm.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xv.asd995.cn

PHP:  public static function f() {}
来源：http://xx.newstarts.cn

JS:   static f() {}
来源：http://ek.muxihuayi.cn

TS:   static f(): void {}
来源：http://gy.bjjhwx.cn

Java: static void f() {}
来源：http://dw.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ps.521024.cn

Ruby: def self.f; end
来源：http://hk.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://yu.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://vl.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://yw.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jr.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dd.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ic.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://th.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://vp.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ir.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://wb.muxihuayi.cn

[G10] 访问控制
来源：http://kj.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://cm.szxytkj.cn

PHP:  public / protected / private
来源：http://zd.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://tk.9csxet.cn

TS:   public / protected / private
来源：http://eb.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://su.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mw.panjiajie.cn

Ruby: public / protected / private
来源：http://us.nicolike.cn

C#:   public / protected / private / internal
来源：http://pl.muxihuayi.cn

[G11] getter / setter
来源：http://ga.newstarts.cn

Py:   @property 与 @x.setter
来源：http://bg.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.521024.cn

JS:   get name() { return this._name; }
来源：http://vz.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://le.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://gy.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dw.newstarts.cn

Ruby: attr_accessor :name
来源：http://wt.szsharing.cn

C#:   public string Name { get; set; }
来源：http://ly.wgjwhj.cn

[G12] 对象转字符串
来源：http://tr.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://qy.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ur.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://va.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://dw.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://qp.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://do.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ub.521024.cn

C#:   public override string ToString() => Name;
来源：http://wo.hnjuh.cn

[G13] 判断对象类型
来源：http://xx.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ba.haigaiapp.cn

PHP:  $u instanceof User
来源：http://pv.521024.cn

JS:   u instanceof User
来源：http://pg.muxihuayi.cn

TS:   u instanceof User
来源：http://zu.chemitech.net.cn

Java: u instanceof User
来源：http://in.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vx.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://kh.9csxet.cn

C#:   u is User
来源：http://bh.9csxet.cn


<!-- 参考信息 -->