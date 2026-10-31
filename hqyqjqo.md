代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ou.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vz.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://zl.hahajie.cn

[E17] 首字母大写
来源：http://qn.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qm.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sm.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gk.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vs.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://me.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zm.nicolike.cn

Ruby: s.capitalize
来源：http://gz.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ca.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://dp.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sh.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tr.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zd.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vv.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gp.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rs.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uo.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vr.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://gy.wgjwhj.cn

Py:   s.splitlines()
来源：http://tl.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uo.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://mf.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://dy.huixiangedu.cn

Java: s.lines().toList()
来源：http://iy.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://yp.bjjhwx.cn

Ruby: s.lines
来源：http://kp.asd995.cn

C#:   s.Split('\n')
来源：http://aw.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://dv.chemitech.net.cn

Py:   if not s:
来源：http://gh.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ji.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ff.shxzukj.cn

TS:   if (s === "") {}
来源：http://oz.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://un.nicolike.cn

Go:   if s == "" {}
来源：http://hu.yuexingan06.cn

Ruby: if s.empty?
来源：http://we.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uk.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ev.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zx.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ox.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zn.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uf.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://th.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://um.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nl.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ar.521024.cn

[E22] 字节长度与字符长度
来源：http://zb.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://af.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ry.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vj.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://py.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tb.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://so.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://xv.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sw.hahajie.cn

================================================================================
来源：http://rq.szsharing.cn

F. 文件与目录
来源：http://nn.muxihuayi.cn

================================================================================
来源：http://ww.9csxet.cn

[F01] 读取整个文件
来源：http://kf.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ce.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://br.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yy.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nf.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ff.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qz.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://qy.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://oi.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ti.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xg.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ys.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://go.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ve.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xg.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qd.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kz.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://fb.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bi.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ij.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gm.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ru.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wd.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ct.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://yt.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qv.huanxung.cn

[F04] 追加写入文件
来源：http://oq.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ol.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://go.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ea.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fz.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jb.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uz.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hc.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ye.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://hg.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hr.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ga.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://wg.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://sa.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nk.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wd.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://el.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ww.colortex.cn

[F06] 删除文件
来源：http://tp.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://lf.asd995.cn

PHP:  unlink("a.txt");
来源：http://wp.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fi.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://br.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nm.colortex.cn

Go:   os.Remove("a.txt")
来源：http://pz.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://og.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://ts.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://ha.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ht.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sa.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://we.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hk.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pg.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://el.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://el.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iu.huixiangedu.cn

[F08] 遍历目录
来源：http://kv.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bk.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://az.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://tb.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://yl.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rc.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yf.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://nd.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://qd.jctech888.com.cn

[F09] 获取文件大小
来源：http://pw.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ic.nicolike.cn

PHP:  filesize("a.txt");
来源：http://wj.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://bc.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ea.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hf.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pe.colortex.cn

Ruby: File.size("a.txt")
来源：http://yk.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://lu.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://eu.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gm.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vw.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mh.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://zv.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nj.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://me.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ni.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nv.colortex.cn

[F11] 复制与移动文件
来源：http://ks.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jv.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gj.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dv.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mq.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kr.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cn.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yv.gzmigu.cn

[F12] CSV 读写
来源：http://yk.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tr.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gl.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hr.jianghongdianzi.cn

TS:   // 同上
来源：http://za.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iu.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://th.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vm.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qo.haigaiapp.cn

================================================================================
来源：http://mi.lnxyls.cn

G. 面向对象
来源：http://vu.shxzukj.cn

================================================================================
来源：http://pj.shxzukj.cn

[G01] 定义类
来源：http://si.nicolike.cn

Py:   class User: pass
来源：http://dk.hnjuh.cn

PHP:  class User {}
来源：http://yu.bjjhwx.cn

JS:   class User {}
来源：http://bf.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://wi.wgjwhj.cn

Java: class User {}
来源：http://ft.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://cj.gzmigu.cn

Ruby: class User; end
来源：http://da.newstarts.cn

C#:   class User {}
来源：http://mr.huanxung.cn

[G02] 构造函数
来源：http://jo.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://bd.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://eq.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ue.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://yz.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://tk.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gm.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://tn.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://tu.shtwfgs.cn

