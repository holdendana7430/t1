代发 wailian999

PHP:  number_format(1234567);
来源：http://nb.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cq.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pv.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ww.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xj.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qf.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://op.jianghongdianzi.cn

[E17] 首字母大写
来源：http://cc.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mr.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wf.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uj.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fs.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kf.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bo.asd995.cn

Ruby: s.capitalize
来源：http://go.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xh.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://fq.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tt.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rm.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wn.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kx.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://od.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ik.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bc.9csxet.cn

[E19] 多行文本按行拆分
来源：http://hf.asd995.cn

Py:   s.splitlines()
来源：http://vh.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uz.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://jm.521024.cn

TS:   s.split(/\r?\n/)
来源：http://go.shtwfgs.cn

Java: s.lines().toList()
来源：http://hy.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://zg.bookmarksfly.cn

Ruby: s.lines
来源：http://fv.nicolike.cn

C#:   s.Split('\n')
来源：http://le.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://ad.yuexingan06.cn

Py:   if not s:
来源：http://ly.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cs.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sr.hahajie.cn

TS:   if (s === "") {}
来源：http://le.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://sm.huixiangedu.cn

Go:   if s == "" {}
来源：http://mb.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://bb.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ac.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://cd.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zp.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ss.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lc.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ms.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oi.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://vg.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fi.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sp.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://md.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ut.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hh.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tz.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mz.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hq.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eu.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://ds.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sy.huixiangedu.cn

================================================================================
来源：http://gt.yuntaijiaju.cn

F. 文件与目录
来源：http://hw.yuexingan06.cn

================================================================================
来源：http://oc.bookmarksfly.cn

[F01] 读取整个文件
来源：http://ld.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dw.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://cd.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tc.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://td.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nm.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ej.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://eg.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://uv.521024.cn

[F02] 逐行读取文件
来源：http://wz.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aw.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ol.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yt.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eb.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ja.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vv.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hg.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://ux.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nt.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vu.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://is.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://so.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qh.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mz.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://jh.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nw.jctech888.com.cn

[F04] 追加写入文件
来源：http://ww.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pq.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bt.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vu.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xo.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pk.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jw.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oc.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://py.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://if.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://as.asd995.cn

PHP:  file_exists("a.txt");
来源：http://sz.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://xe.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://fy.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ke.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mf.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://oc.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://qa.haigaiapp.cn

[F06] 删除文件
来源：http://op.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ii.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://sc.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yk.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mv.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ue.colortex.cn

Go:   os.Remove("a.txt")
来源：http://kr.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://ru.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ip.newstarts.cn

[F07] 创建目录（含多级）
来源：http://vt.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wb.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ey.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gx.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rb.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rw.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hq.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qm.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ri.521024.cn

[F08] 遍历目录
来源：http://cp.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pu.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xe.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://fn.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://fj.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mi.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fx.asd995.cn

Ruby: Dir.children("dir")
来源：http://hg.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://ha.asd995.cn

[F09] 获取文件大小
来源：http://ts.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://fy.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://vm.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://bd.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://gc.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gw.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cj.9csxet.cn

Ruby: File.size("a.txt")
来源：http://nr.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://xt.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://xk.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tp.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jz.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://li.nicolike.cn

TS:   path.extname("a.txt")
来源：http://wt.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hy.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vl.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ej.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ip.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://cn.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://po.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oz.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ag.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oi.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ki.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ze.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gh.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wp.9csxet.cn

[F12] CSV 读写
来源：http://qk.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ts.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hp.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uf.panjiajie.cn

TS:   // 同上
来源：http://qp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wh.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gt.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mt.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wb.shxzskj.cn

================================================================================
来源：http://xr.nszjky.cn

G. 面向对象
来源：http://tm.nszjky.cn

================================================================================
来源：http://td.bjjhwx.cn

[G01] 定义类
来源：http://cm.nicolike.cn

Py:   class User: pass
来源：http://nw.521024.cn

PHP:  class User {}
来源：http://ft.9csxet.cn

JS:   class User {}
来源：http://sq.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://mm.muxihuayi.cn

Java: class User {}
来源：http://wy.nicolike.cn

Go:   type User struct { Name string }
来源：http://ge.yuntaijiaju.cn

Ruby: class User; end
来源：http://lh.bookmarksfly.cn

C#:   class User {}
来源：http://lv.hahajie.cn

[G02] 构造函数
来源：http://bw.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://er.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://tl.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://jy.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://mz.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://fz.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ey.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://yq.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ay.asd995.cn

