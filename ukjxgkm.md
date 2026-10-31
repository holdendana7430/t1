代发 wailian999

[E18] 模板占位符替换
来源：http://bb.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wq.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bi.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ba.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dx.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nl.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mt.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mo.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nx.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://od.chemitech.net.cn

Py:   s.splitlines()
来源：http://ve.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://eg.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://pl.9csxet.cn

Java: s.lines().toList()
来源：http://bw.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://yd.muxihuayi.cn

Ruby: s.lines
来源：http://wx.shtwfgs.cn

C#:   s.Split('\n')
来源：http://td.asd995.cn

[E20] 判断字符串是否为空
来源：http://gv.bjjhwx.cn

Py:   if not s:
来源：http://ca.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://js.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pf.hnjuh.cn

TS:   if (s === "") {}
来源：http://no.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://mt.yuexingan06.cn

Go:   if s == "" {}
来源：http://ge.521024.cn

Ruby: if s.empty?
来源：http://fp.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kz.newstarts.cn

[E21] 超长截断加省略号
来源：http://tg.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ay.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nu.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xq.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nx.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nw.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ws.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fo.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pt.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://pl.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://va.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qo.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dw.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://va.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://no.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://we.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://ca.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://my.hahajie.cn

================================================================================
来源：http://dk.hahajie.cn

F. 文件与目录
来源：http://ja.szsharing.cn

================================================================================
来源：http://km.hnjuh.cn

[F01] 读取整个文件
来源：http://fa.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://em.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://gb.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mj.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bv.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bs.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ld.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://hx.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://kn.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ss.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zd.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jh.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uw.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wf.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vi.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kq.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gc.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rm.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://dh.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ky.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rl.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dd.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kt.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tx.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tt.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://sh.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hr.huanxung.cn

[F04] 追加写入文件
来源：http://yk.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pg.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iv.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ue.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ch.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sp.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cv.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nk.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yy.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://oe.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tt.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ik.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://gg.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://vm.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xy.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gv.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://po.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://lo.haigaiapp.cn

[F06] 删除文件
来源：http://qg.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://to.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://vy.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bv.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://js.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oi.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://hb.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://rx.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://hq.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ff.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ku.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ex.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fd.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kx.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mq.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gj.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bk.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rt.szxytkj.cn

[F08] 遍历目录
来源：http://nw.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xn.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://en.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://fr.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://zi.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ye.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gz.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://pr.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://mg.shxzskj.cn

[F09] 获取文件大小
来源：http://xh.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://hz.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://lk.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://fs.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://we.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ej.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pl.asd995.cn

Ruby: File.size("a.txt")
来源：http://et.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://vr.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://lq.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://he.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sb.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fh.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://bj.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gp.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ns.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wk.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bp.nszjky.cn

[F11] 复制与移动文件
来源：http://zn.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dw.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lb.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ct.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yc.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kr.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ls.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iv.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nv.huixinmuqiang.cn

[F12] CSV 读写
来源：http://rp.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tj.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://we.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tf.hahajie.cn

TS:   // 同上
来源：http://cv.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://so.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vf.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dm.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ry.newstarts.cn

================================================================================
来源：http://ci.newstarts.cn

G. 面向对象
来源：http://om.asd995.cn

================================================================================
来源：http://uk.huixinmuqiang.cn

[G01] 定义类
来源：http://sa.chemitech.net.cn

Py:   class User: pass
来源：http://ns.muxihuayi.cn

PHP:  class User {}
来源：http://qm.yuntaijiaju.cn

JS:   class User {}
来源：http://ln.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://jf.shxzukj.cn

Java: class User {}
来源：http://ii.lnxyls.cn

Go:   type User struct { Name string }
来源：http://nx.yuntaijiaju.cn

Ruby: class User; end
来源：http://km.wgjwhj.cn

C#:   class User {}
来源：http://vq.hnjuh.cn

[G02] 构造函数
来源：http://yp.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://bj.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://we.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://id.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://tx.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://cy.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nq.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://al.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://by.gzmigu.cn

[G03] 实例属性
来源：http://ia.huixiangedu.cn

Py:   self.name = "x"
来源：http://la.hnjuh.cn

PHP:  public string $name = "x";
来源：http://fo.szsharing.cn

JS:   this.name = "x";
来源：http://gw.hahajie.cn

TS:   name: string = "x";
来源：http://xr.newstarts.cn

