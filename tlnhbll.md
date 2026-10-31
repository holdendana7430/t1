代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mm.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://xx.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yn.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xa.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ce.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xt.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://em.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tf.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dn.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fy.szxytkj.cn

[E16] 数字千分位
来源：http://fu.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://ci.panjiajie.cn

PHP:  number_format(1234567);
来源：http://sc.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dp.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uz.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ih.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rh.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://at.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://ih.lnxyls.cn

[E17] 首字母大写
来源：http://pt.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pz.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bi.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gx.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bj.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rq.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qr.521024.cn

Ruby: s.capitalize
来源：http://fd.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ne.shtwfgs.cn

[E18] 模板占位符替换
来源：http://xx.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sw.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rn.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hj.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fd.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zs.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kb.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vs.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fz.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://av.wgjwhj.cn

Py:   s.splitlines()
来源：http://jd.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zx.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://hg.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://eg.muxihuayi.cn

Java: s.lines().toList()
来源：http://vv.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://us.szsharing.cn

Ruby: s.lines
来源：http://ov.muxihuayi.cn

C#:   s.Split('\n')
来源：http://gy.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://dk.yuexingan06.cn

Py:   if not s:
来源：http://ex.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://us.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gz.wgjwhj.cn

TS:   if (s === "") {}
来源：http://cu.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://ji.bookmarksfly.cn

Go:   if s == "" {}
来源：http://qd.nicolike.cn

Ruby: if s.empty?
来源：http://zv.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jq.panjiajie.cn

[E21] 超长截断加省略号
来源：http://sx.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sx.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hr.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://di.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lk.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://fe.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bx.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yj.colortex.cn

[E22] 字节长度与字符长度
来源：http://ze.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ao.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pc.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://md.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qn.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ca.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bp.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://gs.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fq.shtwfgs.cn

================================================================================
来源：http://pu.nicolike.cn

F. 文件与目录
来源：http://tm.newstarts.cn

================================================================================
来源：http://pv.panjiajie.cn

[F01] 读取整个文件
来源：http://re.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lm.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://af.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eu.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://po.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vv.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dp.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://vm.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ew.szxytkj.cn

[F02] 逐行读取文件
来源：http://ij.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uz.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jo.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gi.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://st.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ua.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yw.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gd.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bt.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://qz.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ui.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rp.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cn.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://li.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qv.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://im.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://wr.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dl.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ng.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qb.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fv.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jm.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qp.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://la.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ij.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ej.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qb.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://ql.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uj.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://rt.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ll.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://al.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gt.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lz.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://br.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://se.yuexingan06.cn

[F06] 删除文件
来源：http://lr.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://rz.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://pd.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fg.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vg.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://np.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://re.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://tb.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://bz.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://ur.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uj.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pi.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mq.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cq.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ud.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yz.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://au.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jy.huanxung.cn

[F08] 遍历目录
来源：http://db.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vp.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dr.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://yv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://ac.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ym.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pc.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://ro.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wd.jctech888.com.cn

[F09] 获取文件大小
来源：http://hw.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ub.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://wm.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ac.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://xz.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hp.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lt.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://gf.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://qu.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://mt.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://it.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jt.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sz.nicolike.cn

TS:   path.extname("a.txt")
来源：http://sw.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sd.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://il.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jg.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hg.nicolike.cn

[F11] 复制与移动文件
来源：http://sy.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://os.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uf.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nz.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://of.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ts.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cb.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ku.hahajie.cn

[F12] CSV 读写
来源：http://om.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bk.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xg.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fo.yuntaijiaju.cn

TS:   // 同上
来源：http://ah.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bu.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xw.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zv.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ky.9csxet.cn

================================================================================
来源：http://sv.nicolike.cn

G. 面向对象
来源：http://hq.hnjuh.cn

================================================================================
来源：http://pt.521024.cn

[G01] 定义类
来源：http://cs.colortex.cn

Py:   class User: pass
来源：http://au.hnjuh.cn

PHP:  class User {}
来源：http://dr.9csxet.cn

JS:   class User {}
来源：http://kv.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://bp.hahajie.cn

Java: class User {}
来源：http://hn.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://pd.yuntaijiaju.cn

Ruby: class User; end
来源：http://ap.muxihuayi.cn

C#:   class User {}
来源：http://sb.nszjky.cn

