代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qp.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://bi.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hx.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xd.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ug.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xm.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xv.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wr.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bl.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jd.asd995.cn

[D26] 数组转字符串
来源：http://mq.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://to.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://mo.asd995.cn

JS:   arr.join(", ")
来源：http://zb.panjiajie.cn

TS:   arr.join(", ")
来源：http://nd.gzmigu.cn

Java: String.join(", ", list)
来源：http://uh.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://nd.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://gg.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://qu.colortex.cn

================================================================================
来源：http://uz.yuexingan06.cn

E. 字符串处理
来源：http://ml.shxzskj.cn

================================================================================
来源：http://fb.haigaiapp.cn

[E01] 拼接字符串
来源：http://ly.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uk.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ys.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fh.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cr.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yj.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kf.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xj.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lm.huixiangedu.cn

[E02] 重复字符串
来源：http://ja.huixiangedu.cn

Py:   "ab" * 3
来源：http://pk.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://yy.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://qd.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://qn.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://ve.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://gj.haigaiapp.cn

Ruby: "ab" * 3
来源：http://la.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://su.9csxet.cn

[E03] 截取子串
来源：http://wh.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oc.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qp.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nt.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://iu.colortex.cn

Java: s.substring(1, 4)
来源：http://yn.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gj.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yq.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://ml.lnxyls.cn

[E04] 查找子串位置
来源：http://ub.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://ea.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://rv.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kf.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://zv.hnjuh.cn

Java: s.indexOf("x")
来源：http://az.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://ye.szsharing.cn

Ruby: s.index("x")
来源：http://lw.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://cl.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mr.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jq.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vw.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yz.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cm.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wx.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ki.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yd.shtwfgs.cn

[E06] 替换子串
来源：http://ka.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ko.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://jm.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vc.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://vl.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ve.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vj.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rn.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ck.nszjky.cn

[E07] 按分隔符拆分
来源：http://wo.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fe.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qx.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ca.nicolike.cn

TS:   s.split(",")
来源：http://pc.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sy.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lv.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://lr.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ua.szsharing.cn

[E08] 数组按分隔符合并
来源：http://xu.shxzskj.cn

Py:   ",".join(items)
来源：http://qy.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://jh.huanxung.cn

JS:   items.join(",")
来源：http://js.huanxung.cn

TS:   items.join(",")
来源：http://sq.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://rb.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://xk.bookmarksfly.cn

Ruby: items.join(",")
来源：http://vy.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ha.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ad.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cw.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vz.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://ej.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://pm.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://te.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rn.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gq.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://no.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://xt.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tq.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kl.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://gx.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://wf.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://vb.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xp.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sd.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ox.bjjhwx.cn

[E11] 反转字符串
来源：http://mu.jianghongdianzi.cn

Py:   s[::-1]
来源：http://yi.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://vl.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://bg.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://mq.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wp.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ue.haigaiapp.cn

Ruby: s.reverse
来源：http://vt.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ia.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://dg.muxihuayi.cn

Py:   s.count("a")
来源：http://ys.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://si.szsharing.cn

JS:   s.split("a").length - 1
来源：http://hv.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://np.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nv.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://zd.huixiangedu.cn

Ruby: s.count("a")
来源：http://bw.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://rl.jctech888.com.cn

[E13] 逐字符遍历
来源：http://nl.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://ej.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ot.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nv.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ig.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bw.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zo.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eg.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ab.newstarts.cn

[E14] URL 编码与 Base64
来源：http://lv.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lh.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sg.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rb.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bu.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dz.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gp.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pe.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ga.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://nj.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cx.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ga.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pc.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uw.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vf.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kn.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dn.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aa.shxzskj.cn

[E16] 数字千分位
来源：http://hy.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://wz.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://ea.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qr.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zj.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://po.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://om.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ir.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ra.shxzskj.cn

[E17] 首字母大写
来源：http://oe.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lv.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bs.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cu.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qb.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ie.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fk.jctech888.com.cn

Ruby: s.capitalize
来源：http://lu.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tz.colortex.cn

[E18] 模板占位符替换
来源：http://cp.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dd.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://se.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ph.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eq.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cs.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pl.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ie.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pe.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://sa.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ln.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ur.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://db.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://bc.panjiajie.cn

Java: s.lines().toList()
来源：http://bj.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://af.hnjuh.cn

Ruby: s.lines
来源：http://xo.wgjwhj.cn

C#:   s.Split('\n')
来源：http://fp.521024.cn

[E20] 判断字符串是否为空
来源：http://zh.panjiajie.cn

Py:   if not s:
来源：http://kn.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ql.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://br.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://kl.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://pi.nicolike.cn

Go:   if s == "" {}
来源：http://gm.9csxet.cn

Ruby: if s.empty?
来源：http://qa.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bo.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://bl.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xo.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gv.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qy.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://od.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gi.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://ei.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ld.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ff.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://cz.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kh.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hx.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dy.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qd.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yu.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lo.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://qs.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ja.huanxung.cn

================================================================================
来源：http://qf.yuexingan06.cn

F. 文件与目录
来源：http://xt.gzmigu.cn

================================================================================
来源：http://ns.nszjky.cn

[F01] 读取整个文件
来源：http://pm.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uh.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://gb.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dd.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pt.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ud.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://pa.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://rb.9csxet.cn

[F02] 逐行读取文件
来源：http://ji.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qm.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yk.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pu.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sc.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://no.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pj.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kw.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://al.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://sw.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eq.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ji.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://es.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ht.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://js.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://sr.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mt.bjjhwx.cn

[F04] 追加写入文件
来源：http://px.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ax.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rr.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://re.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ev.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://po.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://le.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fc.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://gu.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kh.521024.cn

PHP:  file_exists("a.txt");
来源：http://ek.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://zz.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://fg.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xn.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://es.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://xw.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://sy.bookmarksfly.cn

[F06] 删除文件
来源：http://ax.newstarts.cn

Py:   os.remove("a.txt")
来源：http://kn.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://qu.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://on.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ko.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pd.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://kd.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://rs.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://hs.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://bo.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pw.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mf.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xj.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xc.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oy.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oc.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ol.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ly.szxytkj.cn

[F08] 遍历目录
来源：http://do.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xl.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qp.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://cp.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://hp.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ma.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://py.hahajie.cn

Ruby: Dir.children("dir")
来源：http://vp.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://wv.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://gw.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://us.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ly.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://le.lnxyls.cn


<!-- 参考信息 -->