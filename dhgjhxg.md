代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pn.szsharing.cn

[E19] 多行文本按行拆分
来源：http://vn.newstarts.cn

Py:   s.splitlines()
来源：http://ue.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qz.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://jc.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://de.wgjwhj.cn

Java: s.lines().toList()
来源：http://ju.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://jx.newstarts.cn

Ruby: s.lines
来源：http://pt.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://jj.asd995.cn

[E20] 判断字符串是否为空
来源：http://md.asd995.cn

Py:   if not s:
来源：http://sh.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qj.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://km.shxzskj.cn

TS:   if (s === "") {}
来源：http://vl.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://xn.szxytkj.cn

Go:   if s == "" {}
来源：http://tv.shxzskj.cn

Ruby: if s.empty?
来源：http://af.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nt.newstarts.cn

[E21] 超长截断加省略号
来源：http://pe.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rt.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nt.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bm.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xm.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cf.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://sp.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gi.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xv.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://cb.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hk.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zz.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sp.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pv.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sp.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ke.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://mm.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fk.asd995.cn

================================================================================
来源：http://qt.muxihuayi.cn

F. 文件与目录
来源：http://lp.newstarts.cn

================================================================================
来源：http://jy.shtwfgs.cn

[F01] 读取整个文件
来源：http://dt.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tn.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://nq.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yz.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yp.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://au.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oh.colortex.cn

Ruby: File.read("a.txt")
来源：http://ny.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://oy.shtwfgs.cn

[F02] 逐行读取文件
来源：http://mp.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ey.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://up.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qz.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://du.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hb.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cp.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yu.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uf.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://zc.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://an.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cg.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mr.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fl.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://th.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vy.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://hb.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dh.colortex.cn

[F04] 追加写入文件
来源：http://cq.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kq.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ha.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xa.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dy.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fn.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jy.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bt.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ss.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://bm.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hq.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://av.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://xa.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://dq.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iq.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qi.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ao.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://gu.huixiangedu.cn

[F06] 删除文件
来源：http://qf.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://kh.9csxet.cn

PHP:  unlink("a.txt");
来源：http://cl.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ve.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mb.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ru.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://ib.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://uy.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://tx.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://lc.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fd.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gy.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sn.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lg.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dq.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nw.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ho.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qu.chemitech.net.cn

[F08] 遍历目录
来源：http://lx.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pp.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jq.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://nb.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://dx.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cq.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ui.nszjky.cn

Ruby: Dir.children("dir")
来源：http://fr.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://pz.szsharing.cn

[F09] 获取文件大小
来源：http://xu.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://me.colortex.cn

PHP:  filesize("a.txt");
来源：http://ce.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://ht.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ab.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fp.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ra.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://hk.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://nf.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://qa.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zm.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dz.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rk.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://sq.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sk.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ks.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://up.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qp.colortex.cn

[F11] 复制与移动文件
来源：http://oq.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ld.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ph.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pq.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kk.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xs.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kd.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ex.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cp.nicolike.cn

[F12] CSV 读写
来源：http://vg.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gv.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qa.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zu.yuexingan06.cn

TS:   // 同上
来源：http://jl.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vw.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://di.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xv.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uq.shtwfgs.cn

================================================================================
来源：http://fy.shxzukj.cn

G. 面向对象
来源：http://gs.asd995.cn

================================================================================
来源：http://zi.hahajie.cn

[G01] 定义类
来源：http://oq.huixinmuqiang.cn

Py:   class User: pass
来源：http://us.hahajie.cn

PHP:  class User {}
来源：http://yw.muxihuayi.cn

JS:   class User {}
来源：http://cf.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://oc.asd995.cn

Java: class User {}
来源：http://bj.521024.cn

Go:   type User struct { Name string }
来源：http://sf.huixiangedu.cn

Ruby: class User; end
来源：http://hs.shxzskj.cn

C#:   class User {}
来源：http://sa.nszjky.cn

[G02] 构造函数
来源：http://tl.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://rq.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://aj.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://zz.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://yg.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://gp.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cu.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://mj.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://jp.colortex.cn

[G03] 实例属性
来源：http://vq.bookmarksfly.cn

Py:   self.name = "x"
来源：http://br.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://eb.panjiajie.cn

JS:   this.name = "x";
来源：http://qf.wgjwhj.cn

TS:   name: string = "x";
来源：http://sw.shtwfgs.cn

Java: private String name;
来源：http://ua.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tv.521024.cn

Ruby: @name = "x"
来源：http://my.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://nk.chemitech.net.cn

[G04] 定义方法
来源：http://st.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://cl.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ns.asd995.cn