Java: private String name;
来源：http://wg.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ju.panjiajie.cn

Ruby: @name = "x"
来源：http://ph.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://ag.colortex.cn

[G04] 定义方法
来源：http://wo.nicolike.cn

Py:   def greet(self): return self.name
来源：http://ds.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pn.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ow.521024.cn

TS:   greet(): string { return this.name; }
来源：http://un.jctech888.com.cn

Java: String greet() { return name; }
来源：http://le.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fk.lnxyls.cn

Ruby: def greet; @name; end
来源：http://gy.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://wk.bjjhwx.cn

[G05] 继承
来源：http://me.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ky.hahajie.cn

PHP:  class Admin extends User {}
来源：http://fs.521024.cn

JS:   class Admin extends User {}
来源：http://yv.huanxung.cn

TS:   class Admin extends User {}
来源：http://xz.wgjwhj.cn

Java: class Admin extends User {}
来源：http://va.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ct.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://kk.9csxet.cn

C#:   class Admin : User {}
来源：http://mz.shxzskj.cn

[G06] 重写方法
来源：http://yv.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://ql.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kr.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://yw.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://ur.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://zc.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ke.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://fz.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://hg.colortex.cn

[G07] 调用父类方法
来源：http://li.bookmarksfly.cn

Py:   super().greet()
来源：http://vd.wgjwhj.cn

PHP:  parent::greet();
来源：http://im.bjjhwx.cn

JS:   super.greet();
来源：http://hw.yuntaijiaju.cn

TS:   super.greet();
来源：http://tf.szxytkj.cn

Java: super.greet();
来源：http://tt.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sq.wgjwhj.cn

Ruby: super
来源：http://lu.9csxet.cn

C#:   base.Greet();
来源：http://bt.szxytkj.cn

[G08] 静态方法与属性
来源：http://vm.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bc.hahajie.cn

PHP:  public static function f() {}
来源：http://sm.nszjky.cn

JS:   static f() {}
来源：http://pr.lnxyls.cn

TS:   static f(): void {}
来源：http://ea.nszjky.cn

Java: static void f() {}
来源：http://bv.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hh.nszjky.cn

Ruby: def self.f; end
来源：http://zo.521024.cn

C#:   public static void F() {}
来源：http://ui.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://kl.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://lr.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://du.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kj.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://jv.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://wk.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://zk.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ah.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://nq.521024.cn

[G10] 访问控制
来源：http://yw.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://gk.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://tm.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://sw.huixinmuqiang.cn

TS:   public / protected / private
来源：http://ek.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://qj.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://os.lnxyls.cn

Ruby: public / protected / private
来源：http://hj.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://pg.asd995.cn

[G11] getter / setter
来源：http://mt.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://bk.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fu.521024.cn

JS:   get name() { return this._name; }
来源：http://sd.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://tm.colortex.cn

Java: public String getName() { return name; }
来源：http://vl.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zg.nszjky.cn

Ruby: attr_accessor :name
来源：http://mv.asd995.cn

C#:   public string Name { get; set; }
来源：http://kn.9csxet.cn

[G12] 对象转字符串
来源：http://gm.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://gk.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pq.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://el.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://fq.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://yg.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mm.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://uc.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://ou.newstarts.cn

[G13] 判断对象类型
来源：http://tq.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://xq.huixiangedu.cn

PHP:  $u instanceof User
来源：http://jg.szxytkj.cn

JS:   u instanceof User
来源：http://ay.huixinmuqiang.cn

TS:   u instanceof User
来源：http://yd.shxzskj.cn

Java: u instanceof User
来源：http://hx.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gl.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://hd.muxihuayi.cn

C#:   u is User
来源：http://cj.szxytkj.cn

[G14] 数据类 / record
来源：http://zb.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lh.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://iz.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://az.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://mx.colortex.cn

Java: record User(String name, int age) {}
来源：http://xx.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://mb.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aw.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://xh.9csxet.cn

[G15] 枚举
来源：http://kd.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dr.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kk.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dm.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qo.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ft.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ys.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://rg.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yk.colortex.cn

[G16] 对象转数组 / 字典
来源：http://qe.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qj.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://lx.szxytkj.cn

JS:   Object.entries(obj)
来源：http://iw.hahajie.cn

TS:   Object.entries(obj)
来源：http://nx.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yx.panjiajie.cn


<!-- 参考信息 -->