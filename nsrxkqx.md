代发 wailian999

Py:   for ch in s: print(ch)
来源：http://kx.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gp.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lo.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xe.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qz.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iz.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sg.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vg.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ij.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sj.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gv.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pg.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://th.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mc.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pt.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ft.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hj.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://ct.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lg.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jx.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pv.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kn.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kk.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hm.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ff.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hj.szxytkj.cn

[E16] 数字千分位
来源：http://lf.newstarts.cn

Py:   f"{1234567:,}"
来源：http://fe.huanxung.cn

PHP:  number_format(1234567);
来源：http://iu.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hq.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://je.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vq.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qp.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://aq.yuexingan06.cn

[E17] 首字母大写
来源：http://ri.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mv.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cv.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://st.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://df.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ad.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://io.panjiajie.cn

Ruby: s.capitalize
来源：http://yu.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rg.colortex.cn

[E18] 模板占位符替换
来源：http://pq.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xu.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jd.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rd.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kq.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qn.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tx.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jq.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ik.asd995.cn

[E19] 多行文本按行拆分
来源：http://rm.haigaiapp.cn

Py:   s.splitlines()
来源：http://pl.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://of.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://nq.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://kj.nszjky.cn

Java: s.lines().toList()
来源：http://hl.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://nb.chemitech.net.cn

Ruby: s.lines
来源：http://wk.szsharing.cn

C#:   s.Split('\n')
来源：http://iv.szsharing.cn

[E20] 判断字符串是否为空
来源：http://dz.huanxung.cn

Py:   if not s:
来源：http://nv.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eq.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gc.nszjky.cn

TS:   if (s === "") {}
来源：http://fb.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://xo.lnxyls.cn

Go:   if s == "" {}
来源：http://oj.huixiangedu.cn

Ruby: if s.empty?
来源：http://lw.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wo.nszjky.cn

[E21] 超长截断加省略号
来源：http://yq.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gz.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://th.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bq.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iu.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jl.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://js.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ix.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://de.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://ux.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zz.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://so.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://io.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jl.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yl.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://or.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://tc.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uh.jctech888.com.cn

================================================================================
来源：http://ll.hahajie.cn

F. 文件与目录
来源：http://kf.szxytkj.cn

================================================================================
来源：http://tv.muxihuayi.cn

[F01] 读取整个文件
来源：http://ic.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vk.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ay.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vw.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://di.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vs.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ks.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://nd.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://km.szsharing.cn

[F02] 逐行读取文件
来源：http://wf.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://il.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ny.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ir.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qe.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cc.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tj.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://za.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ij.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://dr.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wl.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cn.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kd.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ga.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eh.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gz.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qz.hnjuh.cn

[F04] 追加写入文件
来源：http://eq.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rg.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ua.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wh.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ux.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://la.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ts.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ph.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://qi.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xq.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://wz.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://ch.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://zo.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yu.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ba.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://xr.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ji.hnjuh.cn

[F06] 删除文件
来源：http://ct.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://pv.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ls.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yn.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jm.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gy.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://vu.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://hx.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://zf.asd995.cn

[F07] 创建目录（含多级）
来源：http://bl.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zy.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pu.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://so.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qz.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ox.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pm.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ux.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hl.shxzskj.cn

[F08] 遍历目录
来源：http://ia.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kp.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iw.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ix.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://hp.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vd.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yl.asd995.cn

Ruby: Dir.children("dir")
来源：http://ci.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://jd.yuexingan06.cn

[F09] 获取文件大小
来源：http://lk.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://fs.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://nd.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://mr.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://gh.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ms.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ae.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://oa.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://px.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://yb.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kh.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sd.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://du.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://so.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ek.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kh.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vm.szxytkj.cn

[F11] 复制与移动文件
来源：http://vu.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uq.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rd.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hs.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nc.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ky.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hb.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ko.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dc.9csxet.cn

[F12] CSV 读写
来源：http://pe.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xd.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ma.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bh.huanxung.cn

TS:   // 同上
来源：http://rd.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bl.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pe.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yh.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zj.bookmarksfly.cn

