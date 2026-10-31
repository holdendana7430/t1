代发 wailian999

Java: String.join(", ", list)
来源：http://er.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://bo.gzmigu.cn

Ruby: arr.join(", ")
来源：http://fx.nicolike.cn

C#:   string.Join(", ", list)
来源：http://nz.haigaiapp.cn

================================================================================
来源：http://rv.huixiangedu.cn

E. 字符串处理
来源：http://va.szsharing.cn

================================================================================
来源：http://lz.newstarts.cn

[E01] 拼接字符串
来源：http://qd.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nd.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xk.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://si.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hc.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ku.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://na.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xw.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://go.colortex.cn

[E02] 重复字符串
来源：http://em.9csxet.cn

Py:   "ab" * 3
来源：http://ll.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://ez.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://gi.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://cl.hahajie.cn

Java: "ab".repeat(3)
来源：http://wm.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://dd.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://zw.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://js.haigaiapp.cn

[E03] 截取子串
来源：http://bx.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mp.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oe.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://la.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://zc.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://ik.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aw.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ps.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://xf.bjjhwx.cn

[E04] 查找子串位置
来源：http://jx.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://zi.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://se.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sg.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ut.colortex.cn

Java: s.indexOf("x")
来源：http://gq.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://cu.newstarts.cn

Ruby: s.index("x")
来源：http://tk.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://jc.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kd.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ix.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nh.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mv.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gb.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bg.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xs.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nj.asd995.cn

[E06] 替换子串
来源：http://ju.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qq.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://fu.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://no.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://zw.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wz.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fr.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kv.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://hs.szsharing.cn

[E07] 按分隔符拆分
来源：http://db.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://by.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zx.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xn.nszjky.cn

TS:   s.split(",")
来源：http://zd.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cv.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gq.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://kz.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yt.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://hl.hnjuh.cn

Py:   ",".join(items)
来源：http://dd.szxytkj.cn

PHP:  implode(",", $items);
来源：http://gz.shxzskj.cn

JS:   items.join(",")
来源：http://ak.wgjwhj.cn

TS:   items.join(",")
来源：http://qk.haigaiapp.cn

Java: String.join(",", items)
来源：http://rd.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://fs.huixiangedu.cn

Ruby: items.join(",")
来源：http://cx.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ke.szsharing.cn

[E09] 去除所有空白字符
来源：http://ki.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sr.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gw.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://uz.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://xs.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://gx.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cw.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://av.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dg.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://cn.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://od.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bq.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://uc.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://xx.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://gw.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bl.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cu.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ad.chemitech.net.cn

[E11] 反转字符串
来源：http://fd.huixinmuqiang.cn

Py:   s[::-1]
来源：http://eo.szsharing.cn

PHP:  strrev($s);
来源：http://cw.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://kf.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://oj.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://da.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://io.shtwfgs.cn

Ruby: s.reverse
来源：http://wl.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://en.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://ip.yuntaijiaju.cn

Py:   s.count("a")
来源：http://xh.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://hg.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ut.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://qq.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kx.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://ri.chemitech.net.cn

Ruby: s.count("a")
来源：http://ix.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://dn.huanxung.cn

[E13] 逐字符遍历
来源：http://pt.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://xo.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ic.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fj.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vy.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qv.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uh.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qx.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://re.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://lc.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jh.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://na.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bp.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ei.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qb.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bi.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wr.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jl.521024.cn

[E15] HTML 转义 / 反转义
来源：http://uh.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ei.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wq.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pm.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gp.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ue.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hg.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://na.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://td.szxytkj.cn

[E16] 数字千分位
来源：http://vw.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://sf.lnxyls.cn

PHP:  number_format(1234567);
来源：http://nk.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ri.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ya.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tk.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uz.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wd.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ne.bjjhwx.cn

[E17] 首字母大写
来源：http://yd.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zq.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ho.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cq.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://le.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jh.haigaiapp.cn

Ruby: s.capitalize
来源：http://mb.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gq.bjjhwx.cn

[E18] 模板占位符替换
来源：http://tn.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qb.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mt.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tb.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://za.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yi.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mc.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ml.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://on.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://hc.hahajie.cn

Py:   s.splitlines()
来源：http://hs.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zp.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://dh.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://qe.asd995.cn

Java: s.lines().toList()
来源：http://wn.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://dt.gzmigu.cn

Ruby: s.lines
来源：http://ab.szxytkj.cn

C#:   s.Split('\n')
来源：http://mf.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ta.muxihuayi.cn

Py:   if not s:
来源：http://zn.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ey.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://is.hnjuh.cn

TS:   if (s === "") {}
来源：http://jd.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ay.jctech888.com.cn

Go:   if s == "" {}
来源：http://gp.newstarts.cn

Ruby: if s.empty?
来源：http://us.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ia.gzmigu.cn

[E21] 超长截断加省略号
来源：http://ly.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yh.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qs.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gp.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jx.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vw.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://aq.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cf.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bh.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://sd.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://da.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ml.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gh.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://da.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bg.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bi.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://ux.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pe.9csxet.cn

================================================================================
来源：http://wr.hnjuh.cn

F. 文件与目录
来源：http://le.bjjhwx.cn

================================================================================
来源：http://ob.wgjwhj.cn

[F01] 读取整个文件
来源：http://vx.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bg.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://wa.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bj.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cu.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yp.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zh.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://aq.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://jp.szxytkj.cn

[F02] 逐行读取文件
来源：http://gi.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nm.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ei.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sl.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hj.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zf.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ca.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rq.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gx.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ch.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tv.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ow.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eg.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sh.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vw.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gy.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://nm.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vo.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://dc.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vm.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ab.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bt.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://it.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fj.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zx.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mn.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ms.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ww.521024.cn

PHP:  file_exists("a.txt");
来源：http://mb.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://eo.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://xh.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rm.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xi.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://dk.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://ez.szsharing.cn

[F06] 删除文件
来源：http://lz.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://gv.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://la.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ny.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gb.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yu.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://pf.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://pi.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://vp.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://qb.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nl.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ou.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nv.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uj.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ke.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ec.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vz.yuexingan06.cn

[F08] 遍历目录
来源：http://uh.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xu.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://px.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://xw.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://pu.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qe.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oz.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ov.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://hh.yuexingan06.cn

[F09] 获取文件大小
来源：http://ng.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://pe.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://dl.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://pj.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://ov.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://py.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tj.szsharing.cn

Ruby: File.size("a.txt")
来源：http://fq.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mg.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://pe.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rq.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ph.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pr.huanxung.cn

TS:   path.extname("a.txt")
来源：http://kb.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fo.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vi.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ru.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pc.hahajie.cn

[F11] 复制与移动文件
来源：http://on.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://la.szxytkj.cn


<!-- 参考信息 -->