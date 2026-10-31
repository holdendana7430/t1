代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gw.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pn.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ai.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ay.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gp.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pf.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kr.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wj.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jw.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ok.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dt.colortex.cn

[D26] 数组转字符串
来源：http://ax.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://hy.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://yd.9csxet.cn

JS:   arr.join(", ")
来源：http://kr.muxihuayi.cn

TS:   arr.join(", ")
来源：http://rt.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ak.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://vr.szsharing.cn

Ruby: arr.join(", ")
来源：http://hd.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://fe.jianghongdianzi.cn

================================================================================
来源：http://qc.lnxyls.cn

E. 字符串处理
来源：http://tc.szsharing.cn

================================================================================
来源：http://uh.szxytkj.cn

[E01] 拼接字符串
来源：http://um.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hw.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cv.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vz.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sf.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ws.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ay.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mf.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ws.gzmigu.cn

[E02] 重复字符串
来源：http://er.nicolike.cn

Py:   "ab" * 3
来源：http://jf.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.nicolike.cn

JS:   "ab".repeat(3)
来源：http://xo.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://gj.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ug.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://fv.chemitech.net.cn

Ruby: "ab" * 3
来源：http://gz.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lf.hnjuh.cn

[E03] 截取子串
来源：http://jl.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://io.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pk.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ho.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://bk.szxytkj.cn

Java: s.substring(1, 4)
来源：http://nx.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bp.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ar.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://jn.jctech888.com.cn

[E04] 查找子串位置
来源：http://ih.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://zp.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://ql.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://di.huanxung.cn

TS:   s.indexOf("x")
来源：http://az.colortex.cn

Java: s.indexOf("x")
来源：http://bc.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://mz.nicolike.cn

Ruby: s.index("x")
来源：http://qx.newstarts.cn

C#:   s.IndexOf("x")
来源：http://yr.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gq.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yj.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ed.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zz.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cm.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sw.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tq.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ma.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://di.szxytkj.cn

[E06] 替换子串
来源：http://xv.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gu.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://ak.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mb.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://zh.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vo.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vi.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ij.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://eo.szsharing.cn

[E07] 按分隔符拆分
来源：http://id.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xs.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://py.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mc.chemitech.net.cn

TS:   s.split(",")
来源：http://ot.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pg.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zw.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://bn.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jd.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://wk.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://mg.hahajie.cn

PHP:  implode(",", $items);
来源：http://kv.nicolike.cn

JS:   items.join(",")
来源：http://bg.nicolike.cn

TS:   items.join(",")
来源：http://jp.521024.cn

Java: String.join(",", items)
来源：http://gw.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://te.huixiangedu.cn

Ruby: items.join(",")
来源：http://gn.nszjky.cn

C#:   string.Join(",", items)
来源：http://ot.9csxet.cn

[E09] 去除所有空白字符
来源：http://nq.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://er.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dh.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://rc.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://bj.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://gy.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kc.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sm.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mh.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://ch.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nt.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vs.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://zc.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://mi.521024.cn

Java: String.format("%03d", 7)
来源：http://de.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pn.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dv.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lb.haigaiapp.cn

[E11] 反转字符串
来源：http://sk.nicolike.cn

Py:   s[::-1]
来源：http://un.9csxet.cn

PHP:  strrev($s);
来源：http://pv.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://wn.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://mc.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ju.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kf.jctech888.com.cn

Ruby: s.reverse
来源：http://ws.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sp.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://mc.huixinmuqiang.cn

Py:   s.count("a")
来源：http://yp.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://dj.hahajie.cn

JS:   s.split("a").length - 1
来源：http://cc.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://uc.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oe.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://yy.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://af.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://kw.wgjwhj.cn

[E13] 逐字符遍历
来源：http://ns.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://mq.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pm.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sx.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uu.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vb.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dp.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qa.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jo.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://yw.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sf.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://is.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yr.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cr.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xx.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://if.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bn.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rz.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://yi.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rt.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zu.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gu.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fx.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hv.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cq.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://db.szxytkj.cn

[E16] 数字千分位
来源：http://db.521024.cn

Py:   f"{1234567:,}"
来源：http://co.shxzukj.cn

PHP:  number_format(1234567);
来源：http://vz.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hv.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dq.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://os.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mi.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ut.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://gi.szxytkj.cn

[E17] 首字母大写
来源：http://ht.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://os.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ks.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bt.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ki.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ix.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://us.shtwfgs.cn

Ruby: s.capitalize
来源：http://jq.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ol.colortex.cn

[E18] 模板占位符替换
来源：http://es.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ti.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://du.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cx.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ls.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kd.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zx.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fx.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cq.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://yn.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://oe.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jl.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://va.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://nt.newstarts.cn

Java: s.lines().toList()
来源：http://bo.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://yk.nicolike.cn

Ruby: s.lines
来源：http://np.shtwfgs.cn

C#:   s.Split('\n')
来源：http://da.hahajie.cn

[E20] 判断字符串是否为空
来源：http://jz.szxytkj.cn

Py:   if not s:
来源：http://xu.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bk.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fa.szxytkj.cn

TS:   if (s === "") {}
来源：http://wz.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://oz.szxytkj.cn

Go:   if s == "" {}
来源：http://da.huixiangedu.cn

Ruby: if s.empty?
来源：http://zd.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wd.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://wu.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pk.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gy.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ld.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ok.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://zx.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zo.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uj.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://aw.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://td.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sy.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yc.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qc.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ol.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pi.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://zn.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bx.jianghongdianzi.cn

================================================================================
来源：http://jp.jctech888.com.cn

F. 文件与目录
来源：http://xa.hnjuh.cn

================================================================================
来源：http://py.9csxet.cn

[F01] 读取整个文件
来源：http://ss.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yb.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ob.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://we.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://um.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gm.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fb.newstarts.cn

Ruby: File.read("a.txt")
来源：http://lm.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://qy.asd995.cn

[F02] 逐行读取文件
来源：http://sa.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rx.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qn.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fg.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yv.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://td.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mj.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ak.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://pv.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cb.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zo.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vl.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://as.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://og.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dr.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://ew.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kj.chemitech.net.cn

[F04] 追加写入文件
来源：http://hk.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vs.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ff.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zg.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hp.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aj.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ot.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gi.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jg.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://ca.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tk.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://kk.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://rh.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://qn.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fv.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hj.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ea.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://ih.szsharing.cn

[F06] 删除文件
来源：http://iw.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://ei.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://pw.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wy.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hm.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mu.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://ih.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://wq.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://xd.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://lg.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://og.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hi.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ch.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ro.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kh.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ui.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xs.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gf.gzmigu.cn

[F08] 遍历目录
来源：http://he.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jj.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ji.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ro.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://lj.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pf.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bd.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://zp.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://tx.521024.cn

[F09] 获取文件大小
来源：http://zy.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://vv.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://dw.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://oo.jctech888.com.cn


<!-- 参考信息 -->