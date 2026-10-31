代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://pi.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://hf.panjiajie.cn

JS:   arr.join(", ")
来源：http://rh.bjjhwx.cn

TS:   arr.join(", ")
来源：http://rf.colortex.cn

Java: String.join(", ", list)
来源：http://ai.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://ix.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://ga.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://eg.shxzukj.cn

================================================================================
来源：http://fu.gzmigu.cn

E. 字符串处理
来源：http://tb.colortex.cn

================================================================================
来源：http://zg.chemitech.net.cn

[E01] 拼接字符串
来源：http://uo.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dr.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oj.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hp.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cq.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vu.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dq.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fc.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kx.nszjky.cn

[E02] 重复字符串
来源：http://oh.newstarts.cn

Py:   "ab" * 3
来源：http://nh.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://tt.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://ht.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://wn.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://mp.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://so.nicolike.cn

Ruby: "ab" * 3
来源：http://ti.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ep.huanxung.cn

[E03] 截取子串
来源：http://kz.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fz.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tr.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://te.521024.cn

TS:   s.slice(1, 4)
来源：http://qa.nszjky.cn

Java: s.substring(1, 4)
来源：http://jc.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mt.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zd.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://wr.521024.cn

[E04] 查找子串位置
来源：http://ri.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://di.szsharing.cn

PHP:  strpos($s, "x");
来源：http://dt.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yz.panjiajie.cn

TS:   s.indexOf("x")
来源：http://og.hnjuh.cn

Java: s.indexOf("x")
来源：http://bz.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://yi.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://oq.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://fv.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gf.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kc.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gt.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ct.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gf.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sv.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://if.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uy.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ti.huixinmuqiang.cn

[E06] 替换子串
来源：http://yc.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mg.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://hl.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hi.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://ag.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xc.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oe.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sy.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://cy.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://hm.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rb.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ot.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nk.bookmarksfly.cn

TS:   s.split(",")
来源：http://kc.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lw.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rr.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://wh.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jz.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://tp.szxytkj.cn

Py:   ",".join(items)
来源：http://xy.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://sf.shxzukj.cn

JS:   items.join(",")
来源：http://cb.shxzukj.cn

TS:   items.join(",")
来源：http://bl.shtwfgs.cn

Java: String.join(",", items)
来源：http://nx.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ty.bookmarksfly.cn

Ruby: items.join(",")
来源：http://gf.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://et.hahajie.cn

[E09] 去除所有空白字符
来源：http://nf.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ws.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qc.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://vw.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://fa.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://zu.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yh.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vh.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jn.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://np.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nx.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iy.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://zk.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://ii.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://aj.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ga.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://la.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cm.hahajie.cn

[E11] 反转字符串
来源：http://go.shxzskj.cn

Py:   s[::-1]
来源：http://eb.huixiangedu.cn

PHP:  strrev($s);
来源：http://br.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ke.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://yh.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fs.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xn.huixiangedu.cn

Ruby: s.reverse
来源：http://by.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rn.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://bz.lnxyls.cn

Py:   s.count("a")
来源：http://nd.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://ii.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://bf.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://dd.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ga.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://uq.muxihuayi.cn

Ruby: s.count("a")
来源：http://li.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://de.9csxet.cn

[E13] 逐字符遍历
来源：http://dx.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://uw.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://js.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dj.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xo.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jm.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bm.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rt.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tm.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://ig.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pl.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://er.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ty.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vj.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ah.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dn.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pg.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oy.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://yp.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://si.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sq.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cm.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tq.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ju.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aw.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://if.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kf.jctech888.com.cn

[E16] 数字千分位
来源：http://go.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ji.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://hj.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sf.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rs.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ej.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://al.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sf.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://az.9csxet.cn

[E17] 首字母大写
来源：http://ft.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qg.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cw.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qh.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jt.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bo.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yg.chemitech.net.cn

Ruby: s.capitalize
来源：http://cx.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zd.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://pl.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pn.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bh.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://si.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ic.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pg.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qf.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tt.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://gh.shxzskj.cn

Py:   s.splitlines()
来源：http://fu.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sv.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://py.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ww.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://hp.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://ed.jianghongdianzi.cn

Ruby: s.lines
来源：http://so.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ly.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://ik.gzmigu.cn

Py:   if not s:
来源：http://an.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wo.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vz.asd995.cn

TS:   if (s === "") {}
来源：http://oz.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://it.jctech888.com.cn

Go:   if s == "" {}
来源：http://sk.hnjuh.cn

Ruby: if s.empty?
来源：http://ac.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oj.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://az.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tz.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kx.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xs.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jz.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wj.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ss.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ms.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bk.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://ww.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vy.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vy.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://du.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lf.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uf.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gv.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://of.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gw.huixinmuqiang.cn

================================================================================
来源：http://il.hnjuh.cn

F. 文件与目录
来源：http://ph.panjiajie.cn

================================================================================
来源：http://hf.gzmigu.cn

[F01] 读取整个文件
来源：http://ft.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iz.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://dc.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uu.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ue.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://py.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kn.hahajie.cn

Ruby: File.read("a.txt")
来源：http://cf.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://mz.shtwfgs.cn

[F02] 逐行读取文件
来源：http://yj.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gs.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://br.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ue.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ix.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xa.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ww.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yv.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://oe.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://az.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kf.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jw.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iu.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bm.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://pu.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pn.colortex.cn

[F04] 追加写入文件
来源：http://aw.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hn.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ph.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cp.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rs.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://da.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hf.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://js.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lh.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://to.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jw.colortex.cn

PHP:  file_exists("a.txt");
来源：http://co.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://om.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://lh.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tu.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lb.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://mu.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://fb.shtwfgs.cn

[F06] 删除文件
来源：http://gn.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://uv.521024.cn

PHP:  unlink("a.txt");
来源：http://bd.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sx.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nt.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://az.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://rk.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://yz.521024.cn

C#:   File.Delete("a.txt");
来源：http://ts.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://xr.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ja.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ha.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jq.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hl.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://og.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xi.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://do.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ra.521024.cn

[F08] 遍历目录
来源：http://cn.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gs.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://by.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://mm.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://qg.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ks.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oc.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://vy.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://en.huanxung.cn

[F09] 获取文件大小
来源：http://en.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://df.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://me.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ep.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://cd.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zc.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pr.asd995.cn

Ruby: File.size("a.txt")
来源：http://oq.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://li.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://uf.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hv.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zs.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cw.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://wr.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ef.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://io.muxihuayi.cn


<!-- 参考信息 -->