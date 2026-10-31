代发 wailian999

Go:   strings.Join(items, ",")
来源：http://nl.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://yk.szsharing.cn

C#:   string.Join(",", items)
来源：http://ro.shxzskj.cn

[E09] 去除所有空白字符
来源：http://ky.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nd.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xp.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://lx.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://nj.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://cr.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dw.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sg.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vx.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://jq.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tf.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xz.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://mc.521024.cn

TS:   "7".padStart(3, "0")
来源：http://on.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ph.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nc.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lx.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ci.shtwfgs.cn

[E11] 反转字符串
来源：http://lf.huixiangedu.cn

Py:   s[::-1]
来源：http://kl.nszjky.cn

PHP:  strrev($s);
来源：http://dg.asd995.cn

JS:   [...s].reverse().join("")
来源：http://kp.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://mt.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ri.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vr.huixinmuqiang.cn

Ruby: s.reverse
来源：http://um.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rf.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://sg.wgjwhj.cn

Py:   s.count("a")
来源：http://xx.colortex.cn

PHP:  substr_count($s, "a");
来源：http://nr.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://eb.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://xf.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jq.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://ur.9csxet.cn

Ruby: s.count("a")
来源：http://oe.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://ac.lnxyls.cn

[E13] 逐字符遍历
来源：http://jq.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://qj.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ih.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cf.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ol.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qw.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nr.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fo.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://io.newstarts.cn

[E14] URL 编码与 Base64
来源：http://cx.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nc.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gv.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ro.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rq.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yn.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kv.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pa.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://na.521024.cn

[E15] HTML 转义 / 反转义
来源：http://sr.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ac.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wl.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oc.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yd.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ui.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rq.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://np.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ey.lnxyls.cn

[E16] 数字千分位
来源：http://ft.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://ux.9csxet.cn

PHP:  number_format(1234567);
来源：http://hd.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rp.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cv.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eh.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ix.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oh.asd995.cn

C#:   1234567.ToString("N0")
来源：http://af.newstarts.cn

[E17] 首字母大写
来源：http://if.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ro.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pr.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mm.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mi.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xo.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ul.yuexingan06.cn

Ruby: s.capitalize
来源：http://sw.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ps.hahajie.cn

[E18] 模板占位符替换
来源：http://pr.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nm.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qo.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://in.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ir.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kc.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eq.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gx.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fl.huanxung.cn

[E19] 多行文本按行拆分
来源：http://mr.gzmigu.cn

Py:   s.splitlines()
来源：http://me.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ie.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://qi.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://pp.yuexingan06.cn

Java: s.lines().toList()
来源：http://le.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://ud.chemitech.net.cn

Ruby: s.lines
来源：http://ez.szxytkj.cn

C#:   s.Split('\n')
来源：http://nm.hahajie.cn

[E20] 判断字符串是否为空
来源：http://od.chemitech.net.cn

Py:   if not s:
来源：http://ce.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rh.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jr.huanxung.cn

TS:   if (s === "") {}
来源：http://gy.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ob.9csxet.cn

Go:   if s == "" {}
来源：http://oj.shxzskj.cn

Ruby: if s.empty?
来源：http://kk.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sf.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://uj.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ss.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gh.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hy.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yh.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ro.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://in.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yd.nszjky.cn

[E22] 字节长度与字符长度
来源：http://qy.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ly.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bw.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hl.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ml.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yt.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hv.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://ha.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ir.yuexingan06.cn

================================================================================
来源：http://bw.jianghongdianzi.cn

F. 文件与目录
来源：http://xz.shxzukj.cn

================================================================================
来源：http://jf.wgjwhj.cn

[F01] 读取整个文件
来源：http://sw.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sh.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://bx.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vx.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ah.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yv.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fl.9csxet.cn

Ruby: File.read("a.txt")
来源：http://xc.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://va.huixiangedu.cn

