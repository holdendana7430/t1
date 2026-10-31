代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lr.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://mn.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xj.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hd.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hj.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hv.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hs.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jw.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tz.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mj.asd995.cn

[E16] 数字千分位
来源：http://dq.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://gd.newstarts.cn

PHP:  number_format(1234567);
来源：http://gm.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bb.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tp.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qx.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nm.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vk.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://nc.muxihuayi.cn

[E17] 首字母大写
来源：http://yv.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ok.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ki.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gi.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gy.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rd.szxytkj.cn

Ruby: s.capitalize
来源：http://an.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aj.panjiajie.cn

[E18] 模板占位符替换
来源：http://cs.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mu.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cz.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mx.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tm.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nm.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pz.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vv.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ts.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://wx.huixiangedu.cn

Py:   s.splitlines()
来源：http://ls.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jz.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://fm.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://xx.hahajie.cn

Java: s.lines().toList()
来源：http://id.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://sr.9csxet.cn

Ruby: s.lines
来源：http://yb.szxytkj.cn

C#:   s.Split('\n')
来源：http://mp.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://vt.haigaiapp.cn

Py:   if not s:
来源：http://rm.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xw.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vb.gzmigu.cn

TS:   if (s === "") {}
来源：http://ya.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://qu.colortex.cn

Go:   if s == "" {}
来源：http://re.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://fv.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nd.hnjuh.cn

[E21] 超长截断加省略号
来源：http://uq.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fh.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://td.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bb.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cf.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hr.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://uy.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ra.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vk.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://zk.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gv.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ry.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://my.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vf.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sr.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fo.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://jb.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gp.huanxung.cn

================================================================================
来源：http://hs.gzmigu.cn

F. 文件与目录
来源：http://vs.jianghongdianzi.cn

================================================================================
来源：http://wb.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://bj.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sr.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://aj.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xn.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nc.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gx.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dm.521024.cn

Ruby: File.read("a.txt")
来源：http://me.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://mu.muxihuayi.cn

[F02] 逐行读取文件
来源：http://zj.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zk.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ua.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cu.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jw.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ju.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kb.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gz.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sd.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://pb.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dl.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cg.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kt.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ms.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xh.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nh.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://fq.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hr.asd995.cn

[F04] 追加写入文件
来源：http://oq.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dv.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sp.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mm.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kk.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lw.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ck.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pf.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vr.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://rw.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pj.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://li.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://uf.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://sl.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pr.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qr.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://pe.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://ft.haigaiapp.cn

[F06] 删除文件
来源：http://ol.huanxung.cn

Py:   os.remove("a.txt")
来源：http://qd.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ze.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ap.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://od.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xh.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://yl.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://qc.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://hj.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ue.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sl.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://py.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://no.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wn.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ze.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ro.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://os.hnjuh.cn

[F08] 遍历目录
来源：http://yg.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qj.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ml.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://yl.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://nv.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kd.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mp.asd995.cn

Ruby: Dir.children("dir")
来源：http://az.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://dt.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://np.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://ft.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://up.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://lf.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://co.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dv.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oh.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://qd.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://hd.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://hc.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aw.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xn.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ti.nicolike.cn

TS:   path.extname("a.txt")
来源：http://el.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://es.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ex.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://og.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://or.huixiangedu.cn

[F11] 复制与移动文件
来源：http://qs.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mn.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ti.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ud.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lc.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bg.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ft.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ox.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qn.shxzukj.cn

[F12] CSV 读写
来源：http://ll.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cs.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qj.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yq.jianghongdianzi.cn

TS:   // 同上
来源：http://tg.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://st.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ol.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ov.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mo.huixinmuqiang.cn

================================================================================
来源：http://ow.szsharing.cn

G. 面向对象
来源：http://qd.shxzukj.cn

================================================================================
来源：http://dn.yuexingan06.cn

[G01] 定义类
来源：http://lj.muxihuayi.cn

Py:   class User: pass
来源：http://ns.newstarts.cn

PHP:  class User {}
来源：http://bz.jctech888.com.cn

JS:   class User {}
来源：http://bq.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ku.newstarts.cn

Java: class User {}
来源：http://te.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://om.hnjuh.cn

