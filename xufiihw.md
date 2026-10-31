代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zm.nicolike.cn

[E19] 多行文本按行拆分
来源：http://zh.newstarts.cn

Py:   s.splitlines()
来源：http://ul.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sd.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://zz.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://ge.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://qy.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://dh.huixiangedu.cn

Ruby: s.lines
来源：http://qp.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://pm.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://ht.9csxet.cn

Py:   if not s:
来源：http://hw.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mm.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kd.gzmigu.cn

TS:   if (s === "") {}
来源：http://ir.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://jp.newstarts.cn

Go:   if s == "" {}
来源：http://dm.huixiangedu.cn

Ruby: if s.empty?
来源：http://bu.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ry.lnxyls.cn

[E21] 超长截断加省略号
来源：http://ll.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zu.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://je.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ql.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vs.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ry.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ce.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hw.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://kj.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://md.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dn.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vc.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zh.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bh.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zw.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://lp.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zb.jctech888.com.cn

================================================================================
来源：http://dm.521024.cn

F. 文件与目录
来源：http://ai.shxzukj.cn

================================================================================
来源：http://tl.bookmarksfly.cn

[F01] 读取整个文件
来源：http://hz.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pb.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://hn.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xb.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ku.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ng.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kw.asd995.cn

Ruby: File.read("a.txt")
来源：http://zl.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://lq.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://cw.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rv.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yu.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ad.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vp.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vm.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ap.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gm.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aj.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://ed.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xw.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://he.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dy.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tp.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ln.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wo.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://rz.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zy.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://lm.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ax.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oo.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://im.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zg.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ls.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oo.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://no.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ga.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://gs.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yc.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://jr.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://oy.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://bt.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hv.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tz.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://mv.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://db.nszjky.cn

[F06] 删除文件
来源：http://nw.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://uu.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://rq.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gv.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fq.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xq.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://rk.521024.cn

Ruby: File.delete("a.txt")
来源：http://ti.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://mm.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://nd.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ag.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lo.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://se.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eb.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://do.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nv.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yf.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wt.521024.cn

[F08] 遍历目录
来源：http://nc.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fx.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wq.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://vs.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://cw.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iz.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oa.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://qg.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://kd.muxihuayi.cn

[F09] 获取文件大小
来源：http://fm.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://jp.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://fg.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://ic.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://qx.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rf.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kr.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://tx.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://sw.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://pw.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sz.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://is.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ef.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://dh.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xh.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yl.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nc.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://no.asd995.cn

[F11] 复制与移动文件
来源：http://nh.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rd.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hd.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rx.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iu.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ij.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gv.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lk.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uh.yuexingan06.cn

[F12] CSV 读写
来源：http://dy.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ey.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yj.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wh.bookmarksfly.cn

TS:   // 同上
来源：http://qq.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jo.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yi.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gl.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sa.newstarts.cn

================================================================================
来源：http://fg.huanxung.cn

G. 面向对象
来源：http://bt.shtwfgs.cn

================================================================================
来源：http://uo.nszjky.cn

[G01] 定义类
来源：http://mv.colortex.cn

Py:   class User: pass
来源：http://hb.hahajie.cn

PHP:  class User {}
来源：http://jf.9csxet.cn

JS:   class User {}
来源：http://cp.colortex.cn

TS:   class User { name: string = ""; }
来源：http://nq.shxzukj.cn

Java: class User {}
来源：http://gq.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://uo.hahajie.cn

Ruby: class User; end
来源：http://iw.shtwfgs.cn

C#:   class User {}
来源：http://oj.bjjhwx.cn

[G02] 构造函数
来源：http://bm.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ul.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://gm.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://nl.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://pj.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://yg.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yz.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://qv.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.jctech888.com.cn

[G03] 实例属性
来源：http://rh.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://tm.colortex.cn

PHP:  public string $name = "x";
来源：http://ko.huanxung.cn

JS:   this.name = "x";
来源：http://aa.bjjhwx.cn

TS:   name: string = "x";
来源：http://ep.bookmarksfly.cn

Java: private String name;
来源：http://pi.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uq.hahajie.cn

Ruby: @name = "x"
来源：http://ss.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://kb.huixinmuqiang.cn

[G04] 定义方法
来源：http://ch.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://kh.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hw.szsharing.cn

JS:   greet() { return this.name; }
来源：http://qi.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://lq.huixiangedu.cn

