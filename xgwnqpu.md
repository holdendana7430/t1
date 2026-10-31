代发 wailian999

[E18] 模板占位符替换
来源：http://tu.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ho.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wh.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xh.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iy.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://is.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fg.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gd.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ts.hahajie.cn

[E19] 多行文本按行拆分
来源：http://xu.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://vt.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vq.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://jw.521024.cn

TS:   s.split(/\r?\n/)
来源：http://pd.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ln.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ud.muxihuayi.cn

Ruby: s.lines
来源：http://dy.szxytkj.cn

C#:   s.Split('\n')
来源：http://fm.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ns.nicolike.cn

Py:   if not s:
来源：http://vw.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ib.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zi.asd995.cn

TS:   if (s === "") {}
来源：http://uh.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ua.yuexingan06.cn

Go:   if s == "" {}
来源：http://jj.chemitech.net.cn

Ruby: if s.empty?
来源：http://lk.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uu.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://vv.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jf.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ht.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sl.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eu.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pm.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://dz.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vu.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xs.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://cb.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zm.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://us.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mo.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ci.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lv.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ei.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://eh.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rh.nicolike.cn

================================================================================
来源：http://fd.panjiajie.cn

F. 文件与目录
来源：http://kw.lnxyls.cn

================================================================================
来源：http://il.gzmigu.cn

[F01] 读取整个文件
来源：http://wq.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rp.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://da.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ek.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jj.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pq.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mb.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://im.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://zt.yuexingan06.cn

[F02] 逐行读取文件
来源：http://tc.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qg.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zk.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rd.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ub.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eq.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dl.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dh.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ga.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ol.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ds.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ql.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gw.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mu.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ng.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vh.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://qo.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ag.bookmarksfly.cn

[F04] 追加写入文件
来源：http://kc.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vl.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ud.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iv.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yn.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mf.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wf.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ge.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xp.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://ne.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://at.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://rp.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://nb.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://le.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vh.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ls.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://gg.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ga.hahajie.cn

[F06] 删除文件
来源：http://cf.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://qt.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://zm.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://av.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fa.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jc.asd995.cn

Go:   os.Remove("a.txt")
来源：http://pt.asd995.cn

Ruby: File.delete("a.txt")
来源：http://my.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://yc.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ns.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ro.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xe.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jv.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dz.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://km.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ut.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://md.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hu.asd995.cn

[F08] 遍历目录
来源：http://yz.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ua.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cd.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://jc.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ai.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wj.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://de.9csxet.cn

Ruby: Dir.children("dir")
来源：http://db.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ih.szsharing.cn

[F09] 获取文件大小
来源：http://bd.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://bs.521024.cn

PHP:  filesize("a.txt");
来源：http://bw.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://fz.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://cz.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://or.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gy.huanxung.cn

Ruby: File.size("a.txt")
来源：http://kr.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://sx.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://wm.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nz.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fi.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://da.szsharing.cn

TS:   path.extname("a.txt")
来源：http://vo.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xn.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gi.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sw.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yp.nicolike.cn

[F11] 复制与移动文件
来源：http://ua.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jj.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hi.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cj.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ei.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://io.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xy.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ea.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://la.lnxyls.cn

[F12] CSV 读写
来源：http://zp.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dw.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kw.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oa.yuexingan06.cn

TS:   // 同上
来源：http://bk.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://id.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xl.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nr.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mk.muxihuayi.cn

================================================================================
来源：http://ky.yuntaijiaju.cn

G. 面向对象
来源：http://aq.jianghongdianzi.cn

================================================================================
来源：http://wo.huixinmuqiang.cn

[G01] 定义类
来源：http://hc.nszjky.cn

Py:   class User: pass
来源：http://rc.huixinmuqiang.cn

PHP:  class User {}
来源：http://rg.asd995.cn

JS:   class User {}
来源：http://uh.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://op.newstarts.cn

Java: class User {}
来源：http://xg.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://ay.yuexingan06.cn

Ruby: class User; end
来源：http://zl.newstarts.cn

C#:   class User {}
来源：http://tt.szxytkj.cn

[G02] 构造函数
来源：http://bx.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://iq.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://vh.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://gl.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://by.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://st.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nn.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://us.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://ap.huanxung.cn

