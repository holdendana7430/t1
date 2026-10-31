代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vc.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pf.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vv.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vi.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rl.lnxyls.cn

Ruby: s.capitalize
来源：http://br.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://no.huixiangedu.cn

[E18] 模板占位符替换
来源：http://me.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fn.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mb.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iu.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kz.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iz.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sg.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://we.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://na.nszjky.cn

[E19] 多行文本按行拆分
来源：http://iu.shtwfgs.cn

Py:   s.splitlines()
来源：http://us.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ne.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://uv.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ei.nszjky.cn

Java: s.lines().toList()
来源：http://zz.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://uz.shtwfgs.cn

Ruby: s.lines
来源：http://ee.huixiangedu.cn

C#:   s.Split('\n')
来源：http://et.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://te.bookmarksfly.cn

Py:   if not s:
来源：http://yu.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ij.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sk.hahajie.cn

TS:   if (s === "") {}
来源：http://na.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://so.lnxyls.cn

Go:   if s == "" {}
来源：http://ae.chemitech.net.cn

Ruby: if s.empty?
来源：http://zd.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jl.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://ef.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lr.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ts.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ix.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nd.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yc.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://zb.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sv.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uj.huanxung.cn

[E22] 字节长度与字符长度
来源：http://mw.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gw.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ry.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uv.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oa.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oh.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://ut.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fi.szsharing.cn

================================================================================
来源：http://yf.shxzukj.cn

F. 文件与目录
来源：http://pd.huixinmuqiang.cn

================================================================================
来源：http://dn.haigaiapp.cn

[F01] 读取整个文件
来源：http://nf.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iy.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://ok.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ex.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sd.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oh.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kd.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ds.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://lg.szxytkj.cn

[F02] 逐行读取文件
来源：http://fb.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dk.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pa.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ku.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xw.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yc.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ww.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hf.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://me.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://zd.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fe.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ba.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sk.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lf.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qk.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://px.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://mt.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xl.nszjky.cn

[F04] 追加写入文件
来源：http://nz.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nv.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mz.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bo.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qs.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gp.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uz.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pq.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hl.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://lg.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://th.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://qj.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://mo.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://eb.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xt.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wl.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://sx.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://ch.jctech888.com.cn

[F06] 删除文件
来源：http://dc.szsharing.cn

Py:   os.remove("a.txt")
来源：http://gq.newstarts.cn

PHP:  unlink("a.txt");
来源：http://xz.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nr.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ys.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sr.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://xc.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://qw.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://ds.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://me.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ut.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nk.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hg.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lp.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sg.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qv.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vd.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eq.shxzskj.cn

[F08] 遍历目录
来源：http://hy.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yh.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xk.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://gk.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://zz.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fp.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qn.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://dd.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://lc.nicolike.cn

[F09] 获取文件大小
来源：http://xx.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://in.9csxet.cn

PHP:  filesize("a.txt");
来源：http://eu.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://vr.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://wc.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://le.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sj.nicolike.cn

Ruby: File.size("a.txt")
来源：http://dj.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://xt.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ig.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dn.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jv.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qi.newstarts.cn

TS:   path.extname("a.txt")
来源：http://tq.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xa.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nu.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kc.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ix.wgjwhj.cn

[F11] 复制与移动文件
来源：http://ng.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zt.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ev.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vj.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tl.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bo.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ax.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://od.newstarts.cn

[F12] CSV 读写
来源：http://ou.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zq.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pq.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xh.lnxyls.cn

TS:   // 同上
来源：http://dk.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sf.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ot.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ri.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ul.szsharing.cn

================================================================================
来源：http://tl.colortex.cn

G. 面向对象
来源：http://rx.bookmarksfly.cn

================================================================================
来源：http://xg.yuexingan06.cn

[G01] 定义类
来源：http://om.nszjky.cn

Py:   class User: pass
来源：http://hn.huixinmuqiang.cn

PHP:  class User {}
来源：http://sp.huanxung.cn

JS:   class User {}
来源：http://rs.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://gb.huixiangedu.cn

Java: class User {}
来源：http://dd.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://pm.shxzukj.cn

Ruby: class User; end
来源：http://cq.bjjhwx.cn

C#:   class User {}
来源：http://uv.shtwfgs.cn

[G02] 构造函数
来源：http://yd.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://jm.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://nq.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://uu.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://pn.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://cc.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gq.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://gk.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://mp.shxzukj.cn

