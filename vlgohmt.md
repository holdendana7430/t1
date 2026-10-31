代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pu.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pv.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cd.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iz.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wi.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ih.shtwfgs.cn

[E16] 数字千分位
来源：http://go.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://tt.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ry.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mo.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oa.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xd.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yi.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rg.asd995.cn

C#:   1234567.ToString("N0")
来源：http://pt.shxzukj.cn

[E17] 首字母大写
来源：http://lo.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iy.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nj.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mx.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ew.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ds.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://he.bookmarksfly.cn

Ruby: s.capitalize
来源：http://no.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ap.shxzskj.cn

[E18] 模板占位符替换
来源：http://dk.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yi.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nj.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fy.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://he.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nh.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zj.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jo.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jd.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ug.colortex.cn

Py:   s.splitlines()
来源：http://vq.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xx.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ov.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://sw.szxytkj.cn

Java: s.lines().toList()
来源：http://tp.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://hv.9csxet.cn

Ruby: s.lines
来源：http://nb.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://jw.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://xi.huixiangedu.cn

Py:   if not s:
来源：http://wh.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kw.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jq.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://sd.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://fi.panjiajie.cn

Go:   if s == "" {}
来源：http://gh.newstarts.cn

Ruby: if s.empty?
来源：http://zq.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xj.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://wu.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kf.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vh.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bo.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://um.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ax.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://jt.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bj.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qj.9csxet.cn

[E22] 字节长度与字符长度
来源：http://xq.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qz.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://si.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ds.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lf.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ho.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vk.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://uf.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ob.yuexingan06.cn

================================================================================
来源：http://fe.huixiangedu.cn

F. 文件与目录
来源：http://fv.huixiangedu.cn

================================================================================
来源：http://ic.shxzukj.cn

[F01] 读取整个文件
来源：http://pc.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kb.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://zf.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bg.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rf.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ls.colortex.cn

Ruby: File.read("a.txt")
来源：http://aj.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://ro.colortex.cn

[F02] 逐行读取文件
来源：http://dn.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ir.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://av.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kz.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ra.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jg.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sm.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mq.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://st.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://fr.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hx.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rg.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iw.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://om.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ry.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ap.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://kf.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wu.asd995.cn

[F04] 追加写入文件
来源：http://qp.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mf.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gw.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nv.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wt.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qi.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fx.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ig.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wb.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ei.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fg.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://yj.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://mm.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://ff.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gl.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://to.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://pv.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://yp.colortex.cn

[F06] 删除文件
来源：http://so.asd995.cn

Py:   os.remove("a.txt")
来源：http://dz.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://oq.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bw.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uy.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uc.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://iz.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ku.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://da.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ii.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kn.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dn.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dl.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cq.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ym.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ef.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vg.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yg.jianghongdianzi.cn

[F08] 遍历目录
来源：http://gl.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xj.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://my.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://qi.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://wj.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wn.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zd.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://jc.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ls.asd995.cn

[F09] 获取文件大小
来源：http://ee.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://la.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://dr.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://qc.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://bs.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jp.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sx.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ko.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://av.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://ol.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kk.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jh.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tz.9csxet.cn

TS:   path.extname("a.txt")
来源：http://eb.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gj.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ta.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ls.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zu.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://gd.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fb.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fm.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ko.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://so.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ww.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://br.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ht.szsharing.cn

[F12] CSV 读写
来源：http://lm.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ms.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nc.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zy.asd995.cn

TS:   // 同上
来源：http://vh.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jl.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://da.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://em.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jj.szsharing.cn

================================================================================
来源：http://fy.wgjwhj.cn

G. 面向对象
来源：http://yz.panjiajie.cn

================================================================================
来源：http://bw.bjjhwx.cn

[G01] 定义类
来源：http://ne.nicolike.cn

Py:   class User: pass
来源：http://pr.panjiajie.cn

PHP:  class User {}
来源：http://rw.gzmigu.cn

JS:   class User {}
来源：http://np.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://lh.gzmigu.cn

Java: class User {}
来源：http://yf.hnjuh.cn

Go:   type User struct { Name string }
来源：http://kb.panjiajie.cn

Ruby: class User; end
来源：http://fq.jianghongdianzi.cn

