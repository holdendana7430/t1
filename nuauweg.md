代发 wailian999

JS:   [...s].reverse().join("")
来源：http://tz.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://jr.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qj.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ea.521024.cn

Ruby: s.reverse
来源：http://hm.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qd.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://mg.nszjky.cn

Py:   s.count("a")
来源：http://rx.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://tu.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://jx.asd995.cn

TS:   s.split("a").length - 1
来源：http://pm.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ic.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://lw.chemitech.net.cn

Ruby: s.count("a")
来源：http://ri.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://lt.shxzukj.cn

[E13] 逐字符遍历
来源：http://xm.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://gh.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jg.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ze.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gx.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ih.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ff.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zl.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kn.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://yl.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pu.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ee.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yx.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oh.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zz.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kl.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://da.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://va.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://pn.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zf.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hg.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uy.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pb.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wi.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cy.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ht.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://we.huixinmuqiang.cn

[E16] 数字千分位
来源：http://fu.huanxung.cn

Py:   f"{1234567:,}"
来源：http://sk.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://lx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ho.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ld.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kg.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://if.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fa.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://pb.huanxung.cn

[E17] 首字母大写
来源：http://fv.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ev.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gq.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gg.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kd.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ya.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ko.wgjwhj.cn

Ruby: s.capitalize
来源：http://aa.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gb.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://xu.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nb.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cb.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bi.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wl.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cg.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vd.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mh.szsharing.cn

[E19] 多行文本按行拆分
来源：http://lu.nicolike.cn

Py:   s.splitlines()
来源：http://hv.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tf.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://uy.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://uk.gzmigu.cn

Java: s.lines().toList()
来源：http://fj.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://qe.chemitech.net.cn

Ruby: s.lines
来源：http://gn.shxzskj.cn

C#:   s.Split('\n')
来源：http://rc.521024.cn

[E20] 判断字符串是否为空
来源：http://py.hnjuh.cn

Py:   if not s:
来源：http://xf.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fj.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mz.asd995.cn

TS:   if (s === "") {}
来源：http://ww.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://nr.colortex.cn

Go:   if s == "" {}
来源：http://cb.bookmarksfly.cn

Ruby: if s.empty?
来源：http://bs.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lv.shxzskj.cn

[E21] 超长截断加省略号
来源：http://hi.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ih.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sy.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vo.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sd.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bo.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://wf.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vi.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zy.szsharing.cn

[E22] 字节长度与字符长度
来源：http://gb.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aa.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fy.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://or.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ky.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://de.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iu.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://dh.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ot.huanxung.cn

================================================================================
来源：http://vp.521024.cn

F. 文件与目录
来源：http://qa.huixinmuqiang.cn

================================================================================
来源：http://ly.bjjhwx.cn

[F01] 读取整个文件
来源：http://sk.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xp.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://kv.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qn.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qo.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dn.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vb.szsharing.cn

Ruby: File.read("a.txt")
来源：http://jx.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://il.szsharing.cn

[F02] 逐行读取文件
来源：http://fb.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hk.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://em.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fs.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jm.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ah.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://so.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fo.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://av.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://jg.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://il.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xl.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ev.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yp.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bf.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mw.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://xh.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sq.chemitech.net.cn

[F04] 追加写入文件
来源：http://ba.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tw.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nn.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vr.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ej.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xi.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xo.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://st.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xg.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://pl.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tr.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://kx.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://re.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://hh.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kc.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ow.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ah.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://dk.lnxyls.cn

[F06] 删除文件
来源：http://mc.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://sy.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ar.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qj.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://et.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cv.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://de.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://fb.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://xe.asd995.cn

[F07] 创建目录（含多级）
来源：http://mf.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gl.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kh.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nw.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ws.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eh.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bk.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gc.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kb.huixinmuqiang.cn

[F08] 遍历目录
来源：http://si.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sn.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ut.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://hg.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ex.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://so.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mo.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://qd.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://uc.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://pc.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://xe.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://zt.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://hq.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://to.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pf.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://he.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://nc.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://gk.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://bp.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hr.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gl.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dg.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://yz.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rm.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lm.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ad.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tk.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://rp.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xl.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://es.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cx.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ny.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://to.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ws.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vd.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ua.haigaiapp.cn

[F12] CSV 读写
来源：http://wv.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rx.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uf.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wg.shxzskj.cn

TS:   // 同上
来源：http://zj.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uw.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qb.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ex.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ue.gzmigu.cn

================================================================================
来源：http://lj.wgjwhj.cn

G. 面向对象
来源：http://bf.colortex.cn

================================================================================
来源：http://vh.521024.cn

[G01] 定义类
来源：http://bj.panjiajie.cn

Py:   class User: pass
来源：http://xe.wgjwhj.cn

PHP:  class User {}
来源：http://fx.521024.cn

JS:   class User {}
来源：http://dp.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://xf.haigaiapp.cn

Java: class User {}
来源：http://od.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://jo.szsharing.cn

Ruby: class User; end
来源：http://od.521024.cn

C#:   class User {}
来源：http://ib.wgjwhj.cn

[G02] 构造函数
来源：http://ul.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://xz.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://nr.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://jf.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://sb.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://dn.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wc.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://xs.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ug.haigaiapp.cn

[G03] 实例属性
来源：http://ao.hnjuh.cn

Py:   self.name = "x"
来源：http://wv.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://cq.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://yr.muxihuayi.cn

TS:   name: string = "x";
来源：http://hw.newstarts.cn

Java: private String name;
来源：http://sd.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fr.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://xr.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://oh.nszjky.cn

[G04] 定义方法
来源：http://rl.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://eh.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tj.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://oy.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://kb.muxihuayi.cn

Java: String greet() { return name; }
来源：http://il.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pb.shxzukj.cn

Ruby: def greet; @name; end
来源：http://zs.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://tk.521024.cn

[G05] 继承
来源：http://ae.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://li.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://mm.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://cc.newstarts.cn

TS:   class Admin extends User {}
来源：http://in.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://np.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ex.hahajie.cn

Ruby: class Admin < User; end
来源：http://bt.bjjhwx.cn

C#:   class Admin : User {}
来源：http://tb.nicolike.cn

[G06] 重写方法
来源：http://dk.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://ja.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xk.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://sv.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://nt.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://qw.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pg.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://fc.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://mh.gzmigu.cn

[G07] 调用父类方法
来源：http://jk.shxzukj.cn

Py:   super().greet()
来源：http://gv.muxihuayi.cn

PHP:  parent::greet();
来源：http://pj.9csxet.cn

JS:   super.greet();
来源：http://cb.shxzskj.cn

TS:   super.greet();
来源：http://pq.asd995.cn

Java: super.greet();
来源：http://xk.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://go.haigaiapp.cn

Ruby: super
来源：http://pg.bjjhwx.cn

C#:   base.Greet();
来源：http://ej.asd995.cn

[G08] 静态方法与属性
来源：http://rs.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xc.lnxyls.cn

PHP:  public static function f() {}
来源：http://fk.huixiangedu.cn

JS:   static f() {}
来源：http://el.nszjky.cn

TS:   static f(): void {}
来源：http://nt.9csxet.cn

Java: static void f() {}
来源：http://iw.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yx.hnjuh.cn

Ruby: def self.f; end
来源：http://dj.nszjky.cn

C#:   public static void F() {}
来源：http://fq.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://em.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ok.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fy.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zc.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://qk.asd995.cn

Java: interface Shape { double area(); }
来源：http://bw.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://jv.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gc.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://qz.521024.cn


<!-- 参考信息 -->