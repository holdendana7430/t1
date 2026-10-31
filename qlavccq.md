代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ke.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gr.szxytkj.cn

Ruby: s.capitalize
来源：http://ea.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xq.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ka.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fg.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://he.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://og.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jp.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yv.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xm.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ov.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mu.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ck.shtwfgs.cn

Py:   s.splitlines()
来源：http://qb.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iw.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://kt.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://nv.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ba.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://jz.nszjky.cn

Ruby: s.lines
来源：http://vh.hahajie.cn

C#:   s.Split('\n')
来源：http://ny.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ql.jctech888.com.cn

Py:   if not s:
来源：http://tt.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wn.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dh.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://vx.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://zk.nicolike.cn

Go:   if s == "" {}
来源：http://zy.chemitech.net.cn

Ruby: if s.empty?
来源：http://ni.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cy.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://or.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bk.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xr.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://af.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gq.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ux.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://fb.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://li.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rx.9csxet.cn

[E22] 字节长度与字符长度
来源：http://zo.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ho.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bw.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kz.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ak.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mu.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iu.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://zt.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://az.yuexingan06.cn

================================================================================
来源：http://zv.shtwfgs.cn

F. 文件与目录
来源：http://xu.haigaiapp.cn

================================================================================
来源：http://vq.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://gp.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ng.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://xk.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dq.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dk.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://df.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bl.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ag.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ra.colortex.cn

[F02] 逐行读取文件
来源：http://ze.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lu.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sv.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rm.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yf.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cp.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xd.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ve.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://cf.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ic.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gs.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hf.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wx.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pn.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cw.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://fm.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pb.muxihuayi.cn

[F04] 追加写入文件
来源：http://uw.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://no.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ps.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://se.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ub.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hr.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jz.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qu.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ow.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://gw.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sj.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://al.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://bv.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://do.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ca.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sl.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://qi.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://xc.hahajie.cn

[F06] 删除文件
来源：http://mu.asd995.cn

Py:   os.remove("a.txt")
来源：http://di.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://mv.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ny.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pz.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gf.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ji.colortex.cn

Ruby: File.delete("a.txt")
来源：http://zn.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://ne.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://sh.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pp.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fb.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://al.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sp.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ah.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vv.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jw.panjiajie.cn

[F08] 遍历目录
来源：http://bz.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aa.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wm.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://jk.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://rw.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://im.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ky.asd995.cn

Ruby: Dir.children("dir")
来源：http://pz.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ga.jctech888.com.cn

[F09] 获取文件大小
来源：http://zb.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://ch.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ym.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://bt.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://oh.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tw.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xb.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://jp.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://mo.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://iy.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gp.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sx.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ni.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://ol.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oy.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rd.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ee.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zd.shxzukj.cn

[F11] 复制与移动文件
来源：http://yd.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pg.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ul.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xq.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gr.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wr.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ln.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rk.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zz.yuexingan06.cn

[F12] CSV 读写
来源：http://kf.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ro.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vi.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dz.szxytkj.cn

TS:   // 同上
来源：http://hw.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ap.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ot.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vq.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oq.wgjwhj.cn

================================================================================
来源：http://ez.colortex.cn

G. 面向对象
来源：http://qs.colortex.cn

================================================================================
来源：http://gg.muxihuayi.cn

[G01] 定义类
来源：http://ac.asd995.cn

Py:   class User: pass
来源：http://bd.nszjky.cn

PHP:  class User {}
来源：http://ow.shtwfgs.cn

JS:   class User {}
来源：http://fy.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://ta.9csxet.cn

Java: class User {}
来源：http://nb.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://hd.lnxyls.cn

Ruby: class User; end
来源：http://bm.521024.cn

C#:   class User {}
来源：http://ul.gzmigu.cn

[G02] 构造函数
来源：http://ek.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://zz.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://oy.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://tc.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://qy.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://im.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://us.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://jc.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://wl.huixiangedu.cn

[G03] 实例属性
来源：http://ub.shxzskj.cn

Py:   self.name = "x"
来源：http://vy.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://wf.nicolike.cn

