代发 wailian999

Ruby: s.split(",");  s.split
来源：http://in.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gl.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://bx.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ha.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://wh.panjiajie.cn

JS:   items.join(",")
来源：http://mm.yuntaijiaju.cn

TS:   items.join(",")
来源：http://ln.lnxyls.cn

Java: String.join(",", items)
来源：http://km.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://bz.asd995.cn

Ruby: items.join(",")
来源：http://gn.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://xj.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://zy.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://al.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pb.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://zq.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://si.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://cy.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dt.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rt.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iw.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://xz.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fx.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ke.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://ce.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://pk.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://ep.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tj.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ys.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zm.huanxung.cn

[E11] 反转字符串
来源：http://wj.yuexingan06.cn

Py:   s[::-1]
来源：http://cq.lnxyls.cn

PHP:  strrev($s);
来源：http://ig.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ej.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://oj.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xv.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://an.huixinmuqiang.cn

Ruby: s.reverse
来源：http://qz.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xj.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://vs.wgjwhj.cn

Py:   s.count("a")
来源：http://wm.521024.cn

PHP:  substr_count($s, "a");
来源：http://vv.nszjky.cn

JS:   s.split("a").length - 1
来源：http://jm.nicolike.cn

TS:   s.split("a").length - 1
来源：http://tc.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://if.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ot.szsharing.cn

Ruby: s.count("a")
来源：http://tj.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://qm.lnxyls.cn

[E13] 逐字符遍历
来源：http://dq.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://ov.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://di.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qo.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rr.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sc.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lg.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vn.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://om.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://na.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bo.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oi.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ln.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pt.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fa.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wh.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pw.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yp.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://ui.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zu.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vh.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vi.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tb.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pc.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://su.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cq.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ds.yuntaijiaju.cn

[E16] 数字千分位
来源：http://lu.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ae.hahajie.cn

PHP:  number_format(1234567);
来源：http://yn.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ay.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://re.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ie.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kp.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://os.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://pz.szsharing.cn

[E17] 首字母大写
来源：http://km.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cf.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ax.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://op.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qx.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vc.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mx.muxihuayi.cn

Ruby: s.capitalize
来源：http://wa.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sw.asd995.cn

[E18] 模板占位符替换
来源：http://qo.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lf.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fs.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nw.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xy.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mv.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aj.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nl.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hk.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://jf.colortex.cn

Py:   s.splitlines()
来源：http://ku.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xi.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://le.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://dd.panjiajie.cn

Java: s.lines().toList()
来源：http://zb.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://gy.nszjky.cn

Ruby: s.lines
来源：http://yj.521024.cn

C#:   s.Split('\n')
来源：http://yz.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://bg.bjjhwx.cn

Py:   if not s:
来源：http://jw.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sv.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sm.shxzukj.cn

TS:   if (s === "") {}
来源：http://ua.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://gc.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://fm.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://rq.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vz.asd995.cn

[E21] 超长截断加省略号
来源：http://iu.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hn.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fs.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sq.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xr.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vq.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://cw.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fk.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ic.colortex.cn

[E22] 字节长度与字符长度
来源：http://ix.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ge.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cb.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cv.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iw.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://he.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://fg.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yf.szsharing.cn

================================================================================
来源：http://zz.jctech888.com.cn

F. 文件与目录
来源：http://el.szxytkj.cn

================================================================================
来源：http://np.asd995.cn

[F01] 读取整个文件
来源：http://rn.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cd.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ro.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lx.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mr.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gf.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://py.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://cd.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vq.gzmigu.cn

[F02] 逐行读取文件
来源：http://kb.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bz.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yv.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sz.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tg.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pj.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yp.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rb.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qf.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://jt.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lb.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hq.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vt.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qj.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ec.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mx.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://at.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sg.nicolike.cn

[F04] 追加写入文件
来源：http://fw.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nm.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ro.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wv.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ik.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pe.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://om.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://tq.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://no.colortex.cn

PHP:  file_exists("a.txt");
来源：http://rq.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://go.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://av.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tq.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://du.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://dw.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://xx.jctech888.com.cn

[F06] 删除文件
来源：http://xt.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://ew.huanxung.cn

PHP:  unlink("a.txt");
来源：http://yj.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wq.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cp.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xn.521024.cn

Go:   os.Remove("a.txt")
来源：http://im.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://xw.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://da.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://ex.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oj.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ys.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jt.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rl.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ez.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qw.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mt.hahajie.cn

[F08] 遍历目录
来源：http://tt.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hg.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jq.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://bh.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://mp.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ey.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.521024.cn

Ruby: Dir.children("dir")
来源：http://rf.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://xj.lnxyls.cn

[F09] 获取文件大小
来源：http://fh.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://bq.huanxung.cn

PHP:  filesize("a.txt");
来源：http://pe.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ep.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://tn.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kp.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bl.hahajie.cn

Ruby: File.size("a.txt")
来源：http://iw.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://we.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zq.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ns.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dm.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://fi.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ky.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rr.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xz.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xx.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://zg.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hh.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pq.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xs.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xj.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aj.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wc.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ao.yuexingan06.cn

[F12] CSV 读写
来源：http://hv.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ai.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ct.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ob.haigaiapp.cn

TS:   // 同上
来源：http://pc.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vg.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://of.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ww.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rg.szsharing.cn

================================================================================
来源：http://mu.gzmigu.cn

G. 面向对象
来源：http://pj.bookmarksfly.cn

================================================================================
来源：http://el.huanxung.cn

[G01] 定义类
来源：http://pi.asd995.cn

Py:   class User: pass
来源：http://hg.bookmarksfly.cn

PHP:  class User {}
来源：http://fe.huixiangedu.cn

JS:   class User {}
来源：http://qq.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://vf.bjjhwx.cn

Java: class User {}
来源：http://nw.szsharing.cn

Go:   type User struct { Name string }
来源：http://xf.chemitech.net.cn

Ruby: class User; end
来源：http://dy.yuexingan06.cn

C#:   class User {}
来源：http://dw.panjiajie.cn

[G02] 构造函数
来源：http://lc.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://rx.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://rx.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://zg.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://lb.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://rt.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lw.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://sb.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://ig.chemitech.net.cn

[G03] 实例属性
来源：http://ir.chemitech.net.cn

Py:   self.name = "x"
来源：http://xl.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://te.521024.cn

JS:   this.name = "x";
来源：http://st.bjjhwx.cn

TS:   name: string = "x";
来源：http://ze.shtwfgs.cn

Java: private String name;
来源：http://is.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://um.shxzskj.cn

Ruby: @name = "x"
来源：http://hm.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ai.bjjhwx.cn

[G04] 定义方法
来源：http://sc.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://zo.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://og.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://dv.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://td.shxzukj.cn

Java: String greet() { return name; }
来源：http://el.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zf.nszjky.cn

Ruby: def greet; @name; end
来源：http://rb.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://em.shxzukj.cn

[G05] 继承
来源：http://ml.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://hy.hahajie.cn

PHP:  class Admin extends User {}
来源：http://dr.521024.cn

JS:   class Admin extends User {}
来源：http://km.9csxet.cn

TS:   class Admin extends User {}
来源：http://hb.colortex.cn

Java: class Admin extends User {}
来源：http://dp.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ib.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://ic.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://cq.bookmarksfly.cn

[G06] 重写方法
来源：http://wg.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://mm.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ed.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ho.panjiajie.cn


<!-- 参考信息 -->