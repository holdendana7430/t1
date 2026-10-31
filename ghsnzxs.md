代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tm.bjjhwx.cn

Go:   // 手写双层循环
来源：http://sq.newstarts.cn

Ruby: nested.flatten
来源：http://vw.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wv.jianghongdianzi.cn

[D19] 按字段分组
来源：http://hd.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hc.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://el.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rr.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sr.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://at.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://et.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ic.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ld.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://vk.huixiangedu.cn

Py:   Counter(arr)
来源：http://uk.colortex.cn

PHP:  array_count_values($arr);
来源：http://tm.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sj.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kr.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kk.hahajie.cn

Go:   // 手写 map[T]int
来源：http://pe.szsharing.cn

Ruby: arr.tally
来源：http://gu.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iz.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://xt.jianghongdianzi.cn

Py:   x in arr
来源：http://ri.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://vj.colortex.cn

JS:   arr.includes(x)
来源：http://dn.shtwfgs.cn

TS:   arr.includes(x)
来源：http://cx.nicolike.cn

Java: list.contains(x)
来源：http://hi.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://jo.nicolike.cn

Ruby: arr.include?(x)
来源：http://mc.gzmigu.cn

C#:   list.Contains(x)
来源：http://jc.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://qv.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ow.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mt.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ki.wgjwhj.cn

TS:   [...arr];
来源：http://mz.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ar.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tb.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://rr.yuexingan06.cn

C#:   new List<int>(list);
来源：http://pm.hahajie.cn

[D23] reduce 累积计算
来源：http://da.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://do.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yl.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jl.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sp.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fz.hnjuh.cn

Go:   // 手写循环
来源：http://ww.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qq.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cd.521024.cn

[D24] 字典 / Map 基本操作
来源：http://wn.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jo.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hd.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bt.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qe.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sy.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qk.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ev.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://hy.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kr.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ua.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xd.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sl.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ws.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ra.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uv.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ru.521024.cn

[D26] 数组转字符串
来源：http://op.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ct.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://gw.huixiangedu.cn

JS:   arr.join(", ")
来源：http://kq.huanxung.cn

TS:   arr.join(", ")
来源：http://bo.lnxyls.cn

Java: String.join(", ", list)
来源：http://fk.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://uy.nicolike.cn

Ruby: arr.join(", ")
来源：http://cq.szsharing.cn

C#:   string.Join(", ", list)
来源：http://sx.newstarts.cn

================================================================================
来源：http://ti.hnjuh.cn

E. 字符串处理
来源：http://hw.9csxet.cn

================================================================================
来源：http://zk.muxihuayi.cn

[E01] 拼接字符串
来源：http://vq.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sb.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sx.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bo.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://df.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tt.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vi.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gh.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gi.wgjwhj.cn

[E02] 重复字符串
来源：http://fz.gzmigu.cn

Py:   "ab" * 3
来源：http://un.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://au.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://iq.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://bc.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://kg.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://yj.szxytkj.cn

Ruby: "ab" * 3
来源：http://ll.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cr.hahajie.cn

[E03] 截取子串
来源：http://cj.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ev.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lj.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eq.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://gf.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://wx.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://na.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dy.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://hf.gzmigu.cn

[E04] 查找子串位置
来源：http://qz.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://po.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://zq.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zs.nicolike.cn

TS:   s.indexOf("x")
来源：http://tt.9csxet.cn

Java: s.indexOf("x")
来源：http://zi.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://di.shxzskj.cn

Ruby: s.index("x")
来源：http://de.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://tu.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fw.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oq.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fk.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bs.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jw.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://se.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://it.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bf.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ab.huanxung.cn

[E06] 替换子串
来源：http://xe.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xm.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://yx.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://kh.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xw.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://au.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wl.colortex.cn

C#:   s.Replace("a", "b")
来源：http://yc.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://zc.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wc.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wc.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ge.nszjky.cn

TS:   s.split(",")
来源：http://rd.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://av.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://me.521024.cn

