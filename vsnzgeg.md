代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sj.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ps.nszjky.cn

Py:   s.splitlines()
来源：http://jc.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gz.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://nz.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://qf.hahajie.cn

Java: s.lines().toList()
来源：http://zt.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://al.szsharing.cn

Ruby: s.lines
来源：http://dj.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://fc.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://rl.nicolike.cn

Py:   if not s:
来源：http://gq.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yi.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tw.muxihuayi.cn

TS:   if (s === "") {}
来源：http://jp.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://qe.jctech888.com.cn

Go:   if s == "" {}
来源：http://ur.nszjky.cn

Ruby: if s.empty?
来源：http://vd.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vp.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://fg.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vo.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xz.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cf.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://op.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bg.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://oh.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fu.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sm.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://mf.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rn.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hg.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tk.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lo.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qi.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yw.521024.cn

Ruby: s.bytesize;  s.length
来源：http://ug.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ni.huixinmuqiang.cn

================================================================================
来源：http://vc.huanxung.cn

F. 文件与目录
来源：http://ky.shxzukj.cn

================================================================================
来源：http://sl.chemitech.net.cn

[F01] 读取整个文件
来源：http://et.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ki.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://qp.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wg.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cj.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://td.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cf.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://rq.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://vm.haigaiapp.cn

[F02] 逐行读取文件
来源：http://op.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qj.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ry.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ao.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zj.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://le.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lk.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cz.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ff.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wh.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://av.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://da.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xt.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pi.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ii.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://bb.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xr.panjiajie.cn

[F04] 追加写入文件
来源：http://sr.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xf.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zf.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kx.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zg.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://it.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dd.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tl.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fa.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://zj.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zm.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://rj.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://xc.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ly.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kl.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ed.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://xi.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://xc.wgjwhj.cn

[F06] 删除文件
来源：http://oj.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://py.colortex.cn

PHP:  unlink("a.txt");
来源：http://eo.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vk.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rr.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://du.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://vx.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://iu.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://hn.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://bs.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://me.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fk.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xj.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://px.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xl.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lu.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vp.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gx.huixiangedu.cn

[F08] 遍历目录
来源：http://wn.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ew.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ze.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://qt.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://rf.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jp.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://gb.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://if.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://he.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://gk.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://hf.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://gy.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://il.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fi.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pb.521024.cn

Ruby: File.size("a.txt")
来源：http://lj.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ck.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://yv.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hy.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ha.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ie.521024.cn

TS:   path.extname("a.txt")
来源：http://wj.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kj.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ho.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ke.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eg.lnxyls.cn

[F11] 复制与移动文件
来源：http://ep.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://we.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rg.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pu.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tn.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ic.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nn.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oi.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ov.bjjhwx.cn

[F12] CSV 读写
来源：http://oa.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ve.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mg.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ld.jctech888.com.cn

TS:   // 同上
来源：http://ro.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kw.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lm.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ir.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cw.huixiangedu.cn

================================================================================
来源：http://kp.yuntaijiaju.cn

G. 面向对象
来源：http://ja.colortex.cn

================================================================================
来源：http://zx.hnjuh.cn

[G01] 定义类
来源：http://ns.chemitech.net.cn

Py:   class User: pass
来源：http://oh.huanxung.cn

PHP:  class User {}
来源：http://jj.chemitech.net.cn

JS:   class User {}
来源：http://by.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://cl.panjiajie.cn

Java: class User {}
来源：http://ew.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://hy.muxihuayi.cn

Ruby: class User; end
来源：http://kh.muxihuayi.cn

C#:   class User {}
来源：http://yi.asd995.cn

[G02] 构造函数
来源：http://cg.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://cg.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://yt.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://co.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://mf.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://dy.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ht.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://fo.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://od.panjiajie.cn

[G03] 实例属性
来源：http://dc.colortex.cn

Py:   self.name = "x"
来源：http://ox.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://tz.hnjuh.cn

JS:   this.name = "x";
来源：http://it.jctech888.com.cn

TS:   name: string = "x";
来源：http://em.wgjwhj.cn

Java: private String name;
来源：http://np.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ky.nszjky.cn

