代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dc.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pv.muxihuayi.cn

[E16] 数字千分位
来源：http://ix.huanxung.cn

Py:   f"{1234567:,}"
来源：http://px.newstarts.cn

PHP:  number_format(1234567);
来源：http://rt.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ew.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kc.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qv.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://er.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hj.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ia.chemitech.net.cn

[E17] 首字母大写
来源：http://oc.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fa.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qd.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qp.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mr.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lv.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cd.wgjwhj.cn

Ruby: s.capitalize
来源：http://zr.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hq.wgjwhj.cn

[E18] 模板占位符替换
来源：http://cb.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ln.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zp.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tp.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zt.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ia.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zc.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rd.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ka.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://rd.asd995.cn

Py:   s.splitlines()
来源：http://sp.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dh.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ju.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ik.hahajie.cn

Java: s.lines().toList()
来源：http://ea.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://dl.shtwfgs.cn

Ruby: s.lines
来源：http://ds.huixiangedu.cn

C#:   s.Split('\n')
来源：http://wf.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://mp.yuexingan06.cn

Py:   if not s:
来源：http://oc.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rq.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tj.szxytkj.cn

TS:   if (s === "") {}
来源：http://mf.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://jm.bjjhwx.cn

Go:   if s == "" {}
来源：http://tr.muxihuayi.cn

Ruby: if s.empty?
来源：http://li.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ur.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://ly.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://az.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pp.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hd.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lv.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oq.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://du.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://de.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://an.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://vo.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yo.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sw.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pl.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://st.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kx.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wv.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://ot.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lq.huixinmuqiang.cn

================================================================================
来源：http://bt.yuntaijiaju.cn

F. 文件与目录
来源：http://fi.newstarts.cn

================================================================================
来源：http://dg.521024.cn

[F01] 读取整个文件
来源：http://ug.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://la.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://dh.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sm.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dw.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ww.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zd.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://hm.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://kt.muxihuayi.cn

[F02] 逐行读取文件
来源：http://os.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://de.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://by.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fg.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fz.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://us.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xz.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mg.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hd.colortex.cn

[F03] 写入文件（覆盖）
来源：http://ty.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ug.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pm.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qw.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qj.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tj.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cn.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://wg.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yc.hnjuh.cn

[F04] 追加写入文件
来源：http://eg.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://if.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vj.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ru.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://st.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uc.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fj.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://js.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://si.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://gf.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xa.colortex.cn

PHP:  file_exists("a.txt");
来源：http://fu.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://wz.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://tu.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ey.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://an.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://qz.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://jd.chemitech.net.cn

[F06] 删除文件
来源：http://rd.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://lu.nszjky.cn

PHP:  unlink("a.txt");
来源：http://mj.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nd.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zo.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jl.colortex.cn

Go:   os.Remove("a.txt")
来源：http://df.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://hk.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://co.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://sc.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ut.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vc.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rc.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ht.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hi.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ys.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ye.hahajie.cn

[F08] 遍历目录
来源：http://vm.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hm.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hl.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://go.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://im.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://id.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uh.nicolike.cn

Ruby: Dir.children("dir")
来源：http://yz.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://hj.lnxyls.cn

[F09] 获取文件大小
来源：http://zm.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://xk.newstarts.cn

PHP:  filesize("a.txt");
来源：http://oj.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://mm.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://iq.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fo.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cv.asd995.cn

Ruby: File.size("a.txt")
来源：http://tt.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://yp.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://lo.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wn.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lr.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gw.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://up.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jo.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tf.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ga.lnxyls.cn

[F11] 复制与移动文件
来源：http://ap.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hu.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vb.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wm.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pb.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iu.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nk.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://he.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eq.yuexingan06.cn

[F12] CSV 读写
来源：http://cs.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aw.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aj.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fj.huanxung.cn

TS:   // 同上
来源：http://uc.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ic.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://io.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uh.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fd.haigaiapp.cn

================================================================================
来源：http://fu.bookmarksfly.cn

G. 面向对象
来源：http://bp.bookmarksfly.cn

================================================================================
来源：http://kv.wgjwhj.cn

[G01] 定义类
来源：http://dq.huixiangedu.cn

Py:   class User: pass
来源：http://nc.nszjky.cn

PHP:  class User {}
来源：http://xs.bookmarksfly.cn

JS:   class User {}
来源：http://vj.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://po.huixiangedu.cn

