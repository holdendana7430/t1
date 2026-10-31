代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gi.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ht.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://by.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://da.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://pq.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://th.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tg.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lh.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wy.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ib.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sw.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kk.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bt.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://jw.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bs.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ly.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lo.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hu.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jg.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oz.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rt.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://re.shxzukj.cn

[E16] 数字千分位
来源：http://ik.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://wn.nicolike.cn

PHP:  number_format(1234567);
来源：http://mw.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jo.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nd.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zm.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xg.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hq.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://vz.huixiangedu.cn

[E17] 首字母大写
来源：http://ju.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mx.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vb.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vi.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xl.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hv.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zh.wgjwhj.cn

Ruby: s.capitalize
来源：http://lg.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qd.szsharing.cn

[E18] 模板占位符替换
来源：http://ec.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gr.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fj.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iq.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://be.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jx.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iy.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pt.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://se.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ye.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://bd.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cp.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://bo.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ld.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://av.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://dk.muxihuayi.cn

Ruby: s.lines
来源：http://mh.haigaiapp.cn

C#:   s.Split('\n')
来源：http://hh.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://jb.huixiangedu.cn

Py:   if not s:
来源：http://qf.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ig.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ix.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://eo.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://va.jctech888.com.cn

Go:   if s == "" {}
来源：http://dd.shxzskj.cn

Ruby: if s.empty?
来源：http://mo.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sn.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://vc.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cb.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://my.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yk.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xl.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ed.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://li.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fw.521024.cn

[E22] 字节长度与字符长度
来源：http://jg.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://al.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nv.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qy.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ij.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wl.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://qs.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pj.nicolike.cn

================================================================================
来源：http://rb.panjiajie.cn

F. 文件与目录
来源：http://kf.bjjhwx.cn

================================================================================
来源：http://xt.bookmarksfly.cn

[F01] 读取整个文件
来源：http://wn.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dk.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://mk.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eo.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sa.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nq.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dr.521024.cn

Ruby: File.read("a.txt")
来源：http://de.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://bd.szxytkj.cn

[F02] 逐行读取文件
来源：http://lo.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sn.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nq.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://em.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tx.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://od.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yz.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oy.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ma.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://rl.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fy.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xo.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fl.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xv.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tc.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fs.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://hf.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ea.bookmarksfly.cn

[F04] 追加写入文件
来源：http://pw.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qz.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cn.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kf.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://se.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://um.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cx.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ig.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rc.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://hr.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://jr.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://fl.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://mu.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rf.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bn.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://jw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://vc.bookmarksfly.cn

[F06] 删除文件
来源：http://xs.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://hx.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://yb.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qi.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xo.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bt.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://tf.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://tx.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://nx.newstarts.cn

[F07] 创建目录（含多级）
来源：http://cw.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lu.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://of.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ww.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ne.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ss.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jc.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vb.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eh.nicolike.cn

[F08] 遍历目录
来源：http://st.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jq.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iv.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://uj.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://vz.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sm.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ey.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://uj.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://lh.szxytkj.cn

[F09] 获取文件大小
来源：http://fl.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://uv.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://fn.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://cr.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://si.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rd.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sp.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://ny.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://zc.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://qv.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wv.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wf.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dr.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://se.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bu.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://se.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zy.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://px.panjiajie.cn

[F11] 复制与移动文件
来源：http://nj.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gm.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mm.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sp.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iu.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rr.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ra.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jy.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ye.huanxung.cn

[F12] CSV 读写
来源：http://eq.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gg.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bn.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lt.panjiajie.cn

TS:   // 同上
来源：http://fx.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pk.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ze.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wh.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mg.521024.cn

================================================================================
来源：http://he.521024.cn

G. 面向对象
来源：http://qk.9csxet.cn

================================================================================
来源：http://ww.bjjhwx.cn

[G01] 定义类
来源：http://nr.asd995.cn

