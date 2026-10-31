代发 wailian999

[E18] 模板占位符替换
来源：http://qt.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ut.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hs.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gc.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yz.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://us.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qs.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jy.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ok.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://om.gzmigu.cn

Py:   s.splitlines()
来源：http://ld.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ji.521024.cn

JS:   s.split(/\r?\n/)
来源：http://yt.521024.cn

TS:   s.split(/\r?\n/)
来源：http://fh.chemitech.net.cn

Java: s.lines().toList()
来源：http://of.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://nl.lnxyls.cn

Ruby: s.lines
来源：http://ch.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ui.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://qo.panjiajie.cn

Py:   if not s:
来源：http://rv.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://of.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dz.nszjky.cn

TS:   if (s === "") {}
来源：http://op.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://fv.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://gi.colortex.cn

Ruby: if s.empty?
来源：http://nr.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zs.nicolike.cn

[E21] 超长截断加省略号
来源：http://yl.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vf.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gq.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eb.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kc.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lg.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://yg.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hg.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nz.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://cm.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ef.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aq.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sl.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fp.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sq.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://uc.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hb.bjjhwx.cn

================================================================================
来源：http://jo.wgjwhj.cn

F. 文件与目录
来源：http://hd.huanxung.cn

================================================================================
来源：http://pt.yuexingan06.cn

[F01] 读取整个文件
来源：http://gf.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://es.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ll.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://om.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vv.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fv.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uc.9csxet.cn

Ruby: File.read("a.txt")
来源：http://ng.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://pr.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://tu.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zr.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kw.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fg.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pe.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sc.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ge.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gd.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tl.521024.cn

[F03] 写入文件（覆盖）
来源：http://xr.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yd.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://av.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hq.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tb.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nx.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wl.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://at.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xl.szxytkj.cn

[F04] 追加写入文件
来源：http://he.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gh.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cu.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wi.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zq.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jv.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sy.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://do.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://tx.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ve.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://ft.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://xd.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://fi.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xt.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pt.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://hc.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://mi.hnjuh.cn

[F06] 删除文件
来源：http://ra.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://zi.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://qz.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lc.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uc.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://km.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://wl.521024.cn

Ruby: File.delete("a.txt")
来源：http://uf.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://zh.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://mu.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ta.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xb.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cj.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wc.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tc.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ul.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eo.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ai.panjiajie.cn

[F08] 遍历目录
来源：http://jg.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://po.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xe.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://jw.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://rg.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kd.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ws.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ae.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://fp.bookmarksfly.cn

[F09] 获取文件大小
来源：http://jc.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://js.521024.cn

PHP:  filesize("a.txt");
来源：http://cn.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://mg.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://dv.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zb.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rw.nszjky.cn

Ruby: File.size("a.txt")
来源：http://bn.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://kq.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://vj.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://un.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://df.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ix.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kv.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dk.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gb.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cx.szxytkj.cn

[F11] 复制与移动文件
来源：http://hd.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mh.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ma.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://je.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ho.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kn.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rt.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oh.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ti.shtwfgs.cn

[F12] CSV 读写
来源：http://kt.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wk.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dv.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uj.bookmarksfly.cn

TS:   // 同上
来源：http://nf.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ku.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://my.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oc.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nj.newstarts.cn

================================================================================
来源：http://rp.lnxyls.cn

G. 面向对象
来源：http://vy.shxzskj.cn

================================================================================
来源：http://iy.shxzskj.cn

[G01] 定义类
来源：http://wv.shxzukj.cn

Py:   class User: pass
来源：http://cv.bjjhwx.cn

PHP:  class User {}
来源：http://jw.gzmigu.cn

JS:   class User {}
来源：http://vc.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://zm.haigaiapp.cn

Java: class User {}
来源：http://uf.nicolike.cn

Go:   type User struct { Name string }
来源：http://oq.bookmarksfly.cn

Ruby: class User; end
来源：http://fh.huixiangedu.cn

C#:   class User {}
来源：http://jk.hahajie.cn

[G02] 构造函数
来源：http://nj.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://ef.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://td.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://wf.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://oo.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://tx.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pq.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://de.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://uv.shtwfgs.cn

[G03] 实例属性
来源：http://gx.9csxet.cn

Py:   self.name = "x"
来源：http://wx.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://pm.chemitech.net.cn

JS:   this.name = "x";
来源：http://jv.shtwfgs.cn

