代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ln.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gc.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zq.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ma.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ch.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ga.asd995.cn

Ruby: s.capitalize
来源：http://xc.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cm.nszjky.cn

[E18] 模板占位符替换
来源：http://rm.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://me.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://da.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kl.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hu.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bn.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sg.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yo.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ry.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://ku.huixiangedu.cn

Py:   s.splitlines()
来源：http://hm.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lu.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://gr.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://kl.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://ad.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://ey.muxihuayi.cn

Ruby: s.lines
来源：http://ua.szxytkj.cn

C#:   s.Split('\n')
来源：http://ky.colortex.cn

[E20] 判断字符串是否为空
来源：http://kj.bjjhwx.cn

Py:   if not s:
来源：http://bp.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zh.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jt.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ax.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://fm.panjiajie.cn

Go:   if s == "" {}
来源：http://bb.jctech888.com.cn

Ruby: if s.empty?
来源：http://dk.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.shxzskj.cn

[E21] 超长截断加省略号
来源：http://tk.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nx.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tx.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oi.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zt.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fv.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://mk.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oe.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ix.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://em.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://do.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ug.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mk.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://le.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://mu.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xy.nszjky.cn

================================================================================
来源：http://hz.bjjhwx.cn

F. 文件与目录
来源：http://il.hnjuh.cn

================================================================================
来源：http://la.huanxung.cn

[F01] 读取整个文件
来源：http://ph.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yp.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://gi.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fy.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fo.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bv.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xe.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://tc.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://cl.bjjhwx.cn

[F02] 逐行读取文件
来源：http://iy.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pg.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mo.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ca.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hn.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ql.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yq.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tm.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://om.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://vd.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pi.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ex.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hn.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lc.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vx.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zw.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ck.hnjuh.cn

[F04] 追加写入文件
来源：http://kh.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yw.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://io.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qi.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kr.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qm.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mk.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qa.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://ui.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yg.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ru.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://uz.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://qt.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lb.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://dx.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://bs.huanxung.cn

[F06] 删除文件
来源：http://kn.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://va.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ut.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fh.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fr.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nz.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://wx.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://pe.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://zd.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://jy.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gx.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vd.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sp.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mr.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eu.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://my.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bo.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bx.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ve.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wt.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jf.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://hr.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://zy.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sd.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xc.szsharing.cn

Ruby: Dir.children("dir")
来源：http://af.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://zs.muxihuayi.cn

[F09] 获取文件大小
来源：http://ng.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ly.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://uf.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://ni.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://sd.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ze.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rr.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://yu.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://my.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://dw.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fl.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tq.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iy.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://bi.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yd.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kv.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nr.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sx.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://rw.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jx.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://da.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://za.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kk.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://od.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ej.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tf.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jd.hahajie.cn

[F12] CSV 读写
来源：http://zx.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ca.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jk.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.shtwfgs.cn

TS:   // 同上
来源：http://ir.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cm.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ym.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nu.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gk.shtwfgs.cn

================================================================================
来源：http://lc.bjjhwx.cn

G. 面向对象
来源：http://qs.szxytkj.cn

================================================================================
来源：http://ci.huixinmuqiang.cn

[G01] 定义类
来源：http://xt.hahajie.cn

Py:   class User: pass
来源：http://wx.yuntaijiaju.cn

PHP:  class User {}
来源：http://fz.yuntaijiaju.cn

JS:   class User {}
来源：http://oc.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://hx.yuntaijiaju.cn

Java: class User {}
来源：http://ly.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://wx.nszjky.cn

Ruby: class User; end
来源：http://pc.lnxyls.cn

C#:   class User {}
来源：http://we.szsharing.cn

[G02] 构造函数
来源：http://lg.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://bj.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://aa.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://de.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://cp.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://rs.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://az.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://zf.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://dl.bookmarksfly.cn

[G03] 实例属性
来源：http://re.hahajie.cn

Py:   self.name = "x"
来源：http://sb.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://vm.gzmigu.cn

JS:   this.name = "x";
来源：http://md.nicolike.cn

TS:   name: string = "x";
来源：http://zs.shxzukj.cn

Java: private String name;
来源：http://ud.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fl.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://di.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ej.huixinmuqiang.cn

