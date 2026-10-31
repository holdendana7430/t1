代发 wailian999

Java: String.join(", ", list)
来源：http://tq.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://po.nszjky.cn

Ruby: arr.join(", ")
来源：http://fo.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://dq.jianghongdianzi.cn

================================================================================
来源：http://nz.panjiajie.cn

E. 字符串处理
来源：http://pu.gzmigu.cn

================================================================================
来源：http://ui.shxzukj.cn

[E01] 拼接字符串
来源：http://ou.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yd.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ov.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xz.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aj.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ay.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tc.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ha.hahajie.cn

[E02] 重复字符串
来源：http://ut.521024.cn

Py:   "ab" * 3
来源：http://kx.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://lu.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://nv.nszjky.cn

TS:   "ab".repeat(3)
来源：http://ot.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ki.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ji.nicolike.cn

Ruby: "ab" * 3
来源：http://be.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ty.bookmarksfly.cn

[E03] 截取子串
来源：http://hm.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bd.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zw.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jc.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://cn.shxzskj.cn

Java: s.substring(1, 4)
来源：http://iv.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://el.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sg.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ng.colortex.cn

[E04] 查找子串位置
来源：http://dz.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://fk.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://vw.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://va.nszjky.cn

TS:   s.indexOf("x")
来源：http://nu.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ff.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://gk.nicolike.cn

Ruby: s.index("x")
来源：http://vy.newstarts.cn

C#:   s.IndexOf("x")
来源：http://ej.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://te.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qj.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hm.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://af.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kr.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wv.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vf.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fi.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pn.jctech888.com.cn

[E06] 替换子串
来源：http://lw.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://do.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://gg.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fj.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://fr.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qk.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jz.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vz.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://oa.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://cu.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pc.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://se.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cy.szsharing.cn

TS:   s.split(",")
来源：http://zu.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mr.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xa.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://vh.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zv.newstarts.cn

[E08] 数组按分隔符合并
来源：http://nt.gzmigu.cn

Py:   ",".join(items)
来源：http://fi.newstarts.cn

PHP:  implode(",", $items);
来源：http://tm.bjjhwx.cn

JS:   items.join(",")
来源：http://sm.wgjwhj.cn

TS:   items.join(",")
来源：http://iz.colortex.cn

Java: String.join(",", items)
来源：http://hm.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://so.9csxet.cn

Ruby: items.join(",")
来源：http://vc.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://wd.nicolike.cn

[E09] 去除所有空白字符
来源：http://wa.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vb.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qt.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://ie.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://mc.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://gv.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mq.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nf.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dw.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://lq.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xe.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ho.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://my.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://me.colortex.cn

Java: String.format("%03d", 7)
来源：http://gq.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jn.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wc.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dx.asd995.cn

[E11] 反转字符串
来源：http://wr.huixinmuqiang.cn

Py:   s[::-1]
来源：http://mt.shxzukj.cn

PHP:  strrev($s);
来源：http://hs.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://yh.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://op.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mg.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mx.colortex.cn

Ruby: s.reverse
来源：http://rq.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ny.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://qx.nszjky.cn

Py:   s.count("a")
来源：http://ay.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://ws.hahajie.cn

JS:   s.split("a").length - 1
来源：http://aw.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://bh.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kq.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://du.yuexingan06.cn

Ruby: s.count("a")
来源：http://ih.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://dy.yuexingan06.cn

[E13] 逐字符遍历
来源：http://or.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://hg.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ix.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qd.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vj.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tw.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://by.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ca.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ak.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://xk.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jr.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lp.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://in.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://an.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://df.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hs.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yw.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://je.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://oi.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wt.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ee.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gj.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wu.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pr.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xn.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://az.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ze.jctech888.com.cn

[E16] 数字千分位
来源：http://ir.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://qz.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://hh.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xw.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pa.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yf.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ar.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ox.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://aj.shxzukj.cn

[E17] 首字母大写
来源：http://xr.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tp.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ds.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uh.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jl.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cn.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jz.szsharing.cn

Ruby: s.capitalize
来源：http://cb.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gn.521024.cn

[E18] 模板占位符替换
来源：http://mm.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qp.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vc.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yv.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pe.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aq.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zk.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qp.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cz.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://bd.hnjuh.cn

Py:   s.splitlines()
来源：http://gw.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wy.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://nr.521024.cn

TS:   s.split(/\r?\n/)
来源：http://sp.shtwfgs.cn

Java: s.lines().toList()
来源：http://fh.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ih.nszjky.cn

Ruby: s.lines
来源：http://rg.colortex.cn

C#:   s.Split('\n')
来源：http://cn.asd995.cn

[E20] 判断字符串是否为空
来源：http://tp.muxihuayi.cn

Py:   if not s:
来源：http://vl.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oy.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xe.muxihuayi.cn

TS:   if (s === "") {}
来源：http://gm.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://kf.bjjhwx.cn

Go:   if s == "" {}
来源：http://qp.huixiangedu.cn

Ruby: if s.empty?
来源：http://li.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ge.colortex.cn

[E21] 超长截断加省略号
来源：http://pi.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rm.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ps.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iq.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cy.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hx.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://yz.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rd.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://il.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://xj.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jf.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vd.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mk.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ni.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://td.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fr.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://ch.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://du.szsharing.cn

================================================================================
来源：http://qj.shxzukj.cn

F. 文件与目录
来源：http://yu.huanxung.cn

================================================================================
来源：http://os.szsharing.cn

[F01] 读取整个文件
来源：http://tw.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ab.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://av.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nc.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uk.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qm.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wr.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://wq.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://pc.newstarts.cn

[F02] 逐行读取文件
来源：http://od.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eh.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kb.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://me.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qm.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ff.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uq.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pf.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ae.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://gq.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tk.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://st.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ul.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hv.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ex.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jw.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://cq.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.yuexingan06.cn

[F04] 追加写入文件
来源：http://zn.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://np.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xh.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yd.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fe.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gi.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cy.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ld.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fo.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://wc.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zg.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://mi.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://yh.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://rb.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mj.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rc.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://eg.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://jp.shtwfgs.cn

[F06] 删除文件
来源：http://wb.huanxung.cn

Py:   os.remove("a.txt")
来源：http://gk.521024.cn

PHP:  unlink("a.txt");
来源：http://xf.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ta.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lm.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gv.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://ww.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://gy.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://ds.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://hi.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pd.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://td.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xy.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iq.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oi.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wn.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qq.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oh.szsharing.cn

[F08] 遍历目录
来源：http://ko.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ny.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yv.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://on.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://jx.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ry.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rj.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://gw.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://bo.jctech888.com.cn

[F09] 获取文件大小
来源：http://uz.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://om.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://du.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://wp.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://ve.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://in.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gf.521024.cn

Ruby: File.size("a.txt")
来源：http://yp.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://qb.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wb.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zv.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yv.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ox.521024.cn

TS:   path.extname("a.txt")
来源：http://ji.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://to.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ky.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mn.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ac.huanxung.cn

[F11] 复制与移动文件
来源：http://pm.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vk.bookmarksfly.cn


<!-- 参考信息 -->