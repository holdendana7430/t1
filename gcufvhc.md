代发 wailian999

Ruby: s.lines
来源：http://eh.wgjwhj.cn

C#:   s.Split('\n')
来源：http://lm.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://zz.521024.cn

Py:   if not s:
来源：http://hj.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dj.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ws.nicolike.cn

TS:   if (s === "") {}
来源：http://wg.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://vt.huanxung.cn

Go:   if s == "" {}
来源：http://gm.chemitech.net.cn

Ruby: if s.empty?
来源：http://qf.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tu.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://mc.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rq.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vm.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ca.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zw.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://se.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://le.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rg.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kf.hahajie.cn

[E22] 字节长度与字符长度
来源：http://uf.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pa.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tt.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yh.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dj.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qa.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kp.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://dq.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wd.huanxung.cn

================================================================================
来源：http://vu.huixiangedu.cn

F. 文件与目录
来源：http://ou.asd995.cn

================================================================================
来源：http://zc.wgjwhj.cn

[F01] 读取整个文件
来源：http://vm.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://il.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://ts.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qs.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cm.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ei.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vy.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ni.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://je.panjiajie.cn

[F02] 逐行读取文件
来源：http://rk.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dm.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bd.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tx.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zq.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ta.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zb.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uu.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xh.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://tj.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ic.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gs.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eg.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zw.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eg.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jk.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://sv.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wy.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://al.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bd.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ag.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jt.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mj.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fb.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jz.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://km.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ct.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://xf.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gg.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://nv.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ir.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://db.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hi.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ij.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://cy.521024.cn

C#:   File.Exists("a.txt")
来源：http://jl.wgjwhj.cn

[F06] 删除文件
来源：http://zx.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://ck.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://md.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tn.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ja.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hr.asd995.cn

Go:   os.Remove("a.txt")
来源：http://lo.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://kf.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://kd.hahajie.cn

[F07] 创建目录（含多级）
来源：http://qv.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qt.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oi.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ja.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kp.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bb.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zf.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://al.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wk.nszjky.cn

[F08] 遍历目录
来源：http://aa.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dn.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://le.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://ac.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://qb.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gn.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gt.nszjky.cn

Ruby: Dir.children("dir")
来源：http://cc.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://ml.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://gl.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://pi.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://ei.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://wl.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://xt.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ic.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ve.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://dc.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://np.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://hv.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kd.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rs.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cj.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://fa.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rd.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fm.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://em.huanxung.cn

[F11] 复制与移动文件
来源：http://gm.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mz.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ud.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tx.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gw.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ff.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://to.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zb.hnjuh.cn

[F12] CSV 读写
来源：http://si.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hi.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vf.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wt.hahajie.cn

TS:   // 同上
来源：http://gf.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wm.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://it.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fd.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://er.haigaiapp.cn

================================================================================
来源：http://zc.gzmigu.cn

G. 面向对象
来源：http://nk.lnxyls.cn

================================================================================
来源：http://te.chemitech.net.cn

[G01] 定义类
来源：http://jn.hahajie.cn

Py:   class User: pass
来源：http://fi.huixinmuqiang.cn

PHP:  class User {}
来源：http://zk.huixiangedu.cn

JS:   class User {}
来源：http://fn.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://hv.szxytkj.cn

Java: class User {}
来源：http://li.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://hp.haigaiapp.cn

Ruby: class User; end
来源：http://te.jianghongdianzi.cn

C#:   class User {}
来源：http://hj.hnjuh.cn

[G02] 构造函数
来源：http://oa.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://um.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ic.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ko.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://eq.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://gi.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ht.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ym.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://et.lnxyls.cn

[G03] 实例属性
来源：http://nb.muxihuayi.cn

Py:   self.name = "x"
来源：http://tu.lnxyls.cn

PHP:  public string $name = "x";
来源：http://qy.muxihuayi.cn

JS:   this.name = "x";
来源：http://mr.gzmigu.cn

TS:   name: string = "x";
来源：http://ib.jianghongdianzi.cn

Java: private String name;
来源：http://wn.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dm.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://fk.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://tb.haigaiapp.cn

[G04] 定义方法
来源：http://gc.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://tq.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zz.huanxung.cn

JS:   greet() { return this.name; }
来源：http://zz.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://mc.nszjky.cn

Java: String greet() { return name; }
来源：http://vd.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wt.hahajie.cn

Ruby: def greet; @name; end
来源：http://sw.hahajie.cn