[G03] 实例属性
来源：http://hl.szsharing.cn

Py:   self.name = "x"
来源：http://pq.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://wq.bookmarksfly.cn

JS:   this.name = "x";
来源：http://tf.bjjhwx.cn

TS:   name: string = "x";
来源：http://ik.yuexingan06.cn

Java: private String name;
来源：http://ja.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ah.shxzukj.cn

Ruby: @name = "x"
来源：http://vj.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://nc.521024.cn

[G04] 定义方法
来源：http://qe.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ux.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://or.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ur.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://tc.bjjhwx.cn

Java: String greet() { return name; }
来源：http://wo.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vo.panjiajie.cn

Ruby: def greet; @name; end
来源：http://ny.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://nq.gzmigu.cn

[G05] 继承
来源：http://he.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://zv.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://bg.gzmigu.cn

JS:   class Admin extends User {}
来源：http://lv.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://lr.nszjky.cn

Java: class Admin extends User {}
来源：http://ku.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wc.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ry.shxzskj.cn

C#:   class Admin : User {}
来源：http://ml.huixiangedu.cn

[G06] 重写方法
来源：http://ee.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://us.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://aw.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://bq.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://aq.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://op.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lw.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://sk.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://iz.wgjwhj.cn

[G07] 调用父类方法
来源：http://xd.shxzukj.cn

Py:   super().greet()
来源：http://bl.shxzskj.cn

PHP:  parent::greet();
来源：http://oy.huixinmuqiang.cn

JS:   super.greet();
来源：http://rx.yuexingan06.cn

TS:   super.greet();
来源：http://og.chemitech.net.cn

Java: super.greet();
来源：http://fo.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gk.shxzukj.cn

Ruby: super
来源：http://am.shxzskj.cn

C#:   base.Greet();
来源：http://hr.chemitech.net.cn

[G08] 静态方法与属性
来源：http://ih.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aa.huanxung.cn

PHP:  public static function f() {}
来源：http://om.9csxet.cn

JS:   static f() {}
来源：http://hn.bookmarksfly.cn

TS:   static f(): void {}
来源：http://by.asd995.cn

Java: static void f() {}
来源：http://ei.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jv.lnxyls.cn

Ruby: def self.f; end
来源：http://lh.muxihuayi.cn

C#:   public static void F() {}
来源：http://wv.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://dd.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ca.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ra.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rn.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://rq.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://ms.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ny.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ji.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://pf.nszjky.cn

[G10] 访问控制
来源：http://hh.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://qh.muxihuayi.cn

PHP:  public / protected / private
来源：http://nl.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://ok.yuntaijiaju.cn

TS:   public / protected / private
来源：http://aj.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://pt.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pr.yuexingan06.cn

Ruby: public / protected / private
来源：http://yl.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://cr.huixiangedu.cn

[G11] getter / setter
来源：http://ha.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://rg.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fn.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://tp.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://wr.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://fh.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ee.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://cm.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://xn.shxzskj.cn

[G12] 对象转字符串
来源：http://yb.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://hy.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cb.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://vd.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://pk.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ou.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sz.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://il.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://tq.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://mn.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://rp.gzmigu.cn

PHP:  $u instanceof User
来源：http://li.lnxyls.cn

JS:   u instanceof User
来源：http://ne.yuexingan06.cn

TS:   u instanceof User
来源：http://ie.shxzskj.cn

Java: u instanceof User
来源：http://tr.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zd.nicolike.cn

Ruby: u.is_a?(User)
来源：http://dg.yuntaijiaju.cn

C#:   u is User
来源：http://wx.haigaiapp.cn

[G14] 数据类 / record
来源：http://zi.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pj.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rq.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ve.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://xp.521024.cn

Java: record User(String name, int age) {}
来源：http://iv.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://rh.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cg.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://ec.szxytkj.cn

[G15] 枚举
来源：http://sb.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ew.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lj.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hb.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oi.521024.cn

Java: enum Color { RED, GREEN }
来源：http://mi.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ql.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://ep.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uy.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://qa.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mx.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://zz.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://mz.huanxung.cn

TS:   Object.entries(obj)
来源：http://kb.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rj.panjiajie.cn


<!-- 参考信息 -->