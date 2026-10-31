代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://va.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mp.huixinmuqiang.cn

Go:   // 手写循环
来源：http://gg.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vp.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://ii.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qs.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fs.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rc.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rs.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vq.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fu.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mn.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vj.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ms.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jm.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yk.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wi.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lu.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rg.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qe.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aa.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ap.huanxung.cn

[D26] 数组转字符串
来源：http://kn.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://sw.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://pp.huanxung.cn

JS:   arr.join(", ")
来源：http://ec.shxzskj.cn

TS:   arr.join(", ")
来源：http://hr.newstarts.cn

Java: String.join(", ", list)
来源：http://bq.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://lx.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://lo.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://cj.huanxung.cn

================================================================================
来源：http://xi.szsharing.cn

E. 字符串处理
来源：http://at.asd995.cn

================================================================================
来源：http://nh.muxihuayi.cn

[E01] 拼接字符串
来源：http://zh.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xf.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tx.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gh.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lc.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nn.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zi.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mc.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://us.521024.cn

[E02] 重复字符串
来源：http://hz.huanxung.cn

Py:   "ab" * 3
来源：http://qc.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://xu.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ev.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://yy.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://ft.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ay.9csxet.cn

Ruby: "ab" * 3
来源：http://oe.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ae.szxytkj.cn

[E03] 截取子串
来源：http://ib.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nc.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uy.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ai.newstarts.cn

TS:   s.slice(1, 4)
来源：http://lr.shxzskj.cn

Java: s.substring(1, 4)
来源：http://qm.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tb.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://su.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://pl.asd995.cn

[E04] 查找子串位置
来源：http://ny.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.hahajie.cn

PHP:  strpos($s, "x");
来源：http://pa.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yg.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://wq.szsharing.cn

Java: s.indexOf("x")
来源：http://nd.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ig.hahajie.cn

Ruby: s.index("x")
来源：http://rs.521024.cn

C#:   s.IndexOf("x")
来源：http://fj.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vu.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gu.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zw.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qd.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://em.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cn.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sq.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://um.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xd.shxzukj.cn

[E06] 替换子串
来源：http://ci.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ch.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://vo.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://br.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://su.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zb.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jx.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ah.colortex.cn

C#:   s.Replace("a", "b")
来源：http://fo.hnjuh.cn

[E07] 按分隔符拆分
来源：http://hs.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://is.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hb.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ib.521024.cn

TS:   s.split(",")
来源：http://jy.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qu.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cp.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://vs.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yd.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://jy.shxzukj.cn

Py:   ",".join(items)
来源：http://ca.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://hn.bookmarksfly.cn

JS:   items.join(",")
来源：http://ek.panjiajie.cn

TS:   items.join(",")
来源：http://px.yuexingan06.cn

Java: String.join(",", items)
来源：http://uj.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://rl.panjiajie.cn

Ruby: items.join(",")
来源：http://jk.9csxet.cn

C#:   string.Join(",", items)
来源：http://jr.huanxung.cn

[E09] 去除所有空白字符
来源：http://fu.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ff.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gc.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://qq.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://ub.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://kq.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nu.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wq.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lf.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://of.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eu.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iz.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://sc.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://zq.nicolike.cn

Java: String.format("%03d", 7)
来源：http://px.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nf.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ds.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ii.huixiangedu.cn

[E11] 反转字符串
来源：http://qs.nszjky.cn

Py:   s[::-1]
来源：http://gg.newstarts.cn

PHP:  strrev($s);
来源：http://oj.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://to.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://fs.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pz.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oj.bjjhwx.cn

Ruby: s.reverse
来源：http://tn.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xf.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://ym.szxytkj.cn

Py:   s.count("a")
来源：http://cv.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://nn.newstarts.cn

JS:   s.split("a").length - 1
来源：http://hd.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://iv.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yr.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://em.shxzukj.cn

Ruby: s.count("a")
来源：http://vm.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://bq.hnjuh.cn

[E13] 逐字符遍历
来源：http://io.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://hr.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://og.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xi.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ii.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xv.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rg.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zh.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fh.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://pp.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zr.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qv.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xl.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oy.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tw.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wu.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fp.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ff.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://he.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kj.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://in.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mm.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://no.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vm.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pw.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://li.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wp.bjjhwx.cn

[E16] 数字千分位
来源：http://yd.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ze.nicolike.cn

PHP:  number_format(1234567);
来源：http://cw.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rb.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jt.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ic.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ab.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ep.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://un.521024.cn

[E17] 首字母大写
来源：http://fl.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xf.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lt.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oe.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bb.huanxung.cn

Ruby: s.capitalize
来源：http://ei.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ek.szsharing.cn

[E18] 模板占位符替换
来源：http://ce.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qa.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://id.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jh.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://st.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ll.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ue.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yg.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wb.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://uu.huixiangedu.cn

Py:   s.splitlines()
来源：http://gw.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fg.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://yl.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://vy.shtwfgs.cn

Java: s.lines().toList()
来源：http://lz.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://lw.shxzukj.cn

Ruby: s.lines
来源：http://oo.521024.cn

C#:   s.Split('\n')
来源：http://xn.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://vm.jctech888.com.cn

Py:   if not s:
来源：http://jc.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://of.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://we.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ec.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ox.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://tn.nszjky.cn

Ruby: if s.empty?
来源：http://gq.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pw.nszjky.cn

[E21] 超长截断加省略号
来源：http://qb.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lc.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lv.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gp.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xb.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ww.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://bw.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xd.9csxet.cn

[E22] 字节长度与字符长度
来源：http://hq.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eu.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iq.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pk.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lb.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hp.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://et.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ry.521024.cn

================================================================================
来源：http://ve.shxzskj.cn

F. 文件与目录
来源：http://rl.huixinmuqiang.cn

================================================================================
来源：http://ij.szxytkj.cn

[F01] 读取整个文件
来源：http://sq.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ua.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://vk.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bo.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xi.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lj.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eq.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://cy.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://ny.asd995.cn

[F02] 逐行读取文件
来源：http://tz.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jy.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xp.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bx.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cw.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ws.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://of.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xd.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ws.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://mn.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://or.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qn.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://au.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ei.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lk.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iw.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://id.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://br.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://yd.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sw.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gz.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://th.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://un.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zm.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://th.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mo.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bl.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://ey.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nz.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://fn.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ed.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://qc.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oy.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ol.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://mu.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://fz.newstarts.cn

[F06] 删除文件
来源：http://hb.szsharing.cn

Py:   os.remove("a.txt")
来源：http://od.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://cs.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jm.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gu.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xj.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://zz.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://sl.521024.cn

C#:   File.Delete("a.txt");
来源：http://qr.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://za.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tc.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fh.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ig.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mm.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xe.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zs.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mq.szsharing.cn

[F08] 遍历目录
来源：http://jh.panjiajie.cn


<!-- 参考信息 -->