C#:   class User {}
来源：http://vh.newstarts.cn

[G02] 构造函数
来源：http://qb.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://wm.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://bt.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://py.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://mi.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ul.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oh.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://wk.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://iy.szsharing.cn

[G03] 实例属性
来源：http://si.gzmigu.cn

Py:   self.name = "x"
来源：http://fe.lnxyls.cn

PHP:  public string $name = "x";
来源：http://db.shxzukj.cn

JS:   this.name = "x";
来源：http://mi.huixiangedu.cn

TS:   name: string = "x";
来源：http://il.muxihuayi.cn

Java: private String name;
来源：http://zt.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eg.colortex.cn

Ruby: @name = "x"
来源：http://nx.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ji.muxihuayi.cn

[G04] 定义方法
来源：http://pv.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://qd.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fn.szsharing.cn

JS:   greet() { return this.name; }
来源：http://re.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://li.huanxung.cn

Java: String greet() { return name; }
来源：http://ct.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://it.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://ni.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://jt.shxzukj.cn

[G05] 继承
来源：http://po.asd995.cn

Py:   class Admin(User): pass
来源：http://ts.nszjky.cn

PHP:  class Admin extends User {}
来源：http://re.521024.cn

JS:   class Admin extends User {}
来源：http://tu.nszjky.cn

TS:   class Admin extends User {}
来源：http://nm.szsharing.cn

Java: class Admin extends User {}
来源：http://dq.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fv.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://oy.nszjky.cn

C#:   class Admin : User {}
来源：http://fb.yuntaijiaju.cn

[G06] 重写方法
来源：http://lf.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ja.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jl.asd995.cn

JS:   greet() { return "admin"; }
来源：http://ut.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://iu.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://ux.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vx.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ak.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://zr.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://aw.haigaiapp.cn

Py:   super().greet()
来源：http://bg.chemitech.net.cn

PHP:  parent::greet();
来源：http://mx.bjjhwx.cn

JS:   super.greet();
来源：http://kn.yuntaijiaju.cn

TS:   super.greet();
来源：http://dg.huanxung.cn

Java: super.greet();
来源：http://mz.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ea.huixinmuqiang.cn

Ruby: super
来源：http://sk.haigaiapp.cn

C#:   base.Greet();
来源：http://lj.gzmigu.cn

[G08] 静态方法与属性
来源：http://ck.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bv.bjjhwx.cn

PHP:  public static function f() {}
来源：http://ts.9csxet.cn

JS:   static f() {}
来源：http://wx.yuexingan06.cn

TS:   static f(): void {}
来源：http://um.521024.cn

Java: static void f() {}
来源：http://gc.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cd.szsharing.cn

Ruby: def self.f; end
来源：http://lu.nszjky.cn

C#:   public static void F() {}
来源：http://nx.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://di.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://hx.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uc.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://md.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://jw.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://hv.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://yy.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gn.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://ji.muxihuayi.cn

[G10] 访问控制
来源：http://wf.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://jf.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://eq.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://sj.nicolike.cn

TS:   public / protected / private
来源：http://da.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://oe.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lk.shtwfgs.cn

Ruby: public / protected / private
来源：http://wn.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ie.521024.cn

[G11] getter / setter
来源：http://sg.nicolike.cn

Py:   @property 与 @x.setter
来源：http://bl.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wf.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://sy.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://lb.nicolike.cn

Java: public String getName() { return name; }
来源：http://cs.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ed.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://bv.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://px.asd995.cn

[G12] 对象转字符串
来源：http://li.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://kl.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fu.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://dq.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://mt.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://wk.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://la.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://tp.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://dq.asd995.cn

[G13] 判断对象类型
来源：http://th.gzmigu.cn

Py:   isinstance(u, User)
来源：http://ja.bjjhwx.cn

PHP:  $u instanceof User
来源：http://fz.521024.cn

JS:   u instanceof User
来源：http://mo.wgjwhj.cn

TS:   u instanceof User
来源：http://kc.asd995.cn

Java: u instanceof User
来源：http://al.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gx.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://kb.bookmarksfly.cn

C#:   u is User
来源：http://yo.asd995.cn


<!-- 参考信息 -->