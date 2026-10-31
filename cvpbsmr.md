代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wn.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lf.wgjwhj.cn

Ruby: s.capitalize
来源：http://fj.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iz.shtwfgs.cn

[E18] 模板占位符替换
来源：http://mf.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ff.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pk.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lp.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vo.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jw.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://si.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://wp.szsharing.cn

Py:   s.splitlines()
来源：http://hc.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wy.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ba.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://wp.bjjhwx.cn

Java: s.lines().toList()
来源：http://uu.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://zn.yuntaijiaju.cn

Ruby: s.lines
来源：http://tu.shxzukj.cn

C#:   s.Split('\n')
来源：http://ss.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://od.szsharing.cn

Py:   if not s:
来源：http://rw.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://he.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gu.colortex.cn

TS:   if (s === "") {}
来源：http://tc.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://ea.newstarts.cn

Go:   if s == "" {}
来源：http://ip.wgjwhj.cn

Ruby: if s.empty?
来源：http://aa.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vo.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ez.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vf.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yc.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xy.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://da.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kw.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://nl.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hj.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://js.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://hn.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ar.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://um.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bj.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oh.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://on.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mp.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://ri.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qu.bjjhwx.cn

================================================================================
来源：http://ko.shxzukj.cn

F. 文件与目录
来源：http://ns.hahajie.cn

================================================================================
来源：http://ps.nicolike.cn

[F01] 读取整个文件
来源：http://lb.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rk.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://ew.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ls.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bt.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lc.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ew.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://bo.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://uo.bjjhwx.cn

[F02] 逐行读取文件
来源：http://dc.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cx.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pv.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lw.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gs.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ol.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bg.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aj.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fk.asd995.cn

[F03] 写入文件（覆盖）
来源：http://bs.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mq.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qj.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wy.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aw.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ot.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://np.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ax.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iw.colortex.cn

[F04] 追加写入文件
来源：http://kw.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://re.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oh.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mv.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ts.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tb.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fc.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ft.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rn.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://wa.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zy.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://ao.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://wa.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://cr.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zs.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://im.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://bn.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://xx.huixinmuqiang.cn

[F06] 删除文件
来源：http://kp.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://qz.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://fy.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lz.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dp.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://om.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://gi.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://dc.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://zt.hahajie.cn

[F07] 创建目录（含多级）
来源：http://jp.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xj.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ny.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hd.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gy.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ln.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ho.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xe.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cs.muxihuayi.cn

[F08] 遍历目录
来源：http://dc.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cs.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qm.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://bt.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://si.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uz.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pg.hahajie.cn

Ruby: Dir.children("dir")
来源：http://rp.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://mc.muxihuayi.cn

[F09] 获取文件大小
来源：http://uo.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://ti.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://jf.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://km.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://ht.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://im.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dd.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ce.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://pt.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://tt.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fm.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tk.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ew.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://ml.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ao.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fj.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mh.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ep.chemitech.net.cn

[F11] 复制与移动文件
来源：http://wq.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uv.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fd.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ae.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qf.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tv.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yc.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://et.bjjhwx.cn

[F12] CSV 读写
来源：http://ft.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tp.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bk.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://an.huixiangedu.cn

TS:   // 同上
来源：http://tg.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bo.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ak.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dc.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dq.huanxung.cn

================================================================================
来源：http://ns.wgjwhj.cn

G. 面向对象
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://ci.huixiangedu.cn

[G01] 定义类
来源：http://bb.haigaiapp.cn

Py:   class User: pass
来源：http://lm.newstarts.cn

PHP:  class User {}
来源：http://rk.panjiajie.cn

JS:   class User {}
来源：http://ku.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://di.chemitech.net.cn

Java: class User {}
来源：http://sw.shxzukj.cn

Go:   type User struct { Name string }
来源：http://xj.shxzskj.cn

Ruby: class User; end
来源：http://nx.yuntaijiaju.cn

C#:   class User {}
来源：http://ku.panjiajie.cn

[G02] 构造函数
来源：http://tb.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://ja.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://bl.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://sy.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://hz.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://pe.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tv.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ye.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://kl.shxzskj.cn

[G03] 实例属性
来源：http://sq.hnjuh.cn

Py:   self.name = "x"
来源：http://il.shxzukj.cn

PHP:  public string $name = "x";
来源：http://ho.asd995.cn

JS:   this.name = "x";
来源：http://xv.szsharing.cn