[G03] 实例属性
来源：http://kc.lnxyls.cn

Py:   self.name = "x"
来源：http://wb.hnjuh.cn

PHP:  public string $name = "x";
来源：http://jf.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ru.yuexingan06.cn

TS:   name: string = "x";
来源：http://ii.shtwfgs.cn

Java: private String name;
来源：http://bh.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ix.huanxung.cn

Ruby: @name = "x"
来源：http://tg.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://qh.hnjuh.cn

[G04] 定义方法
来源：http://fp.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://yz.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://py.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://zh.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://kb.yuexingan06.cn

Java: String greet() { return name; }
来源：http://in.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nl.huanxung.cn

Ruby: def greet; @name; end
来源：http://bx.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://ml.wgjwhj.cn

[G05] 继承
来源：http://gh.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://dz.szsharing.cn

PHP:  class Admin extends User {}
来源：http://tm.shxzukj.cn

JS:   class Admin extends User {}
来源：http://vc.nicolike.cn

TS:   class Admin extends User {}
来源：http://ln.jctech888.com.cn

Java: class Admin extends User {}
来源：http://uc.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bd.nszjky.cn

Ruby: class Admin < User; end
来源：http://at.shxzukj.cn

C#:   class Admin : User {}
来源：http://bp.panjiajie.cn

[G06] 重写方法
来源：http://ao.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://yg.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wa.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://st.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://wc.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://gw.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nl.asd995.cn

Ruby: def greet; "admin"; end
来源：http://wp.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://ew.shtwfgs.cn

[G07] 调用父类方法
来源：http://rc.newstarts.cn

Py:   super().greet()
来源：http://py.muxihuayi.cn

PHP:  parent::greet();
来源：http://be.gzmigu.cn

JS:   super.greet();
来源：http://tt.bookmarksfly.cn

TS:   super.greet();
来源：http://uo.huixinmuqiang.cn

Java: super.greet();
来源：http://it.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cj.szsharing.cn

Ruby: super
来源：http://sp.szxytkj.cn

C#:   base.Greet();
来源：http://aj.asd995.cn

[G08] 静态方法与属性
来源：http://rn.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dx.asd995.cn

PHP:  public static function f() {}
来源：http://pf.bjjhwx.cn

JS:   static f() {}
来源：http://fy.521024.cn

TS:   static f(): void {}
来源：http://en.szxytkj.cn

Java: static void f() {}
来源：http://sg.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://es.yuexingan06.cn

Ruby: def self.f; end
来源：http://hv.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://pm.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://tl.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://jx.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wj.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://im.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://sj.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://vb.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://gt.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hf.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://uk.lnxyls.cn

[G10] 访问控制
来源：http://sr.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pv.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ng.colortex.cn

JS:   #private 字段；其余公开
来源：http://ha.shxzukj.cn

TS:   public / protected / private
来源：http://ks.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://xv.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wr.jctech888.com.cn

Ruby: public / protected / private
来源：http://ry.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://uw.bookmarksfly.cn

[G11] getter / setter
来源：http://gy.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://vx.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wh.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://aa.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://xk.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://pg.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kq.panjiajie.cn

Ruby: attr_accessor :name
来源：http://hf.nszjky.cn

C#:   public string Name { get; set; }
来源：http://vz.muxihuayi.cn

[G12] 对象转字符串
来源：http://mz.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://uz.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yl.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://zy.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://iv.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://kt.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cw.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://wc.colortex.cn

C#:   public override string ToString() => Name;
来源：http://lp.asd995.cn

[G13] 判断对象类型
来源：http://rm.hahajie.cn

Py:   isinstance(u, User)
来源：http://iv.asd995.cn

PHP:  $u instanceof User
来源：http://jf.shxzskj.cn

JS:   u instanceof User
来源：http://zz.nszjky.cn

TS:   u instanceof User
来源：http://sw.huixiangedu.cn

Java: u instanceof User
来源：http://pk.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://if.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://dy.asd995.cn

C#:   u is User
来源：http://ba.shtwfgs.cn

[G14] 数据类 / record
来源：http://rd.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gn.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://uw.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jy.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://jj.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://fa.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://zu.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hp.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ci.muxihuayi.cn

[G15] 枚举
来源：http://go.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hr.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qg.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://on.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qc.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://mf.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rv.muxihuayi.cn


<!-- 参考信息 -->