[G02] 构造函数
来源：http://gi.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://bh.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://gk.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ml.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://jx.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://lz.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zm.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jg.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://yp.521024.cn

[G03] 实例属性
来源：http://bj.muxihuayi.cn

Py:   self.name = "x"
来源：http://rv.panjiajie.cn

PHP:  public string $name = "x";
来源：http://zj.shxzskj.cn

JS:   this.name = "x";
来源：http://ku.panjiajie.cn

TS:   name: string = "x";
来源：http://ge.gzmigu.cn

Java: private String name;
来源：http://aa.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xi.shtwfgs.cn

Ruby: @name = "x"
来源：http://ss.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://us.bookmarksfly.cn

[G04] 定义方法
来源：http://yq.asd995.cn

Py:   def greet(self): return self.name
来源：http://er.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ii.szsharing.cn

JS:   greet() { return this.name; }
来源：http://hw.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://la.szsharing.cn

Java: String greet() { return name; }
来源：http://tn.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://us.nszjky.cn

Ruby: def greet; @name; end
来源：http://xs.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ob.gzmigu.cn

[G05] 继承
来源：http://pg.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://op.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://sd.shxzskj.cn

JS:   class Admin extends User {}
来源：http://zk.shxzukj.cn

TS:   class Admin extends User {}
来源：http://ze.yuexingan06.cn

Java: class Admin extends User {}
来源：http://uz.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mo.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://kz.hnjuh.cn

C#:   class Admin : User {}
来源：http://ed.yuntaijiaju.cn

[G06] 重写方法
来源：http://fe.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://cn.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qz.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://jo.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://se.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://gm.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ec.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://sx.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://la.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://xo.wgjwhj.cn

Py:   super().greet()
来源：http://bu.szxytkj.cn

PHP:  parent::greet();
来源：http://uy.asd995.cn

JS:   super.greet();
来源：http://to.yuntaijiaju.cn

TS:   super.greet();
来源：http://tp.gzmigu.cn

Java: super.greet();
来源：http://dk.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tg.asd995.cn

Ruby: super
来源：http://ka.gzmigu.cn

C#:   base.Greet();
来源：http://aa.nicolike.cn

[G08] 静态方法与属性
来源：http://vc.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vf.shxzskj.cn

PHP:  public static function f() {}
来源：http://bv.521024.cn

JS:   static f() {}
来源：http://ke.jctech888.com.cn

TS:   static f(): void {}
来源：http://gv.9csxet.cn

Java: static void f() {}
来源：http://ij.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cv.shxzskj.cn

Ruby: def self.f; end
来源：http://nc.shtwfgs.cn

C#:   public static void F() {}
来源：http://wv.szsharing.cn

[G09] 接口 / 抽象类
来源：http://oa.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://qe.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://au.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kr.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://xa.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://ci.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://lm.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://de.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://kx.yuexingan06.cn

[G10] 访问控制
来源：http://eo.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://gk.bjjhwx.cn

PHP:  public / protected / private
来源：http://mo.9csxet.cn

JS:   #private 字段；其余公开
来源：http://zk.jianghongdianzi.cn

TS:   public / protected / private
来源：http://qh.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://mo.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tk.wgjwhj.cn

Ruby: public / protected / private
来源：http://cu.colortex.cn

C#:   public / protected / private / internal
来源：http://vw.hnjuh.cn

[G11] getter / setter
来源：http://nw.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://eq.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bm.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://kj.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://vb.nicolike.cn

Java: public String getName() { return name; }
来源：http://rh.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://el.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://we.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://zs.yuexingan06.cn

[G12] 对象转字符串
来源：http://nm.521024.cn

Py:   def __str__(self): return self.name
来源：http://zz.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bw.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://ms.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ch.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://pg.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kc.colortex.cn

Ruby: def to_s; @name; end
来源：http://nl.colortex.cn

C#:   public override string ToString() => Name;
来源：http://qm.chemitech.net.cn

[G13] 判断对象类型
来源：http://jm.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://cj.521024.cn

PHP:  $u instanceof User
来源：http://fm.bjjhwx.cn

JS:   u instanceof User
来源：http://qj.wgjwhj.cn

TS:   u instanceof User
来源：http://aj.asd995.cn


<!-- 参考信息 -->