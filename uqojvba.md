代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lo.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cr.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yg.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uq.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mq.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ov.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rq.szsharing.cn

[D26] 数组转字符串
来源：http://tv.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://hb.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://he.9csxet.cn

JS:   arr.join(", ")
来源：http://ca.szsharing.cn

TS:   arr.join(", ")
来源：http://lx.521024.cn

Java: String.join(", ", list)
来源：http://vo.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://dz.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://ht.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://dz.shxzskj.cn

================================================================================
来源：http://xh.bookmarksfly.cn

E. 字符串处理
来源：http://se.szsharing.cn

================================================================================
来源：http://ny.bjjhwx.cn

[E01] 拼接字符串
来源：http://nh.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jh.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lz.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ya.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jf.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://az.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fo.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ak.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yj.gzmigu.cn

[E02] 重复字符串
来源：http://sr.hnjuh.cn

Py:   "ab" * 3
来源：http://cz.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://az.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://oi.newstarts.cn

TS:   "ab".repeat(3)
来源：http://zu.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://az.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://jl.shxzskj.cn

Ruby: "ab" * 3
来源：http://ne.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gf.colortex.cn

[E03] 截取子串
来源：http://bv.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oo.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sm.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xb.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://lr.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://vg.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cn.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yp.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ky.bookmarksfly.cn

[E04] 查找子串位置
来源：http://fo.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://fy.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://eg.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pf.asd995.cn

TS:   s.indexOf("x")
来源：http://ft.shxzskj.cn

Java: s.indexOf("x")
来源：http://ap.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://tx.huanxung.cn

Ruby: s.index("x")
来源：http://ba.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://tp.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pb.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hn.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bf.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gt.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aw.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://io.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yu.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pv.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lb.haigaiapp.cn

[E06] 替换子串
来源：http://al.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iu.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://em.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fa.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://wo.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://un.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dy.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yg.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://hr.lnxyls.cn

[E07] 按分隔符拆分
来源：http://dn.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dl.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ci.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cq.hnjuh.cn

TS:   s.split(",")
来源：http://lf.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bf.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tc.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ut.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sb.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://gs.muxihuayi.cn

Py:   ",".join(items)
来源：http://xx.panjiajie.cn

PHP:  implode(",", $items);
来源：http://vn.bookmarksfly.cn

JS:   items.join(",")
来源：http://mx.521024.cn

TS:   items.join(",")
来源：http://ut.asd995.cn

Java: String.join(",", items)
来源：http://tn.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://hq.szsharing.cn

Ruby: items.join(",")
来源：http://ar.nicolike.cn

C#:   string.Join(",", items)
来源：http://sx.huanxung.cn

[E09] 去除所有空白字符
来源：http://gb.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dh.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://av.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://ob.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://wg.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://ps.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mg.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sd.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qx.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ff.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yd.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cy.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://wo.521024.cn

TS:   "7".padStart(3, "0")
来源：http://xn.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ht.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://po.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yp.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dd.shtwfgs.cn

[E11] 反转字符串
来源：http://ub.szxytkj.cn

Py:   s[::-1]
来源：http://yg.panjiajie.cn

PHP:  strrev($s);
来源：http://yo.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://dh.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://cd.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ap.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zi.colortex.cn

Ruby: s.reverse
来源：http://qm.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ai.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://vb.bjjhwx.cn

Py:   s.count("a")
来源：http://xz.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ng.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://ve.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://je.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iw.colortex.cn

Go:   strings.Count(s, "a")
来源：http://wf.huixiangedu.cn

Ruby: s.count("a")
来源：http://mb.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://jr.newstarts.cn

[E13] 逐字符遍历
来源：http://eg.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://qe.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zy.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pk.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oq.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dg.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ci.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sk.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xt.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://ko.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yv.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zj.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ka.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cy.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://by.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iq.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sk.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://nf.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ga.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rs.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ao.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cd.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wv.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ol.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tb.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cu.asd995.cn

[E16] 数字千分位
来源：http://xs.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://vy.nicolike.cn

PHP:  number_format(1234567);
来源：http://im.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bi.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xt.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zs.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bo.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://co.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://kp.haigaiapp.cn

[E17] 首字母大写
来源：http://mr.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iu.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dq.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vt.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://id.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dv.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.yuexingan06.cn

Ruby: s.capitalize
来源：http://od.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yl.asd995.cn

[E18] 模板占位符替换
来源：http://go.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wg.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cq.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sp.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wf.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kd.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jo.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jj.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cw.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://bi.hahajie.cn

Py:   s.splitlines()
来源：http://rd.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fv.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ff.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://kr.colortex.cn

Java: s.lines().toList()
来源：http://do.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://lj.bookmarksfly.cn

Ruby: s.lines
来源：http://wb.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://yw.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://gv.wgjwhj.cn

Py:   if not s:
来源：http://al.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xp.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vo.huixiangedu.cn

TS:   if (s === "") {}
来源：http://ci.521024.cn

Java: if (s.isEmpty()) {}
来源：http://sr.szxytkj.cn

Go:   if s == "" {}
来源：http://mu.newstarts.cn

Ruby: if s.empty?
来源：http://sx.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sg.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://br.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vz.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qb.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://on.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zn.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iv.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://yw.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://io.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vq.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://aq.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ck.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mt.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wy.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wc.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tr.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rt.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://vr.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yo.chemitech.net.cn

================================================================================
来源：http://tf.shxzukj.cn

F. 文件与目录
来源：http://bs.jianghongdianzi.cn

================================================================================
来源：http://rd.shxzskj.cn

[F01] 读取整个文件
来源：http://il.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mk.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://zv.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bu.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ei.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cl.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xn.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://db.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ly.muxihuayi.cn

[F02] 逐行读取文件
来源：http://sh.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zl.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sm.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fo.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mh.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yf.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://to.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zu.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lv.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://iz.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ev.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yo.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bs.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cy.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ix.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ed.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://ga.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gt.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://vz.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://to.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://na.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hy.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gh.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ou.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nm.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://os.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mu.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://bv.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://li.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://ba.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://nu.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ga.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sr.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mm.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://eq.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ti.yuexingan06.cn

[F06] 删除文件
来源：http://ax.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ur.521024.cn

PHP:  unlink("a.txt");
来源：http://xa.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ai.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nr.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zq.521024.cn

Go:   os.Remove("a.txt")
来源：http://dt.colortex.cn

Ruby: File.delete("a.txt")
来源：http://ns.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://nz.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ej.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ny.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jw.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sj.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gv.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xn.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://no.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dr.gzmigu.cn

[F08] 遍历目录
来源：http://zv.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gx.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://md.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://mp.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://uv.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wx.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mb.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://tu.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://kc.hahajie.cn

[F09] 获取文件大小
来源：http://qk.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://xn.huanxung.cn

PHP:  filesize("a.txt");
来源：http://qh.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://jk.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://nh.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iu.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ip.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://xd.jianghongdianzi.cn


<!-- 参考信息 -->