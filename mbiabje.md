代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yz.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sq.gzmigu.cn

TS:   if (s === "") {}
来源：http://lx.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://lo.lnxyls.cn

Go:   if s == "" {}
来源：http://mu.jctech888.com.cn

Ruby: if s.empty?
来源：http://zj.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dj.lnxyls.cn

[E21] 超长截断加省略号
来源：http://iz.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vv.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vq.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dp.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tx.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wf.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://fe.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://an.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fg.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://hq.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kd.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bz.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mc.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://br.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xu.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oz.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://bd.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ev.9csxet.cn

================================================================================
来源：http://qc.colortex.cn

F. 文件与目录
来源：http://rq.lnxyls.cn

================================================================================
来源：http://ux.newstarts.cn

[F01] 读取整个文件
来源：http://tq.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vm.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://bf.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uh.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jz.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wu.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uz.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://pf.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://qh.lnxyls.cn

[F02] 逐行读取文件
来源：http://yw.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vr.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://is.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ns.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lw.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sb.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vi.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ts.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gq.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ik.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eh.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://se.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yi.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kk.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://om.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://xf.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mm.jctech888.com.cn

[F04] 追加写入文件
来源：http://of.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fy.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nm.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mt.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://le.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yn.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qd.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fv.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pv.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://bi.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://un.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://yl.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://cn.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://oo.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kl.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://at.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://we.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://bw.chemitech.net.cn

[F06] 删除文件
来源：http://rx.9csxet.cn

Py:   os.remove("a.txt")
来源：http://al.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://sw.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://el.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ob.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oc.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://oa.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://wf.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://qm.9csxet.cn

[F07] 创建目录（含多级）
来源：http://ii.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qh.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ss.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jz.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xk.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cj.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zu.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nj.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ck.chemitech.net.cn

[F08] 遍历目录
来源：http://uu.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lm.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uc.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://mn.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://me.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uc.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zu.521024.cn

Ruby: Dir.children("dir")
来源：http://ir.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://gn.panjiajie.cn

[F09] 获取文件大小
来源：http://ku.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://qy.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://vw.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ku.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://cv.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hv.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jo.asd995.cn

Ruby: File.size("a.txt")
来源：http://qn.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://ci.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://el.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wl.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cz.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jy.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://yc.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yr.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ag.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ug.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eg.521024.cn

[F11] 复制与移动文件
来源：http://ws.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yu.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ns.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gl.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ov.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ai.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nf.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://js.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://it.nicolike.cn

[F12] CSV 读写
来源：http://es.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tb.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ix.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hp.colortex.cn

TS:   // 同上
来源：http://bg.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vv.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xx.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gv.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ea.huanxung.cn

================================================================================
来源：http://uo.haigaiapp.cn

G. 面向对象
来源：http://rl.bookmarksfly.cn

================================================================================
来源：http://oo.hahajie.cn

[G01] 定义类
来源：http://wo.szxytkj.cn

Py:   class User: pass
来源：http://kf.wgjwhj.cn

PHP:  class User {}
来源：http://cn.bookmarksfly.cn

JS:   class User {}
来源：http://fv.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://yl.shtwfgs.cn

Java: class User {}
来源：http://by.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://wx.jctech888.com.cn

Ruby: class User; end
来源：http://ds.asd995.cn

C#:   class User {}
来源：http://fr.wgjwhj.cn

[G02] 构造函数
来源：http://nt.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ik.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://aj.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://wr.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ol.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://cd.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://um.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://mr.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://qh.lnxyls.cn

[G03] 实例属性
来源：http://pf.521024.cn

Py:   self.name = "x"
来源：http://tk.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ba.muxihuayi.cn

JS:   this.name = "x";
来源：http://hs.lnxyls.cn

TS:   name: string = "x";
来源：http://lj.521024.cn

Java: private String name;
来源：http://ou.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://le.panjiajie.cn

Ruby: @name = "x"
来源：http://qm.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ev.huixiangedu.cn

[G04] 定义方法
来源：http://sq.hahajie.cn

Py:   def greet(self): return self.name
来源：http://rq.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xm.newstarts.cn

JS:   greet() { return this.name; }
来源：http://pd.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://oz.hnjuh.cn

Java: String greet() { return name; }
来源：http://it.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xh.panjiajie.cn

