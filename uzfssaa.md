代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://bu.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nz.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fj.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gl.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oj.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://cv.chemitech.net.cn

Py:   s.splitlines()
来源：http://jb.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ov.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://xk.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://pn.huanxung.cn

Java: s.lines().toList()
来源：http://zf.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://gn.yuexingan06.cn

Ruby: s.lines
来源：http://fe.shxzskj.cn

C#:   s.Split('\n')
来源：http://kj.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ib.szxytkj.cn

Py:   if not s:
来源：http://xz.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zj.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vm.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://id.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://al.chemitech.net.cn

Go:   if s == "" {}
来源：http://ws.nszjky.cn

Ruby: if s.empty?
来源：http://ex.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ym.panjiajie.cn

[E21] 超长截断加省略号
来源：http://jx.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yz.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nd.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pg.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jw.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jb.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ot.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bm.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://md.9csxet.cn

[E22] 字节长度与字符长度
来源：http://qw.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cx.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ql.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mn.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sx.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vx.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vm.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://my.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uv.wgjwhj.cn

================================================================================
来源：http://ld.nszjky.cn

F. 文件与目录
来源：http://lm.jianghongdianzi.cn

================================================================================
来源：http://mt.asd995.cn

[F01] 读取整个文件
来源：http://xh.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yx.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://ra.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vq.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mz.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oy.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xf.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://yr.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://wc.szxytkj.cn

[F02] 逐行读取文件
来源：http://bm.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fz.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dp.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jv.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://av.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ku.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oj.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iq.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vh.colortex.cn

[F03] 写入文件（覆盖）
来源：http://nl.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ha.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wx.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jn.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wh.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zy.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jn.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ha.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jd.nszjky.cn

[F04] 追加写入文件
来源：http://ni.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pu.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pi.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ot.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bq.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bs.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fi.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://is.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nn.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://rt.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kv.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://fn.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://ap.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://gd.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mv.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wh.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://oe.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://wr.shxzskj.cn

[F06] 删除文件
来源：http://re.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://sd.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://xx.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vx.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xs.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jj.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ta.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ws.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://rb.huanxung.cn

[F07] 创建目录（含多级）
来源：http://xb.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kp.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yp.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tf.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gy.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tm.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lr.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nn.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ru.newstarts.cn

[F08] 遍历目录
来源：http://rn.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ej.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hi.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://gd.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://vb.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hw.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fn.newstarts.cn

Ruby: Dir.children("dir")
来源：http://sa.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://di.lnxyls.cn

[F09] 获取文件大小
来源：http://ef.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://xy.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://wj.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://gk.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://xe.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://er.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xu.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://gq.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://xh.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://di.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kn.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gc.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kq.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://is.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qk.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://py.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qu.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mp.huanxung.cn

[F11] 复制与移动文件
来源：http://jj.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vs.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qe.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fb.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pn.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ss.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hs.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qb.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ar.yuexingan06.cn

[F12] CSV 读写
来源：http://yv.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zb.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ea.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wg.huanxung.cn

TS:   // 同上
来源：http://ec.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kt.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dz.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gu.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hk.nicolike.cn

================================================================================
来源：http://fm.szsharing.cn

G. 面向对象
来源：http://ww.gzmigu.cn

================================================================================
来源：http://ad.panjiajie.cn

[G01] 定义类
来源：http://dk.nszjky.cn

Py:   class User: pass
来源：http://ou.shxzskj.cn

PHP:  class User {}
来源：http://gr.szxytkj.cn

JS:   class User {}
来源：http://zw.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://so.hahajie.cn

Java: class User {}
来源：http://oz.nszjky.cn

Go:   type User struct { Name string }
来源：http://bb.hahajie.cn

Ruby: class User; end
来源：http://st.jctech888.com.cn

C#:   class User {}
来源：http://xc.newstarts.cn

[G02] 构造函数
来源：http://tp.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ni.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://cr.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://bz.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://nn.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ig.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yf.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://by.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://xg.szsharing.cn

[G03] 实例属性
来源：http://po.haigaiapp.cn

Py:   self.name = "x"
来源：http://hg.shxzskj.cn

PHP:  public string $name = "x";
来源：http://gd.muxihuayi.cn

JS:   this.name = "x";
来源：http://ut.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://zn.huanxung.cn

Java: private String name;
来源：http://ti.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.asd995.cn

