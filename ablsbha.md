代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mg.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bq.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ve.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xr.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://se.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pa.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://su.hahajie.cn

[D26] 数组转字符串
来源：http://co.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://zm.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://mr.hahajie.cn

JS:   arr.join(", ")
来源：http://ww.haigaiapp.cn

TS:   arr.join(", ")
来源：http://mn.chemitech.net.cn

Java: String.join(", ", list)
来源：http://rj.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ng.521024.cn

Ruby: arr.join(", ")
来源：http://to.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://om.chemitech.net.cn

================================================================================
来源：http://gf.hnjuh.cn

E. 字符串处理
来源：http://jw.521024.cn

================================================================================
来源：http://ei.chemitech.net.cn

[E01] 拼接字符串
来源：http://uz.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mf.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ep.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mm.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ye.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vo.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zn.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mj.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fy.shtwfgs.cn

[E02] 重复字符串
来源：http://lv.asd995.cn

Py:   "ab" * 3
来源：http://oy.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ab.asd995.cn

JS:   "ab".repeat(3)
来源：http://nw.9csxet.cn

TS:   "ab".repeat(3)
来源：http://lj.szsharing.cn

Java: "ab".repeat(3)
来源：http://yq.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://pp.jctech888.com.cn

Ruby: "ab" * 3
来源：http://gf.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gm.bjjhwx.cn

[E03] 截取子串
来源：http://am.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://on.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ka.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pj.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://vc.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ef.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://le.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://va.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ey.nszjky.cn

[E04] 查找子串位置
来源：http://ti.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ut.hahajie.cn

PHP:  strpos($s, "x");
来源：http://bd.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nw.panjiajie.cn

TS:   s.indexOf("x")
来源：http://fl.newstarts.cn

Java: s.indexOf("x")
来源：http://ai.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://va.nicolike.cn

Ruby: s.index("x")
来源：http://lf.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://yu.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://io.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kv.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tt.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://et.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wg.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://va.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vy.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ws.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mk.jctech888.com.cn

[E06] 替换子串
来源：http://kw.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ck.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://hh.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jv.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://ym.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lu.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lu.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mv.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://be.521024.cn

[E07] 按分隔符拆分
来源：http://yt.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qk.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yd.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://re.newstarts.cn

TS:   s.split(",")
来源：http://oa.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ol.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ck.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://iz.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://id.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://xh.gzmigu.cn

Py:   ",".join(items)
来源：http://yq.shxzukj.cn

PHP:  implode(",", $items);
来源：http://gl.bookmarksfly.cn

JS:   items.join(",")
来源：http://rr.haigaiapp.cn

TS:   items.join(",")
来源：http://tx.asd995.cn

Java: String.join(",", items)
来源：http://lx.asd995.cn

Go:   strings.Join(items, ",")
来源：http://zx.521024.cn

Ruby: items.join(",")
来源：http://vz.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://re.shxzukj.cn

[E09] 去除所有空白字符
来源：http://ps.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eu.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lz.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yn.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://jl.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://vw.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nh.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jd.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bi.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://cy.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lx.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xa.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://fa.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://au.hahajie.cn

Java: String.format("%03d", 7)
来源：http://iw.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ke.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dr.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qp.nicolike.cn

[E11] 反转字符串
来源：http://ry.szsharing.cn

Py:   s[::-1]
来源：http://um.panjiajie.cn

PHP:  strrev($s);
来源：http://pw.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://bp.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://ce.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fr.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vh.huixinmuqiang.cn

Ruby: s.reverse
来源：http://mh.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kg.newstarts.cn

[E12] 统计某字符出现次数
来源：http://pi.asd995.cn

Py:   s.count("a")
来源：http://vx.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://kt.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://ep.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://kj.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hi.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://mn.9csxet.cn

Ruby: s.count("a")
来源：http://kf.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://tb.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://dw.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://mt.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bs.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fc.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pm.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fo.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qs.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qe.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zg.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://iz.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rh.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bo.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qg.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wy.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pq.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ur.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hh.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://er.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://ih.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mf.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kj.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ru.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://em.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jl.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tp.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://be.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zo.jianghongdianzi.cn

[E16] 数字千分位
来源：http://wl.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://my.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://eh.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ps.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ip.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gt.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yt.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rp.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://zi.lnxyls.cn

[E17] 首字母大写
来源：http://xy.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uz.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://do.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hu.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ji.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sr.shxzskj.cn

Ruby: s.capitalize
来源：http://kv.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ln.521024.cn

[E18] 模板占位符替换
来源：http://yb.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ir.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nh.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qg.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ph.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ww.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://av.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lf.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zo.colortex.cn

[E19] 多行文本按行拆分
来源：http://ox.colortex.cn

Py:   s.splitlines()
来源：http://kf.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cb.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://la.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://dc.shxzukj.cn

Java: s.lines().toList()
来源：http://ia.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://vl.muxihuayi.cn

Ruby: s.lines
来源：http://wz.szsharing.cn

C#:   s.Split('\n')
来源：http://kg.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://jl.asd995.cn

Py:   if not s:
来源：http://sp.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cl.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://te.9csxet.cn

TS:   if (s === "") {}
来源：http://jc.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://ld.shxzukj.cn

Go:   if s == "" {}
来源：http://wt.bjjhwx.cn

Ruby: if s.empty?
来源：http://ms.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://al.hahajie.cn

[E21] 超长截断加省略号
来源：http://jy.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aw.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://te.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ip.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://af.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ge.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://fm.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://re.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sa.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://tj.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wu.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iq.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wg.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uc.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ee.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bp.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://yr.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ks.bookmarksfly.cn

================================================================================
来源：http://dg.nicolike.cn

F. 文件与目录
来源：http://nt.newstarts.cn

================================================================================
来源：http://eh.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://gf.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://em.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ub.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zh.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ks.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jd.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qh.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://gp.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://rk.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://yr.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ft.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jt.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://op.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ck.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mk.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wp.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ub.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fn.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://wb.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://if.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cp.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://go.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vi.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vm.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rg.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://wb.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zp.huixiangedu.cn

[F04] 追加写入文件
来源：http://oy.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vn.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://id.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pi.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zc.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://es.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qh.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ry.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ob.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qk.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://we.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://my.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ax.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pe.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hu.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://vx.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://hq.newstarts.cn

[F06] 删除文件
来源：http://ui.huanxung.cn

Py:   os.remove("a.txt")
来源：http://ic.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://pn.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://br.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hm.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nj.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://hf.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://kr.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://wt.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://fc.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oj.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ei.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zy.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qf.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://if.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jg.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jr.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qc.huanxung.cn

[F08] 遍历目录
来源：http://ww.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ra.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ks.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ju.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://je.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yo.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cz.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://aw.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://kd.newstarts.cn

[F09] 获取文件大小
来源：http://je.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://nb.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://yc.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://ca.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://gf.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jd.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cp.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://so.colortex.cn


<!-- 参考信息 -->