代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hg.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oo.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oi.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://np.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kr.asd995.cn

[E19] 多行文本按行拆分
来源：http://fx.wgjwhj.cn

Py:   s.splitlines()
来源：http://tc.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tb.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://zu.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://dc.newstarts.cn

Java: s.lines().toList()
来源：http://vr.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://nj.9csxet.cn

Ruby: s.lines
来源：http://oe.szsharing.cn

C#:   s.Split('\n')
来源：http://ma.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://zq.521024.cn

Py:   if not s:
来源：http://wh.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zk.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qn.szxytkj.cn

TS:   if (s === "") {}
来源：http://ss.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://wp.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://st.nicolike.cn

Ruby: if s.empty?
来源：http://dl.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yp.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://tf.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bx.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jn.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yn.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wl.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qe.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://np.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mz.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zs.hahajie.cn

[E22] 字节长度与字符长度
来源：http://jx.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hb.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://te.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://df.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ya.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ia.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ad.521024.cn

Ruby: s.bytesize;  s.length
来源：http://lv.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oc.hahajie.cn

================================================================================
来源：http://qz.bjjhwx.cn

F. 文件与目录
来源：http://np.shxzukj.cn

================================================================================
来源：http://rs.newstarts.cn

[F01] 读取整个文件
来源：http://pk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cp.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://ru.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ee.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ll.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bl.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wg.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://qc.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://go.huixiangedu.cn

[F02] 逐行读取文件
来源：http://xy.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xe.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dv.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mw.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tw.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oi.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://af.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jw.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nx.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://xi.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://go.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sr.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gy.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ko.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fn.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mk.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://yi.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ti.shtwfgs.cn

[F04] 追加写入文件
来源：http://ct.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dz.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gt.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qk.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ic.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ig.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://do.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://um.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sd.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://xu.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pm.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://pm.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://fm.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://ya.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gv.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dc.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://sq.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://bn.lnxyls.cn

[F06] 删除文件
来源：http://bb.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://cd.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://ak.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://js.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zv.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lp.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://qr.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://kd.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://ci.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://xg.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qj.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rx.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nd.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rc.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gp.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dc.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://am.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lw.huixiangedu.cn

[F08] 遍历目录
来源：http://sh.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fe.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://do.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://qg.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ck.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aw.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ut.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://yk.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://yk.9csxet.cn

[F09] 获取文件大小
来源：http://cm.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://fz.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://do.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ci.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://me.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fd.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lf.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ft.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://js.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://rg.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://an.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zi.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://np.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://yj.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tk.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fm.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ko.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rn.jctech888.com.cn

[F11] 复制与移动文件
来源：http://xv.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ka.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vd.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://np.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sw.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mu.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://be.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bb.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ng.bookmarksfly.cn

[F12] CSV 读写
来源：http://vi.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rk.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tx.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://of.panjiajie.cn

TS:   // 同上
来源：http://lg.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kq.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ax.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fh.bookmarksfly.cn

================================================================================
来源：http://mx.bjjhwx.cn

G. 面向对象
来源：http://jb.9csxet.cn

================================================================================
来源：http://ly.huixiangedu.cn

[G01] 定义类
来源：http://ti.colortex.cn

Py:   class User: pass
来源：http://hh.panjiajie.cn

PHP:  class User {}
来源：http://nm.newstarts.cn

JS:   class User {}
来源：http://nb.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://lo.gzmigu.cn

Java: class User {}
来源：http://io.nicolike.cn

Go:   type User struct { Name string }
来源：http://jg.nicolike.cn

Ruby: class User; end
来源：http://yr.asd995.cn

C#:   class User {}
来源：http://dr.gzmigu.cn

[G02] 构造函数
来源：http://tl.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://ts.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://el.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://mf.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ue.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://it.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ax.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://vd.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://kk.lnxyls.cn

[G03] 实例属性
来源：http://cv.gzmigu.cn

Py:   self.name = "x"
来源：http://ww.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://ol.nszjky.cn