TS:   name: string = "x";
来源：http://uo.muxihuayi.cn

Java: private String name;
来源：http://ha.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://of.chemitech.net.cn

Ruby: @name = "x"
来源：http://mk.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ck.yuexingan06.cn

[G04] 定义方法
来源：http://jk.521024.cn

Py:   def greet(self): return self.name
来源：http://yq.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ky.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://vx.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://gt.gzmigu.cn

Java: String greet() { return name; }
来源：http://to.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gf.szxytkj.cn

Ruby: def greet; @name; end
来源：http://vx.nicolike.cn

C#:   public string Greet() => Name;
来源：http://oc.huixiangedu.cn

[G05] 继承
来源：http://bq.szsharing.cn

Py:   class Admin(User): pass
来源：http://wo.huanxung.cn

PHP:  class Admin extends User {}
来源：http://tg.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://ej.lnxyls.cn

TS:   class Admin extends User {}
来源：http://wl.nicolike.cn

Java: class Admin extends User {}
来源：http://io.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://as.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://cn.hahajie.cn

C#:   class Admin : User {}
来源：http://ck.szsharing.cn

[G06] 重写方法
来源：http://rb.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://cc.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gk.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://yd.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://cm.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jo.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tg.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://mf.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://dj.wgjwhj.cn

[G07] 调用父类方法
来源：http://gq.yuntaijiaju.cn

Py:   super().greet()
来源：http://et.shxzskj.cn

PHP:  parent::greet();
来源：http://cq.nszjky.cn

JS:   super.greet();
来源：http://oi.bjjhwx.cn

TS:   super.greet();
来源：http://vz.szsharing.cn

Java: super.greet();
来源：http://wa.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lb.shtwfgs.cn

Ruby: super
来源：http://vv.gzmigu.cn

C#:   base.Greet();
来源：http://pf.hahajie.cn

[G08] 静态方法与属性
来源：http://ut.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lq.asd995.cn

PHP:  public static function f() {}
来源：http://nq.chemitech.net.cn

JS:   static f() {}
来源：http://vr.asd995.cn

TS:   static f(): void {}
来源：http://mw.9csxet.cn

Java: static void f() {}
来源：http://tb.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bf.bjjhwx.cn

Ruby: def self.f; end
来源：http://cv.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://ak.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://hf.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://ha.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yq.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ok.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://fc.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://bu.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://hv.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jq.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://wa.shxzskj.cn

[G10] 访问控制
来源：http://lc.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://uh.colortex.cn

PHP:  public / protected / private
来源：http://dn.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ws.jctech888.com.cn

TS:   public / protected / private
来源：http://ed.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://yk.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ej.nicolike.cn

Ruby: public / protected / private
来源：http://ax.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://ed.bjjhwx.cn

[G11] getter / setter
来源：http://rq.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://vn.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ng.newstarts.cn

JS:   get name() { return this._name; }
来源：http://ij.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://zn.shxzukj.cn

Java: public String getName() { return name; }
来源：http://gk.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://am.panjiajie.cn

Ruby: attr_accessor :name
来源：http://ef.asd995.cn

C#:   public string Name { get; set; }
来源：http://ue.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ko.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://gj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ph.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://pl.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ga.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://wj.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qd.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://qa.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://di.shxzukj.cn

[G13] 判断对象类型
来源：http://rn.colortex.cn

Py:   isinstance(u, User)
来源：http://bh.shtwfgs.cn

PHP:  $u instanceof User
来源：http://sk.jctech888.com.cn

JS:   u instanceof User
来源：http://yk.lnxyls.cn

TS:   u instanceof User
来源：http://ad.shxzukj.cn

Java: u instanceof User
来源：http://nt.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://av.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://is.shtwfgs.cn

C#:   u is User
来源：http://iq.szxytkj.cn

[G14] 数据类 / record
来源：http://ft.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://np.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://hy.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vt.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ud.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://gq.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://qa.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vc.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://pk.shxzskj.cn

[G15] 枚举
来源：http://qg.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ad.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wd.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gc.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ob.521024.cn

Java: enum Color { RED, GREEN }
来源：http://jr.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pu.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://qa.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zb.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ua.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uf.521024.cn

PHP:  get_object_vars($obj);
来源：http://ez.panjiajie.cn

JS:   Object.entries(obj)
来源：http://rd.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://wu.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uy.huanxung.cn


<!-- 参考信息 -->