Ruby: def greet; @name; end
来源：http://cu.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://dz.shxzukj.cn

[G05] 继承
来源：http://ks.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://yr.newstarts.cn

PHP:  class Admin extends User {}
来源：http://op.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://sh.521024.cn

TS:   class Admin extends User {}
来源：http://ow.gzmigu.cn

Java: class Admin extends User {}
来源：http://xe.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://at.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://rn.szsharing.cn

C#:   class Admin : User {}
来源：http://uq.szxytkj.cn

[G06] 重写方法
来源：http://kp.colortex.cn

Py:   def greet(self): return "admin"
来源：http://yw.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bc.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://nm.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://ys.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xa.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ms.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ke.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://yh.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://nv.shtwfgs.cn

Py:   super().greet()
来源：http://sc.hahajie.cn

PHP:  parent::greet();
来源：http://ge.bookmarksfly.cn

JS:   super.greet();
来源：http://eq.9csxet.cn

TS:   super.greet();
来源：http://yb.nicolike.cn

Java: super.greet();
来源：http://rw.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xr.haigaiapp.cn

Ruby: super
来源：http://qt.bjjhwx.cn

C#:   base.Greet();
来源：http://np.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ip.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bx.9csxet.cn

PHP:  public static function f() {}
来源：http://vs.shtwfgs.cn

JS:   static f() {}
来源：http://uq.shtwfgs.cn

TS:   static f(): void {}
来源：http://mo.newstarts.cn

Java: static void f() {}
来源：http://fv.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dt.colortex.cn

Ruby: def self.f; end
来源：http://oq.chemitech.net.cn

C#:   public static void F() {}
来源：http://wj.newstarts.cn

[G09] 接口 / 抽象类
来源：http://xl.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ul.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ec.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xx.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://lm.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://ik.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://ft.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yu.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://hy.jianghongdianzi.cn

[G10] 访问控制
来源：http://nh.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://zr.huanxung.cn

PHP:  public / protected / private
来源：http://qz.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://xo.hahajie.cn

TS:   public / protected / private
来源：http://py.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://bg.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ig.newstarts.cn

Ruby: public / protected / private
来源：http://ko.hnjuh.cn

C#:   public / protected / private / internal
来源：http://eu.muxihuayi.cn

[G11] getter / setter
来源：http://jp.nszjky.cn

Py:   @property 与 @x.setter
来源：http://ox.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://go.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://lg.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ur.521024.cn

Java: public String getName() { return name; }
来源：http://ti.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rt.panjiajie.cn

Ruby: attr_accessor :name
来源：http://bv.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://kz.hahajie.cn

[G12] 对象转字符串
来源：http://pa.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ii.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wm.colortex.cn

JS:   toString() { return this.name; }
来源：http://ui.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://cj.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://er.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ok.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://di.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://vw.wgjwhj.cn

[G13] 判断对象类型
来源：http://fv.colortex.cn

Py:   isinstance(u, User)
来源：http://ax.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ot.nszjky.cn

JS:   u instanceof User
来源：http://ly.muxihuayi.cn

TS:   u instanceof User
来源：http://dp.szxytkj.cn

Java: u instanceof User
来源：http://ia.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qz.nszjky.cn

Ruby: u.is_a?(User)
来源：http://lg.wgjwhj.cn

C#:   u is User
来源：http://gm.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://sd.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://go.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://cq.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vc.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://gl.newstarts.cn

Java: record User(String name, int age) {}
来源：http://sf.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://qo.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vh.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://pg.gzmigu.cn

[G15] 枚举
来源：http://kq.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gs.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xy.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jg.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uo.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://qt.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ic.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ug.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ch.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://mc.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bo.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://cg.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ud.lnxyls.cn

TS:   Object.entries(obj)
来源：http://wu.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gh.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hj.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://lf.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://si.huixiangedu.cn

================================================================================
来源：http://bo.9csxet.cn

H. 异常与错误处理
来源：http://dl.shtwfgs.cn

================================================================================
来源：http://qo.bjjhwx.cn

[H01] try / catch 基础
来源：http://zd.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://op.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vx.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://os.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kl.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gq.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ov.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://om.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fp.nicolike.cn

[H02] finally / ensure 收尾
来源：http://fb.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://td.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gj.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ce.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tn.9csxet.cn


<!-- 参考信息 -->