JS:   greet() { return this.name; }
来源：http://dv.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://nd.shxzskj.cn

Java: String greet() { return name; }
来源：http://pw.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fx.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://vt.newstarts.cn

C#:   public string Greet() => Name;
来源：http://vd.newstarts.cn

[G05] 继承
来源：http://el.shxzukj.cn

Py:   class Admin(User): pass
来源：http://sm.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://jb.nszjky.cn

JS:   class Admin extends User {}
来源：http://yu.szxytkj.cn

TS:   class Admin extends User {}
来源：http://zj.huixiangedu.cn

Java: class Admin extends User {}
来源：http://xy.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jj.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://td.nszjky.cn

C#:   class Admin : User {}
来源：http://hl.shxzskj.cn

[G06] 重写方法
来源：http://yr.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://cv.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vo.asd995.cn

JS:   greet() { return "admin"; }
来源：http://vf.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://up.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://vf.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wi.colortex.cn

Ruby: def greet; "admin"; end
来源：http://tu.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://mv.lnxyls.cn

[G07] 调用父类方法
来源：http://rt.wgjwhj.cn

Py:   super().greet()
来源：http://sh.muxihuayi.cn

PHP:  parent::greet();
来源：http://eq.hahajie.cn

JS:   super.greet();
来源：http://or.huixiangedu.cn

TS:   super.greet();
来源：http://nc.szxytkj.cn

Java: super.greet();
来源：http://xo.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://za.jctech888.com.cn

Ruby: super
来源：http://nj.newstarts.cn

C#:   base.Greet();
来源：http://ad.muxihuayi.cn

[G08] 静态方法与属性
来源：http://sp.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://em.shxzskj.cn

PHP:  public static function f() {}
来源：http://gh.gzmigu.cn

JS:   static f() {}
来源：http://xi.gzmigu.cn

TS:   static f(): void {}
来源：http://du.bookmarksfly.cn

Java: static void f() {}
来源：http://cn.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lt.shxzskj.cn

Ruby: def self.f; end
来源：http://tb.panjiajie.cn

C#:   public static void F() {}
来源：http://le.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://hu.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://tx.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qa.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://to.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://uo.newstarts.cn

Java: interface Shape { double area(); }
来源：http://eh.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://qq.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xq.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://fk.wgjwhj.cn

[G10] 访问控制
来源：http://mm.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.huixiangedu.cn

PHP:  public / protected / private
来源：http://mo.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://rq.szsharing.cn

TS:   public / protected / private
来源：http://jt.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://tm.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xz.huanxung.cn

Ruby: public / protected / private
来源：http://vh.huanxung.cn

C#:   public / protected / private / internal
来源：http://pj.nicolike.cn

[G11] getter / setter
来源：http://rv.521024.cn

Py:   @property 与 @x.setter
来源：http://us.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dk.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://wx.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://yv.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ke.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qj.hahajie.cn

Ruby: attr_accessor :name
来源：http://pm.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://gw.shxzskj.cn

[G12] 对象转字符串
来源：http://md.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://vh.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://af.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://es.521024.cn

TS:   toString(): string { return this.name; }
来源：http://ri.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://cb.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zl.521024.cn

Ruby: def to_s; @name; end
来源：http://si.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ep.bookmarksfly.cn

[G13] 判断对象类型
来源：http://sz.asd995.cn

Py:   isinstance(u, User)
来源：http://ti.newstarts.cn

PHP:  $u instanceof User
来源：http://ph.chemitech.net.cn

JS:   u instanceof User
来源：http://mh.gzmigu.cn

TS:   u instanceof User
来源：http://vx.huixiangedu.cn

Java: u instanceof User
来源：http://iq.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wm.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://nl.szsharing.cn

C#:   u is User
来源：http://go.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://vo.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nw.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ns.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ic.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://nc.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://kc.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://ef.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xr.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ec.huixiangedu.cn

[G15] 枚举
来源：http://ld.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mj.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fu.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eg.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ve.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://kr.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sf.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://od.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://do.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://ih.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gt.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://uc.asd995.cn

JS:   Object.entries(obj)
来源：http://ag.gzmigu.cn

TS:   Object.entries(obj)
来源：http://mc.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://va.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eh.huanxung.cn

Ruby: obj.instance_variables
来源：http://yi.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ia.hahajie.cn

================================================================================
来源：http://bm.yuntaijiaju.cn

H. 异常与错误处理
来源：http://oj.bookmarksfly.cn

================================================================================
来源：http://zk.jctech888.com.cn

[H01] try / catch 基础
来源：http://dh.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yq.shtwfgs.cn


<!-- 参考信息 -->