TS:   name: string = "x";
来源：http://hz.yuntaijiaju.cn

Java: private String name;
来源：http://ac.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ab.asd995.cn

Ruby: @name = "x"
来源：http://zv.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://sg.szsharing.cn

[G04] 定义方法
来源：http://of.nicolike.cn

Py:   def greet(self): return self.name
来源：http://si.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://te.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://zi.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://rd.nszjky.cn

Java: String greet() { return name; }
来源：http://bj.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ov.hahajie.cn

Ruby: def greet; @name; end
来源：http://zq.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://js.hnjuh.cn

[G05] 继承
来源：http://nw.shxzskj.cn

Py:   class Admin(User): pass
来源：http://yj.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://zu.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://wc.newstarts.cn

TS:   class Admin extends User {}
来源：http://jg.lnxyls.cn

Java: class Admin extends User {}
来源：http://um.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yi.hahajie.cn

Ruby: class Admin < User; end
来源：http://xf.shxzskj.cn

C#:   class Admin : User {}
来源：http://dq.szxytkj.cn

[G06] 重写方法
来源：http://ij.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://kq.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jh.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://ds.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://kq.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://jo.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://az.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://xw.521024.cn

C#:   public override string Greet() => "admin";
来源：http://sz.521024.cn

[G07] 调用父类方法
来源：http://lm.yuntaijiaju.cn

Py:   super().greet()
来源：http://vx.huanxung.cn

PHP:  parent::greet();
来源：http://ez.521024.cn

JS:   super.greet();
来源：http://pm.szxytkj.cn

TS:   super.greet();
来源：http://ps.shtwfgs.cn

Java: super.greet();
来源：http://cv.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uy.asd995.cn

Ruby: super
来源：http://vm.szsharing.cn

C#:   base.Greet();
来源：http://pe.shxzukj.cn

[G08] 静态方法与属性
来源：http://ib.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eq.9csxet.cn

PHP:  public static function f() {}
来源：http://jz.huanxung.cn

JS:   static f() {}
来源：http://bo.yuexingan06.cn

TS:   static f(): void {}
来源：http://vv.shtwfgs.cn

Java: static void f() {}
来源：http://dn.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uv.bookmarksfly.cn

Ruby: def self.f; end
来源：http://wr.haigaiapp.cn

C#:   public static void F() {}
来源：http://uh.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://jy.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://vw.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rc.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nw.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://xh.huanxung.cn

Java: interface Shape { double area(); }
来源：http://rd.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://eh.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cl.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://sy.colortex.cn

[G10] 访问控制
来源：http://ao.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://fs.yuexingan06.cn

PHP:  public / protected / private
来源：http://cj.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://yo.hahajie.cn

TS:   public / protected / private
来源：http://eu.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://mx.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ic.shxzukj.cn

Ruby: public / protected / private
来源：http://oe.lnxyls.cn

C#:   public / protected / private / internal
来源：http://wv.huanxung.cn

[G11] getter / setter
来源：http://de.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://nw.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mm.nszjky.cn

JS:   get name() { return this._name; }
来源：http://ak.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://gw.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://er.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ey.colortex.cn

Ruby: attr_accessor :name
来源：http://xh.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://ky.haigaiapp.cn

[G12] 对象转字符串
来源：http://hg.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://ih.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ml.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://bs.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://hf.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://ht.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cu.hahajie.cn

Ruby: def to_s; @name; end
来源：http://vt.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://yq.jctech888.com.cn

[G13] 判断对象类型
来源：http://fy.huanxung.cn

Py:   isinstance(u, User)
来源：http://th.yuexingan06.cn

PHP:  $u instanceof User
来源：http://tr.huixiangedu.cn

JS:   u instanceof User
来源：http://ji.jctech888.com.cn

TS:   u instanceof User
来源：http://hc.9csxet.cn

Java: u instanceof User
来源：http://rj.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ht.521024.cn

Ruby: u.is_a?(User)
来源：http://oe.colortex.cn

C#:   u is User
来源：http://bh.colortex.cn

[G14] 数据类 / record
来源：http://ty.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lo.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://cj.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://im.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://br.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://wf.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://ks.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hj.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://kw.asd995.cn

[G15] 枚举
来源：http://hk.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eo.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xf.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fx.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://so.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://jy.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ga.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://sg.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fc.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://wc.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hp.asd995.cn


<!-- 参考信息 -->