Ruby: class User; end
来源：http://ye.muxihuayi.cn

C#:   class User {}
来源：http://io.shxzskj.cn

[G02] 构造函数
来源：http://qh.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://sb.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://nw.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://ey.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://wx.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://af.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vt.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qz.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://fy.huanxung.cn

[G03] 实例属性
来源：http://tx.shxzukj.cn

Py:   self.name = "x"
来源：http://qk.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://gr.asd995.cn

JS:   this.name = "x";
来源：http://ac.szsharing.cn

TS:   name: string = "x";
来源：http://sn.jctech888.com.cn

Java: private String name;
来源：http://fw.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ir.bookmarksfly.cn

Ruby: @name = "x"
来源：http://mn.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://qu.hahajie.cn

[G04] 定义方法
来源：http://wg.9csxet.cn

Py:   def greet(self): return self.name
来源：http://wn.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tm.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://vm.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://tz.521024.cn

Java: String greet() { return name; }
来源：http://am.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wm.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://sq.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://wn.muxihuayi.cn

[G05] 继承
来源：http://yy.shxzukj.cn

Py:   class Admin(User): pass
来源：http://gi.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://rz.colortex.cn

JS:   class Admin extends User {}
来源：http://nq.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://qw.shxzskj.cn

Java: class Admin extends User {}
来源：http://ne.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pi.panjiajie.cn

Ruby: class Admin < User; end
来源：http://hm.shxzskj.cn

C#:   class Admin : User {}
来源：http://vq.huixiangedu.cn

[G06] 重写方法
来源：http://vc.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://pt.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fa.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://hm.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://vx.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://dx.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ki.asd995.cn

Ruby: def greet; "admin"; end
来源：http://hp.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://dx.huanxung.cn

[G07] 调用父类方法
来源：http://rn.muxihuayi.cn

Py:   super().greet()
来源：http://wi.asd995.cn

PHP:  parent::greet();
来源：http://af.yuntaijiaju.cn

JS:   super.greet();
来源：http://bk.panjiajie.cn

TS:   super.greet();
来源：http://is.szxytkj.cn

Java: super.greet();
来源：http://bo.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ca.9csxet.cn

Ruby: super
来源：http://dm.szsharing.cn

C#:   base.Greet();
来源：http://ln.yuexingan06.cn

[G08] 静态方法与属性
来源：http://mz.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oo.nszjky.cn

PHP:  public static function f() {}
来源：http://ns.colortex.cn

JS:   static f() {}
来源：http://da.shxzukj.cn

TS:   static f(): void {}
来源：http://cq.gzmigu.cn

Java: static void f() {}
来源：http://hc.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://my.huanxung.cn

Ruby: def self.f; end
来源：http://em.haigaiapp.cn

C#:   public static void F() {}
来源：http://gg.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://ln.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ts.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ks.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zk.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://ik.hahajie.cn

Java: interface Shape { double area(); }
来源：http://gy.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://pn.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fh.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://xk.szxytkj.cn

[G10] 访问控制
来源：http://iv.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://yv.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://lb.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://ko.jianghongdianzi.cn

TS:   public / protected / private
来源：http://jn.521024.cn

Java: public / protected / private / 默认包级
来源：http://ap.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tq.521024.cn

Ruby: public / protected / private
来源：http://se.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://cm.gzmigu.cn

[G11] getter / setter
来源：http://xs.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://io.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sj.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://xa.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://ls.nszjky.cn

Java: public String getName() { return name; }
来源：http://zs.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tr.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://zr.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://mb.jctech888.com.cn

[G12] 对象转字符串
来源：http://bu.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://rp.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wf.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://xv.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://iq.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://jl.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://df.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://cj.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://kd.nszjky.cn

[G13] 判断对象类型
来源：http://fg.shxzskj.cn

Py:   isinstance(u, User)
来源：http://uo.muxihuayi.cn

PHP:  $u instanceof User
来源：http://sj.yuntaijiaju.cn

JS:   u instanceof User
来源：http://nn.9csxet.cn

TS:   u instanceof User
来源：http://jz.bookmarksfly.cn


<!-- 参考信息 -->