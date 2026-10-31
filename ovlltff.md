代发 wailian999

Ruby: s.lines
来源：http://nw.huixiangedu.cn

C#:   s.Split('\n')
来源：http://az.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://kc.jctech888.com.cn

Py:   if not s:
来源：http://ft.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zy.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://py.newstarts.cn

TS:   if (s === "") {}
来源：http://ys.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://rf.panjiajie.cn

Go:   if s == "" {}
来源：http://zw.shtwfgs.cn

Ruby: if s.empty?
来源：http://nq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zm.colortex.cn

[E21] 超长截断加省略号
来源：http://sb.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pn.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cp.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wg.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gn.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ei.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://wh.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ql.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://en.nszjky.cn

[E22] 字节长度与字符长度
来源：http://vu.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kd.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://by.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ba.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vp.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sa.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dx.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://aq.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zc.bookmarksfly.cn

================================================================================
来源：http://kb.newstarts.cn

F. 文件与目录
来源：http://gs.nicolike.cn

================================================================================
来源：http://tk.szsharing.cn

[F01] 读取整个文件
来源：http://dd.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cg.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://ee.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wn.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ks.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://um.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xo.hahajie.cn

Ruby: File.read("a.txt")
来源：http://cj.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://jw.nszjky.cn

[F02] 逐行读取文件
来源：http://yn.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fv.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ro.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jp.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://od.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tw.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://do.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fv.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gw.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ye.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://un.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xb.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://np.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pt.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xi.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mg.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://cg.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://si.shtwfgs.cn

[F04] 追加写入文件
来源：http://xv.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jc.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oa.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dd.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ou.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gg.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sw.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ag.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ak.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://of.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pp.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://me.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://vn.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://xr.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vt.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ye.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://in.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://de.lnxyls.cn

[F06] 删除文件
来源：http://oy.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://zs.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://dr.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jc.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wz.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://la.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://vs.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://sc.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://sb.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://mt.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dd.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mi.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oz.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lj.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ll.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jf.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qu.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pa.521024.cn

[F08] 遍历目录
来源：http://vi.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://te.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jt.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://za.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://fj.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rd.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://il.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://ji.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://xj.nszjky.cn

[F09] 获取文件大小
来源：http://gc.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://vx.9csxet.cn

PHP:  filesize("a.txt");
来源：http://ke.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://yz.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://al.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ps.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tv.asd995.cn

Ruby: File.size("a.txt")
来源：http://gk.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://nr.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://tt.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yq.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zs.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nq.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://wj.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hv.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ow.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uh.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pr.chemitech.net.cn

[F11] 复制与移动文件
来源：http://oy.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xv.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dh.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ng.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gs.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bj.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qy.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pb.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nh.bjjhwx.cn

[F12] CSV 读写
来源：http://cs.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qk.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lh.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kt.szxytkj.cn

TS:   // 同上
来源：http://fv.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yg.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rf.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mi.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qj.nszjky.cn

================================================================================
来源：http://ap.521024.cn

G. 面向对象
来源：http://iv.nicolike.cn

================================================================================
来源：http://fn.colortex.cn

[G01] 定义类
来源：http://eq.huixiangedu.cn

Py:   class User: pass
来源：http://vb.haigaiapp.cn

PHP:  class User {}
来源：http://ww.szsharing.cn

JS:   class User {}
来源：http://cv.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://xp.szsharing.cn

Java: class User {}
来源：http://jm.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://hi.panjiajie.cn

Ruby: class User; end
来源：http://hw.newstarts.cn

C#:   class User {}
来源：http://ah.yuntaijiaju.cn

[G02] 构造函数
来源：http://mn.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://tg.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://ge.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://nr.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://xb.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://cu.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hl.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://lc.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://rj.gzmigu.cn

[G03] 实例属性
来源：http://fj.nszjky.cn

Py:   self.name = "x"
来源：http://ap.colortex.cn

PHP:  public string $name = "x";
来源：http://ib.asd995.cn

JS:   this.name = "x";
来源：http://vt.nicolike.cn

TS:   name: string = "x";
来源：http://zv.jianghongdianzi.cn

Java: private String name;
来源：http://gz.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ya.9csxet.cn

Ruby: @name = "x"
来源：http://bs.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://xb.hnjuh.cn