Py:   class User: pass
来源：http://js.chemitech.net.cn

PHP:  class User {}
来源：http://nr.gzmigu.cn

JS:   class User {}
来源：http://ap.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://sv.huixinmuqiang.cn

Java: class User {}
来源：http://an.szsharing.cn

Go:   type User struct { Name string }
来源：http://mu.shtwfgs.cn

Ruby: class User; end
来源：http://cp.shxzukj.cn

C#:   class User {}
来源：http://in.hnjuh.cn

[G02] 构造函数
来源：http://tt.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://st.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://im.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://nt.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://wo.521024.cn

Java: User(String name) { this.name = name; }
来源：http://eq.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pd.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://rl.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://yt.huanxung.cn

[G03] 实例属性
来源：http://km.panjiajie.cn

Py:   self.name = "x"
来源：http://sz.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://cu.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://yw.jctech888.com.cn

TS:   name: string = "x";
来源：http://og.szxytkj.cn

Java: private String name;
来源：http://zc.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sb.muxihuayi.cn

Ruby: @name = "x"
来源：http://uu.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://rm.shxzskj.cn

[G04] 定义方法
来源：http://ww.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://jh.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ut.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://vo.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ra.hnjuh.cn

Java: String greet() { return name; }
来源：http://qn.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hn.szsharing.cn

Ruby: def greet; @name; end
来源：http://ek.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://lu.szxytkj.cn

[G05] 继承
来源：http://nr.colortex.cn

Py:   class Admin(User): pass
来源：http://sc.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://si.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://wj.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ol.nszjky.cn

Java: class Admin extends User {}
来源：http://wt.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uc.gzmigu.cn

Ruby: class Admin < User; end
来源：http://ll.gzmigu.cn

C#:   class Admin : User {}
来源：http://dl.haigaiapp.cn

[G06] 重写方法
来源：http://uj.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://vv.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://et.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://yr.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://tc.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://cb.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lb.521024.cn

Ruby: def greet; "admin"; end
来源：http://ez.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://vw.shtwfgs.cn

[G07] 调用父类方法
来源：http://bz.shxzskj.cn

Py:   super().greet()
来源：http://zf.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://vm.yuntaijiaju.cn

JS:   super.greet();
来源：http://dp.huixiangedu.cn

TS:   super.greet();
来源：http://xx.colortex.cn

Java: super.greet();
来源：http://wm.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jz.hahajie.cn

Ruby: super
来源：http://qy.shtwfgs.cn

C#:   base.Greet();
来源：http://bx.nicolike.cn

[G08] 静态方法与属性
来源：http://lz.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nt.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://bd.bookmarksfly.cn

JS:   static f() {}
来源：http://sm.nszjky.cn

TS:   static f(): void {}
来源：http://sq.521024.cn

Java: static void f() {}
来源：http://wb.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qz.szsharing.cn

Ruby: def self.f; end
来源：http://xm.muxihuayi.cn

C#:   public static void F() {}
来源：http://pe.szsharing.cn

[G09] 接口 / 抽象类
来源：http://or.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://zx.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rc.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dv.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://pm.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://st.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://md.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://il.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://ce.lnxyls.cn

[G10] 访问控制
来源：http://in.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kv.9csxet.cn

PHP:  public / protected / private
来源：http://oc.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ca.bookmarksfly.cn

TS:   public / protected / private
来源：http://pn.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://hy.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jg.gzmigu.cn

Ruby: public / protected / private
来源：http://hv.lnxyls.cn

C#:   public / protected / private / internal
来源：http://sc.hnjuh.cn

[G11] getter / setter
来源：http://ph.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://so.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ki.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://rf.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://yy.panjiajie.cn

Java: public String getName() { return name; }
来源：http://gv.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nc.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ng.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://pz.muxihuayi.cn

[G12] 对象转字符串
来源：http://cr.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://jc.huanxung.cn


<!-- 参考信息 -->