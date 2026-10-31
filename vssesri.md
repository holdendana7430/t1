代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ym.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ub.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://sp.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ae.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tx.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ej.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wa.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dk.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://df.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tv.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eh.muxihuayi.cn

[D26] 数组转字符串
来源：http://gm.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://hu.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://dw.szsharing.cn

JS:   arr.join(", ")
来源：http://pc.shxzskj.cn

TS:   arr.join(", ")
来源：http://zj.shxzukj.cn

Java: String.join(", ", list)
来源：http://aa.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://zl.521024.cn

Ruby: arr.join(", ")
来源：http://vb.colortex.cn

C#:   string.Join(", ", list)
来源：http://gy.szsharing.cn

================================================================================
来源：http://vz.shxzukj.cn

E. 字符串处理
来源：http://vj.shtwfgs.cn

================================================================================
来源：http://pu.wgjwhj.cn

[E01] 拼接字符串
来源：http://yy.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fs.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://re.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gz.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wu.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tv.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qz.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pq.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vx.colortex.cn

[E02] 重复字符串
来源：http://gm.huanxung.cn

Py:   "ab" * 3
来源：http://cy.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://my.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://lo.nicolike.cn

TS:   "ab".repeat(3)
来源：http://vs.lnxyls.cn

Java: "ab".repeat(3)
来源：http://oe.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://bt.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://aa.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rv.newstarts.cn

[E03] 截取子串
来源：http://mg.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tp.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xz.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yp.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://fk.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://ol.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ib.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gi.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://sy.gzmigu.cn

[E04] 查找子串位置
来源：http://al.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://vm.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ay.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://th.nszjky.cn

TS:   s.indexOf("x")
来源：http://dv.hahajie.cn

Java: s.indexOf("x")
来源：http://gn.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://gy.panjiajie.cn

Ruby: s.index("x")
来源：http://wu.nszjky.cn

C#:   s.IndexOf("x")
来源：http://fh.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ff.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eh.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bx.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tt.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zp.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://am.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://an.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uz.bjjhwx.cn

[E06] 替换子串
来源：http://hy.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rk.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://yk.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dp.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://xr.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vh.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fe.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bp.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://cs.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://uw.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eu.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://su.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ot.szxytkj.cn

TS:   s.split(",")
来源：http://mz.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ix.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pu.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://ds.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uj.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://pn.haigaiapp.cn

Py:   ",".join(items)
来源：http://zw.asd995.cn

PHP:  implode(",", $items);
来源：http://zu.yuntaijiaju.cn

JS:   items.join(",")
来源：http://yx.shxzukj.cn

TS:   items.join(",")
来源：http://mz.9csxet.cn

Java: String.join(",", items)
来源：http://mn.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://kx.yuexingan06.cn

Ruby: items.join(",")
来源：http://ui.gzmigu.cn

C#:   string.Join(",", items)
来源：http://uc.lnxyls.cn

[E09] 去除所有空白字符
来源：http://kd.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nd.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yy.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://vu.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://ub.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://cl.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wl.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://no.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yk.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://nl.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://il.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kl.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://bb.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://ta.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://lt.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ir.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nu.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iz.huixiangedu.cn

[E11] 反转字符串
来源：http://sy.newstarts.cn

Py:   s[::-1]
来源：http://cv.shxzukj.cn

PHP:  strrev($s);
来源：http://fd.521024.cn

JS:   [...s].reverse().join("")
来源：http://ud.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://ps.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jj.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sj.huixiangedu.cn

Ruby: s.reverse
来源：http://di.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://do.521024.cn

[E12] 统计某字符出现次数
来源：http://bx.szsharing.cn

Py:   s.count("a")
来源：http://uj.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://mn.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://km.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://hl.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xx.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://ws.colortex.cn

Ruby: s.count("a")
来源：http://aq.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://bk.shxzskj.cn

[E13] 逐字符遍历
来源：http://mw.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://oo.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fh.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kn.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nb.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vp.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bw.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://az.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pv.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://og.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fa.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qf.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sp.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kz.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ek.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://au.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zt.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ou.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://oa.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vq.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bh.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ah.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ub.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nq.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://be.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ol.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nx.jctech888.com.cn

[E16] 数字千分位
来源：http://iq.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://tl.hahajie.cn

PHP:  number_format(1234567);
来源：http://zr.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pn.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gy.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nj.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zh.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ld.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://hf.colortex.cn

[E17] 首字母大写
来源：http://ag.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vn.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sl.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://an.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://it.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gx.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wv.asd995.cn

Ruby: s.capitalize
来源：http://sf.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hq.colortex.cn

[E18] 模板占位符替换
来源：http://fc.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fz.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jn.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hb.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hs.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://px.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rs.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://le.szsharing.cn

[E19] 多行文本按行拆分
来源：http://tc.hahajie.cn

Py:   s.splitlines()
来源：http://ib.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://an.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://ak.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ol.haigaiapp.cn

Java: s.lines().toList()
来源：http://mo.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ou.huixiangedu.cn

Ruby: s.lines
来源：http://rb.huixiangedu.cn

C#:   s.Split('\n')
来源：http://xz.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://cc.szsharing.cn

Py:   if not s:
来源：http://mo.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yq.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gk.521024.cn

TS:   if (s === "") {}
来源：http://za.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://pb.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://mm.panjiajie.cn

Ruby: if s.empty?
来源：http://mf.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nt.asd995.cn

[E21] 超长截断加省略号
来源：http://sc.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wu.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ib.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uf.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dt.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fh.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ug.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bi.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cr.hahajie.cn

[E22] 字节长度与字符长度
来源：http://ki.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jt.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oa.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ye.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mk.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vy.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://dt.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ip.shtwfgs.cn

================================================================================
来源：http://sq.shxzskj.cn

F. 文件与目录
来源：http://qb.hnjuh.cn

================================================================================
来源：http://pw.bookmarksfly.cn

[F01] 读取整个文件
来源：http://gl.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zw.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://rs.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://se.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nb.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nv.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jv.colortex.cn

Ruby: File.read("a.txt")
来源：http://xd.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://yu.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://cd.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bu.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mj.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pk.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://te.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gb.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cj.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rp.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://qk.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cu.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rv.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bk.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rp.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ns.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dj.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ni.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ll.nicolike.cn

[F04] 追加写入文件
来源：http://cj.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://he.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ry.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ct.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://he.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sn.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qc.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ef.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nl.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ik.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sh.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://fj.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://lg.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://zq.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://je.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wh.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://bm.521024.cn

C#:   File.Exists("a.txt")
来源：http://cu.szxytkj.cn

[F06] 删除文件
来源：http://oe.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://da.colortex.cn

PHP:  unlink("a.txt");
来源：http://ob.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iq.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://md.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://db.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://rf.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://xf.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://wm.asd995.cn

[F07] 创建目录（含多级）
来源：http://yy.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ld.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xu.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qa.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qd.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vj.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vu.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zz.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yh.huixiangedu.cn

[F08] 遍历目录
来源：http://nc.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kr.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xx.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ze.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://fg.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cq.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://re.szsharing.cn

Ruby: Dir.children("dir")
来源：http://dz.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://vm.gzmigu.cn

[F09] 获取文件大小
来源：http://qs.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ea.colortex.cn

PHP:  filesize("a.txt");
来源：http://ln.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ey.panjiajie.cn


<!-- 参考信息 -->