JS:   this.name = "x";
来源：http://en.huixiangedu.cn

TS:   name: string = "x";
来源：http://ax.shxzskj.cn

Java: private String name;
来源：http://na.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tn.bookmarksfly.cn

Ruby: @name = "x"
来源：http://su.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ue.lnxyls.cn

[G04] 定义方法
来源：http://qi.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://wp.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qc.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://qe.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://yp.shxzukj.cn

Java: String greet() { return name; }
来源：http://ul.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sl.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://xq.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://es.shxzukj.cn

[G05] 继承
来源：http://ww.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://eg.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://sg.hahajie.cn

JS:   class Admin extends User {}
来源：http://ub.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://wn.shxzskj.cn

Java: class Admin extends User {}
来源：http://bq.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fb.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://xn.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://rj.521024.cn

[G06] 重写方法
来源：http://xh.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ka.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zy.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://jb.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://cz.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://gi.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://as.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://yk.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://jh.bjjhwx.cn

[G07] 调用父类方法
来源：http://bg.colortex.cn

Py:   super().greet()
来源：http://ls.wgjwhj.cn

PHP:  parent::greet();
来源：http://br.hnjuh.cn

JS:   super.greet();
来源：http://mk.szxytkj.cn

TS:   super.greet();
来源：http://yn.shxzukj.cn

Java: super.greet();
来源：http://ye.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://un.szxytkj.cn

Ruby: super
来源：http://pc.hahajie.cn

C#:   base.Greet();
来源：http://of.hahajie.cn

[G08] 静态方法与属性
来源：http://dj.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kv.muxihuayi.cn

PHP:  public static function f() {}
来源：http://fw.szxytkj.cn

JS:   static f() {}
来源：http://xl.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://dw.shtwfgs.cn

Java: static void f() {}
来源：http://ta.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ip.wgjwhj.cn

Ruby: def self.f; end
来源：http://ei.haigaiapp.cn

C#:   public static void F() {}
来源：http://rw.nicolike.cn

[G09] 接口 / 抽象类
来源：http://fo.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://fd.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wx.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ty.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://df.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://qj.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://ke.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xa.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://op.bookmarksfly.cn

[G10] 访问控制
来源：http://hn.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://sa.bookmarksfly.cn

PHP:  public / protected / private
来源：http://sv.9csxet.cn

JS:   #private 字段；其余公开
来源：http://jg.huanxung.cn

TS:   public / protected / private
来源：http://qw.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://ij.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dv.gzmigu.cn

Ruby: public / protected / private
来源：http://tw.lnxyls.cn

C#:   public / protected / private / internal
来源：http://ko.yuntaijiaju.cn

[G11] getter / setter
来源：http://mk.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://ib.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zg.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://lh.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://mn.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://yh.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gb.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://vf.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://ys.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://bj.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://je.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tq.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://kv.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://zt.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://px.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xg.szsharing.cn

Ruby: def to_s; @name; end
来源：http://jk.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://xb.panjiajie.cn

[G13] 判断对象类型
来源：http://ys.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://xk.gzmigu.cn

PHP:  $u instanceof User
来源：http://yk.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ru.yuexingan06.cn

TS:   u instanceof User
来源：http://ap.wgjwhj.cn

Java: u instanceof User
来源：http://lw.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aa.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://pp.huixiangedu.cn

C#:   u is User
来源：http://ch.hahajie.cn

[G14] 数据类 / record
来源：http://fw.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ne.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://bw.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sx.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://nt.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ye.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://vl.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nr.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://vw.jianghongdianzi.cn

[G15] 枚举
来源：http://wl.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nn.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lb.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ye.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kz.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://wc.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://is.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://hc.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dv.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://vt.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mm.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://et.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://hx.newstarts.cn

TS:   Object.entries(obj)
来源：http://ic.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lk.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://um.nicolike.cn

Ruby: obj.instance_variables
来源：http://qg.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://wd.yuexingan06.cn

================================================================================
来源：http://ve.szsharing.cn


<!-- 参考信息 -->