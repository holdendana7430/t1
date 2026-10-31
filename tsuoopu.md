代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ls.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kc.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://gy.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rm.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pv.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://es.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://op.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mw.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cm.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oa.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sd.chemitech.net.cn

[D26] 数组转字符串
来源：http://wa.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://ui.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://uw.szxytkj.cn

JS:   arr.join(", ")
来源：http://jd.muxihuayi.cn

TS:   arr.join(", ")
来源：http://dp.nicolike.cn

Java: String.join(", ", list)
来源：http://pl.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://oz.nszjky.cn

Ruby: arr.join(", ")
来源：http://eu.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://bx.hnjuh.cn

================================================================================
来源：http://de.szsharing.cn

E. 字符串处理
来源：http://cy.jianghongdianzi.cn

================================================================================
来源：http://hs.shtwfgs.cn

[E01] 拼接字符串
来源：http://yo.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cg.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://co.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jq.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pu.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wr.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bo.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hw.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jy.jctech888.com.cn

[E02] 重复字符串
来源：http://kd.huanxung.cn

Py:   "ab" * 3
来源：http://yh.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://tw.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://yv.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://tz.nicolike.cn

Java: "ab".repeat(3)
来源：http://dz.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://gf.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://zg.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zw.muxihuayi.cn

[E03] 截取子串
来源：http://vw.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oy.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vf.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tv.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://cx.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://xa.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kn.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uw.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://kh.shxzukj.cn

[E04] 查找子串位置
来源：http://af.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://xx.9csxet.cn

PHP:  strpos($s, "x");
来源：http://nm.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sw.panjiajie.cn

TS:   s.indexOf("x")
来源：http://lq.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://zv.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://ru.haigaiapp.cn

Ruby: s.index("x")
来源：http://um.521024.cn

C#:   s.IndexOf("x")
来源：http://oi.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lf.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://un.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dl.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ua.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lv.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qh.nszjky.cn

[E06] 替换子串
来源：http://iw.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nn.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://qs.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://mc.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ex.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ot.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ns.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://kf.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://vy.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://do.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vh.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hn.gzmigu.cn

TS:   s.split(",")
来源：http://eb.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vy.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gr.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://nz.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jp.hahajie.cn

[E08] 数组按分隔符合并
来源：http://xl.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://zz.521024.cn

PHP:  implode(",", $items);
来源：http://lt.hnjuh.cn

JS:   items.join(",")
来源：http://go.gzmigu.cn

TS:   items.join(",")
来源：http://jh.gzmigu.cn

Java: String.join(",", items)
来源：http://fz.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://wu.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://wp.newstarts.cn

C#:   string.Join(",", items)
来源：http://jk.hahajie.cn

[E09] 去除所有空白字符
来源：http://oy.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gd.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ym.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://os.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://hl.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://bo.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fr.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pp.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ip.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://sc.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ns.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://le.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://lv.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://kw.9csxet.cn

Java: String.format("%03d", 7)
来源：http://ww.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://js.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lv.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pb.yuexingan06.cn

[E11] 反转字符串
来源：http://ne.haigaiapp.cn

Py:   s[::-1]
来源：http://ts.chemitech.net.cn

PHP:  strrev($s);
来源：http://ub.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://pv.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://uj.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tm.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wk.huanxung.cn

Ruby: s.reverse
来源：http://pi.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gb.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ab.huanxung.cn

Py:   s.count("a")
来源：http://ao.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://cq.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://vn.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ia.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hi.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://rk.huixiangedu.cn

Ruby: s.count("a")
来源：http://sq.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://ty.wgjwhj.cn

[E13] 逐字符遍历
来源：http://qe.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://hl.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ko.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ck.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dy.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bm.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://af.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sg.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zd.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://ax.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oj.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sn.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lg.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zd.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qf.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vy.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ni.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://el.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://mq.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gp.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://od.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hh.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ti.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rr.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vy.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://az.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://px.yuexingan06.cn

[E16] 数字千分位
来源：http://mb.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://eq.szsharing.cn

PHP:  number_format(1234567);
来源：http://lg.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wy.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xs.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tc.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bo.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xa.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://xh.9csxet.cn

[E17] 首字母大写
来源：http://iz.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zr.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pe.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iq.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ow.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ja.asd995.cn

Ruby: s.capitalize
来源：http://dj.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hq.hahajie.cn

[E18] 模板占位符替换
来源：http://yq.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yi.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qo.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xt.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ja.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rw.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oe.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://og.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rc.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://fl.szxytkj.cn

Py:   s.splitlines()
来源：http://wh.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uf.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://tr.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://sd.jctech888.com.cn

Java: s.lines().toList()
来源：http://iv.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://vn.huixiangedu.cn

Ruby: s.lines
来源：http://kh.jctech888.com.cn

C#:   s.Split('\n')
来源：http://wh.newstarts.cn

[E20] 判断字符串是否为空
来源：http://fs.panjiajie.cn

Py:   if not s:
来源：http://kd.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sx.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ye.lnxyls.cn

TS:   if (s === "") {}
来源：http://zb.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://ef.521024.cn

Go:   if s == "" {}
来源：http://qa.shtwfgs.cn

Ruby: if s.empty?
来源：http://rk.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fz.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://xb.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zo.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ky.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ch.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ru.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ed.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://kn.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lx.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tl.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://gd.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tj.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fh.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sf.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jx.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://no.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bd.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://qu.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://do.szxytkj.cn

================================================================================
来源：http://go.wgjwhj.cn

F. 文件与目录
来源：http://wc.wgjwhj.cn

================================================================================
来源：http://vd.huanxung.cn

[F01] 读取整个文件
来源：http://fi.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zu.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://mq.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gq.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zb.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ps.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://je.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://xb.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://nc.huixiangedu.cn

[F02] 逐行读取文件
来源：http://ty.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hs.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://al.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lt.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eg.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xz.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tt.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ib.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jt.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://xi.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fu.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mx.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wj.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://at.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pt.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hq.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://fz.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uu.colortex.cn

[F04] 追加写入文件
来源：http://sy.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gw.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hg.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hr.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mq.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mk.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aj.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sb.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xv.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://mh.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ky.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://ms.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ie.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://yn.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ih.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xl.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://zb.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://pg.shtwfgs.cn

[F06] 删除文件
来源：http://dq.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://pf.hahajie.cn

PHP:  unlink("a.txt");
来源：http://kb.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fx.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ml.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fl.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://fs.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://zo.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://ad.szsharing.cn

[F07] 创建目录（含多级）
来源：http://ec.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jf.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qg.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jb.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nj.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hr.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rn.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uy.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fi.newstarts.cn

[F08] 遍历目录
来源：http://ci.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://am.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mq.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ps.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://me.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nj.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vr.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://zm.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://rq.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://ht.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://mm.newstarts.cn

PHP:  filesize("a.txt");
来源：http://wi.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://rh.gzmigu.cn


<!-- 参考信息 -->