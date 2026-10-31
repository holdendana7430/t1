代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qh.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gn.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dz.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://yn.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://fv.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://cr.521024.cn

JS:   arr.join(", ")
来源：http://cx.muxihuayi.cn

TS:   arr.join(", ")
来源：http://pn.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://xo.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://tj.hnjuh.cn

Ruby: arr.join(", ")
来源：http://ub.asd995.cn

C#:   string.Join(", ", list)
来源：http://kf.nicolike.cn

================================================================================
来源：http://zu.hnjuh.cn

E. 字符串处理
来源：http://mw.nszjky.cn

================================================================================
来源：http://gv.hahajie.cn

[E01] 拼接字符串
来源：http://dd.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zc.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ni.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ne.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jo.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ij.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nn.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gj.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bc.521024.cn

[E02] 重复字符串
来源：http://fv.panjiajie.cn

Py:   "ab" * 3
来源：http://vy.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://wg.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://el.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://rq.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ng.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://gq.chemitech.net.cn

Ruby: "ab" * 3
来源：http://hm.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hs.nicolike.cn

[E03] 截取子串
来源：http://ba.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xo.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dt.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ph.nicolike.cn

Java: s.substring(1, 4)
来源：http://hs.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ng.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pe.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://wc.szxytkj.cn

[E04] 查找子串位置
来源：http://lq.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://yd.szsharing.cn

PHP:  strpos($s, "x");
来源：http://hr.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dk.newstarts.cn

TS:   s.indexOf("x")
来源：http://wj.colortex.cn

Java: s.indexOf("x")
来源：http://dt.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://bn.colortex.cn

Ruby: s.index("x")
来源：http://js.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://zg.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vp.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qy.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fd.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mq.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qk.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uf.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yr.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wt.huixinmuqiang.cn

[E06] 替换子串
来源：http://ui.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yy.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ms.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sl.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://bs.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qz.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lh.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jt.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://nw.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://tj.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vp.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kd.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ub.hahajie.cn

TS:   s.split(",")
来源：http://ji.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vm.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jx.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://di.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://da.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://sy.huixiangedu.cn

Py:   ",".join(items)
来源：http://vu.shxzskj.cn

PHP:  implode(",", $items);
来源：http://ks.huixinmuqiang.cn

JS:   items.join(",")
来源：http://md.wgjwhj.cn

TS:   items.join(",")
来源：http://ri.panjiajie.cn

Java: String.join(",", items)
来源：http://eq.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://zg.gzmigu.cn

Ruby: items.join(",")
来源：http://ca.hahajie.cn

C#:   string.Join(",", items)
来源：http://sc.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://vo.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mh.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sk.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://jv.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://dq.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://jk.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mi.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kb.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ug.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ba.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oa.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kw.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://nv.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://pq.nszjky.cn

Java: String.format("%03d", 7)
来源：http://cc.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yn.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sq.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xm.bookmarksfly.cn

[E11] 反转字符串
来源：http://th.chemitech.net.cn

Py:   s[::-1]
来源：http://gx.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://yt.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://tj.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://tu.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://py.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ar.muxihuayi.cn

Ruby: s.reverse
来源：http://bl.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ek.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://xb.bookmarksfly.cn

Py:   s.count("a")
来源：http://uq.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://aj.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://om.szsharing.cn

TS:   s.split("a").length - 1
来源：http://tq.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ke.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://od.chemitech.net.cn

Ruby: s.count("a")
来源：http://rw.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://og.wgjwhj.cn

[E13] 逐字符遍历
来源：http://kv.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://vm.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xc.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kd.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bw.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fi.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uq.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://js.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uv.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://yj.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eh.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://md.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kl.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iu.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sn.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tb.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hs.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ag.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://tc.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bk.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qt.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tx.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yi.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tn.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rm.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jw.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ry.nszjky.cn

[E16] 数字千分位
来源：http://ce.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://ey.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://cs.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://na.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vm.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dn.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wz.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vx.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://kp.bookmarksfly.cn

[E17] 首字母大写
来源：http://ft.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yu.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nv.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cl.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aq.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bl.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qd.huanxung.cn

Ruby: s.capitalize
来源：http://mt.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qt.chemitech.net.cn

[E18] 模板占位符替换
来源：http://op.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ag.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bg.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wi.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ny.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pr.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tw.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sk.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://od.huanxung.cn

[E19] 多行文本按行拆分
来源：http://hg.shxzskj.cn

Py:   s.splitlines()
来源：http://sf.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zo.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://as.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://cv.nicolike.cn

Java: s.lines().toList()
来源：http://ia.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://wq.lnxyls.cn

Ruby: s.lines
来源：http://gi.bjjhwx.cn

C#:   s.Split('\n')
来源：http://ly.asd995.cn

[E20] 判断字符串是否为空
来源：http://vf.yuexingan06.cn

Py:   if not s:
来源：http://cr.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ep.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lq.colortex.cn

TS:   if (s === "") {}
来源：http://um.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://km.szsharing.cn

Go:   if s == "" {}
来源：http://fn.nicolike.cn

Ruby: if s.empty?
来源：http://io.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ef.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://hp.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kj.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ma.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jh.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://je.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zn.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://yj.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ux.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gd.9csxet.cn

[E22] 字节长度与字符长度
来源：http://yw.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gd.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nj.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mq.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lc.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jh.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yq.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://ph.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jf.szsharing.cn

================================================================================
来源：http://zf.yuexingan06.cn

F. 文件与目录
来源：http://cc.szxytkj.cn

================================================================================
来源：http://oi.asd995.cn

[F01] 读取整个文件
来源：http://ol.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ik.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://nl.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fj.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xb.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eg.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vy.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://qe.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://ju.panjiajie.cn

[F02] 逐行读取文件
来源：http://mf.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qs.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rt.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wn.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xt.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fl.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fh.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uw.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kh.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://xe.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fz.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wd.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ef.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tt.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yp.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jf.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://lt.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ez.chemitech.net.cn

[F04] 追加写入文件
来源：http://yb.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rs.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zi.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://or.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ks.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lo.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ae.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gt.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ci.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://oc.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iy.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://qy.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://re.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://qh.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tg.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://az.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://fl.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ru.jctech888.com.cn

[F06] 删除文件
来源：http://ef.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://xg.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ck.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://is.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gf.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jk.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://zs.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://mj.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://nd.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://rf.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gs.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mf.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ib.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jf.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hu.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pf.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qw.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cf.hahajie.cn

[F08] 遍历目录
来源：http://ei.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zy.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ub.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://ng.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ds.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lu.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zv.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://bt.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://db.yuexingan06.cn

[F09] 获取文件大小
来源：http://eb.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://pp.nszjky.cn

PHP:  filesize("a.txt");
来源：http://gk.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://hk.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://gt.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ga.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hy.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://cn.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ww.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://iy.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vs.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ga.lnxyls.cn


<!-- 参考信息 -->