JS:   this.name = "x";
来源：http://jb.muxihuayi.cn

TS:   name: string = "x";
来源：http://ev.panjiajie.cn

Java: private String name;
来源：http://wo.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vb.bookmarksfly.cn

Ruby: @name = "x"
来源：http://se.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://lf.yuexingan06.cn

[G04] 定义方法
来源：http://xn.colortex.cn

Py:   def greet(self): return self.name
来源：http://gm.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mu.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://zj.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://gf.hahajie.cn

Java: String greet() { return name; }
来源：http://su.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://js.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://pz.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://tj.lnxyls.cn

[G05] 继承
来源：http://lt.hahajie.cn

Py:   class Admin(User): pass
来源：http://tp.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://cn.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://pp.nicolike.cn

TS:   class Admin extends User {}
来源：http://st.asd995.cn

Java: class Admin extends User {}
来源：http://vf.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kh.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://eh.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ye.bookmarksfly.cn

[G06] 重写方法
来源：http://dc.521024.cn

Py:   def greet(self): return "admin"
来源：http://jr.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sz.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://md.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://ul.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ba.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xe.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://tw.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://hk.hnjuh.cn

[G07] 调用父类方法
来源：http://sg.shxzukj.cn

Py:   super().greet()
来源：http://um.shtwfgs.cn

PHP:  parent::greet();
来源：http://jr.panjiajie.cn

JS:   super.greet();
来源：http://nd.bjjhwx.cn

TS:   super.greet();
来源：http://lm.jianghongdianzi.cn

Java: super.greet();
来源：http://ax.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mu.chemitech.net.cn

Ruby: super
来源：http://za.asd995.cn

C#:   base.Greet();
来源：http://br.shxzskj.cn

[G08] 静态方法与属性
来源：http://pg.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jl.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://st.shtwfgs.cn

JS:   static f() {}
来源：http://hz.shtwfgs.cn

TS:   static f(): void {}
来源：http://px.521024.cn

Java: static void f() {}
来源：http://xw.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hg.lnxyls.cn

Ruby: def self.f; end
来源：http://yw.panjiajie.cn

C#:   public static void F() {}
来源：http://ic.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://oo.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://jr.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iy.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tz.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://lh.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://py.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://jp.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tv.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://kq.hahajie.cn

[G10] 访问控制
来源：http://pi.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://de.chemitech.net.cn

PHP:  public / protected / private
来源：http://uc.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://mp.asd995.cn

TS:   public / protected / private
来源：http://pd.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://hd.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ww.jctech888.com.cn

Ruby: public / protected / private
来源：http://yh.szsharing.cn

C#:   public / protected / private / internal
来源：http://wt.huixiangedu.cn

[G11] getter / setter
来源：http://vm.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://cw.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ko.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ir.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://gp.521024.cn

Java: public String getName() { return name; }
来源：http://lt.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://am.newstarts.cn

Ruby: attr_accessor :name
来源：http://sb.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://wo.asd995.cn

[G12] 对象转字符串
来源：http://fh.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://xw.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ea.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://ut.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://rs.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://vg.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lx.hahajie.cn

Ruby: def to_s; @name; end
来源：http://vc.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://zj.nicolike.cn

[G13] 判断对象类型
来源：http://ql.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://do.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ne.szsharing.cn

JS:   u instanceof User
来源：http://on.shtwfgs.cn

TS:   u instanceof User
来源：http://fp.bjjhwx.cn

Java: u instanceof User
来源：http://mc.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wc.521024.cn

Ruby: u.is_a?(User)
来源：http://rc.hahajie.cn

C#:   u is User
来源：http://ab.lnxyls.cn

[G14] 数据类 / record
来源：http://bf.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hk.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://px.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ox.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://eq.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ik.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://pq.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://em.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://sc.wgjwhj.cn

[G15] 枚举
来源：http://bp.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nb.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ma.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tx.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eq.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://hn.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zc.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://mr.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://be.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://dt.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ee.bjjhwx.cn


<!-- 参考信息 -->