[G03] 实例属性
来源：http://mq.szxytkj.cn

Py:   self.name = "x"
来源：http://zh.hnjuh.cn

PHP:  public string $name = "x";
来源：http://zl.9csxet.cn

JS:   this.name = "x";
来源：http://uw.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://gd.521024.cn

Java: private String name;
来源：http://js.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jf.yuexingan06.cn

Ruby: @name = "x"
来源：http://pl.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://ig.gzmigu.cn

[G04] 定义方法
来源：http://it.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://wt.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sq.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://cn.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://so.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://jl.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tg.panjiajie.cn

Ruby: def greet; @name; end
来源：http://oy.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://ab.szsharing.cn

[G05] 继承
来源：http://of.lnxyls.cn

Py:   class Admin(User): pass
来源：http://zd.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://st.hnjuh.cn

JS:   class Admin extends User {}
来源：http://ej.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://yz.yuexingan06.cn

Java: class Admin extends User {}
来源：http://ko.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yd.huanxung.cn

Ruby: class Admin < User; end
来源：http://ie.huixiangedu.cn

C#:   class Admin : User {}
来源：http://lm.yuexingan06.cn

[G06] 重写方法
来源：http://ta.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://ne.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ni.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://cm.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://hb.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://lb.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://np.colortex.cn

Ruby: def greet; "admin"; end
来源：http://fw.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://tx.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://yw.wgjwhj.cn

Py:   super().greet()
来源：http://mp.bookmarksfly.cn

PHP:  parent::greet();
来源：http://pn.colortex.cn

JS:   super.greet();
来源：http://qn.521024.cn

TS:   super.greet();
来源：http://ob.shxzskj.cn

Java: super.greet();
来源：http://jt.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xh.panjiajie.cn

Ruby: super
来源：http://dj.521024.cn

C#:   base.Greet();
来源：http://ze.yuexingan06.cn

[G08] 静态方法与属性
来源：http://di.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://my.newstarts.cn

PHP:  public static function f() {}
来源：http://oq.hahajie.cn

JS:   static f() {}
来源：http://np.shxzukj.cn

TS:   static f(): void {}
来源：http://sy.9csxet.cn

Java: static void f() {}
来源：http://zu.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xa.bookmarksfly.cn

Ruby: def self.f; end
来源：http://ym.yuexingan06.cn

C#:   public static void F() {}
来源：http://zj.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://hs.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://xp.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ai.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cz.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://nf.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://gi.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://rg.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ni.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://sh.gzmigu.cn

[G10] 访问控制
来源：http://vd.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://oc.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gs.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://gl.huixiangedu.cn

TS:   public / protected / private
来源：http://ne.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://ut.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hi.shxzukj.cn

Ruby: public / protected / private
来源：http://jj.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://ow.huixinmuqiang.cn

[G11] getter / setter
来源：http://wd.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://ne.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yx.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ki.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://wd.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://dg.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zj.521024.cn

Ruby: attr_accessor :name
来源：http://me.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://fg.hnjuh.cn

[G12] 对象转字符串
来源：http://ax.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://yb.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rh.nicolike.cn

JS:   toString() { return this.name; }
来源：http://td.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://kv.521024.cn

Java: @Override public String toString() { return name; }
来源：http://ek.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ad.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://ff.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://sh.shxzskj.cn

[G13] 判断对象类型
来源：http://nn.lnxyls.cn

Py:   isinstance(u, User)
来源：http://qg.yuexingan06.cn

PHP:  $u instanceof User
来源：http://wp.panjiajie.cn

JS:   u instanceof User
来源：http://mv.asd995.cn

TS:   u instanceof User
来源：http://nc.panjiajie.cn

Java: u instanceof User
来源：http://jj.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qb.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ji.bookmarksfly.cn

C#:   u is User
来源：http://dm.szsharing.cn

[G14] 数据类 / record
来源：http://jt.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kp.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://hj.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fe.521024.cn

TS:   type User = { name: string; age: number };
来源：http://sg.521024.cn

Java: record User(String name, int age) {}
来源：http://tv.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://uw.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rb.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://cb.hnjuh.cn

[G15] 枚举
来源：http://xs.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nf.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wv.colortex.cn


<!-- 参考信息 -->