Ruby: s.split(",");  s.split
来源：http://ax.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ek.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://du.521024.cn

Py:   ",".join(items)
来源：http://wa.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://xk.muxihuayi.cn

JS:   items.join(",")
来源：http://ac.bjjhwx.cn

TS:   items.join(",")
来源：http://gq.colortex.cn

Java: String.join(",", items)
来源：http://ya.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://xe.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://vr.9csxet.cn

C#:   string.Join(",", items)
来源：http://ry.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://ec.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tl.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uu.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://ka.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ya.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://so.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bu.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dy.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uv.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://re.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vt.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fr.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://pu.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://au.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://hg.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nr.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rh.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hi.chemitech.net.cn

[E11] 反转字符串
来源：http://sc.bookmarksfly.cn

Py:   s[::-1]
来源：http://xy.szsharing.cn

PHP:  strrev($s);
来源：http://og.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://ze.colortex.cn

TS:   [...s].reverse().join("")
来源：http://uk.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qt.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wg.lnxyls.cn

Ruby: s.reverse
来源：http://yr.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nu.nicolike.cn

[E12] 统计某字符出现次数
来源：http://zp.yuntaijiaju.cn

Py:   s.count("a")
来源：http://sq.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://qs.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://ol.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://in.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lf.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://tz.nszjky.cn

Ruby: s.count("a")
来源：http://jc.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://ds.colortex.cn

[E13] 逐字符遍历
来源：http://iu.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://yl.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gk.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ym.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zo.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wn.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ii.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ug.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qc.521024.cn

[E14] URL 编码与 Base64
来源：http://am.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://di.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gb.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rq.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bu.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tk.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cx.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://se.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ks.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://gn.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jo.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ja.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ij.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bx.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jr.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ky.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jh.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vy.bookmarksfly.cn

[E16] 数字千分位
来源：http://df.szsharing.cn

Py:   f"{1234567:,}"
来源：http://bm.gzmigu.cn

PHP:  number_format(1234567);
来源：http://bj.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ay.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iu.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mg.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fp.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ad.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://fn.szxytkj.cn

[E17] 首字母大写
来源：http://ex.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wo.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rd.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bd.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zv.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rs.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mr.shxzskj.cn

Ruby: s.capitalize
来源：http://pr.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vl.asd995.cn

[E18] 模板占位符替换
来源：http://ke.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kb.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vk.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uh.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dh.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yd.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ym.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sx.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ld.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://tv.hnjuh.cn

Py:   s.splitlines()
来源：http://if.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aj.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://xf.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://cb.haigaiapp.cn

Java: s.lines().toList()
来源：http://vt.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ax.bjjhwx.cn

Ruby: s.lines
来源：http://uj.szsharing.cn

C#:   s.Split('\n')
来源：http://nu.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://ma.hahajie.cn

Py:   if not s:
来源：http://km.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ud.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ru.nicolike.cn

TS:   if (s === "") {}
来源：http://ju.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://bg.asd995.cn

Go:   if s == "" {}
来源：http://fe.shxzukj.cn

Ruby: if s.empty?
来源：http://nj.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.hnjuh.cn

[E21] 超长截断加省略号
来源：http://ug.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sx.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cs.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tv.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dc.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cb.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://yb.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dw.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lu.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://lm.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tg.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ec.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jo.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ec.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sm.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ek.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://mm.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ys.jianghongdianzi.cn

================================================================================
来源：http://iy.chemitech.net.cn

F. 文件与目录
来源：http://zq.nicolike.cn

================================================================================
来源：http://fb.jctech888.com.cn

[F01] 读取整个文件
来源：http://gm.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ke.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://xw.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fb.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://if.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://he.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qx.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://lp.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://ph.szxytkj.cn

[F02] 逐行读取文件
来源：http://ew.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gs.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vp.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wp.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sl.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zj.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mc.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yd.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://kd.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hy.gzmigu.cn


<!-- 参考信息 -->