[G03] 实例属性
来源：http://sc.bjjhwx.cn

Py:   self.name = "x"
来源：http://if.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://sz.szsharing.cn

JS:   this.name = "x";
来源：http://yr.nszjky.cn

TS:   name: string = "x";
来源：http://kn.hahajie.cn

Java: private String name;
来源：http://sn.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nd.szsharing.cn

Ruby: @name = "x"
来源：http://qi.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://fs.szsharing.cn

[G04] 定义方法
来源：http://em.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://cg.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ja.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://mo.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://cc.huixiangedu.cn

Java: String greet() { return name; }
来源：http://pg.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zn.nicolike.cn

Ruby: def greet; @name; end
来源：http://ke.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://vm.nszjky.cn

[G05] 继承
来源：http://ca.hahajie.cn

Py:   class Admin(User): pass
来源：http://rt.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://lz.szsharing.cn

JS:   class Admin extends User {}
来源：http://sf.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://fb.9csxet.cn

Java: class Admin extends User {}
来源：http://sp.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uo.szxytkj.cn

Ruby: class Admin < User; end
来源：http://ec.yuexingan06.cn

C#:   class Admin : User {}
来源：http://jg.chemitech.net.cn

[G06] 重写方法
来源：http://ii.521024.cn

Py:   def greet(self): return "admin"
来源：http://ub.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oh.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://bk.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://up.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://uc.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wq.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://kx.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://gv.gzmigu.cn

[G07] 调用父类方法
来源：http://wm.szsharing.cn

Py:   super().greet()
来源：http://ou.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://ju.wgjwhj.cn

JS:   super.greet();
来源：http://ha.gzmigu.cn

TS:   super.greet();
来源：http://if.haigaiapp.cn

Java: super.greet();
来源：http://ev.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gn.9csxet.cn

Ruby: super
来源：http://bc.huixiangedu.cn

C#:   base.Greet();
来源：http://nq.muxihuayi.cn

[G08] 静态方法与属性
来源：http://vk.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://he.newstarts.cn

PHP:  public static function f() {}
来源：http://wo.szsharing.cn

JS:   static f() {}
来源：http://tj.lnxyls.cn

TS:   static f(): void {}
来源：http://qg.shxzskj.cn

Java: static void f() {}
来源：http://mg.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ao.colortex.cn

Ruby: def self.f; end
来源：http://vy.shxzskj.cn

C#:   public static void F() {}
来源：http://zt.hahajie.cn

[G09] 接口 / 抽象类
来源：http://tm.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://ul.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kf.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cg.521024.cn

TS:   interface Shape { area(): number; }
来源：http://qc.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://ei.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://sj.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uw.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ac.muxihuayi.cn

[G10] 访问控制
来源：http://oq.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://sz.nicolike.cn

PHP:  public / protected / private
来源：http://yp.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://gk.newstarts.cn

TS:   public / protected / private
来源：http://mb.asd995.cn

Java: public / protected / private / 默认包级
来源：http://st.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hi.hahajie.cn

Ruby: public / protected / private
来源：http://wb.shxzskj.cn

C#:   public / protected / private / internal
来源：http://zx.jctech888.com.cn

[G11] getter / setter
来源：http://xo.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://yw.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kb.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://mz.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://kx.szxytkj.cn

Java: public String getName() { return name; }
来源：http://kv.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ej.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://go.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://ds.lnxyls.cn

[G12] 对象转字符串
来源：http://aq.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://yy.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wz.521024.cn

JS:   toString() { return this.name; }
来源：http://yz.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://fu.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://mr.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kc.nszjky.cn

Ruby: def to_s; @name; end
来源：http://im.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://iw.huanxung.cn

[G13] 判断对象类型
来源：http://oo.panjiajie.cn

Py:   isinstance(u, User)
来源：http://my.wgjwhj.cn

PHP:  $u instanceof User
来源：http://pd.hnjuh.cn

JS:   u instanceof User
来源：http://nh.colortex.cn

TS:   u instanceof User
来源：http://nu.shxzskj.cn

Java: u instanceof User
来源：http://ll.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tc.huanxung.cn

Ruby: u.is_a?(User)
来源：http://zc.jctech888.com.cn

C#:   u is User
来源：http://wd.shxzukj.cn

[G14] 数据类 / record
来源：http://gw.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tn.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ln.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ld.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://wr.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://fa.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://dg.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uu.colortex.cn


<!-- 参考信息 -->