Ruby: @name = "x"
来源：http://eo.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://fj.jianghongdianzi.cn

[G04] 定义方法
来源：http://hl.huanxung.cn

Py:   def greet(self): return self.name
来源：http://si.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bq.hahajie.cn

JS:   greet() { return this.name; }
来源：http://xc.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://te.521024.cn

Java: String greet() { return name; }
来源：http://jn.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xg.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://dp.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://fh.nicolike.cn

[G05] 继承
来源：http://pa.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://qr.9csxet.cn

PHP:  class Admin extends User {}
来源：http://kh.newstarts.cn

JS:   class Admin extends User {}
来源：http://ux.hahajie.cn

TS:   class Admin extends User {}
来源：http://wl.gzmigu.cn

Java: class Admin extends User {}
来源：http://jk.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nk.szsharing.cn

Ruby: class Admin < User; end
来源：http://ld.jctech888.com.cn

C#:   class Admin : User {}
来源：http://hc.9csxet.cn

[G06] 重写方法
来源：http://fc.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://pp.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://az.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://bt.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://up.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://cd.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fj.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://gh.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://vi.521024.cn

[G07] 调用父类方法
来源：http://rz.panjiajie.cn

Py:   super().greet()
来源：http://ou.lnxyls.cn

PHP:  parent::greet();
来源：http://rq.bjjhwx.cn

JS:   super.greet();
来源：http://zc.colortex.cn

TS:   super.greet();
来源：http://lb.lnxyls.cn

Java: super.greet();
来源：http://ke.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jr.shxzskj.cn

Ruby: super
来源：http://ou.hahajie.cn

C#:   base.Greet();
来源：http://ct.lnxyls.cn

[G08] 静态方法与属性
来源：http://iw.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pw.jctech888.com.cn

PHP:  public static function f() {}
来源：http://hl.huanxung.cn

JS:   static f() {}
来源：http://li.wgjwhj.cn

TS:   static f(): void {}
来源：http://qj.colortex.cn

Java: static void f() {}
来源：http://by.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://es.521024.cn

Ruby: def self.f; end
来源：http://ub.shtwfgs.cn

C#:   public static void F() {}
来源：http://mc.szsharing.cn

[G09] 接口 / 抽象类
来源：http://yb.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://ka.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wc.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fl.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://kn.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://qy.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://nk.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xr.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://wm.panjiajie.cn

[G10] 访问控制
来源：http://nn.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://oe.nicolike.cn

PHP:  public / protected / private
来源：http://fx.colortex.cn

JS:   #private 字段；其余公开
来源：http://xy.bjjhwx.cn

TS:   public / protected / private
来源：http://js.colortex.cn

Java: public / protected / private / 默认包级
来源：http://lb.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vy.nicolike.cn

Ruby: public / protected / private
来源：http://we.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://tq.huixinmuqiang.cn

[G11] getter / setter
来源：http://qc.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://uj.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eh.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://nf.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://rq.521024.cn

Java: public String getName() { return name; }
来源：http://dd.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gk.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://yv.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://wi.szsharing.cn

[G12] 对象转字符串
来源：http://ai.asd995.cn

Py:   def __str__(self): return self.name
来源：http://lt.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qn.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://gm.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://gp.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://ne.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://po.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://jb.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://xj.lnxyls.cn

[G13] 判断对象类型
来源：http://cr.hahajie.cn

Py:   isinstance(u, User)
来源：http://jc.asd995.cn

PHP:  $u instanceof User
来源：http://zz.shxzukj.cn

JS:   u instanceof User
来源：http://ja.521024.cn

TS:   u instanceof User
来源：http://ha.muxihuayi.cn

Java: u instanceof User
来源：http://fi.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ff.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://gk.wgjwhj.cn

C#:   u is User
来源：http://fs.hahajie.cn

[G14] 数据类 / record
来源：http://ck.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zx.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://dk.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kj.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://wt.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://wa.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ej.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rk.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://re.lnxyls.cn

[G15] 枚举
来源：http://br.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://em.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tt.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rj.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fn.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://rs.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ep.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://tf.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cd.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://fz.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yk.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://ti.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://gl.9csxet.cn

TS:   Object.entries(obj)
来源：http://hk.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ri.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qm.asd995.cn

Ruby: obj.instance_variables
来源：http://yv.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://uy.shxzukj.cn

================================================================================
来源：http://pr.521024.cn


<!-- 参考信息 -->