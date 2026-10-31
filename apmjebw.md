代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wa.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ow.shxzskj.cn

Ruby: s.capitalize
来源：http://eg.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ts.shxzskj.cn

[E18] 模板占位符替换
来源：http://si.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dt.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bp.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mo.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dz.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ry.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://le.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qs.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zs.colortex.cn

[E19] 多行文本按行拆分
来源：http://lh.huixiangedu.cn

Py:   s.splitlines()
来源：http://fw.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dt.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://lz.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://rm.muxihuayi.cn

Java: s.lines().toList()
来源：http://bp.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://lw.shxzskj.cn

Ruby: s.lines
来源：http://al.szsharing.cn

C#:   s.Split('\n')
来源：http://sh.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://kv.jianghongdianzi.cn

Py:   if not s:
来源：http://td.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rs.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xs.nicolike.cn

TS:   if (s === "") {}
来源：http://nj.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://rv.muxihuayi.cn

Go:   if s == "" {}
来源：http://gz.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://fs.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ct.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://ay.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ph.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uh.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wj.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kb.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cj.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://nf.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lv.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fr.asd995.cn

[E22] 字节长度与字符长度
来源：http://ch.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ql.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://md.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://on.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ca.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qk.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://je.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://gg.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lg.haigaiapp.cn

================================================================================
来源：http://hh.jianghongdianzi.cn

F. 文件与目录
来源：http://lf.gzmigu.cn

================================================================================
来源：http://uj.lnxyls.cn

[F01] 读取整个文件
来源：http://pl.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kq.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://dx.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wu.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pq.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hx.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sm.szsharing.cn

Ruby: File.read("a.txt")
来源：http://pd.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://hk.9csxet.cn

[F02] 逐行读取文件
来源：http://wr.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rp.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qn.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yd.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ko.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://or.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://il.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sb.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://es.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ng.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gd.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eu.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cf.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cp.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://du.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://an.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zn.shxzskj.cn

[F04] 追加写入文件
来源：http://mw.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lj.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uv.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hm.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ui.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hm.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ni.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qb.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pw.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://st.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tj.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://ep.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://ef.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://cq.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://as.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://js.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://ee.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ai.bookmarksfly.cn

[F06] 删除文件
来源：http://pp.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://fz.szsharing.cn

PHP:  unlink("a.txt");
来源：http://ak.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://so.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yy.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://px.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://qd.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://qp.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://bb.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://fr.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://an.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kd.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bp.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wl.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lx.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ij.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sy.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ug.wgjwhj.cn

[F08] 遍历目录
来源：http://hf.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qm.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iv.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://ne.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://tc.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ex.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zd.newstarts.cn

Ruby: Dir.children("dir")
来源：http://vu.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://uw.bjjhwx.cn

[F09] 获取文件大小
来源：http://si.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://gp.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ud.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://vg.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://od.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mu.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rc.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://ga.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://mj.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://do.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ae.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iy.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://on.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://yy.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tj.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fl.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ky.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ut.nicolike.cn

[F11] 复制与移动文件
来源：http://qz.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://to.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wz.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sr.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wc.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tu.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ns.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zn.bookmarksfly.cn

[F12] CSV 读写
来源：http://th.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dv.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fr.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cy.shtwfgs.cn

TS:   // 同上
来源：http://ph.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ma.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qj.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bj.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ob.nicolike.cn

================================================================================
来源：http://gg.shxzukj.cn

G. 面向对象
来源：http://zd.lnxyls.cn

================================================================================
来源：http://lc.hahajie.cn

[G01] 定义类
来源：http://jr.chemitech.net.cn

Py:   class User: pass
来源：http://wi.newstarts.cn

PHP:  class User {}
来源：http://ea.hnjuh.cn

JS:   class User {}
来源：http://xi.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ef.shxzskj.cn

Java: class User {}
来源：http://ee.huanxung.cn

Go:   type User struct { Name string }
来源：http://ie.panjiajie.cn

Ruby: class User; end
来源：http://hl.521024.cn

C#:   class User {}
来源：http://tv.shtwfgs.cn

[G02] 构造函数
来源：http://zu.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://zn.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://fk.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://rs.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://dy.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://fz.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zy.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ha.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://rs.hahajie.cn

