代发 wailian999

Go:   strings.Join(items, ",")
来源：http://nr.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://oi.szsharing.cn

C#:   string.Join(",", items)
来源：http://ge.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://rq.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wo.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yd.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://ob.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://xf.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://fo.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oo.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kx.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://im.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://fl.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tr.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qg.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://cq.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://ep.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://na.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dp.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ba.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fo.jctech888.com.cn

[E11] 反转字符串
来源：http://or.nicolike.cn

Py:   s[::-1]
来源：http://ik.colortex.cn

PHP:  strrev($s);
来源：http://dm.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://tp.asd995.cn

TS:   [...s].reverse().join("")
来源：http://yy.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mq.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jr.newstarts.cn

Ruby: s.reverse
来源：http://mh.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hm.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://hh.shtwfgs.cn

Py:   s.count("a")
来源：http://hg.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://zq.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ml.colortex.cn

TS:   s.split("a").length - 1
来源：http://gq.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rg.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://bu.yuexingan06.cn

Ruby: s.count("a")
来源：http://xe.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://gj.9csxet.cn

[E13] 逐字符遍历
来源：http://hl.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://tb.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tq.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mq.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ro.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nz.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ur.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://se.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jl.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://kh.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nh.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mn.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xt.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://be.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jr.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ns.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ur.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mq.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ao.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tc.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ku.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mf.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oy.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ud.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tn.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ck.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rh.shtwfgs.cn

[E16] 数字千分位
来源：http://yr.colortex.cn

Py:   f"{1234567:,}"
来源：http://co.hahajie.cn

PHP:  number_format(1234567);
来源：http://jx.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wq.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rd.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://db.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mw.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hx.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://iv.hnjuh.cn

[E17] 首字母大写
来源：http://fp.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qh.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gh.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ao.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lq.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qv.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sk.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://bk.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rq.szxytkj.cn

[E18] 模板占位符替换
来源：http://be.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ps.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gd.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xi.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://la.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wd.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://st.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bn.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zt.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://pg.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://in.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yf.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://ek.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://lg.lnxyls.cn

Java: s.lines().toList()
来源：http://ic.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://fj.yuntaijiaju.cn

Ruby: s.lines
来源：http://sj.shxzukj.cn

C#:   s.Split('\n')
来源：http://gd.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://bn.hahajie.cn

Py:   if not s:
来源：http://mw.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ul.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://le.szxytkj.cn

TS:   if (s === "") {}
来源：http://mk.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://cf.chemitech.net.cn

Go:   if s == "" {}
来源：http://hv.hahajie.cn

Ruby: if s.empty?
来源：http://sy.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xk.nszjky.cn

[E21] 超长截断加省略号
来源：http://gq.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://og.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sj.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ni.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vg.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://gt.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ab.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qg.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://xo.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fb.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cn.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://og.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hg.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xg.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oi.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://ms.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://vb.szsharing.cn

F. 文件与目录
来源：http://gi.wgjwhj.cn

================================================================================
来源：http://zh.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://xv.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://of.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://xe.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kx.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ej.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gu.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tn.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://uj.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://jh.chemitech.net.cn

[F02] 逐行读取文件
来源：http://mb.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zi.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yn.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://do.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vb.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dg.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kh.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vv.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kw.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://rx.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jw.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ea.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://at.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mg.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ug.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ge.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://bd.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oa.szxytkj.cn

[F04] 追加写入文件
来源：http://uv.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://he.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pf.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mn.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xl.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vs.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kh.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lv.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xq.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://vx.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kj.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://ww.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ob.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://xy.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ez.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vk.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://ai.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://nz.shxzskj.cn

[F06] 删除文件
来源：http://um.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://gv.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://zm.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ng.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://st.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fj.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ag.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://nm.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://dv.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://hd.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oo.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gb.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tq.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vz.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ad.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zm.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vj.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dl.521024.cn

[F08] 遍历目录
来源：http://ly.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://es.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rp.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://wj.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://yu.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lb.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jl.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://nm.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://hb.huanxung.cn

[F09] 获取文件大小
来源：http://nq.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://vv.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://jn.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://zg.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://bc.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cc.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xz.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://bt.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://de.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://bh.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ej.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mz.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xt.521024.cn

TS:   path.extname("a.txt")
来源：http://tq.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jx.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jz.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yp.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lq.shxzskj.cn

[F11] 复制与移动文件
来源：http://ss.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://al.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ps.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lq.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pt.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pq.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ow.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gm.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ke.szsharing.cn

[F12] CSV 读写
来源：http://rb.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zp.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rc.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xb.521024.cn

TS:   // 同上
来源：http://el.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ds.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ji.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ju.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wd.hahajie.cn

================================================================================
来源：http://yg.szsharing.cn

G. 面向对象
来源：http://bv.bjjhwx.cn

================================================================================
来源：http://oo.huixinmuqiang.cn

[G01] 定义类
来源：http://tq.huanxung.cn

Py:   class User: pass
来源：http://hp.colortex.cn

PHP:  class User {}
来源：http://ve.huixiangedu.cn

JS:   class User {}
来源：http://bs.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://pr.bjjhwx.cn

Java: class User {}
来源：http://mo.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://kl.shxzukj.cn

Ruby: class User; end
来源：http://ui.haigaiapp.cn

C#:   class User {}
来源：http://ev.shtwfgs.cn

[G02] 构造函数
来源：http://ne.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://qa.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://iz.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ps.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://zq.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://ds.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rc.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://to.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://dl.asd995.cn

[G03] 实例属性
来源：http://ep.chemitech.net.cn

Py:   self.name = "x"
来源：http://jv.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://ss.9csxet.cn

JS:   this.name = "x";
来源：http://zv.yuexingan06.cn

TS:   name: string = "x";
来源：http://lz.haigaiapp.cn

Java: private String name;
来源：http://nx.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xv.newstarts.cn

Ruby: @name = "x"
来源：http://hr.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://ui.jianghongdianzi.cn

[G04] 定义方法
来源：http://wx.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://yv.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oh.hahajie.cn

JS:   greet() { return this.name; }
来源：http://no.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://kv.9csxet.cn

Java: String greet() { return name; }
来源：http://nf.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qk.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://yi.szsharing.cn

C#:   public string Greet() => Name;
来源：http://nv.wgjwhj.cn

[G05] 继承
来源：http://xu.shxzukj.cn

Py:   class Admin(User): pass
来源：http://gw.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://og.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ue.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ir.chemitech.net.cn

Java: class Admin extends User {}
来源：http://cp.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nc.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://iy.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ka.jianghongdianzi.cn

[G06] 重写方法
来源：http://vu.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://rv.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ub.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://zf.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://wa.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://gv.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://np.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://tz.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://hk.gzmigu.cn

[G07] 调用父类方法
来源：http://lx.9csxet.cn

Py:   super().greet()
来源：http://yf.shxzukj.cn

PHP:  parent::greet();
来源：http://tv.szsharing.cn


<!-- 参考信息 -->