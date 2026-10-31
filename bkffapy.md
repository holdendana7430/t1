代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fb.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bd.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://eo.newstarts.cn

[E17] 首字母大写
来源：http://mm.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://so.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://km.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sz.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gk.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cl.shxzukj.cn

Ruby: s.capitalize
来源：http://qj.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ob.jctech888.com.cn

[E18] 模板占位符替换
来源：http://pg.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ha.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kn.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wz.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vt.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://da.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kr.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zq.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zs.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://de.shxzukj.cn

Py:   s.splitlines()
来源：http://ky.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ww.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://yb.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://th.lnxyls.cn

Java: s.lines().toList()
来源：http://ro.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://li.muxihuayi.cn

Ruby: s.lines
来源：http://wf.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ci.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://nh.nicolike.cn

Py:   if not s:
来源：http://pw.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kj.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ka.521024.cn

TS:   if (s === "") {}
来源：http://ph.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ja.huanxung.cn

Go:   if s == "" {}
来源：http://du.huixiangedu.cn

Ruby: if s.empty?
来源：http://ik.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sk.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://tl.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gp.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dv.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://el.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rn.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hf.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://au.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jm.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wj.colortex.cn

[E22] 字节长度与字符长度
来源：http://lu.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rn.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bc.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kv.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://az.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ta.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sj.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://xr.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dd.yuexingan06.cn

================================================================================
来源：http://yu.521024.cn

F. 文件与目录
来源：http://yu.9csxet.cn

================================================================================
来源：http://cf.asd995.cn

[F01] 读取整个文件
来源：http://ie.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rg.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://yx.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pz.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lb.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hf.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kg.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://nx.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://go.nicolike.cn

[F02] 逐行读取文件
来源：http://oc.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://az.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zm.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qx.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yu.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zy.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ht.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qv.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hq.521024.cn

[F03] 写入文件（覆盖）
来源：http://su.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jy.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://og.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wx.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yg.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jm.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://sm.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aq.shtwfgs.cn

[F04] 追加写入文件
来源：http://pw.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rq.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gq.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vc.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pt.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gk.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lb.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://os.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xq.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ql.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kn.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ww.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ht.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://zq.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jm.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://us.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://du.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://wd.lnxyls.cn

[F06] 删除文件
来源：http://cg.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://vc.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://iw.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xw.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ac.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bl.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://jj.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://mo.521024.cn

C#:   File.Delete("a.txt");
来源：http://hl.nszjky.cn

[F07] 创建目录（含多级）
来源：http://zf.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qn.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ts.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uy.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ep.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nf.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dn.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sj.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rg.shxzskj.cn

[F08] 遍历目录
来源：http://wi.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ab.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://io.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://xj.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://qg.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gr.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ly.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://dw.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://sw.shxzskj.cn

[F09] 获取文件大小
来源：http://ol.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://es.nicolike.cn

PHP:  filesize("a.txt");
来源：http://nl.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://xn.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://bw.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://te.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pe.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://en.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://qe.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://uv.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ii.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://em.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mr.9csxet.cn

TS:   path.extname("a.txt")
来源：http://lb.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xk.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ui.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tw.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fe.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://ey.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nj.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ah.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zz.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ir.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hk.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xx.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uy.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ku.9csxet.cn

[F12] CSV 读写
来源：http://es.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://de.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rc.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dq.bookmarksfly.cn

TS:   // 同上
来源：http://pc.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mb.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hc.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xy.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ob.haigaiapp.cn

================================================================================
来源：http://tr.haigaiapp.cn

G. 面向对象
来源：http://ct.chemitech.net.cn

================================================================================
来源：http://fe.nszjky.cn

[G01] 定义类
来源：http://wu.huanxung.cn

Py:   class User: pass
来源：http://jh.nicolike.cn

PHP:  class User {}
来源：http://gy.wgjwhj.cn

JS:   class User {}
来源：http://km.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://pl.muxihuayi.cn

Java: class User {}
来源：http://gj.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://sh.yuexingan06.cn

Ruby: class User; end
来源：http://yb.chemitech.net.cn

C#:   class User {}
来源：http://hw.haigaiapp.cn