[F02] 逐行读取文件
来源：http://pq.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xc.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nx.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://em.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ip.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xi.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://co.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://eh.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ri.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kp.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://it.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zs.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lc.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tm.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://od.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vk.newstarts.cn

[F04] 追加写入文件
来源：http://oi.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rr.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zx.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://na.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xl.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://do.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zc.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xn.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bl.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://zi.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fp.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://jm.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://au.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://rk.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zj.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fe.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://yz.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://vf.asd995.cn

[F06] 删除文件
来源：http://nn.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://sf.asd995.cn

PHP:  unlink("a.txt");
来源：http://oj.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yz.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gy.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fg.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://kn.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://hz.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://dk.521024.cn

[F07] 创建目录（含多级）
来源：http://cw.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://am.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sy.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eb.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ua.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zd.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ky.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yk.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xm.asd995.cn

[F08] 遍历目录
来源：http://xt.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oy.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://er.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://wc.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://xv.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yl.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ff.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://yb.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://dv.wgjwhj.cn

[F09] 获取文件大小
来源：http://bo.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://hc.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://pp.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://df.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://lz.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qy.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yw.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://lz.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://as.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://sc.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kg.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iw.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hd.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://jt.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wt.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jc.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rd.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ew.hahajie.cn

[F11] 复制与移动文件
来源：http://au.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://js.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lx.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wy.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qq.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://od.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xd.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yk.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kb.bookmarksfly.cn

[F12] CSV 读写
来源：http://pe.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://md.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ja.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://de.colortex.cn

TS:   // 同上
来源：http://pf.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vp.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gm.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vk.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yv.shxzukj.cn

================================================================================
来源：http://rl.yuntaijiaju.cn

G. 面向对象
来源：http://lv.gzmigu.cn

================================================================================
来源：http://gw.gzmigu.cn

[G01] 定义类
来源：http://qu.nszjky.cn

Py:   class User: pass
来源：http://ox.jctech888.com.cn

PHP:  class User {}
来源：http://tp.shxzukj.cn

JS:   class User {}
来源：http://da.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://hm.szsharing.cn

Java: class User {}
来源：http://cl.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://fb.newstarts.cn

Ruby: class User; end
来源：http://ka.yuexingan06.cn

C#:   class User {}
来源：http://bh.newstarts.cn

[G02] 构造函数
来源：http://xf.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ql.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://qi.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ul.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://pk.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://lb.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tx.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://nc.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://vb.shxzukj.cn

[G03] 实例属性
来源：http://ij.hnjuh.cn

Py:   self.name = "x"
来源：http://lz.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://yt.gzmigu.cn

JS:   this.name = "x";
来源：http://tq.wgjwhj.cn

TS:   name: string = "x";
来源：http://oo.shtwfgs.cn

Java: private String name;
来源：http://fn.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lm.huixiangedu.cn

Ruby: @name = "x"
来源：http://ms.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://yc.haigaiapp.cn

[G04] 定义方法
来源：http://mp.colortex.cn

Py:   def greet(self): return self.name
来源：http://mb.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hs.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://bp.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://vn.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ay.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ds.9csxet.cn

Ruby: def greet; @name; end
来源：http://jv.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://bf.nszjky.cn

[G05] 继承
来源：http://yu.asd995.cn

Py:   class Admin(User): pass
来源：http://qv.nszjky.cn

PHP:  class Admin extends User {}
来源：http://ix.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://np.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://yv.hahajie.cn

Java: class Admin extends User {}
来源：http://gl.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dj.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://ku.521024.cn

C#:   class Admin : User {}
来源：http://bo.colortex.cn

[G06] 重写方法
来源：http://wu.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://zi.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ua.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://qs.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://os.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://kq.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gu.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://ml.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://iu.bjjhwx.cn

[G07] 调用父类方法
来源：http://uc.wgjwhj.cn

Py:   super().greet()
来源：http://pk.hahajie.cn

PHP:  parent::greet();
来源：http://sg.szxytkj.cn


<!-- 参考信息 -->