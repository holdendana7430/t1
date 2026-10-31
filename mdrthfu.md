代发 wailian999

JS:   [...s].reverse().join("")
来源：http://em.521024.cn

TS:   [...s].reverse().join("")
来源：http://lv.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vk.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vk.lnxyls.cn

Ruby: s.reverse
来源：http://ln.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vs.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://lq.hahajie.cn

Py:   s.count("a")
来源：http://qf.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://hc.nszjky.cn

JS:   s.split("a").length - 1
来源：http://pv.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://kb.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pe.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://og.nicolike.cn

Ruby: s.count("a")
来源：http://xd.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://mi.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ws.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://hs.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dx.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ou.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pv.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ec.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://co.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://el.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ql.colortex.cn

[E14] URL 编码与 Base64
来源：http://iv.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wq.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hq.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wk.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mb.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nv.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gw.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nl.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nw.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://of.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gz.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rh.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vn.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hv.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://js.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jo.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mm.lnxyls.cn

[E16] 数字千分位
来源：http://vc.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://dl.nszjky.cn

PHP:  number_format(1234567);
来源：http://tz.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fc.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kj.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jv.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qs.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ah.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://gz.9csxet.cn

[E17] 首字母大写
来源：http://fe.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kl.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fv.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ga.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vt.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wv.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zs.nszjky.cn

Ruby: s.capitalize
来源：http://jd.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aq.bjjhwx.cn

[E18] 模板占位符替换
来源：http://oz.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rp.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://az.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jg.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ml.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mz.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kb.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xp.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://au.szsharing.cn

[E19] 多行文本按行拆分
来源：http://bm.lnxyls.cn

Py:   s.splitlines()
来源：http://ft.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gh.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://wi.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://wt.wgjwhj.cn

Java: s.lines().toList()
来源：http://vz.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://sx.wgjwhj.cn

Ruby: s.lines
来源：http://za.nszjky.cn

C#:   s.Split('\n')
来源：http://ux.newstarts.cn

[E20] 判断字符串是否为空
来源：http://zy.hahajie.cn

Py:   if not s:
来源：http://rq.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xk.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sl.hahajie.cn

TS:   if (s === "") {}
来源：http://rf.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://zx.lnxyls.cn

Go:   if s == "" {}
来源：http://ap.gzmigu.cn

Ruby: if s.empty?
来源：http://dc.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ed.521024.cn

[E21] 超长截断加省略号
来源：http://zk.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wb.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lh.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hl.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cr.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qa.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://rv.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mk.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tj.colortex.cn

[E22] 字节长度与字符长度
来源：http://gv.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yz.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bq.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ea.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bn.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://vs.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cz.szxytkj.cn

================================================================================
来源：http://jf.haigaiapp.cn

F. 文件与目录
来源：http://fq.huixinmuqiang.cn

================================================================================
来源：http://uw.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ly.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tc.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://eh.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ze.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sx.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cl.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sh.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://be.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://qg.gzmigu.cn

[F02] 逐行读取文件
来源：http://mz.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zg.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hr.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kd.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cu.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wo.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ti.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bp.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gn.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://id.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kv.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vx.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fw.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://er.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kd.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ae.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lp.hahajie.cn

[F04] 追加写入文件
来源：http://yx.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rf.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gx.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://na.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lv.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uj.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lj.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yx.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://td.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xq.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://vc.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://gx.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ni.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ch.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fi.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://of.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://dm.panjiajie.cn

[F06] 删除文件
来源：http://zf.nszjky.cn

Py:   os.remove("a.txt")
来源：http://lt.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://dc.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yq.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uv.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cb.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://uk.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://kv.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://pg.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://zk.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ci.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://of.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ut.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wd.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qa.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ow.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vh.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fa.nszjky.cn

[F08] 遍历目录
来源：http://xj.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ps.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ek.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://ib.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://yd.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://od.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://qr.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ki.huanxung.cn

[F09] 获取文件大小
来源：http://uu.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://cq.hahajie.cn

PHP:  filesize("a.txt");
来源：http://nq.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://bi.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://yl.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ts.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kn.huanxung.cn