C#:   public string Greet() => Name;
来源：http://me.szxytkj.cn

[G05] 继承
来源：http://kj.9csxet.cn

Py:   class Admin(User): pass
来源：http://vp.nszjky.cn

PHP:  class Admin extends User {}
来源：http://lj.hahajie.cn

JS:   class Admin extends User {}
来源：http://jn.nicolike.cn

TS:   class Admin extends User {}
来源：http://nr.colortex.cn

Java: class Admin extends User {}
来源：http://va.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hr.nszjky.cn

Ruby: class Admin < User; end
来源：http://uq.haigaiapp.cn

C#:   class Admin : User {}
来源：http://cp.asd995.cn

[G06] 重写方法
来源：http://fh.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://gu.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vs.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://po.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://nt.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://io.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rj.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://yr.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://gz.hnjuh.cn

[G07] 调用父类方法
来源：http://gq.colortex.cn

Py:   super().greet()
来源：http://ll.szxytkj.cn

PHP:  parent::greet();
来源：http://fp.wgjwhj.cn

JS:   super.greet();
来源：http://nu.szsharing.cn

TS:   super.greet();
来源：http://ap.hnjuh.cn

Java: super.greet();
来源：http://fi.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uj.shxzukj.cn

Ruby: super
来源：http://mj.gzmigu.cn

C#:   base.Greet();
来源：http://eh.szsharing.cn

[G08] 静态方法与属性
来源：http://ju.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fl.hnjuh.cn

PHP:  public static function f() {}
来源：http://rr.huixiangedu.cn

JS:   static f() {}
来源：http://wj.huixiangedu.cn

TS:   static f(): void {}
来源：http://vl.colortex.cn

Java: static void f() {}
来源：http://uv.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ij.yuexingan06.cn

Ruby: def self.f; end
来源：http://tu.nicolike.cn

C#:   public static void F() {}
来源：http://fy.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://xq.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://xa.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rk.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wl.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://wn.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://bf.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://yk.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ds.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://ol.chemitech.net.cn

[G10] 访问控制
来源：http://zp.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://bd.colortex.cn

PHP:  public / protected / private
来源：http://rt.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://ik.huanxung.cn

TS:   public / protected / private
来源：http://re.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://zu.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hv.lnxyls.cn

Ruby: public / protected / private
来源：http://je.9csxet.cn

C#:   public / protected / private / internal
来源：http://iq.bookmarksfly.cn

[G11] getter / setter
来源：http://ls.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://su.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zd.nszjky.cn

JS:   get name() { return this._name; }
来源：http://cl.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://et.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://cn.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cb.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://dn.colortex.cn

C#:   public string Name { get; set; }
来源：http://qi.asd995.cn

[G12] 对象转字符串
来源：http://th.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://qs.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mf.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://eq.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://ke.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://zd.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hahajie.cn

Ruby: def to_s; @name; end
来源：http://lv.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://hp.shtwfgs.cn

[G13] 判断对象类型
来源：http://ow.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://fm.bjjhwx.cn

PHP:  $u instanceof User
来源：http://pa.shtwfgs.cn

JS:   u instanceof User
来源：http://qj.hnjuh.cn

TS:   u instanceof User
来源：http://qr.9csxet.cn

Java: u instanceof User
来源：http://qk.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ou.9csxet.cn

Ruby: u.is_a?(User)
来源：http://lu.yuexingan06.cn

C#:   u is User
来源：http://mc.hnjuh.cn

[G14] 数据类 / record
来源：http://jh.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cb.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://sa.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mx.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://pp.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://hf.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://tc.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sx.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://il.521024.cn

[G15] 枚举
来源：http://jt.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sb.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ef.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cr.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ux.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ei.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ck.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://xz.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pg.asd995.cn

[G16] 对象转数组 / 字典
来源：http://nk.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wq.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://gp.shxzukj.cn

JS:   Object.entries(obj)
来源：http://yk.lnxyls.cn

TS:   Object.entries(obj)
来源：http://xf.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ek.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fz.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://yv.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://by.huanxung.cn

================================================================================
来源：http://ef.bjjhwx.cn

H. 异常与错误处理
来源：http://av.asd995.cn

================================================================================
来源：http://bn.szsharing.cn

[H01] try / catch 基础
来源：http://qa.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hb.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dw.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ei.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nd.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xv.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dt.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ka.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cm.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xo.huixinmuqiang.cn


<!-- 参考信息 -->