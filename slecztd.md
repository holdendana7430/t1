代发 wailian999

PHP:  substr_count($s, "a");
来源：http://np.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://lj.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://bu.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gf.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://mj.colortex.cn

Ruby: s.count("a")
来源：http://ro.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://hp.yuexingan06.cn

[E13] 逐字符遍历
来源：http://bj.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://kd.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xn.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fq.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ou.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ys.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kp.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://in.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://qq.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vy.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yg.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dv.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ow.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ht.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cm.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lw.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tg.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://yq.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pb.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oq.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://as.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://li.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qy.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kz.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pd.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lv.asd995.cn

[E16] 数字千分位
来源：http://zs.hahajie.cn

Py:   f"{1234567:,}"
来源：http://jl.shxzskj.cn

PHP:  number_format(1234567);
来源：http://jq.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ug.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dz.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ss.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gg.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://db.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://lv.newstarts.cn

[E17] 首字母大写
来源：http://hu.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lk.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ev.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ne.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://at.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bm.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yc.shxzukj.cn

Ruby: s.capitalize
来源：http://df.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ew.muxihuayi.cn

[E18] 模板占位符替换
来源：http://if.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bj.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ms.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hw.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eh.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lj.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ds.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kw.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sb.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://vo.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ax.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ic.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://qn.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://yd.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://wr.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ng.9csxet.cn

Ruby: s.lines
来源：http://ii.newstarts.cn

C#:   s.Split('\n')
来源：http://hd.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ma.nszjky.cn

Py:   if not s:
来源：http://ux.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tk.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://an.szxytkj.cn

TS:   if (s === "") {}
来源：http://il.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://gh.nszjky.cn

Go:   if s == "" {}
来源：http://jh.asd995.cn

Ruby: if s.empty?
来源：http://lu.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mx.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://po.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://is.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ir.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fo.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ep.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mu.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ju.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ca.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://so.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://jj.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cu.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pf.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ym.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wc.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://no.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qk.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://gm.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ie.shtwfgs.cn

================================================================================
来源：http://ja.9csxet.cn

F. 文件与目录
来源：http://um.colortex.cn

================================================================================
来源：http://ot.hnjuh.cn

[F01] 读取整个文件
来源：http://bw.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ui.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://cs.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nd.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ip.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xa.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bf.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://eo.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://jh.shtwfgs.cn

[F02] 逐行读取文件
来源：http://fl.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mj.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gt.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aq.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zp.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ax.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mu.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://di.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://mw.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tz.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zy.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zu.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://st.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nm.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kt.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://am.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ef.muxihuayi.cn

[F04] 追加写入文件
来源：http://rb.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sa.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://me.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eh.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ie.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fd.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nj.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mw.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hi.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://wb.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ay.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://vy.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://fk.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://ig.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jy.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://es.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://cj.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://ye.huanxung.cn

[F06] 删除文件
来源：http://il.9csxet.cn

Py:   os.remove("a.txt")
来源：http://ot.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://ih.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xi.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ev.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zh.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://ai.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://yz.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://gg.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://vt.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zk.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://js.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yq.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bd.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oy.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wv.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kp.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cg.panjiajie.cn

[F08] 遍历目录
来源：http://qw.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ko.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gp.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://st.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://jo.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qc.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xk.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://tf.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://tp.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://va.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://hd.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://cz.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://em.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://cf.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mg.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hr.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://dd.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://wh.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://ow.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jo.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vo.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qj.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://wy.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wc.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ys.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uo.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ft.panjiajie.cn

[F11] 复制与移动文件
来源：http://wi.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ba.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vz.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rp.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yq.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uq.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rz.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dz.shxzukj.cn

[F12] CSV 读写
来源：http://nk.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dy.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gt.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kq.huixinmuqiang.cn

TS:   // 同上
来源：http://lw.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hl.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ta.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vx.muxihuayi.cn

================================================================================
来源：http://iv.lnxyls.cn