[G04] 定义方法
来源：http://kj.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://mg.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rb.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://sd.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://ug.hahajie.cn

Java: String greet() { return name; }
来源：http://wj.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qh.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://hh.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://av.nicolike.cn

[G05] 继承
来源：http://xv.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://um.9csxet.cn

PHP:  class Admin extends User {}
来源：http://wm.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://re.newstarts.cn

TS:   class Admin extends User {}
来源：http://bs.szxytkj.cn

Java: class Admin extends User {}
来源：http://jq.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ix.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://ks.newstarts.cn

C#:   class Admin : User {}
来源：http://gu.bjjhwx.cn

[G06] 重写方法
来源：http://cp.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://az.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eq.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://np.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://om.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://sb.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tw.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://py.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://hs.haigaiapp.cn

[G07] 调用父类方法
来源：http://we.yuexingan06.cn

Py:   super().greet()
来源：http://uh.szxytkj.cn

PHP:  parent::greet();
来源：http://vo.jctech888.com.cn

JS:   super.greet();
来源：http://uk.jianghongdianzi.cn

TS:   super.greet();
来源：http://hw.newstarts.cn

Java: super.greet();
来源：http://ak.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wq.haigaiapp.cn

Ruby: super
来源：http://vr.haigaiapp.cn

C#:   base.Greet();
来源：http://bi.panjiajie.cn

[G08] 静态方法与属性
来源：http://ae.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ww.jctech888.com.cn

PHP:  public static function f() {}
来源：http://dd.jctech888.com.cn

JS:   static f() {}
来源：http://rr.shxzukj.cn

TS:   static f(): void {}
来源：http://jt.bookmarksfly.cn

Java: static void f() {}
来源：http://pc.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qg.bookmarksfly.cn

Ruby: def self.f; end
来源：http://nq.huixiangedu.cn

C#:   public static void F() {}
来源：http://th.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://pv.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://in.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hf.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://sx.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://wq.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ob.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mh.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://pn.huanxung.cn

[G10] 访问控制
来源：http://qa.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://uo.hahajie.cn

PHP:  public / protected / private
来源：http://ml.asd995.cn

JS:   #private 字段；其余公开
来源：http://aq.lnxyls.cn

TS:   public / protected / private
来源：http://sh.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://oq.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ci.huixiangedu.cn

Ruby: public / protected / private
来源：http://mh.szxytkj.cn

C#:   public / protected / private / internal
来源：http://il.haigaiapp.cn

[G11] getter / setter
来源：http://zv.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://hp.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yh.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gv.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ug.colortex.cn

Java: public String getName() { return name; }
来源：http://wo.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://we.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://gl.nicolike.cn

C#:   public string Name { get; set; }
来源：http://hg.panjiajie.cn

[G12] 对象转字符串
来源：http://oe.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://si.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://po.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://iq.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://wm.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://eb.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cw.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://er.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://dn.jctech888.com.cn

[G13] 判断对象类型
来源：http://ta.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://uk.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://lb.9csxet.cn

JS:   u instanceof User
来源：http://rm.huixiangedu.cn

TS:   u instanceof User
来源：http://ux.nszjky.cn

Java: u instanceof User
来源：http://dw.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lj.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://mt.wgjwhj.cn

C#:   u is User
来源：http://ot.shxzukj.cn

[G14] 数据类 / record
来源：http://vc.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://am.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://lf.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kl.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://pv.newstarts.cn

Java: record User(String name, int age) {}
来源：http://xs.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://zu.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mo.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://on.lnxyls.cn

[G15] 枚举
来源：http://rd.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gb.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tz.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lq.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zh.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://xn.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ac.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://ft.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tf.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://xy.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rf.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://hv.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://gi.521024.cn

TS:   Object.entries(obj)
来源：http://ti.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nd.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ie.shxzukj.cn

Ruby: obj.instance_variables
来源：http://mo.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://gt.szxytkj.cn

================================================================================
来源：http://ut.wgjwhj.cn

H. 异常与错误处理
来源：http://ej.nszjky.cn

================================================================================
来源：http://yk.521024.cn

[H01] try / catch 基础
来源：http://bk.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zo.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qu.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kk.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ol.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ei.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://st.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cs.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bc.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://dr.hahajie.cn


<!-- 参考信息 -->