[G04] 定义方法
来源：http://bo.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://dg.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kg.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://nb.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://eu.hnjuh.cn

Java: String greet() { return name; }
来源：http://mu.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uo.nicolike.cn

Ruby: def greet; @name; end
来源：http://lk.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://uq.bjjhwx.cn

[G05] 继承
来源：http://hv.huanxung.cn

Py:   class Admin(User): pass
来源：http://gu.huanxung.cn

PHP:  class Admin extends User {}
来源：http://pf.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://nm.szxytkj.cn

TS:   class Admin extends User {}
来源：http://gb.nszjky.cn

Java: class Admin extends User {}
来源：http://fy.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://li.hahajie.cn

Ruby: class Admin < User; end
来源：http://tw.asd995.cn

C#:   class Admin : User {}
来源：http://kj.newstarts.cn

[G06] 重写方法
来源：http://hy.521024.cn

Py:   def greet(self): return "admin"
来源：http://rt.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://by.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://xy.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://lh.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://ty.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uk.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://iz.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://pk.nicolike.cn

[G07] 调用父类方法
来源：http://ee.huixinmuqiang.cn

Py:   super().greet()
来源：http://la.wgjwhj.cn

PHP:  parent::greet();
来源：http://zj.szxytkj.cn

JS:   super.greet();
来源：http://lm.521024.cn

TS:   super.greet();
来源：http://jf.newstarts.cn

Java: super.greet();
来源：http://ii.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wv.lnxyls.cn

Ruby: super
来源：http://bf.9csxet.cn

C#:   base.Greet();
来源：http://kd.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://vi.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vp.shxzukj.cn

PHP:  public static function f() {}
来源：http://da.shtwfgs.cn

JS:   static f() {}
来源：http://sk.shxzskj.cn

TS:   static f(): void {}
来源：http://vh.jianghongdianzi.cn

Java: static void f() {}
来源：http://mk.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xr.shxzukj.cn

Ruby: def self.f; end
来源：http://gr.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://ln.hahajie.cn

[G09] 接口 / 抽象类
来源：http://yv.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://wx.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ln.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oy.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://pm.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://yb.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://hq.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fa.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://cy.nszjky.cn

[G10] 访问控制
来源：http://tj.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://lk.szsharing.cn

PHP:  public / protected / private
来源：http://bw.hahajie.cn

JS:   #private 字段；其余公开
来源：http://mv.jctech888.com.cn

TS:   public / protected / private
来源：http://so.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://ho.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gd.521024.cn

Ruby: public / protected / private
来源：http://sa.hahajie.cn

C#:   public / protected / private / internal
来源：http://gf.haigaiapp.cn

[G11] getter / setter
来源：http://dp.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://sz.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hf.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://ts.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://sz.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ty.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wg.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://xa.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ee.panjiajie.cn

[G12] 对象转字符串
来源：http://qi.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://xv.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ry.newstarts.cn

JS:   toString() { return this.name; }
来源：http://ub.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://od.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://yd.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://am.521024.cn

Ruby: def to_s; @name; end
来源：http://ak.asd995.cn

C#:   public override string ToString() => Name;
来源：http://ur.gzmigu.cn

[G13] 判断对象类型
来源：http://ah.colortex.cn

Py:   isinstance(u, User)
来源：http://gt.gzmigu.cn

PHP:  $u instanceof User
来源：http://kz.shtwfgs.cn

JS:   u instanceof User
来源：http://cw.bjjhwx.cn

TS:   u instanceof User
来源：http://sr.shxzukj.cn

Java: u instanceof User
来源：http://vr.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zv.521024.cn

Ruby: u.is_a?(User)
来源：http://gq.huixinmuqiang.cn

C#:   u is User
来源：http://yi.shxzukj.cn

[G14] 数据类 / record
来源：http://us.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lh.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://lr.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lt.521024.cn

TS:   type User = { name: string; age: number };
来源：http://gj.szsharing.cn

Java: record User(String name, int age) {}
来源：http://fy.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ii.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ak.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://rl.shtwfgs.cn

[G15] 枚举
来源：http://ac.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gt.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yt.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bh.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://us.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://fi.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bs.shxzskj.cn


<!-- 参考信息 -->