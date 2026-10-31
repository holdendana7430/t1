代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://fq.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zj.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gv.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xl.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hh.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://bt.gzmigu.cn

Py:   s.splitlines()
来源：http://sb.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ae.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://ry.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://jj.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://zi.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://fe.bjjhwx.cn

Ruby: s.lines
来源：http://lk.haigaiapp.cn

C#:   s.Split('\n')
来源：http://gi.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://ij.hnjuh.cn

Py:   if not s:
来源：http://su.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dq.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ij.521024.cn

TS:   if (s === "") {}
来源：http://qr.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://ou.colortex.cn

Go:   if s == "" {}
来源：http://xr.colortex.cn

Ruby: if s.empty?
来源：http://rc.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qx.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ka.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://es.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yh.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jx.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zw.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://me.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://te.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ku.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jw.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ih.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nm.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://en.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uq.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xr.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qo.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ju.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://ex.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yp.hnjuh.cn

================================================================================
来源：http://ex.huixinmuqiang.cn

F. 文件与目录
来源：http://us.huanxung.cn

================================================================================
来源：http://cw.huixiangedu.cn

[F01] 读取整个文件
来源：http://sj.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tr.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://gt.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://em.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xo.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ge.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dj.9csxet.cn

Ruby: File.read("a.txt")
来源：http://kn.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://iy.yuexingan06.cn

[F02] 逐行读取文件
来源：http://no.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hm.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fy.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ip.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ad.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cs.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zw.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ar.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hp.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ic.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ut.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jd.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kb.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bo.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zb.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rq.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ox.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fb.521024.cn

[F04] 追加写入文件
来源：http://sv.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://im.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ke.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rk.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://um.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fr.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gc.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xp.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rp.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://zh.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://gb.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://uq.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://ok.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://li.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wo.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://av.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://zz.szsharing.cn

[F06] 删除文件
来源：http://sn.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://bo.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://ht.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fm.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bt.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wp.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://fq.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://cp.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://gn.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ai.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ko.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hw.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yj.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ww.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ro.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yw.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wa.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://na.lnxyls.cn

[F08] 遍历目录
来源：http://yt.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ag.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oz.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://ws.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://eh.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ze.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fn.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://np.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://ji.nszjky.cn

[F09] 获取文件大小
来源：http://ff.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ps.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ok.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://tv.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://pz.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rv.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wg.newstarts.cn

Ruby: File.size("a.txt")
来源：http://oy.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ny.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://wa.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://we.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bt.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ka.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://nk.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kr.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vf.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tl.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ly.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ve.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yh.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bc.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vr.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nk.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fo.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wl.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ka.chemitech.net.cn

[F12] CSV 读写
来源：http://lm.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sw.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jm.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wh.newstarts.cn

TS:   // 同上
来源：http://vi.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rh.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://id.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xi.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uq.asd995.cn

================================================================================
来源：http://xo.chemitech.net.cn

G. 面向对象
来源：http://fc.nszjky.cn

================================================================================
来源：http://be.szsharing.cn

[G01] 定义类
来源：http://ai.hnjuh.cn

Py:   class User: pass
来源：http://fj.huanxung.cn

PHP:  class User {}
来源：http://oc.bookmarksfly.cn

JS:   class User {}
来源：http://ou.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ao.9csxet.cn

Java: class User {}
来源：http://um.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://bo.newstarts.cn

Ruby: class User; end
来源：http://jr.bjjhwx.cn

C#:   class User {}
来源：http://up.lnxyls.cn

[G02] 构造函数
来源：http://ol.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://zz.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://nh.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://rp.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://ps.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://se.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oz.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://fc.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://eh.hnjuh.cn

[G03] 实例属性
来源：http://lo.bjjhwx.cn

Py:   self.name = "x"
来源：http://nm.nszjky.cn

PHP:  public string $name = "x";
来源：http://qp.colortex.cn

JS:   this.name = "x";
来源：http://at.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://za.panjiajie.cn

Java: private String name;
来源：http://sg.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://so.szxytkj.cn

