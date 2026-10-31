代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ru.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ai.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ep.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qo.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://di.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sr.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://pj.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nt.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://op.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ad.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dn.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qv.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ft.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gq.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ua.panjiajie.cn

[D26] 数组转字符串
来源：http://fm.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://uc.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://ir.szsharing.cn

JS:   arr.join(", ")
来源：http://ec.huanxung.cn

TS:   arr.join(", ")
来源：http://vq.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://yj.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://ou.asd995.cn

Ruby: arr.join(", ")
来源：http://em.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ui.hnjuh.cn

================================================================================
来源：http://on.muxihuayi.cn

E. 字符串处理
来源：http://qi.panjiajie.cn

================================================================================
来源：http://jq.newstarts.cn

[E01] 拼接字符串
来源：http://td.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xn.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://up.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://di.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vc.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tb.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://va.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jn.muxihuayi.cn

[E02] 重复字符串
来源：http://wl.521024.cn

Py:   "ab" * 3
来源：http://dp.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://rl.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://zq.szsharing.cn

TS:   "ab".repeat(3)
来源：http://fx.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://qc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://ql.shxzskj.cn

Ruby: "ab" * 3
来源：http://lt.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zh.yuntaijiaju.cn

[E03] 截取子串
来源：http://tt.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bx.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uo.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vm.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://di.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ww.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vf.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kw.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://bl.lnxyls.cn

[E04] 查找子串位置
来源：http://nv.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://tr.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ir.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gw.nszjky.cn

TS:   s.indexOf("x")
来源：http://ju.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://iu.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://ah.lnxyls.cn

Ruby: s.index("x")
来源：http://jr.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://rh.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ik.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://es.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mf.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://op.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tu.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hu.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nr.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cs.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://md.bjjhwx.cn

[E06] 替换子串
来源：http://tu.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sc.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ab.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gv.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://vo.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zq.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yu.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ea.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://xm.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://hr.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pl.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zk.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qt.haigaiapp.cn

TS:   s.split(",")
来源：http://pg.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://it.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pj.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://ls.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bv.colortex.cn

[E08] 数组按分隔符合并
来源：http://jj.gzmigu.cn

Py:   ",".join(items)
来源：http://tc.asd995.cn

PHP:  implode(",", $items);
来源：http://lm.wgjwhj.cn

JS:   items.join(",")
来源：http://tf.szsharing.cn

TS:   items.join(",")
来源：http://wh.panjiajie.cn

Java: String.join(",", items)
来源：http://gt.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://jc.yuexingan06.cn

Ruby: items.join(",")
来源：http://gx.shxzskj.cn

C#:   string.Join(",", items)
来源：http://nl.521024.cn

[E09] 去除所有空白字符
来源：http://zc.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rd.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ej.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://la.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://qa.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://gd.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dg.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gm.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fz.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://rk.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://no.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://si.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://ce.521024.cn

TS:   "7".padStart(3, "0")
来源：http://gt.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://qx.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lk.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cl.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ew.chemitech.net.cn

[E11] 反转字符串
来源：http://iu.nszjky.cn

Py:   s[::-1]
来源：http://kd.asd995.cn

PHP:  strrev($s);
来源：http://dx.asd995.cn

JS:   [...s].reverse().join("")
来源：http://qj.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://kr.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kd.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iv.huixinmuqiang.cn

Ruby: s.reverse
来源：http://xg.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://un.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://cn.asd995.cn

Py:   s.count("a")
来源：http://xq.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ki.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://mc.szsharing.cn

TS:   s.split("a").length - 1
来源：http://ix.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rn.asd995.cn

Go:   strings.Count(s, "a")
来源：http://jm.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://fb.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://mm.muxihuayi.cn

[E13] 逐字符遍历
来源：http://dw.asd995.cn

Py:   for ch in s: print(ch)
来源：http://cx.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bi.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eu.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sv.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kn.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pp.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ps.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xy.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://gi.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zf.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mk.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sx.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://el.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oa.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ez.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ij.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yq.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://qc.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xi.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dl.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pz.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vs.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dc.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uo.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tx.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wl.hnjuh.cn

[E16] 数字千分位
来源：http://dd.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://bd.521024.cn

PHP:  number_format(1234567);
来源：http://tp.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ba.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gj.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ub.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qj.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wy.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://le.muxihuayi.cn

[E17] 首字母大写
来源：http://nj.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yo.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qm.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://be.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jv.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tn.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dn.szsharing.cn

Ruby: s.capitalize
来源：http://yp.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ih.muxihuayi.cn

[E18] 模板占位符替换
来源：http://oh.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sv.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pn.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ch.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qz.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yv.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lm.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hy.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tk.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://au.asd995.cn

Py:   s.splitlines()
来源：http://fk.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mf.521024.cn

JS:   s.split(/\r?\n/)
来源：http://cd.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://dt.shxzukj.cn

Java: s.lines().toList()
来源：http://of.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://gd.lnxyls.cn

Ruby: s.lines
来源：http://gh.nszjky.cn

C#:   s.Split('\n')
来源：http://rr.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://kt.newstarts.cn

Py:   if not s:
来源：http://eb.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ta.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://of.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://vn.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ul.bookmarksfly.cn

Go:   if s == "" {}
来源：http://wx.huanxung.cn

Ruby: if s.empty?
来源：http://ll.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ua.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://du.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uf.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oq.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tf.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ev.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://og.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://up.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rq.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mk.521024.cn

[E22] 字节长度与字符长度
来源：http://wn.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vs.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vp.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ao.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kt.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zu.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://go.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://nw.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wf.szxytkj.cn

================================================================================
来源：http://vi.9csxet.cn

F. 文件与目录
来源：http://bv.wgjwhj.cn

================================================================================
来源：http://sr.haigaiapp.cn

[F01] 读取整个文件
来源：http://mm.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ha.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://jl.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zi.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qu.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hm.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uy.huanxung.cn

Ruby: File.read("a.txt")
来源：http://bo.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://os.yuexingan06.cn

[F02] 逐行读取文件
来源：http://ac.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xm.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yk.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ao.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lz.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sb.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hq.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ve.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kl.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://xt.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gn.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bc.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yg.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://se.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ek.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lb.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ij.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rd.nicolike.cn

[F04] 追加写入文件
来源：http://ew.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fj.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fr.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rz.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rw.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ah.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ab.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://na.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mo.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://xh.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://we.colortex.cn

PHP:  file_exists("a.txt");
来源：http://lm.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://bt.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://iz.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xt.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nq.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://as.asd995.cn

C#:   File.Exists("a.txt")
来源：http://jb.szsharing.cn

[F06] 删除文件
来源：http://tf.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://yo.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://fg.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://le.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wh.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ug.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://rq.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://cw.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://pq.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://is.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cy.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uu.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ue.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ja.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yv.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wh.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nl.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.lnxyls.cn

[F08] 遍历目录
来源：http://xw.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ay.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fc.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://fx.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://gw.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wv.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ce.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://zb.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://vi.chemitech.net.cn


<!-- 参考信息 -->