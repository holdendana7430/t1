代发 wailian999

Ruby: s.reverse
来源：http://nt.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vi.hahajie.cn

[E12] 统计某字符出现次数
来源：http://bu.colortex.cn

Py:   s.count("a")
来源：http://mv.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://xc.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://um.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://sm.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fb.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://dh.jctech888.com.cn

Ruby: s.count("a")
来源：http://gy.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://py.colortex.cn

[E13] 逐字符遍历
来源：http://in.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://mi.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ec.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jp.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ax.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nv.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kg.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hw.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mk.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://dk.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ec.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bo.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vh.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eb.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yo.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://em.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kn.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ac.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://ia.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://px.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bc.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sc.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ub.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://en.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cj.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lz.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://se.nicolike.cn

[E16] 数字千分位
来源：http://nv.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://pk.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://de.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zo.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lm.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://og.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://av.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://op.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://nx.521024.cn

[E17] 首字母大写
来源：http://ga.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nn.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jj.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sc.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cy.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jf.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hi.wgjwhj.cn

Ruby: s.capitalize
来源：http://fu.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dc.gzmigu.cn

[E18] 模板占位符替换
来源：http://nb.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dq.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kn.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kk.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fe.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mk.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nb.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jn.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nt.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ts.nszjky.cn

Py:   s.splitlines()
来源：http://do.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bz.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://wx.521024.cn

TS:   s.split(/\r?\n/)
来源：http://jl.huanxung.cn

Java: s.lines().toList()
来源：http://tg.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://sg.shtwfgs.cn

Ruby: s.lines
来源：http://as.shxzskj.cn

C#:   s.Split('\n')
来源：http://mz.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://ad.asd995.cn

Py:   if not s:
来源：http://zn.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fq.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dq.asd995.cn

TS:   if (s === "") {}
来源：http://dw.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://sm.shtwfgs.cn

Go:   if s == "" {}
来源：http://uk.wgjwhj.cn

Ruby: if s.empty?
来源：http://av.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://er.newstarts.cn

[E21] 超长截断加省略号
来源：http://fo.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sc.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lt.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gn.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://en.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://mk.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uh.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uj.asd995.cn

[E22] 字节长度与字符长度
来源：http://jj.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jo.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yr.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://je.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cu.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ke.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ya.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ta.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dv.lnxyls.cn

================================================================================
来源：http://zy.shxzukj.cn

F. 文件与目录
来源：http://et.jianghongdianzi.cn

================================================================================
来源：http://xw.shtwfgs.cn

[F01] 读取整个文件
来源：http://vo.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iz.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://dh.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://id.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xt.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vi.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yh.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://qh.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ai.shxzskj.cn

[F02] 逐行读取文件
来源：http://iq.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hl.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wi.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://np.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hh.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://am.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jx.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yt.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tc.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://wk.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zr.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hl.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pk.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tt.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hm.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iq.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://gy.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dc.huanxung.cn

[F04] 追加写入文件
来源：http://wf.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bv.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ar.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jo.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sw.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xs.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sl.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xj.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://sm.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gc.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://tk.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://yf.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://xh.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sd.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bq.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://hh.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://tn.huixiangedu.cn

[F06] 删除文件
来源：http://it.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://hn.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://xg.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ff.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lw.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sr.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://rr.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://sv.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://wm.nicolike.cn

[F07] 创建目录（含多级）
来源：http://tr.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ne.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kh.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ca.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bt.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vh.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gb.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ar.jianghongdianzi.cn

[F08] 遍历目录
来源：http://bz.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vo.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lk.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://yq.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://cq.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kg.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ry.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://gb.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://ev.9csxet.cn

[F09] 获取文件大小
来源：http://of.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ie.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://pw.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://nt.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://na.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gq.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fn.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://ht.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://qu.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://kk.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bs.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aq.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tm.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://jp.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kr.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vv.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ep.hnjuh.cn

[F11] 复制与移动文件
来源：http://tp.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nc.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zh.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vf.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ya.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ot.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rw.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ip.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rx.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ro.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yn.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://un.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cj.lnxyls.cn

TS:   // 同上
来源：http://yi.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sl.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qn.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vk.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mk.shxzskj.cn

================================================================================
来源：http://wn.521024.cn

G. 面向对象
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://ka.nicolike.cn

[G01] 定义类
来源：http://ox.9csxet.cn

Py:   class User: pass
来源：http://qh.panjiajie.cn

PHP:  class User {}
来源：http://rg.shtwfgs.cn

JS:   class User {}
来源：http://kf.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://tu.huanxung.cn

Java: class User {}
来源：http://vi.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ha.szsharing.cn

Ruby: class User; end
来源：http://rl.chemitech.net.cn

C#:   class User {}
来源：http://tm.bookmarksfly.cn

[G02] 构造函数
来源：http://jl.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://yr.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://uw.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://we.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://cv.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://al.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tf.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://dc.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://fx.jctech888.com.cn

[G03] 实例属性
来源：http://xt.521024.cn

Py:   self.name = "x"
来源：http://vs.panjiajie.cn

PHP:  public string $name = "x";
来源：http://sb.bookmarksfly.cn

JS:   this.name = "x";
来源：http://ei.nicolike.cn

TS:   name: string = "x";
来源：http://ld.521024.cn

Java: private String name;
来源：http://ru.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gy.colortex.cn

Ruby: @name = "x"
来源：http://gi.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://nq.9csxet.cn

[G04] 定义方法
来源：http://wf.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://bj.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tm.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://nk.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://tt.hahajie.cn

Java: String greet() { return name; }
来源：http://cq.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gt.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://dv.hahajie.cn

C#:   public string Greet() => Name;
来源：http://wn.yuexingan06.cn

[G05] 继承
来源：http://ha.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://tz.huanxung.cn

PHP:  class Admin extends User {}
来源：http://ig.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://br.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://bw.huanxung.cn

Java: class Admin extends User {}
来源：http://pv.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://el.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://kt.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://fy.521024.cn

[G06] 重写方法
来源：http://li.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://ym.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wk.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://hd.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ph.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://gj.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ys.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://np.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://zl.yuexingan06.cn

[G07] 调用父类方法
来源：http://on.bookmarksfly.cn

Py:   super().greet()
来源：http://pq.521024.cn

PHP:  parent::greet();
来源：http://cn.bookmarksfly.cn

JS:   super.greet();
来源：http://le.bookmarksfly.cn

TS:   super.greet();
来源：http://qi.shxzskj.cn

Java: super.greet();
来源：http://ni.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rh.panjiajie.cn

Ruby: super
来源：http://iq.huanxung.cn

C#:   base.Greet();
来源：http://wv.panjiajie.cn

[G08] 静态方法与属性
来源：http://go.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mr.huanxung.cn

PHP:  public static function f() {}
来源：http://ji.hnjuh.cn

JS:   static f() {}
来源：http://nk.colortex.cn

TS:   static f(): void {}
来源：http://li.nicolike.cn

Java: static void f() {}
来源：http://ls.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nc.gzmigu.cn

Ruby: def self.f; end
来源：http://yf.panjiajie.cn

C#:   public static void F() {}
来源：http://xx.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://ds.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://yh.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bo.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pk.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://nz.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://vf.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://nb.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mh.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://bi.shxzskj.cn

[G10] 访问控制
来源：http://ln.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://oc.huanxung.cn

PHP:  public / protected / private
来源：http://qv.521024.cn

JS:   #private 字段；其余公开
来源：http://yz.yuexingan06.cn


<!-- 参考信息 -->