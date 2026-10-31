代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xe.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://gb.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://eu.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://ie.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://tz.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vp.szxytkj.cn

TS:   Math.max(...arr);
来源：http://ei.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mo.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fp.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://hp.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://pp.521024.cn

[D18] 扁平化嵌套数组
来源：http://py.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://df.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://in.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gt.szsharing.cn

TS:   nested.flat();
来源：http://ap.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sl.asd995.cn

Go:   // 手写双层循环
来源：http://se.hnjuh.cn

Ruby: nested.flatten
来源：http://ir.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ss.lnxyls.cn

[D19] 按字段分组
来源：http://jj.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://id.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vk.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ax.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rb.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rs.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://pb.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uh.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://su.asd995.cn

[D20] 统计每个元素出现次数
来源：http://dk.jctech888.com.cn

Py:   Counter(arr)
来源：http://ph.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://tj.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kn.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mh.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yg.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://eu.huanxung.cn

Ruby: arr.tally
来源：http://nc.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jn.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://sp.muxihuayi.cn

Py:   x in arr
来源：http://xh.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://yu.chemitech.net.cn

JS:   arr.includes(x)
来源：http://yc.hahajie.cn

TS:   arr.includes(x)
来源：http://nr.panjiajie.cn

Java: list.contains(x)
来源：http://hc.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://bh.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://bb.asd995.cn

C#:   list.Contains(x)
来源：http://ot.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://uz.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fw.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oo.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mc.muxihuayi.cn

TS:   [...arr];
来源：http://mn.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://pv.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ko.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://mf.shtwfgs.cn

C#:   new List<int>(list);
来源：http://az.shxzskj.cn

[D23] reduce 累积计算
来源：http://nq.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zh.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xj.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gw.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ti.hahajie.cn

Go:   // 手写循环
来源：http://gw.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lw.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ng.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://nm.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ph.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lp.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dg.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ta.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://um.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ht.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xq.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sc.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://wh.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gm.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kj.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yl.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dh.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://up.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jf.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://da.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bm.asd995.cn

[D26] 数组转字符串
来源：http://mf.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://pn.asd995.cn

PHP:  implode(", ", $arr);
来源：http://lx.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ew.hahajie.cn

TS:   arr.join(", ")
来源：http://rw.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://gb.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ns.hnjuh.cn

Ruby: arr.join(", ")
来源：http://jx.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://re.huixiangedu.cn

================================================================================
来源：http://sa.yuexingan06.cn

E. 字符串处理
来源：http://vm.wgjwhj.cn

================================================================================
来源：http://jg.wgjwhj.cn

[E01] 拼接字符串
来源：http://ho.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tn.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xb.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jj.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fo.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wq.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wz.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://da.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oa.bjjhwx.cn

[E02] 重复字符串
来源：http://el.shxzskj.cn

Py:   "ab" * 3
来源：http://ci.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ei.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://rb.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ou.521024.cn

Java: "ab".repeat(3)
来源：http://gz.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://nw.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://xi.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mf.shtwfgs.cn

[E03] 截取子串
来源：http://no.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uq.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://li.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ab.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://fa.hahajie.cn

Java: s.substring(1, 4)
来源：http://mt.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ua.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ii.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://hh.nicolike.cn

[E04] 查找子串位置
来源：http://fo.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://ak.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://mn.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://co.panjiajie.cn

TS:   s.indexOf("x")
来源：http://sm.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://tg.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://up.haigaiapp.cn

Ruby: s.index("x")
来源：http://ip.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://fx.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tr.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tp.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://et.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iq.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://we.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://je.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ry.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lc.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://un.huixiangedu.cn

[E06] 替换子串
来源：http://za.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://az.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://rg.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vo.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://bg.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://am.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bi.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tv.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ov.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://am.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://py.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ba.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://za.nszjky.cn

TS:   s.split(",")
来源：http://lm.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oe.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wn.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ff.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://id.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://ml.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://la.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://pk.hahajie.cn

JS:   items.join(",")
来源：http://bm.colortex.cn

TS:   items.join(",")
来源：http://yp.haigaiapp.cn

Java: String.join(",", items)
来源：http://zz.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://go.asd995.cn

Ruby: items.join(",")
来源：http://xu.shxzskj.cn

C#:   string.Join(",", items)
来源：http://zg.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://nm.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ck.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://do.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wk.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://uc.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://gd.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ms.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://do.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ui.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://kj.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xv.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bg.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://wy.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://yu.newstarts.cn

Java: String.format("%03d", 7)
来源：http://kp.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tc.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yq.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kj.asd995.cn

[E11] 反转字符串
来源：http://nl.asd995.cn

Py:   s[::-1]
来源：http://lq.nicolike.cn

PHP:  strrev($s);
来源：http://bh.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://be.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://mr.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ci.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ea.gzmigu.cn

Ruby: s.reverse
来源：http://ju.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://en.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ip.haigaiapp.cn

Py:   s.count("a")
来源：http://kn.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://zk.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://js.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://eh.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wy.521024.cn

Go:   strings.Count(s, "a")
来源：http://fy.bookmarksfly.cn

Ruby: s.count("a")
来源：http://qn.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://vg.haigaiapp.cn

[E13] 逐字符遍历
来源：http://hv.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://uj.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://be.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ea.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nd.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ub.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kh.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jt.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lj.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://hz.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ml.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dx.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ju.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ck.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zk.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tg.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xf.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://er.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://ct.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sc.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sl.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vh.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kj.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qh.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ei.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bm.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hq.haigaiapp.cn

[E16] 数字千分位
来源：http://hr.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ee.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://cy.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ml.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qk.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dn.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uu.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uy.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://fa.szxytkj.cn

[E17] 首字母大写
来源：http://jm.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pb.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yi.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hy.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zh.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xn.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ko.hnjuh.cn

Ruby: s.capitalize
来源：http://ac.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://on.jctech888.com.cn

[E18] 模板占位符替换
来源：http://wy.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hb.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zw.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://br.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gn.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ba.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gl.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ex.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ts.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://sk.huanxung.cn

Py:   s.splitlines()
来源：http://qv.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ws.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ca.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://du.shxzukj.cn

Java: s.lines().toList()
来源：http://qt.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://no.yuntaijiaju.cn

Ruby: s.lines
来源：http://ey.shxzskj.cn

C#:   s.Split('\n')
来源：http://ib.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://ig.huanxung.cn

Py:   if not s:
来源：http://vq.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oc.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://br.szxytkj.cn

TS:   if (s === "") {}
来源：http://co.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://gq.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://sx.yuexingan06.cn

Ruby: if s.empty?
来源：http://uc.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://au.hahajie.cn

[E21] 超长截断加省略号
来源：http://bi.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vz.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hg.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://je.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oj.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://gc.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dt.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uc.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://sl.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zh.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ec.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bi.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fl.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pa.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dj.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://xc.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lk.yuexingan06.cn

================================================================================
来源：http://tt.huanxung.cn

F. 文件与目录
来源：http://iu.nszjky.cn

================================================================================
来源：http://dn.colortex.cn

[F01] 读取整个文件
来源：http://iq.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fm.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ak.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ia.521024.cn


<!-- 参考信息 -->