Ruby: @name = "x"
来源：http://uu.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://kn.hnjuh.cn

[G04] 定义方法
来源：http://ep.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://hq.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qj.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://ui.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://xd.colortex.cn

Java: String greet() { return name; }
来源：http://mo.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xb.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://hl.newstarts.cn

C#:   public string Greet() => Name;
来源：http://kv.asd995.cn

[G05] 继承
来源：http://wf.colortex.cn

Py:   class Admin(User): pass
来源：http://jn.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://aw.nicolike.cn

JS:   class Admin extends User {}
来源：http://op.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://yn.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ak.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xl.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://vm.haigaiapp.cn

C#:   class Admin : User {}
来源：http://au.huixiangedu.cn

[G06] 重写方法
来源：http://bu.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ep.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fy.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://dr.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://tc.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ur.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tw.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://po.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://rh.szxytkj.cn

[G07] 调用父类方法
来源：http://ru.521024.cn

Py:   super().greet()
来源：http://rc.shtwfgs.cn

PHP:  parent::greet();
来源：http://ls.nicolike.cn

JS:   super.greet();
来源：http://pt.chemitech.net.cn

TS:   super.greet();
来源：http://sm.lnxyls.cn

Java: super.greet();
来源：http://vf.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qv.szxytkj.cn

Ruby: super
来源：http://rm.jianghongdianzi.cn

C#:   base.Greet();
来源：http://vq.jctech888.com.cn

[G08] 静态方法与属性
来源：http://mg.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mt.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://rc.huixiangedu.cn

JS:   static f() {}
来源：http://ga.asd995.cn

TS:   static f(): void {}
来源：http://qm.bjjhwx.cn

Java: static void f() {}
来源：http://ui.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ib.nicolike.cn

Ruby: def self.f; end
来源：http://sb.panjiajie.cn

C#:   public static void F() {}
来源：http://hb.nicolike.cn

[G09] 接口 / 抽象类
来源：http://xc.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://dt.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ov.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://by.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://sv.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://kl.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://kz.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hn.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ck.huixinmuqiang.cn

[G10] 访问控制
来源：http://qf.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://gk.szsharing.cn

PHP:  public / protected / private
来源：http://ie.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://pg.colortex.cn

TS:   public / protected / private
来源：http://gn.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ee.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wt.panjiajie.cn

Ruby: public / protected / private
来源：http://lp.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ne.yuexingan06.cn

[G11] getter / setter
来源：http://du.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ta.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ey.nicolike.cn

JS:   get name() { return this._name; }
来源：http://xc.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://ev.colortex.cn

Java: public String getName() { return name; }
来源：http://qg.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kq.colortex.cn

Ruby: attr_accessor :name
来源：http://hh.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://ly.hahajie.cn

[G12] 对象转字符串
来源：http://pl.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://co.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://la.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://gr.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://tx.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://xv.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zi.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://zk.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://fp.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://pq.huanxung.cn

Py:   isinstance(u, User)
来源：http://wh.panjiajie.cn

PHP:  $u instanceof User
来源：http://fu.hahajie.cn

JS:   u instanceof User
来源：http://un.huixinmuqiang.cn

TS:   u instanceof User
来源：http://ge.shxzskj.cn

Java: u instanceof User
来源：http://wm.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gk.nicolike.cn

Ruby: u.is_a?(User)
来源：http://mw.jianghongdianzi.cn

C#:   u is User
来源：http://li.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://gp.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qs.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://cu.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bo.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://sb.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://kt.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://od.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ny.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://vl.huanxung.cn

[G15] 枚举
来源：http://ad.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gu.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ml.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ut.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tx.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://iu.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xt.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://oy.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iz.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://wq.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rx.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://fo.hahajie.cn

JS:   Object.entries(obj)
来源：http://cs.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://dx.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gu.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jl.521024.cn

Ruby: obj.instance_variables
来源：http://ba.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://gw.huixiangedu.cn

================================================================================
来源：http://cn.muxihuayi.cn


<!-- 参考信息 -->