Java: class User {}
来源：http://sw.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://uc.521024.cn

Ruby: class User; end
来源：http://ak.chemitech.net.cn

C#:   class User {}
来源：http://ru.nicolike.cn

[G02] 构造函数
来源：http://yo.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://in.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://tq.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://ks.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://qa.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://bw.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iy.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ry.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ft.wgjwhj.cn

[G03] 实例属性
来源：http://fy.9csxet.cn

Py:   self.name = "x"
来源：http://bn.huanxung.cn

PHP:  public string $name = "x";
来源：http://ak.lnxyls.cn

JS:   this.name = "x";
来源：http://qj.shxzskj.cn

TS:   name: string = "x";
来源：http://pi.chemitech.net.cn

Java: private String name;
来源：http://ly.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lh.nicolike.cn

Ruby: @name = "x"
来源：http://pl.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://gg.jctech888.com.cn

[G04] 定义方法
来源：http://ae.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://xa.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ec.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://ds.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://mm.newstarts.cn

Java: String greet() { return name; }
来源：http://eg.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jg.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://mb.szsharing.cn

C#:   public string Greet() => Name;
来源：http://sl.lnxyls.cn

[G05] 继承
来源：http://yu.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://rc.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://nm.shxzskj.cn

JS:   class Admin extends User {}
来源：http://xk.asd995.cn

TS:   class Admin extends User {}
来源：http://ai.jctech888.com.cn

Java: class Admin extends User {}
来源：http://ru.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://px.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://qj.wgjwhj.cn

C#:   class Admin : User {}
来源：http://us.szsharing.cn

[G06] 重写方法
来源：http://yg.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://bk.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zc.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://py.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://mn.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://fc.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://id.asd995.cn

Ruby: def greet; "admin"; end
来源：http://fz.521024.cn

C#:   public override string Greet() => "admin";
来源：http://zn.nszjky.cn

[G07] 调用父类方法
来源：http://ef.bookmarksfly.cn

Py:   super().greet()
来源：http://in.shtwfgs.cn

PHP:  parent::greet();
来源：http://tg.szsharing.cn

JS:   super.greet();
来源：http://gr.shxzukj.cn

TS:   super.greet();
来源：http://tx.shtwfgs.cn

Java: super.greet();
来源：http://wv.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lx.9csxet.cn

Ruby: super
来源：http://mo.hahajie.cn

C#:   base.Greet();
来源：http://ow.muxihuayi.cn

[G08] 静态方法与属性
来源：http://bp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tg.hahajie.cn

PHP:  public static function f() {}
来源：http://er.yuexingan06.cn

JS:   static f() {}
来源：http://vm.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://mq.muxihuayi.cn

Java: static void f() {}
来源：http://nq.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uu.lnxyls.cn

Ruby: def self.f; end
来源：http://cd.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://um.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://et.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://fs.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ck.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tt.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://sl.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://zy.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://tx.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eh.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://fk.chemitech.net.cn

[G10] 访问控制
来源：http://hl.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://do.hahajie.cn

PHP:  public / protected / private
来源：http://ok.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://os.bookmarksfly.cn

TS:   public / protected / private
来源：http://fh.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://au.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sf.nicolike.cn

Ruby: public / protected / private
来源：http://lx.szxytkj.cn

C#:   public / protected / private / internal
来源：http://bk.hnjuh.cn

[G11] getter / setter
来源：http://rq.hahajie.cn

Py:   @property 与 @x.setter
来源：http://mw.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jy.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://fd.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://xv.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://nk.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iv.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://vp.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://yf.nszjky.cn

[G12] 对象转字符串
来源：http://pv.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://cy.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zv.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://lm.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://xs.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://gd.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://by.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ah.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://io.newstarts.cn

[G13] 判断对象类型
来源：http://zl.szsharing.cn

Py:   isinstance(u, User)
来源：http://ud.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ej.bjjhwx.cn

JS:   u instanceof User
来源：http://fj.bookmarksfly.cn

TS:   u instanceof User
来源：http://cx.shxzskj.cn

Java: u instanceof User
来源：http://tp.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://la.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://gt.wgjwhj.cn

C#:   u is User
来源：http://nb.lnxyls.cn

[G14] 数据类 / record
来源：http://le.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fo.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://vg.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iv.wgjwhj.cn


<!-- 参考信息 -->