代发 wailian999

================================================================================
来源：http://kl.asd995.cn

E. 字符串处理
来源：http://xp.bookmarksfly.cn

================================================================================
来源：http://ms.wgjwhj.cn

[E01] 拼接字符串
来源：http://np.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eg.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dv.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xv.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://if.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xo.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rx.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xb.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ja.newstarts.cn

[E02] 重复字符串
来源：http://wt.muxihuayi.cn

Py:   "ab" * 3
来源：http://tb.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://uq.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://jj.szsharing.cn

TS:   "ab".repeat(3)
来源：http://bp.hnjuh.cn

Java: "ab".repeat(3)
来源：http://ia.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://wp.nszjky.cn

Ruby: "ab" * 3
来源：http://xb.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lr.szxytkj.cn

[E03] 截取子串
来源：http://cn.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://co.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wv.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uq.huanxung.cn

TS:   s.slice(1, 4)
来源：http://jp.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://fm.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://et.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cq.asd995.cn

C#:   s.Substring(1, 3)
来源：http://yb.colortex.cn

[E04] 查找子串位置
来源：http://kf.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://so.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://yp.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bw.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://aa.521024.cn

Java: s.indexOf("x")
来源：http://zh.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://bh.bjjhwx.cn

Ruby: s.index("x")
来源：http://ay.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://hu.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pg.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://by.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ph.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ii.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zo.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cc.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://df.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ez.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://er.shxzskj.cn

[E06] 替换子串
来源：http://uf.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mi.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://sm.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kh.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://kp.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sq.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zr.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ou.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ub.gzmigu.cn

[E07] 按分隔符拆分
来源：http://lz.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xp.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ax.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ux.hahajie.cn

TS:   s.split(",")
来源：http://kv.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xz.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wc.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://zr.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xs.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://ow.hnjuh.cn

Py:   ",".join(items)
来源：http://gl.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://gx.asd995.cn

JS:   items.join(",")
来源：http://sl.haigaiapp.cn

TS:   items.join(",")
来源：http://bg.shxzskj.cn

Java: String.join(",", items)
来源：http://kn.521024.cn

Go:   strings.Join(items, ",")
来源：http://je.colortex.cn

Ruby: items.join(",")
来源：http://mg.huanxung.cn

C#:   string.Join(",", items)
来源：http://qn.521024.cn

[E09] 去除所有空白字符
来源：http://yz.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ae.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ej.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://ga.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://vk.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://hk.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rb.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ei.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ux.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://bi.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ef.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xu.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ow.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://cd.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://hw.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bj.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ti.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dn.bookmarksfly.cn

[E11] 反转字符串
来源：http://iw.newstarts.cn

Py:   s[::-1]
来源：http://du.521024.cn

PHP:  strrev($s);
来源：http://vg.asd995.cn

JS:   [...s].reverse().join("")
来源：http://bg.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://xg.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zo.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kl.colortex.cn

Ruby: s.reverse
来源：http://pr.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ha.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://ih.nszjky.cn

Py:   s.count("a")
来源：http://rv.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://uc.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://yc.asd995.cn

TS:   s.split("a").length - 1
来源：http://vt.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://di.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ym.yuexingan06.cn

Ruby: s.count("a")
来源：http://qo.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://vo.gzmigu.cn

[E13] 逐字符遍历
来源：http://nj.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://gd.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://am.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ee.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qw.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://si.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ns.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qv.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://di.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://vx.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://va.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sj.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sx.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zj.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ai.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://re.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nb.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://as.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ve.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://np.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ju.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sf.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hr.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lv.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://am.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rh.521024.cn

[E16] 数字千分位
来源：http://sn.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://uk.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://tf.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://en.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nq.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cv.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ns.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cq.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://qy.jianghongdianzi.cn

[E17] 首字母大写
来源：http://fq.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ka.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yc.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sc.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ik.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ia.hahajie.cn

Ruby: s.capitalize
来源：http://ea.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://no.panjiajie.cn

[E18] 模板占位符替换
来源：http://ls.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kf.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://an.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qy.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sf.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ax.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xa.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ob.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qt.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://un.521024.cn

Py:   s.splitlines()
来源：http://ep.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yv.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://gi.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://vx.colortex.cn

Java: s.lines().toList()
来源：http://vk.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://nx.lnxyls.cn

Ruby: s.lines
来源：http://bl.szsharing.cn

C#:   s.Split('\n')
来源：http://fy.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://or.jianghongdianzi.cn

Py:   if not s:
来源：http://vo.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rb.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wz.yuexingan06.cn

TS:   if (s === "") {}
来源：http://jy.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://cp.lnxyls.cn

Go:   if s == "" {}
来源：http://az.bjjhwx.cn

Ruby: if s.empty?
来源：http://kp.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xg.asd995.cn

[E21] 超长截断加省略号
来源：http://yu.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xt.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://di.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ql.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rr.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yf.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ht.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eg.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xw.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://mw.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lv.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fs.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lq.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rf.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jr.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://by.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://ax.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nf.jianghongdianzi.cn

================================================================================
来源：http://hu.huixinmuqiang.cn

F. 文件与目录
来源：http://rz.haigaiapp.cn

================================================================================
来源：http://wb.gzmigu.cn

[F01] 读取整个文件
来源：http://no.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nr.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ip.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yx.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aj.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aa.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iu.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://cu.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://lb.chemitech.net.cn

[F02] 逐行读取文件
来源：http://hg.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fl.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bs.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://un.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uk.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ew.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nl.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kq.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ou.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bl.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pk.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gj.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://md.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://py.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jx.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://hx.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kt.nszjky.cn

[F04] 追加写入文件
来源：http://vm.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hr.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wn.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wo.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ur.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mx.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sk.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mm.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bn.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://vs.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xc.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://yd.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://am.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://xz.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bp.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bs.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://dt.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://kb.jianghongdianzi.cn

[F06] 删除文件
来源：http://df.newstarts.cn

Py:   os.remove("a.txt")
来源：http://uf.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://gb.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oc.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://es.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kc.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://uy.asd995.cn

Ruby: File.delete("a.txt")
来源：http://hi.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://to.nszjky.cn

[F07] 创建目录（含多级）
来源：http://kh.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fb.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rj.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pv.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xq.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rd.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ag.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mg.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bw.gzmigu.cn

[F08] 遍历目录
来源：http://qs.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rr.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://km.521024.cn

JS:   fs.readdirSync("dir")
来源：http://xq.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://md.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ph.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yj.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://li.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://lf.bookmarksfly.cn

[F09] 获取文件大小
来源：http://lc.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://vs.9csxet.cn

PHP:  filesize("a.txt");
来源：http://km.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://sf.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://qt.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mk.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lb.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://vx.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://no.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://ok.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ll.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jp.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ep.nicolike.cn

TS:   path.extname("a.txt")
来源：http://tt.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zq.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vc.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ud.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qz.asd995.cn

[F11] 复制与移动文件
来源：http://lm.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zg.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vy.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cl.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uf.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gu.huixinmuqiang.cn


<!-- 参考信息 -->