================================================================================
来源：http://vh.chemitech.net.cn

G. 面向对象
来源：http://ow.hnjuh.cn

================================================================================
来源：http://ka.jianghongdianzi.cn

[G01] 定义类
来源：http://ni.shxzskj.cn

Py:   class User: pass
来源：http://nl.lnxyls.cn

PHP:  class User {}
来源：http://an.chemitech.net.cn

JS:   class User {}
来源：http://yc.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://wg.newstarts.cn

Java: class User {}
来源：http://cb.hahajie.cn

Go:   type User struct { Name string }
来源：http://ye.jctech888.com.cn

Ruby: class User; end
来源：http://nc.szxytkj.cn

C#:   class User {}
来源：http://mp.huixinmuqiang.cn

[G02] 构造函数
来源：http://qi.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://kg.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://tr.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://bi.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://mb.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://vl.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ly.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://tg.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://uf.hahajie.cn

[G03] 实例属性
来源：http://ad.panjiajie.cn

Py:   self.name = "x"
来源：http://wy.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://kq.shxzukj.cn

JS:   this.name = "x";
来源：http://an.chemitech.net.cn

TS:   name: string = "x";
来源：http://xx.huixinmuqiang.cn

Java: private String name;
来源：http://jf.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ox.gzmigu.cn

Ruby: @name = "x"
来源：http://ex.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://fs.bjjhwx.cn

[G04] 定义方法
来源：http://fv.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://dy.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hs.521024.cn

JS:   greet() { return this.name; }
来源：http://nd.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ek.9csxet.cn

Java: String greet() { return name; }
来源：http://wf.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nj.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://vt.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://je.bjjhwx.cn

[G05] 继承
来源：http://bg.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://af.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://kk.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ak.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://wm.9csxet.cn

Java: class Admin extends User {}
来源：http://hw.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ud.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://np.huixiangedu.cn

C#:   class Admin : User {}
来源：http://xz.yuexingan06.cn

[G06] 重写方法
来源：http://pl.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://wu.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ga.521024.cn

JS:   greet() { return "admin"; }
来源：http://or.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://af.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://rt.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iu.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ek.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://cd.szxytkj.cn

[G07] 调用父类方法
来源：http://fl.huanxung.cn

Py:   super().greet()
来源：http://wv.muxihuayi.cn

PHP:  parent::greet();
来源：http://qy.bjjhwx.cn

JS:   super.greet();
来源：http://nr.newstarts.cn

TS:   super.greet();
来源：http://mq.haigaiapp.cn

Java: super.greet();
来源：http://mx.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://do.huixiangedu.cn

Ruby: super
来源：http://cd.hahajie.cn

C#:   base.Greet();
来源：http://mo.haigaiapp.cn

[G08] 静态方法与属性
来源：http://fa.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xg.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://id.huixinmuqiang.cn

JS:   static f() {}
来源：http://hd.gzmigu.cn

TS:   static f(): void {}
来源：http://kd.shxzskj.cn

Java: static void f() {}
来源：http://lt.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nr.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://br.yuexingan06.cn

C#:   public static void F() {}
来源：http://zn.hahajie.cn

[G09] 接口 / 抽象类
来源：http://qs.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://uc.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zg.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://il.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://gm.newstarts.cn

Java: interface Shape { double area(); }
来源：http://dc.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ir.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iv.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://dz.panjiajie.cn

[G10] 访问控制
来源：http://kw.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://gf.szsharing.cn

PHP:  public / protected / private
来源：http://fn.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://od.szxytkj.cn

TS:   public / protected / private
来源：http://zt.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://yv.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pe.jctech888.com.cn

Ruby: public / protected / private
来源：http://lm.nicolike.cn

C#:   public / protected / private / internal
来源：http://qe.wgjwhj.cn

[G11] getter / setter
来源：http://nf.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://ih.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gn.asd995.cn

JS:   get name() { return this._name; }
来源：http://hw.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://up.szsharing.cn

Java: public String getName() { return name; }
来源：http://ze.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mm.jctech888.com.cn


<!-- 参考信息 -->