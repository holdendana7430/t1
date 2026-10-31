代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mw.panjiajie.cn

TS:   if (s === "") {}
来源：http://ia.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://ko.shxzukj.cn

Go:   if s == "" {}
来源：http://ew.bjjhwx.cn

Ruby: if s.empty?
来源：http://aj.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rn.szsharing.cn

[E21] 超长截断加省略号
来源：http://yl.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xk.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mq.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cs.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ro.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pk.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://us.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lt.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yc.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://az.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bh.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://px.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pg.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qt.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ed.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ns.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://zc.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dq.hahajie.cn

================================================================================
来源：http://qq.nszjky.cn

F. 文件与目录
来源：http://pz.hahajie.cn

================================================================================
来源：http://hb.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ak.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ij.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://hw.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vq.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://om.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://co.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xy.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://tq.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://nl.jctech888.com.cn

[F02] 逐行读取文件
来源：http://mi.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ry.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wf.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jp.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oe.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hi.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vn.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xa.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://fk.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hj.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://si.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://re.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jz.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zp.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sn.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://rg.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wp.shxzukj.cn

[F04] 追加写入文件
来源：http://ul.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zo.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://db.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zn.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pj.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uq.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ws.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qg.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vw.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://wg.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bq.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://fs.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://el.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://df.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gg.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vo.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://bd.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://pj.shxzukj.cn

[F06] 删除文件
来源：http://bd.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://np.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://nk.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xs.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ea.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fv.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://cn.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://cv.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://oy.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ir.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://se.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://da.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zd.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xz.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yh.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://do.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://if.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eg.haigaiapp.cn

[F08] 遍历目录
来源：http://nx.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ld.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pt.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://jk.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://bf.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ap.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ss.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://em.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://mf.huixiangedu.cn

[F09] 获取文件大小
来源：http://ig.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://so.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://fh.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://al.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://bb.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cs.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hr.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://zt.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://nn.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://fz.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zb.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yf.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://st.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://yy.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dq.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sx.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kc.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://re.bjjhwx.cn

[F11] 复制与移动文件
来源：http://fn.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ek.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ev.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://da.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://di.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rk.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vu.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://da.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vz.huixiangedu.cn

[F12] CSV 读写
来源：http://jo.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qk.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pt.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rd.bookmarksfly.cn

TS:   // 同上
来源：http://vz.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ge.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uj.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tm.szsharing.cn

================================================================================
来源：http://hn.wgjwhj.cn

G. 面向对象
来源：http://ra.huanxung.cn

================================================================================
来源：http://jd.bookmarksfly.cn

[G01] 定义类
来源：http://wq.hahajie.cn

Py:   class User: pass
来源：http://lx.gzmigu.cn

PHP:  class User {}
来源：http://bn.colortex.cn

JS:   class User {}
来源：http://hg.asd995.cn

TS:   class User { name: string = ""; }
来源：http://oi.szxytkj.cn

Java: class User {}
来源：http://ds.gzmigu.cn

Go:   type User struct { Name string }
来源：http://od.gzmigu.cn

Ruby: class User; end
来源：http://fl.huixiangedu.cn

C#:   class User {}
来源：http://ha.jianghongdianzi.cn

[G02] 构造函数
来源：http://ze.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://ht.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://fb.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://jq.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://df.521024.cn

Java: User(String name) { this.name = name; }
来源：http://vv.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jf.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ag.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://og.newstarts.cn

[G03] 实例属性
来源：http://ca.chemitech.net.cn

Py:   self.name = "x"
来源：http://dj.huanxung.cn

PHP:  public string $name = "x";
来源：http://ff.hahajie.cn

JS:   this.name = "x";
来源：http://rb.panjiajie.cn

TS:   name: string = "x";
来源：http://nu.nszjky.cn

Java: private String name;
来源：http://ak.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nw.colortex.cn

Ruby: @name = "x"
来源：http://ii.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://tk.wgjwhj.cn

[G04] 定义方法
来源：http://hy.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://pw.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tw.szsharing.cn

JS:   greet() { return this.name; }
来源：http://bp.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://fa.521024.cn

Java: String greet() { return name; }
来源：http://tl.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lp.lnxyls.cn

Ruby: def greet; @name; end
来源：http://du.nicolike.cn

