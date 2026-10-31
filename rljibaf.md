代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://ed.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vq.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://av.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jx.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bp.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://wu.muxihuayi.cn

Py:   s.splitlines()
来源：http://rw.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://be.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://oz.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://yi.colortex.cn

Java: s.lines().toList()
来源：http://ho.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://qa.huixinmuqiang.cn

Ruby: s.lines
来源：http://cc.shtwfgs.cn

C#:   s.Split('\n')
来源：http://vo.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ts.szsharing.cn

Py:   if not s:
来源：http://mh.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gh.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vj.huanxung.cn

TS:   if (s === "") {}
来源：http://fb.521024.cn

Java: if (s.isEmpty()) {}
来源：http://nu.hahajie.cn

Go:   if s == "" {}
来源：http://um.bjjhwx.cn

Ruby: if s.empty?
来源：http://pf.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fw.newstarts.cn

[E21] 超长截断加省略号
来源：http://sj.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ns.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ly.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mh.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://px.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zq.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://rs.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nh.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qq.huanxung.cn

[E22] 字节长度与字符长度
来源：http://vj.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ht.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pa.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://an.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gn.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ml.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kh.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://co.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mp.lnxyls.cn

================================================================================
来源：http://hg.gzmigu.cn

F. 文件与目录
来源：http://oy.nicolike.cn

================================================================================
来源：http://vf.gzmigu.cn

[F01] 读取整个文件
来源：http://ce.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xs.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://cs.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ex.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yb.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rw.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dt.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://uj.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://kt.wgjwhj.cn

[F02] 逐行读取文件
来源：http://xu.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ql.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://od.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mq.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dq.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ua.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://of.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bz.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://or.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://oi.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ew.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dj.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ta.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gi.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yd.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rk.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://qm.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xf.hnjuh.cn

[F04] 追加写入文件
来源：http://wg.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qy.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xw.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ud.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kz.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://km.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bw.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vj.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://jv.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tx.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://jy.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://mx.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://wj.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qv.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gi.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://qx.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://sm.521024.cn

[F06] 删除文件
来源：http://cj.9csxet.cn

Py:   os.remove("a.txt")
来源：http://lb.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://st.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hp.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nd.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mx.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://ps.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://lq.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ir.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://sc.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gb.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ah.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rc.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ez.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fw.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://te.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ox.panjiajie.cn

[F08] 遍历目录
来源：http://kl.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://um.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ky.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://tp.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ya.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bl.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wr.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://gk.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://nz.gzmigu.cn

[F09] 获取文件大小
来源：http://mz.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://fw.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://fx.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://gd.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://hy.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lg.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bj.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://xu.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://dg.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://gj.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gd.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ex.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mr.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ve.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zy.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zx.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ay.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bq.newstarts.cn

[F11] 复制与移动文件
来源：http://si.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ty.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fy.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uy.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rw.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vq.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rg.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fj.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://os.521024.cn

[F12] CSV 读写
来源：http://pb.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cv.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ws.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nu.asd995.cn

TS:   // 同上
来源：http://zt.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://up.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bi.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cc.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yv.haigaiapp.cn

================================================================================
来源：http://ox.chemitech.net.cn

G. 面向对象
来源：http://oj.szsharing.cn

================================================================================
来源：http://rd.shtwfgs.cn

[G01] 定义类
来源：http://ir.shxzukj.cn

Py:   class User: pass
来源：http://pt.shxzskj.cn

PHP:  class User {}
来源：http://sz.shxzskj.cn

JS:   class User {}
来源：http://lc.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://sa.shtwfgs.cn

Java: class User {}
来源：http://so.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://vv.yuexingan06.cn

Ruby: class User; end
来源：http://xw.gzmigu.cn

C#:   class User {}
来源：http://yp.nicolike.cn

[G02] 构造函数
来源：http://yo.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://fo.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://xa.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://rk.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://iv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://cn.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bs.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ix.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://sl.chemitech.net.cn

[G03] 实例属性
来源：http://mv.nicolike.cn

Py:   self.name = "x"
来源：http://uy.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://cy.9csxet.cn

JS:   this.name = "x";
来源：http://xx.nicolike.cn

TS:   name: string = "x";
来源：http://lr.chemitech.net.cn