[G02] 构造函数
来源：http://mi.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://ir.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://eg.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://mz.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://rn.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://md.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ok.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ni.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://aj.hahajie.cn

[G03] 实例属性
来源：http://nf.nicolike.cn

Py:   self.name = "x"
来源：http://vb.szxytkj.cn

PHP:  public string $name = "x";
来源：http://wf.szxytkj.cn

JS:   this.name = "x";
来源：http://cf.hnjuh.cn

TS:   name: string = "x";
来源：http://cw.muxihuayi.cn

Java: private String name;
来源：http://ps.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pd.hnjuh.cn

Ruby: @name = "x"
来源：http://kr.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://cx.shxzukj.cn

[G04] 定义方法
来源：http://ud.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://jy.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ui.newstarts.cn

JS:   greet() { return this.name; }
来源：http://qa.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://vv.shxzukj.cn

Java: String greet() { return name; }
来源：http://eo.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xj.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://tr.asd995.cn

C#:   public string Greet() => Name;
来源：http://sq.521024.cn

[G05] 继承
来源：http://bd.9csxet.cn

Py:   class Admin(User): pass
来源：http://qb.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://yu.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ht.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://cz.shxzskj.cn

Java: class Admin extends User {}
来源：http://fv.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bm.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://de.jctech888.com.cn

C#:   class Admin : User {}
来源：http://sr.521024.cn

[G06] 重写方法
来源：http://ud.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://sx.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rf.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://qk.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://yn.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://xe.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://td.asd995.cn

Ruby: def greet; "admin"; end
来源：http://mz.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://fy.huixiangedu.cn

[G07] 调用父类方法
来源：http://nt.asd995.cn

Py:   super().greet()
来源：http://vp.gzmigu.cn

PHP:  parent::greet();
来源：http://jv.huixiangedu.cn

JS:   super.greet();
来源：http://ci.jianghongdianzi.cn

TS:   super.greet();
来源：http://ps.huixiangedu.cn

Java: super.greet();
来源：http://tv.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ll.haigaiapp.cn

Ruby: super
来源：http://zw.shtwfgs.cn

C#:   base.Greet();
来源：http://jy.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ia.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://np.panjiajie.cn

PHP:  public static function f() {}
来源：http://oy.wgjwhj.cn

JS:   static f() {}
来源：http://nn.colortex.cn

TS:   static f(): void {}
来源：http://ab.bookmarksfly.cn

Java: static void f() {}
来源：http://wo.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ln.asd995.cn

Ruby: def self.f; end
来源：http://zg.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://hb.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://tb.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://sc.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fr.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wb.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://ao.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://oi.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://co.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mv.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://mv.haigaiapp.cn

[G10] 访问控制
来源：http://az.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://oi.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://xz.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://aw.muxihuayi.cn

TS:   public / protected / private
来源：http://ot.colortex.cn

Java: public / protected / private / 默认包级
来源：http://oh.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nh.haigaiapp.cn

Ruby: public / protected / private
来源：http://gc.szxytkj.cn

C#:   public / protected / private / internal
来源：http://ex.muxihuayi.cn

[G11] getter / setter
来源：http://th.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://wz.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hj.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://hp.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://xs.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://qz.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ti.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://oh.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://yz.muxihuayi.cn

[G12] 对象转字符串
来源：http://jw.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://ta.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gy.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://nv.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://rl.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://iy.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sh.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://zc.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://wy.szxytkj.cn

[G13] 判断对象类型
来源：http://vs.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://am.asd995.cn

PHP:  $u instanceof User
来源：http://fa.nszjky.cn

JS:   u instanceof User
来源：http://cm.shxzskj.cn

TS:   u instanceof User
来源：http://om.colortex.cn

Java: u instanceof User
来源：http://hb.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ds.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://tj.colortex.cn

C#:   u is User
来源：http://en.haigaiapp.cn

[G14] 数据类 / record
来源：http://vw.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sh.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://sz.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mw.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://tg.asd995.cn

Java: record User(String name, int age) {}
来源：http://er.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://hl.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zj.521024.cn

C#:   record User(string Name, int Age);
来源：http://cd.521024.cn

[G15] 枚举
来源：http://ru.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iz.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uy.hahajie.cn


<!-- 参考信息 -->