Ruby: @name = "x"
来源：http://gx.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://uj.gzmigu.cn

[G04] 定义方法
来源：http://pu.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://tk.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qd.szsharing.cn

JS:   greet() { return this.name; }
来源：http://vb.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://mu.nicolike.cn

Java: String greet() { return name; }
来源：http://hw.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uv.szxytkj.cn

Ruby: def greet; @name; end
来源：http://rj.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://qn.hnjuh.cn

[G05] 继承
来源：http://ng.lnxyls.cn

Py:   class Admin(User): pass
来源：http://hh.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://xf.huanxung.cn

JS:   class Admin extends User {}
来源：http://ed.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://tb.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://xg.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ex.hahajie.cn

Ruby: class Admin < User; end
来源：http://yg.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://fe.jctech888.com.cn

[G06] 重写方法
来源：http://ds.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://xz.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iv.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://vu.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://bn.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://id.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ge.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ae.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://da.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://fa.bookmarksfly.cn

Py:   super().greet()
来源：http://zi.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://rz.colortex.cn

JS:   super.greet();
来源：http://eh.bookmarksfly.cn

TS:   super.greet();
来源：http://zz.colortex.cn

Java: super.greet();
来源：http://vv.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kx.szxytkj.cn

Ruby: super
来源：http://uy.wgjwhj.cn

C#:   base.Greet();
来源：http://mc.muxihuayi.cn

[G08] 静态方法与属性
来源：http://oq.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://we.gzmigu.cn

PHP:  public static function f() {}
来源：http://oj.colortex.cn

JS:   static f() {}
来源：http://cb.newstarts.cn

TS:   static f(): void {}
来源：http://ze.hahajie.cn

Java: static void f() {}
来源：http://io.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wy.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://fv.shxzukj.cn

C#:   public static void F() {}
来源：http://kg.colortex.cn

[G09] 接口 / 抽象类
来源：http://nd.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://jq.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lh.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wo.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://iy.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://vw.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ed.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pd.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://cx.nicolike.cn

[G10] 访问控制
来源：http://ji.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://wy.szsharing.cn

PHP:  public / protected / private
来源：http://au.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://je.bjjhwx.cn

TS:   public / protected / private
来源：http://cc.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://tw.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gt.521024.cn

Ruby: public / protected / private
来源：http://xv.lnxyls.cn

C#:   public / protected / private / internal
来源：http://pf.shxzukj.cn

[G11] getter / setter
来源：http://uw.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://sk.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ev.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://ay.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ub.colortex.cn

Java: public String getName() { return name; }
来源：http://tz.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oe.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://jb.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://gy.huanxung.cn

[G12] 对象转字符串
来源：http://xy.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://og.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ew.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://pi.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://ls.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://qi.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://el.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ai.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://lx.asd995.cn

[G13] 判断对象类型
来源：http://hh.panjiajie.cn

Py:   isinstance(u, User)
来源：http://vw.chemitech.net.cn

PHP:  $u instanceof User
来源：http://as.wgjwhj.cn

JS:   u instanceof User
来源：http://rd.shxzskj.cn

TS:   u instanceof User
来源：http://yj.hahajie.cn

Java: u instanceof User
来源：http://rt.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qk.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://fh.jianghongdianzi.cn

C#:   u is User
来源：http://wt.panjiajie.cn

[G14] 数据类 / record
来源：http://hy.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oh.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://om.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wa.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://mr.colortex.cn

Java: record User(String name, int age) {}
来源：http://cu.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://jm.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jh.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://al.szsharing.cn

[G15] 枚举
来源：http://ww.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://he.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vk.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wq.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eh.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ae.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kz.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://aq.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ly.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ej.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bt.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://um.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://nm.9csxet.cn

TS:   Object.entries(obj)
来源：http://uk.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jh.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bo.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://dd.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://pt.shxzukj.cn

================================================================================
来源：http://ve.shxzskj.cn

H. 异常与错误处理
来源：http://ip.shxzukj.cn

================================================================================
来源：http://nm.shxzukj.cn

[H01] try / catch 基础
来源：http://nh.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ec.jianghongdianzi.cn


<!-- 参考信息 -->