Java: String greet() { return name; }
来源：http://ru.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fe.nicolike.cn

Ruby: def greet; @name; end
来源：http://sq.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://xu.jctech888.com.cn

[G05] 继承
来源：http://qo.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://xo.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://vw.hahajie.cn

JS:   class Admin extends User {}
来源：http://kq.newstarts.cn

TS:   class Admin extends User {}
来源：http://io.colortex.cn

Java: class Admin extends User {}
来源：http://wx.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://em.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ae.9csxet.cn

C#:   class Admin : User {}
来源：http://vq.jctech888.com.cn

[G06] 重写方法
来源：http://ui.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://fw.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ma.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://uj.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://bf.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://av.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hf.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://wj.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://et.muxihuayi.cn

[G07] 调用父类方法
来源：http://ea.szxytkj.cn

Py:   super().greet()
来源：http://pr.hnjuh.cn

PHP:  parent::greet();
来源：http://kp.bookmarksfly.cn

JS:   super.greet();
来源：http://hi.huixiangedu.cn

TS:   super.greet();
来源：http://az.lnxyls.cn

Java: super.greet();
来源：http://iu.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wk.bjjhwx.cn

Ruby: super
来源：http://rp.huanxung.cn

C#:   base.Greet();
来源：http://yg.szxytkj.cn

[G08] 静态方法与属性
来源：http://it.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fg.asd995.cn

PHP:  public static function f() {}
来源：http://ak.szxytkj.cn

JS:   static f() {}
来源：http://fo.panjiajie.cn

TS:   static f(): void {}
来源：http://jq.huixinmuqiang.cn

Java: static void f() {}
来源：http://zu.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qw.colortex.cn

Ruby: def self.f; end
来源：http://ay.shxzukj.cn

C#:   public static void F() {}
来源：http://ly.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://hh.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://fq.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fb.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xu.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://av.nszjky.cn

Java: interface Shape { double area(); }
来源：http://pp.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://ud.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pl.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://pz.shxzskj.cn

[G10] 访问控制
来源：http://uv.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://af.bookmarksfly.cn

PHP:  public / protected / private
来源：http://wx.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ra.asd995.cn

TS:   public / protected / private
来源：http://ys.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://qv.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eq.yuexingan06.cn

Ruby: public / protected / private
来源：http://ri.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://vr.hahajie.cn

[G11] getter / setter
来源：http://ut.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://rd.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ld.newstarts.cn

JS:   get name() { return this._name; }
来源：http://pj.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://rv.panjiajie.cn

Java: public String getName() { return name; }
来源：http://yh.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uq.huanxung.cn

Ruby: attr_accessor :name
来源：http://dl.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://kz.hnjuh.cn

[G12] 对象转字符串
来源：http://dc.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://rq.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vw.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://my.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://zi.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://sh.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wa.521024.cn

Ruby: def to_s; @name; end
来源：http://bp.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://qe.hnjuh.cn

[G13] 判断对象类型
来源：http://ev.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://ko.yuexingan06.cn

PHP:  $u instanceof User
来源：http://yb.yuntaijiaju.cn

JS:   u instanceof User
来源：http://xm.asd995.cn

TS:   u instanceof User
来源：http://qi.nszjky.cn

Java: u instanceof User
来源：http://sp.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mz.szsharing.cn

Ruby: u.is_a?(User)
来源：http://zq.shtwfgs.cn

C#:   u is User
来源：http://na.9csxet.cn

[G14] 数据类 / record
来源：http://nb.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gm.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rg.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yo.521024.cn

TS:   type User = { name: string; age: number };
来源：http://fj.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ql.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ef.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hn.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://yu.huixiangedu.cn

[G15] 枚举
来源：http://nh.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ib.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://go.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ag.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hm.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://hm.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dw.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://rp.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gu.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ef.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ak.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://kp.nszjky.cn

JS:   Object.entries(obj)
来源：http://kd.nszjky.cn

TS:   Object.entries(obj)
来源：http://le.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vx.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://of.nszjky.cn

Ruby: obj.instance_variables
来源：http://rg.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://xd.lnxyls.cn

================================================================================
来源：http://ry.521024.cn

H. 异常与错误处理
来源：http://ty.chemitech.net.cn

================================================================================
来源：http://iw.gzmigu.cn

[H01] try / catch 基础
来源：http://ao.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://df.panjiajie.cn


<!-- 参考信息 -->