C#:   public string Greet() => Name;
来源：http://uz.521024.cn

[G05] 继承
来源：http://qg.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://xb.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://ow.lnxyls.cn

JS:   class Admin extends User {}
来源：http://sd.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://bq.wgjwhj.cn

Java: class Admin extends User {}
来源：http://co.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vo.521024.cn

Ruby: class Admin < User; end
来源：http://nd.lnxyls.cn

C#:   class Admin : User {}
来源：http://gn.szxytkj.cn

[G06] 重写方法
来源：http://lr.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://fl.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ou.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ql.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ln.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://pj.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://er.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://cy.521024.cn

C#:   public override string Greet() => "admin";
来源：http://px.hnjuh.cn

[G07] 调用父类方法
来源：http://tx.jianghongdianzi.cn

Py:   super().greet()
来源：http://lm.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://yt.yuexingan06.cn

JS:   super.greet();
来源：http://kz.hahajie.cn

TS:   super.greet();
来源：http://tz.nicolike.cn

Java: super.greet();
来源：http://bw.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ib.newstarts.cn

Ruby: super
来源：http://ei.wgjwhj.cn

C#:   base.Greet();
来源：http://lu.9csxet.cn

[G08] 静态方法与属性
来源：http://hl.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fo.hahajie.cn

PHP:  public static function f() {}
来源：http://uo.szsharing.cn

JS:   static f() {}
来源：http://tx.yuexingan06.cn

TS:   static f(): void {}
来源：http://yl.nicolike.cn

Java: static void f() {}
来源：http://ui.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vv.shxzukj.cn

Ruby: def self.f; end
来源：http://sp.huixiangedu.cn

C#:   public static void F() {}
来源：http://zj.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://ky.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://wz.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ox.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vb.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://dc.huanxung.cn

Java: interface Shape { double area(); }
来源：http://ce.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://fn.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pr.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://cm.wgjwhj.cn

[G10] 访问控制
来源：http://um.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pk.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://bv.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ld.shtwfgs.cn

TS:   public / protected / private
来源：http://kw.521024.cn

Java: public / protected / private / 默认包级
来源：http://fh.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fs.newstarts.cn

Ruby: public / protected / private
来源：http://xc.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://wy.hahajie.cn

[G11] getter / setter
来源：http://bw.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://du.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hd.nszjky.cn

JS:   get name() { return this._name; }
来源：http://ew.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://vg.9csxet.cn

Java: public String getName() { return name; }
来源：http://uk.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ru.lnxyls.cn

Ruby: attr_accessor :name
来源：http://hr.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://ac.haigaiapp.cn

[G12] 对象转字符串
来源：http://fd.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://mz.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xf.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://eo.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://tw.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://pe.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nd.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://le.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://do.wgjwhj.cn

[G13] 判断对象类型
来源：http://kc.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://pl.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ms.panjiajie.cn

JS:   u instanceof User
来源：http://xj.bookmarksfly.cn

TS:   u instanceof User
来源：http://xi.haigaiapp.cn

Java: u instanceof User
来源：http://hl.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ze.nszjky.cn

Ruby: u.is_a?(User)
来源：http://dc.gzmigu.cn

C#:   u is User
来源：http://uc.huixiangedu.cn

[G14] 数据类 / record
来源：http://zk.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jg.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://et.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nw.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://yf.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ie.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://pp.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wu.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://cr.gzmigu.cn

[G15] 枚举
来源：http://rm.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zo.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://km.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vw.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jg.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://tn.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vy.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://xj.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hi.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://hk.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cp.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://pg.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://rl.lnxyls.cn

TS:   Object.entries(obj)
来源：http://vu.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cu.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qs.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://vr.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://gp.huixiangedu.cn

================================================================================
来源：http://mi.huanxung.cn

H. 异常与错误处理
来源：http://ck.yuntaijiaju.cn

================================================================================
来源：http://eb.shxzskj.cn

[H01] try / catch 基础
来源：http://fa.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://te.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pp.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xh.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://us.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vd.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ab.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ml.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://si.newstarts.cn

[H02] finally / ensure 收尾
来源：http://lm.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zw.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nw.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lz.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ie.huanxung.cn


<!-- 参考信息 -->