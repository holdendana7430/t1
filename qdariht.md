代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ap.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qf.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://or.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bh.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ch.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zd.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://og.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ar.huixinmuqiang.cn

[E06] 替换子串
来源：http://dm.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hw.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ya.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ir.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://ma.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://di.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rd.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tn.colortex.cn

C#:   s.Replace("a", "b")
来源：http://xf.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://pu.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dq.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sf.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bf.colortex.cn

TS:   s.split(",")
来源：http://mz.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://st.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oc.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://mk.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yd.newstarts.cn

[E08] 数组按分隔符合并
来源：http://sy.bjjhwx.cn

Py:   ",".join(items)
来源：http://xe.shxzskj.cn

PHP:  implode(",", $items);
来源：http://ee.yuntaijiaju.cn

JS:   items.join(",")
来源：http://wm.9csxet.cn

TS:   items.join(",")
来源：http://vy.wgjwhj.cn

Java: String.join(",", items)
来源：http://sy.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://rl.panjiajie.cn

Ruby: items.join(",")
来源：http://sm.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://rv.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://ky.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jr.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://so.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://wg.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://sy.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://lr.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sq.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ub.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ob.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://kt.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kl.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zr.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ia.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://er.szsharing.cn

Java: String.format("%03d", 7)
来源：http://nu.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ml.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nb.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cm.jctech888.com.cn

[E11] 反转字符串
来源：http://en.wgjwhj.cn

Py:   s[::-1]
来源：http://mk.hnjuh.cn

PHP:  strrev($s);
来源：http://aj.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://vt.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://zb.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xs.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gy.shtwfgs.cn

Ruby: s.reverse
来源：http://fo.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sp.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://qi.huanxung.cn

Py:   s.count("a")
来源：http://pe.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://ob.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://qb.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://cz.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rj.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://gv.asd995.cn

Ruby: s.count("a")
来源：http://su.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://di.muxihuayi.cn

[E13] 逐字符遍历
来源：http://oz.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://me.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wa.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ab.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nd.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nv.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hp.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gh.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mo.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://dh.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://si.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mg.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pw.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://at.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jp.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://th.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hg.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rt.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://ro.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wv.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uh.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sn.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nr.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://es.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hc.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oe.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hg.bookmarksfly.cn

[E16] 数字千分位
来源：http://xu.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://cx.huanxung.cn

PHP:  number_format(1234567);
来源：http://xm.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ke.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vr.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ib.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pa.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ow.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://jy.newstarts.cn

[E17] 首字母大写
来源：http://vo.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wv.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fs.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://re.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ma.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iu.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wz.colortex.cn

Ruby: s.capitalize
来源：http://ib.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://at.szxytkj.cn

[E18] 模板占位符替换
来源：http://se.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fh.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pb.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qh.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zr.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yi.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xh.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ox.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ut.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://pf.yuexingan06.cn

Py:   s.splitlines()
来源：http://ib.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xi.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://yp.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ct.lnxyls.cn

Java: s.lines().toList()
来源：http://wa.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://jd.szsharing.cn

Ruby: s.lines
来源：http://qx.shxzukj.cn

C#:   s.Split('\n')
来源：http://fa.521024.cn

[E20] 判断字符串是否为空
来源：http://hq.panjiajie.cn

Py:   if not s:
来源：http://io.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uu.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xk.szsharing.cn

TS:   if (s === "") {}
来源：http://xb.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://nl.hnjuh.cn

Go:   if s == "" {}
来源：http://fs.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://ju.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dw.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://nu.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vw.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dy.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kj.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lg.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dl.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://cx.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vi.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kx.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://oz.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://au.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ap.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ba.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pf.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yb.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ki.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://ug.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lm.lnxyls.cn

================================================================================
来源：http://yp.bjjhwx.cn

F. 文件与目录
来源：http://sa.bookmarksfly.cn

================================================================================
来源：http://am.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://jy.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gg.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ph.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wr.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tt.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ur.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ca.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://ml.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://tj.huanxung.cn

[F02] 逐行读取文件
来源：http://ih.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ko.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://au.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iq.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cz.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yz.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rm.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://za.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sm.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://xp.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://km.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kx.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ex.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oi.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bm.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fj.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ru.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xb.nszjky.cn

[F04] 追加写入文件
来源：http://cx.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nx.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ga.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://in.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nq.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iu.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yf.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bl.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cw.521024.cn

[F05] 判断文件或目录是否存在
来源：http://sa.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://le.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://om.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://yw.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://nd.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ds.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ha.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://uk.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://pj.newstarts.cn

[F06] 删除文件
来源：http://sw.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://dz.asd995.cn

PHP:  unlink("a.txt");
来源：http://xh.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ot.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wk.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sf.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://of.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://lg.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://wz.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://zd.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kb.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://st.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mg.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hs.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://og.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jt.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cv.haigaiapp.cn

[F08] 遍历目录
来源：http://gw.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gi.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dz.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://dq.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://em.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ja.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sp.colortex.cn

Ruby: Dir.children("dir")
来源：http://uu.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://nr.jctech888.com.cn

[F09] 获取文件大小
来源：http://vf.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://ri.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://lb.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://sj.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://ql.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ob.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://po.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://mh.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://zk.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://fd.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bm.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xr.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zx.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://jq.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cd.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://td.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mt.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gt.nicolike.cn

[F11] 复制与移动文件
来源：http://le.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ct.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wq.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wz.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://to.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xa.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mq.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ag.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zu.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sn.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vs.newstarts.cn

TS:   // 同上
来源：http://ob.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aa.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xz.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://up.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qz.huanxung.cn

================================================================================
来源：http://ya.huixiangedu.cn

G. 面向对象
来源：http://st.gzmigu.cn

================================================================================
来源：http://xv.lnxyls.cn

[G01] 定义类
来源：http://bs.huanxung.cn

Py:   class User: pass
来源：http://rq.huanxung.cn

PHP:  class User {}
来源：http://aw.521024.cn

JS:   class User {}
来源：http://xt.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://lw.9csxet.cn

Java: class User {}
来源：http://ps.hnjuh.cn

Go:   type User struct { Name string }
来源：http://pf.huanxung.cn

Ruby: class User; end
来源：http://ir.huixinmuqiang.cn

C#:   class User {}
来源：http://sw.newstarts.cn

[G02] 构造函数
来源：http://fy.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://np.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://kx.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://tr.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://yn.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://pa.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uc.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vi.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://tb.szsharing.cn

[G03] 实例属性
来源：http://dn.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://ol.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://lt.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ua.yuexingan06.cn

TS:   name: string = "x";
来源：http://dw.jianghongdianzi.cn

Java: private String name;
来源：http://fn.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gy.nicolike.cn


<!-- 参考信息 -->