Java: private String name;
来源：http://hv.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uy.yuexingan06.cn

Ruby: @name = "x"
来源：http://uk.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://wn.haigaiapp.cn

[G04] 定义方法
来源：http://me.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://gr.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ha.521024.cn

JS:   greet() { return this.name; }
来源：http://gy.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://hg.huanxung.cn

Java: String greet() { return name; }
来源：http://pu.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wp.szsharing.cn

Ruby: def greet; @name; end
来源：http://ao.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://pr.newstarts.cn

[G05] 继承
来源：http://wg.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://bj.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://zy.nicolike.cn

JS:   class Admin extends User {}
来源：http://wk.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://zw.nszjky.cn

Java: class Admin extends User {}
来源：http://pq.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lc.asd995.cn

Ruby: class Admin < User; end
来源：http://zj.asd995.cn

C#:   class Admin : User {}
来源：http://nq.shxzskj.cn

[G06] 重写方法
来源：http://ff.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://iz.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://em.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://fu.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://yi.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ac.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mu.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://rk.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://br.panjiajie.cn

[G07] 调用父类方法
来源：http://lt.hnjuh.cn

Py:   super().greet()
来源：http://dz.muxihuayi.cn

PHP:  parent::greet();
来源：http://fi.lnxyls.cn

JS:   super.greet();
来源：http://hh.newstarts.cn

TS:   super.greet();
来源：http://qz.panjiajie.cn

Java: super.greet();
来源：http://id.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rg.colortex.cn

Ruby: super
来源：http://ro.jctech888.com.cn

C#:   base.Greet();
来源：http://qb.colortex.cn

[G08] 静态方法与属性
来源：http://ew.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wz.muxihuayi.cn

PHP:  public static function f() {}
来源：http://dx.colortex.cn

JS:   static f() {}
来源：http://ki.yuexingan06.cn

TS:   static f(): void {}
来源：http://lb.newstarts.cn

Java: static void f() {}
来源：http://iw.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ga.haigaiapp.cn

Ruby: def self.f; end
来源：http://wx.colortex.cn

C#:   public static void F() {}
来源：http://gq.asd995.cn

[G09] 接口 / 抽象类
来源：http://if.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://pu.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jl.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bo.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://jv.colortex.cn

Java: interface Shape { double area(); }
来源：http://ur.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://yn.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://so.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://rn.muxihuayi.cn

[G10] 访问控制
来源：http://zm.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ss.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://fe.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://kl.hahajie.cn

TS:   public / protected / private
来源：http://cy.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://ui.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sm.panjiajie.cn

Ruby: public / protected / private
来源：http://wa.521024.cn

C#:   public / protected / private / internal
来源：http://uo.chemitech.net.cn

[G11] getter / setter
来源：http://to.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ug.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vx.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://mv.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://kf.huanxung.cn

Java: public String getName() { return name; }
来源：http://iq.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wy.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://fr.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://rr.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://ht.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://tr.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pr.colortex.cn

JS:   toString() { return this.name; }
来源：http://km.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://oa.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://dx.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://io.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://ow.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://po.szsharing.cn

[G13] 判断对象类型
来源：http://qm.nszjky.cn

Py:   isinstance(u, User)
来源：http://we.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://al.muxihuayi.cn

JS:   u instanceof User
来源：http://wj.shxzukj.cn

TS:   u instanceof User
来源：http://oc.huixinmuqiang.cn

Java: u instanceof User
来源：http://vw.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ua.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://uz.nszjky.cn

C#:   u is User
来源：http://jx.szsharing.cn

[G14] 数据类 / record
来源：http://mi.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ap.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://qs.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tm.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://wp.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://sj.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ap.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ch.asd995.cn

C#:   record User(string Name, int Age);
来源：http://qn.nszjky.cn

[G15] 枚举
来源：http://ov.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fo.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sk.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hc.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ba.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://uv.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qj.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://vk.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ld.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://lk.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vq.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://hc.hahajie.cn

JS:   Object.entries(obj)
来源：http://ut.9csxet.cn

TS:   Object.entries(obj)
来源：http://zx.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mr.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qp.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://aq.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://zv.bookmarksfly.cn

================================================================================
来源：http://bd.nszjky.cn


<!-- 参考信息 -->