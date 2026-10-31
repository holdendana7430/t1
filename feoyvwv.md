代发 wailian999

Ruby: arr.tally
来源：http://ps.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wf.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://qb.nszjky.cn

Py:   x in arr
来源：http://qh.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://lf.yuexingan06.cn

JS:   arr.includes(x)
来源：http://oh.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://qi.szxytkj.cn

Java: list.contains(x)
来源：http://dv.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://jv.panjiajie.cn

Ruby: arr.include?(x)
来源：http://mw.hnjuh.cn

C#:   list.Contains(x)
来源：http://px.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ru.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ij.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xx.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wd.chemitech.net.cn

TS:   [...arr];
来源：http://da.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://sh.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://or.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://uq.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ub.lnxyls.cn

[D23] reduce 累积计算
来源：http://ro.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ib.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qp.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mx.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gi.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yf.newstarts.cn

Go:   // 手写循环
来源：http://ha.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xz.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iz.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://ol.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wr.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ld.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gb.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yd.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gy.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ip.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oq.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xk.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://ua.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lr.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ym.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rd.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sa.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wy.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cr.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cx.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tb.huixiangedu.cn

[D26] 数组转字符串
来源：http://zn.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://bv.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://ui.shtwfgs.cn

JS:   arr.join(", ")
来源：http://dd.panjiajie.cn

TS:   arr.join(", ")
来源：http://js.shxzukj.cn

Java: String.join(", ", list)
来源：http://hs.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bc.asd995.cn

Ruby: arr.join(", ")
来源：http://vj.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://pz.muxihuayi.cn

================================================================================
来源：http://il.bjjhwx.cn

E. 字符串处理
来源：http://el.yuntaijiaju.cn

================================================================================
来源：http://pw.nicolike.cn

[E01] 拼接字符串
来源：http://zn.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gj.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qa.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sv.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uu.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ol.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ml.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xc.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kr.muxihuayi.cn

[E02] 重复字符串
来源：http://sx.newstarts.cn

Py:   "ab" * 3
来源：http://iq.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://pl.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://yg.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://cd.szsharing.cn

Java: "ab".repeat(3)
来源：http://pc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://yx.haigaiapp.cn

Ruby: "ab" * 3
来源：http://ic.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ca.haigaiapp.cn

[E03] 截取子串
来源：http://gm.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lz.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ca.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://te.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://xb.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://bb.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mo.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fn.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://rc.wgjwhj.cn

[E04] 查找子串位置
来源：http://km.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://aq.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://wm.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vs.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://jt.lnxyls.cn

Java: s.indexOf("x")
来源：http://ds.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://uy.shxzukj.cn

Ruby: s.index("x")
来源：http://qa.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://xj.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vu.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kp.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kl.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vo.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iu.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ai.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fe.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hr.muxihuayi.cn

[E06] 替换子串
来源：http://uy.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yl.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://on.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ru.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://op.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fr.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cx.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dj.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://tz.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://xi.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xy.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gg.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qi.asd995.cn

TS:   s.split(",")
来源：http://wz.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lf.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aq.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://yq.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ay.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://yu.colortex.cn

Py:   ",".join(items)
来源：http://lz.9csxet.cn

PHP:  implode(",", $items);
来源：http://hv.yuexingan06.cn

JS:   items.join(",")
来源：http://qv.shtwfgs.cn

TS:   items.join(",")
来源：http://op.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://xf.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://kd.newstarts.cn

Ruby: items.join(",")
来源：http://jk.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://sc.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://uf.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zz.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cq.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://fh.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ak.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://un.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ow.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ch.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://su.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://eq.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bw.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ky.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://kr.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://up.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://er.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rb.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fm.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bh.wgjwhj.cn

[E11] 反转字符串
来源：http://rh.muxihuayi.cn

Py:   s[::-1]
来源：http://bn.shtwfgs.cn

PHP:  strrev($s);
来源：http://zf.asd995.cn

JS:   [...s].reverse().join("")
来源：http://jn.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://az.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ej.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ok.szxytkj.cn

Ruby: s.reverse
来源：http://sb.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ym.asd995.cn

[E12] 统计某字符出现次数
来源：http://mj.shxzukj.cn

Py:   s.count("a")
来源：http://hd.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ys.nszjky.cn

JS:   s.split("a").length - 1
来源：http://sl.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://fm.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hg.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://rh.521024.cn

Ruby: s.count("a")
来源：http://iu.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://se.jctech888.com.cn

[E13] 逐字符遍历
来源：http://rb.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://vz.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zb.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gi.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kb.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tw.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://du.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rg.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bs.hahajie.cn

[E14] URL 编码与 Base64
来源：http://uz.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pa.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zu.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hd.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pl.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rm.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xm.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sz.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vh.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://uq.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://il.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gl.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ek.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ha.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ec.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://td.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dz.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uv.yuexingan06.cn

[E16] 数字千分位
来源：http://rz.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://sn.asd995.cn

PHP:  number_format(1234567);
来源：http://mf.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dj.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ba.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://op.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ru.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gn.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://if.newstarts.cn

[E17] 首字母大写
来源：http://jx.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ka.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ft.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qz.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://md.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dr.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ej.shxzskj.cn

Ruby: s.capitalize
来源：http://bo.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nz.asd995.cn

[E18] 模板占位符替换
来源：http://rt.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fp.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ur.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://md.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://co.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cz.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pf.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nr.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jv.newstarts.cn

[E19] 多行文本按行拆分
来源：http://lg.521024.cn

Py:   s.splitlines()
来源：http://va.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lz.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://dn.521024.cn

TS:   s.split(/\r?\n/)
来源：http://go.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://va.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://qj.521024.cn

Ruby: s.lines
来源：http://fp.colortex.cn

C#:   s.Split('\n')
来源：http://ez.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://sq.yuexingan06.cn

Py:   if not s:
来源：http://bn.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mu.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hn.lnxyls.cn

TS:   if (s === "") {}
来源：http://zz.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://dj.szsharing.cn

Go:   if s == "" {}
来源：http://dw.huanxung.cn

Ruby: if s.empty?
来源：http://vo.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hj.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://kp.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zm.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nj.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cg.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cd.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://up.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jq.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rk.9csxet.cn

[E22] 字节长度与字符长度
来源：http://zd.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://me.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fe.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zm.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zu.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://im.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ct.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://jz.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fu.gzmigu.cn

================================================================================
来源：http://ij.lnxyls.cn

F. 文件与目录
来源：http://zj.panjiajie.cn

================================================================================
来源：http://hb.9csxet.cn

[F01] 读取整个文件
来源：http://hu.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zy.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://gc.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hs.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zu.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tt.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://li.szsharing.cn

Ruby: File.read("a.txt")
来源：http://dr.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://mh.chemitech.net.cn

[F02] 逐行读取文件
来源：http://el.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://re.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dr.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rb.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kb.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://js.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uy.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gq.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://ln.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://se.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ad.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uq.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://an.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://by.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://jc.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ub.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://iy.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qt.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fs.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xq.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xj.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vn.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zu.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pf.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://df.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bc.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://cj.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://mi.lnxyls.cn


<!-- 参考信息 -->