Ruby: File.size("a.txt")
来源：http://yl.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://hy.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ck.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bw.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rx.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hp.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ad.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pi.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yt.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yr.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jm.wgjwhj.cn

[F11] 复制与移动文件
来源：http://nn.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ey.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ih.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ra.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vk.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qn.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fd.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wi.shxzskj.cn

[F12] CSV 读写
来源：http://aj.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xe.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://du.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hb.szsharing.cn

TS:   // 同上
来源：http://rm.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bp.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nr.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cl.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xy.hnjuh.cn

================================================================================
来源：http://jn.9csxet.cn

G. 面向对象
来源：http://ro.hnjuh.cn

================================================================================
来源：http://uc.nicolike.cn

[G01] 定义类
来源：http://wq.chemitech.net.cn

Py:   class User: pass
来源：http://so.lnxyls.cn

PHP:  class User {}
来源：http://sq.hahajie.cn

JS:   class User {}
来源：http://ua.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://fs.wgjwhj.cn

Java: class User {}
来源：http://uy.huanxung.cn

Go:   type User struct { Name string }
来源：http://ro.9csxet.cn

Ruby: class User; end
来源：http://lz.huanxung.cn

C#:   class User {}
来源：http://sr.yuntaijiaju.cn

[G02] 构造函数
来源：http://mc.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://ig.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://bo.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://uf.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://bp.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://bx.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://os.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://vx.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://ph.panjiajie.cn

[G03] 实例属性
来源：http://wk.muxihuayi.cn

Py:   self.name = "x"
来源：http://wf.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://ur.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://hl.haigaiapp.cn

TS:   name: string = "x";
来源：http://ov.haigaiapp.cn

Java: private String name;
来源：http://iy.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iy.bookmarksfly.cn

Ruby: @name = "x"
来源：http://zq.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://mj.asd995.cn

[G04] 定义方法
来源：http://ah.hahajie.cn

Py:   def greet(self): return self.name
来源：http://ro.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ma.nszjky.cn

JS:   greet() { return this.name; }
来源：http://cq.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://hk.wgjwhj.cn

Java: String greet() { return name; }
来源：http://af.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uj.newstarts.cn

Ruby: def greet; @name; end
来源：http://pq.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://vk.yuexingan06.cn

[G05] 继承
来源：http://wd.nszjky.cn

Py:   class Admin(User): pass
来源：http://ax.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://wi.huanxung.cn

JS:   class Admin extends User {}
来源：http://bk.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://fe.shtwfgs.cn

Java: class Admin extends User {}
来源：http://hu.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jf.gzmigu.cn

Ruby: class Admin < User; end
来源：http://ao.huixiangedu.cn

C#:   class Admin : User {}
来源：http://ok.hnjuh.cn

[G06] 重写方法
来源：http://va.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://km.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cp.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://ib.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://gc.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://bq.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xh.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://nd.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://qx.chemitech.net.cn

[G07] 调用父类方法
来源：http://bi.muxihuayi.cn

Py:   super().greet()
来源：http://vo.shxzukj.cn

PHP:  parent::greet();
来源：http://hx.chemitech.net.cn

JS:   super.greet();
来源：http://ve.bjjhwx.cn

TS:   super.greet();
来源：http://ru.hahajie.cn

Java: super.greet();
来源：http://sk.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cd.newstarts.cn

Ruby: super
来源：http://og.bjjhwx.cn

C#:   base.Greet();
来源：http://wx.hahajie.cn

[G08] 静态方法与属性
来源：http://ss.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iq.9csxet.cn

PHP:  public static function f() {}
来源：http://wv.hnjuh.cn

JS:   static f() {}
来源：http://md.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://le.huixinmuqiang.cn

Java: static void f() {}
来源：http://ky.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ky.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://by.lnxyls.cn

C#:   public static void F() {}
来源：http://jf.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://tc.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://oo.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uf.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zg.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://zz.9csxet.cn

Java: interface Shape { double area(); }
来源：http://bd.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://rv.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ot.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://iu.shxzukj.cn


<!-- 参考信息 -->