[G03] 实例属性
来源：http://tt.bjjhwx.cn

Py:   self.name = "x"
来源：http://id.521024.cn

PHP:  public string $name = "x";
来源：http://dc.szsharing.cn

JS:   this.name = "x";
来源：http://xz.9csxet.cn

TS:   name: string = "x";
来源：http://lg.nszjky.cn

Java: private String name;
来源：http://jw.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ha.hnjuh.cn

Ruby: @name = "x"
来源：http://vn.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://kn.wgjwhj.cn

[G04] 定义方法
来源：http://io.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://fa.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oi.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://my.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://fy.yuexingan06.cn

Java: String greet() { return name; }
来源：http://iv.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cx.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://hv.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://hx.chemitech.net.cn

[G05] 继承
来源：http://qi.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://fe.huanxung.cn

PHP:  class Admin extends User {}
来源：http://gz.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ht.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ci.muxihuayi.cn

Java: class Admin extends User {}
来源：http://lq.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dy.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://rf.9csxet.cn

C#:   class Admin : User {}
来源：http://xx.szxytkj.cn

[G06] 重写方法
来源：http://ay.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ub.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bz.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://be.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://fe.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ln.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tk.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://au.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://bb.yuexingan06.cn

[G07] 调用父类方法
来源：http://wo.bjjhwx.cn

Py:   super().greet()
来源：http://pu.hnjuh.cn

PHP:  parent::greet();
来源：http://qy.lnxyls.cn

JS:   super.greet();
来源：http://pi.jctech888.com.cn

TS:   super.greet();
来源：http://ul.shxzskj.cn

Java: super.greet();
来源：http://rb.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yy.colortex.cn

Ruby: super
来源：http://za.521024.cn

C#:   base.Greet();
来源：http://nx.wgjwhj.cn

[G08] 静态方法与属性
来源：http://xf.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://on.shxzskj.cn

PHP:  public static function f() {}
来源：http://zq.nicolike.cn

JS:   static f() {}
来源：http://vy.colortex.cn

TS:   static f(): void {}
来源：http://of.colortex.cn

Java: static void f() {}
来源：http://po.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dk.panjiajie.cn

Ruby: def self.f; end
来源：http://ez.521024.cn

C#:   public static void F() {}
来源：http://cd.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://qm.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://fq.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ff.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oo.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://kr.newstarts.cn

Java: interface Shape { double area(); }
来源：http://de.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://nd.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xr.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ca.haigaiapp.cn

[G10] 访问控制
来源：http://dm.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://ip.szsharing.cn

PHP:  public / protected / private
来源：http://ti.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://ue.yuntaijiaju.cn

TS:   public / protected / private
来源：http://il.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://nl.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kq.9csxet.cn

Ruby: public / protected / private
来源：http://ku.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://ah.huixiangedu.cn

[G11] getter / setter
来源：http://op.colortex.cn

Py:   @property 与 @x.setter
来源：http://jq.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://to.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://wa.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://th.nszjky.cn

Java: public String getName() { return name; }
来源：http://dz.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nd.newstarts.cn

Ruby: attr_accessor :name
来源：http://uc.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://wq.shtwfgs.cn

[G12] 对象转字符串
来源：http://ez.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://fa.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eg.9csxet.cn

JS:   toString() { return this.name; }
来源：http://ki.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://jd.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://by.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wj.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://dl.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://kh.gzmigu.cn

[G13] 判断对象类型
来源：http://zx.lnxyls.cn

Py:   isinstance(u, User)
来源：http://li.shtwfgs.cn

PHP:  $u instanceof User
来源：http://yt.asd995.cn

JS:   u instanceof User
来源：http://lr.jianghongdianzi.cn

TS:   u instanceof User
来源：http://vl.huixinmuqiang.cn

Java: u instanceof User
来源：http://em.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gp.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://ri.hahajie.cn

C#:   u is User
来源：http://dh.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://vk.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iu.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ny.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qq.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://xd.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://be.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://oc.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sn.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://ui.gzmigu.cn

[G15] 枚举
来源：http://ha.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qt.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cc.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fy.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zz.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://hc.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://at.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://do.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xt.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://pu.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ms.szsharing.cn


<!-- 参考信息 -->