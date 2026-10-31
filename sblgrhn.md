代发 wailian999

[D23] reduce 累积计算
来源：http://ad.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://um.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ky.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oy.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mf.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uz.huixinmuqiang.cn

Go:   // 手写循环
来源：http://yx.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vp.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qm.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://lm.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sp.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nx.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jo.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rz.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ka.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rp.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://by.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ad.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://cx.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pa.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uy.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gp.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zu.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tl.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zo.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hf.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tj.wgjwhj.cn

[D26] 数组转字符串
来源：http://zw.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://xc.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://oj.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://ws.szxytkj.cn

TS:   arr.join(", ")
来源：http://jr.nszjky.cn

Java: String.join(", ", list)
来源：http://wc.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://ky.newstarts.cn

Ruby: arr.join(", ")
来源：http://sd.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ae.haigaiapp.cn

================================================================================
来源：http://le.jctech888.com.cn

E. 字符串处理
来源：http://wg.wgjwhj.cn

================================================================================
来源：http://rh.lnxyls.cn

[E01] 拼接字符串
来源：http://bw.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kv.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://en.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ep.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rq.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tx.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gm.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xj.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bi.huanxung.cn

[E02] 重复字符串
来源：http://lp.szxytkj.cn

Py:   "ab" * 3
来源：http://wm.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://xn.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ju.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://tb.hnjuh.cn

Java: "ab".repeat(3)
来源：http://jz.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://xm.huanxung.cn

Ruby: "ab" * 3
来源：http://rg.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gw.nicolike.cn

[E03] 截取子串
来源：http://uz.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xx.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://or.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mz.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://zq.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://qn.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mw.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ox.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ot.gzmigu.cn

[E04] 查找子串位置
来源：http://uq.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://sg.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://sf.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ye.nszjky.cn

TS:   s.indexOf("x")
来源：http://uk.asd995.cn

Java: s.indexOf("x")
来源：http://tt.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ll.szxytkj.cn

Ruby: s.index("x")
来源：http://xb.huanxung.cn

C#:   s.IndexOf("x")
来源：http://jb.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iq.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oo.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qx.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xm.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ga.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://td.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gj.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ul.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zh.asd995.cn

[E06] 替换子串
来源：http://mn.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pm.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://oh.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oq.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://yh.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://md.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yi.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ul.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://mc.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://lq.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xx.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ew.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hg.shxzskj.cn

TS:   s.split(",")
来源：http://de.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hs.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mf.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://mu.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fj.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ou.muxihuayi.cn

Py:   ",".join(items)
来源：http://bn.gzmigu.cn

PHP:  implode(",", $items);
来源：http://so.wgjwhj.cn

JS:   items.join(",")
来源：http://jc.huixiangedu.cn

TS:   items.join(",")
来源：http://xc.521024.cn

Java: String.join(",", items)
来源：http://uo.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://df.huanxung.cn

Ruby: items.join(",")
来源：http://mb.shxzskj.cn

C#:   string.Join(",", items)
来源：http://kt.nszjky.cn

[E09] 去除所有空白字符
来源：http://fy.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ir.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kl.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://tc.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://rh.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://ei.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dn.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sz.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mi.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://gl.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gn.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ik.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://rz.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://ug.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://ed.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yi.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nq.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zx.gzmigu.cn

[E11] 反转字符串
来源：http://io.colortex.cn

Py:   s[::-1]
来源：http://mq.nszjky.cn

PHP:  strrev($s);
来源：http://hi.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://qg.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://ie.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gf.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xj.yuntaijiaju.cn

Ruby: s.reverse
来源：http://fx.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ig.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://tx.szxytkj.cn

Py:   s.count("a")
来源：http://vz.asd995.cn

PHP:  substr_count($s, "a");
来源：http://tq.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://er.nicolike.cn

TS:   s.split("a").length - 1
来源：http://dc.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yh.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://do.nicolike.cn

Ruby: s.count("a")
来源：http://gc.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://ez.panjiajie.cn

[E13] 逐字符遍历
来源：http://pc.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://kn.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dt.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qu.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dj.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://og.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dv.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vc.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nu.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://tw.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fg.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://te.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qn.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gr.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://di.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://de.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gc.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://op.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://hc.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wr.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vs.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ba.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aw.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nl.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://le.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qz.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wy.szsharing.cn

[E16] 数字千分位
来源：http://oi.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://mk.9csxet.cn

PHP:  number_format(1234567);
来源：http://ar.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cv.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yu.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ao.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://re.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tw.521024.cn

C#:   1234567.ToString("N0")
来源：http://kj.gzmigu.cn

[E17] 首字母大写
来源：http://ux.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ke.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kt.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://it.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eo.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bp.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://uy.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dr.szxytkj.cn

[E18] 模板占位符替换
来源：http://qw.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ty.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ku.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://un.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sg.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ij.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yg.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ju.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://xm.9csxet.cn

Py:   s.splitlines()
来源：http://we.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hq.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://yv.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://ce.panjiajie.cn

Java: s.lines().toList()
来源：http://vt.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://md.chemitech.net.cn

Ruby: s.lines
来源：http://tt.lnxyls.cn

C#:   s.Split('\n')
来源：http://tz.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://mn.chemitech.net.cn

Py:   if not s:
来源：http://bu.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wr.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lm.haigaiapp.cn

TS:   if (s === "") {}
来源：http://vi.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://kz.chemitech.net.cn

Go:   if s == "" {}
来源：http://cv.panjiajie.cn

Ruby: if s.empty?
来源：http://ut.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rg.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://lb.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ab.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pu.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hi.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nv.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zk.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://yg.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ea.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pg.521024.cn

[E22] 字节长度与字符长度
来源：http://br.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yl.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uy.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bz.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mm.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://up.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rj.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://ia.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cl.asd995.cn

================================================================================
来源：http://ft.jianghongdianzi.cn

F. 文件与目录
来源：http://yn.gzmigu.cn

================================================================================
来源：http://gd.newstarts.cn

[F01] 读取整个文件
来源：http://ba.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pz.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://hf.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xk.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hb.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uc.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ql.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://qf.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://zl.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://dj.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yj.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ol.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mm.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fv.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kq.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://as.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ty.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rj.asd995.cn

[F03] 写入文件（覆盖）
来源：http://ef.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bp.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ey.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://of.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nq.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tl.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ij.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://oj.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lw.newstarts.cn

[F04] 追加写入文件
来源：http://kj.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://we.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bd.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ff.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pd.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eu.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ab.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nq.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xh.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://cz.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nh.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://sb.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://jk.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://wp.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aj.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lx.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://zf.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://kc.muxihuayi.cn

[F06] 删除文件
来源：http://th.9csxet.cn

Py:   os.remove("a.txt")
来源：http://ov.szsharing.cn

PHP:  unlink("a.txt");
来源：http://yd.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lm.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fb.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wd.521024.cn

Go:   os.Remove("a.txt")
来源：http://uc.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://ac.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://yg.nszjky.cn

[F07] 创建目录（含多级）
来源：http://hs.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bz.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tq.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fy.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sm.shxzukj.cn


<!-- 参考信息 -->