G. 面向对象
来源：http://in.yuntaijiaju.cn

================================================================================
来源：http://tw.9csxet.cn

[G01] 定义类
来源：http://nb.nszjky.cn

Py:   class User: pass
来源：http://qs.huixiangedu.cn

PHP:  class User {}
来源：http://fb.jianghongdianzi.cn

JS:   class User {}
来源：http://so.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://no.jctech888.com.cn

Java: class User {}
来源：http://sn.521024.cn

Go:   type User struct { Name string }
来源：http://lj.jianghongdianzi.cn

Ruby: class User; end
来源：http://ky.chemitech.net.cn

C#:   class User {}
来源：http://jw.lnxyls.cn

[G02] 构造函数
来源：http://vf.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ae.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ik.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://le.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://sh.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://qy.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pg.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ww.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://am.hnjuh.cn

[G03] 实例属性
来源：http://vc.shxzukj.cn

Py:   self.name = "x"
来源：http://um.shxzukj.cn

PHP:  public string $name = "x";
来源：http://zi.wgjwhj.cn

JS:   this.name = "x";
来源：http://kq.bjjhwx.cn

TS:   name: string = "x";
来源：http://uz.9csxet.cn

Java: private String name;
来源：http://fy.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://im.yuexingan06.cn

Ruby: @name = "x"
来源：http://gl.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://kj.colortex.cn

[G04] 定义方法
来源：http://ph.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://hk.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tl.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://id.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://ni.gzmigu.cn

Java: String greet() { return name; }
来源：http://qg.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ld.shxzskj.cn

Ruby: def greet; @name; end
来源：http://yf.colortex.cn

C#:   public string Greet() => Name;
来源：http://uy.huixiangedu.cn

[G05] 继承
来源：http://js.shxzukj.cn

Py:   class Admin(User): pass
来源：http://mz.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://rn.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ss.newstarts.cn

TS:   class Admin extends User {}
来源：http://dh.hahajie.cn

Java: class Admin extends User {}
来源：http://ch.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ey.szsharing.cn

Ruby: class Admin < User; end
来源：http://xm.yuexingan06.cn

C#:   class Admin : User {}
来源：http://kd.asd995.cn

[G06] 重写方法
来源：http://fa.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ly.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fi.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://xe.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://ff.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://gv.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bh.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://ia.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://qx.nszjky.cn

[G07] 调用父类方法
来源：http://hf.wgjwhj.cn

Py:   super().greet()
来源：http://ry.szsharing.cn

PHP:  parent::greet();
来源：http://ov.9csxet.cn

JS:   super.greet();
来源：http://pk.huanxung.cn

TS:   super.greet();
来源：http://gy.yuntaijiaju.cn

Java: super.greet();
来源：http://ao.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://od.szsharing.cn

Ruby: super
来源：http://on.shxzskj.cn

C#:   base.Greet();
来源：http://am.muxihuayi.cn

[G08] 静态方法与属性
来源：http://zy.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xq.haigaiapp.cn

PHP:  public static function f() {}
来源：http://ww.lnxyls.cn

JS:   static f() {}
来源：http://tg.shtwfgs.cn

TS:   static f(): void {}
来源：http://tp.wgjwhj.cn

Java: static void f() {}
来源：http://qj.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://og.szsharing.cn

Ruby: def self.f; end
来源：http://lm.yuexingan06.cn

C#:   public static void F() {}
来源：http://zv.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://ds.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://za.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://er.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://em.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://kz.nicolike.cn

Java: interface Shape { double area(); }
来源：http://bu.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://in.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rl.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://xa.yuexingan06.cn

[G10] 访问控制
来源：http://ia.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://rs.panjiajie.cn

PHP:  public / protected / private
来源：http://uu.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://oo.jianghongdianzi.cn

TS:   public / protected / private
来源：http://wj.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://dy.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nd.shtwfgs.cn

Ruby: public / protected / private
来源：http://ld.yuexingan06.cn


<!-- 参考信息 -->