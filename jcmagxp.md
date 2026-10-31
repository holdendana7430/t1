代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ka.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://gt.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fz.bookmarksfly.cn

TS:   nested.flat();
来源：http://cj.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eu.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://wf.shxzskj.cn

Ruby: nested.flatten
来源：http://pk.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lq.muxihuayi.cn

[D19] 按字段分组
来源：http://jn.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ih.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://js.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yw.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cz.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ix.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://ta.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ub.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gb.521024.cn

[D20] 统计每个元素出现次数
来源：http://mc.haigaiapp.cn

Py:   Counter(arr)
来源：http://dm.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ge.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vf.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rl.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jn.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://mi.asd995.cn

Ruby: arr.tally
来源：http://ji.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mf.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://aq.shtwfgs.cn

Py:   x in arr
来源：http://ff.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://tp.gzmigu.cn

JS:   arr.includes(x)
来源：http://uy.huixiangedu.cn

TS:   arr.includes(x)
来源：http://yu.haigaiapp.cn

Java: list.contains(x)
来源：http://tc.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://xf.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://qg.szsharing.cn

C#:   list.Contains(x)
来源：http://jy.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://uq.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://da.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ee.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ig.huixiangedu.cn

TS:   [...arr];
来源：http://lj.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://qj.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cm.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://if.9csxet.cn

C#:   new List<int>(list);
来源：http://un.szsharing.cn

[D23] reduce 累积计算
来源：http://vo.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fk.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vx.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zh.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mp.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fo.yuexingan06.cn

Go:   // 手写循环
来源：http://ye.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lz.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uw.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://gw.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ni.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ar.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zf.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zu.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pg.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://td.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jw.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zh.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://wh.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pd.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cq.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hu.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hb.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vx.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fi.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ky.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://to.colortex.cn

[D26] 数组转字符串
来源：http://gj.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://il.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://gy.nszjky.cn

JS:   arr.join(", ")
来源：http://mk.newstarts.cn

TS:   arr.join(", ")
来源：http://ce.nicolike.cn

Java: String.join(", ", list)
来源：http://li.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://oq.lnxyls.cn

Ruby: arr.join(", ")
来源：http://pd.asd995.cn

C#:   string.Join(", ", list)
来源：http://ks.muxihuayi.cn

================================================================================
来源：http://rl.yuexingan06.cn

E. 字符串处理
来源：http://et.shxzskj.cn

================================================================================
来源：http://cr.hnjuh.cn

[E01] 拼接字符串
来源：http://sw.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nz.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xq.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nr.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yd.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ew.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jh.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rx.lnxyls.cn

[E02] 重复字符串
来源：http://ud.hnjuh.cn

Py:   "ab" * 3
来源：http://ud.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://hh.nicolike.cn

JS:   "ab".repeat(3)
来源：http://sh.521024.cn

TS:   "ab".repeat(3)
来源：http://pj.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://sk.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://vl.colortex.cn

Ruby: "ab" * 3
来源：http://qk.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nm.jianghongdianzi.cn

[E03] 截取子串
来源：http://zk.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gw.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wk.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hu.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://xw.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://cx.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://em.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sk.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://cj.hahajie.cn

[E04] 查找子串位置
来源：http://ar.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://ck.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://df.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://em.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://hc.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ap.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://bt.shxzskj.cn

Ruby: s.index("x")
来源：http://be.9csxet.cn

C#:   s.IndexOf("x")
来源：http://vc.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://se.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rp.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sf.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://th.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://om.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fb.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zr.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sw.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://as.lnxyls.cn

[E06] 替换子串
来源：http://yw.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jp.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://wp.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://df.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ei.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ie.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ar.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bb.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://qd.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://de.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ms.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://um.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oe.huanxung.cn

TS:   s.split(",")
来源：http://qp.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ab.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nz.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://ty.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gh.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://xn.huixiangedu.cn

Py:   ",".join(items)
来源：http://gu.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://wq.wgjwhj.cn

JS:   items.join(",")
来源：http://ib.jianghongdianzi.cn

TS:   items.join(",")
来源：http://po.wgjwhj.cn

Java: String.join(",", items)
来源：http://wn.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ml.hnjuh.cn

Ruby: items.join(",")
来源：http://ay.newstarts.cn

C#:   string.Join(",", items)
来源：http://qw.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://ms.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ww.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ft.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ry.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ri.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://ap.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rs.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ep.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sb.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://yq.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lb.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sr.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://ys.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://ej.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://dn.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pj.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qi.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ds.yuexingan06.cn

[E11] 反转字符串
来源：http://bf.huixinmuqiang.cn

Py:   s[::-1]
来源：http://zp.panjiajie.cn

PHP:  strrev($s);
来源：http://sf.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://ow.asd995.cn

TS:   [...s].reverse().join("")
来源：http://qn.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tf.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hw.jctech888.com.cn

Ruby: s.reverse
来源：http://kg.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wj.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://ow.huanxung.cn

Py:   s.count("a")
来源：http://np.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://tk.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ep.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ea.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://da.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://pa.bookmarksfly.cn

Ruby: s.count("a")
来源：http://qi.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://wu.jctech888.com.cn

[E13] 逐字符遍历
来源：http://hf.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://we.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://it.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gw.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rs.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jn.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://if.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://le.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bw.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://sr.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ys.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ph.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ks.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bj.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gf.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ty.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hd.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ui.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://mx.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xn.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zk.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zv.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ww.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fd.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gj.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zd.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yb.hnjuh.cn

[E16] 数字千分位
来源：http://ln.521024.cn

Py:   f"{1234567:,}"
来源：http://nk.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://nu.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nj.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ot.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pj.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wz.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://su.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://ly.nicolike.cn

[E17] 首字母大写
来源：http://mq.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fu.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kx.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uy.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wj.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ze.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vh.lnxyls.cn

Ruby: s.capitalize
来源：http://xf.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cp.chemitech.net.cn

[E18] 模板占位符替换
来源：http://oc.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qn.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kp.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zd.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ex.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://br.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cw.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qd.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://an.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://yd.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://xc.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zr.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://hb.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://hu.chemitech.net.cn

Java: s.lines().toList()
来源：http://fh.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://ap.shtwfgs.cn

Ruby: s.lines
来源：http://vh.wgjwhj.cn

C#:   s.Split('\n')
来源：http://jg.szsharing.cn

[E20] 判断字符串是否为空
来源：http://ub.szsharing.cn

Py:   if not s:
来源：http://mj.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ms.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qw.newstarts.cn

TS:   if (s === "") {}
来源：http://pn.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://no.bjjhwx.cn

Go:   if s == "" {}
来源：http://yk.shxzukj.cn

Ruby: if s.empty?
来源：http://se.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.lnxyls.cn

[E21] 超长截断加省略号
来源：http://bv.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gu.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rt.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xt.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://km.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qa.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://hz.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wb.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wv.huanxung.cn

[E22] 字节长度与字符长度
来源：http://cj.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eq.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xk.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hs.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vt.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hn.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fj.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://qj.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cq.nicolike.cn

================================================================================
来源：http://jc.nszjky.cn

F. 文件与目录
来源：http://nn.lnxyls.cn

================================================================================
来源：http://co.yuexingan06.cn

[F01] 读取整个文件
来源：http://mo.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://at.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://zk.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ij.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mx.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zg.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vn.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://wv.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://cv.521024.cn

[F02] 逐行读取文件
来源：http://sp.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jz.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aq.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ax.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wo.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cj.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ud.hnjuh.cn


<!-- 参考信息 -->