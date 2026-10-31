代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ag.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://qt.shxzskj.cn

[D17] 最大值与最小值
来源：http://hy.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://vl.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://tl.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://we.shxzskj.cn

TS:   Math.max(...arr);
来源：http://qf.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hp.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lb.asd995.cn

Ruby: arr.max;  arr.min
来源：http://ln.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://wm.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://es.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qy.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://po.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zf.huixinmuqiang.cn

TS:   nested.flat();
来源：http://oz.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nx.newstarts.cn

Go:   // 手写双层循环
来源：http://lg.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://dn.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bg.szxytkj.cn

[D19] 按字段分组
来源：http://mg.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ms.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xp.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rl.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kq.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ea.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://sb.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ke.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vv.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://df.lnxyls.cn

Py:   Counter(arr)
来源：http://bp.nicolike.cn

PHP:  array_count_values($arr);
来源：http://eb.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dn.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rn.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nb.asd995.cn

Go:   // 手写 map[T]int
来源：http://nd.bjjhwx.cn

Ruby: arr.tally
来源：http://ch.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wm.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://gp.huanxung.cn

Py:   x in arr
来源：http://yk.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ca.haigaiapp.cn

JS:   arr.includes(x)
来源：http://ht.nicolike.cn

TS:   arr.includes(x)
来源：http://je.jianghongdianzi.cn

Java: list.contains(x)
来源：http://cd.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://nd.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://qi.lnxyls.cn

C#:   list.Contains(x)
来源：http://mr.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://vi.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ca.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sg.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iu.shtwfgs.cn

TS:   [...arr];
来源：http://zh.9csxet.cn

Java: new ArrayList<>(list);
来源：http://uo.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zj.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://vs.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://be.muxihuayi.cn

[D23] reduce 累积计算
来源：http://xr.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zz.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vv.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ah.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xk.szsharing.cn

Go:   // 手写循环
来源：http://uh.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sc.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lv.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ju.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xo.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qx.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sz.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bo.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ja.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qu.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bw.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mb.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://vu.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hj.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lh.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ty.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fr.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mb.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://em.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mc.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tl.nicolike.cn

[D26] 数组转字符串
来源：http://yw.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ub.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://gw.huixiangedu.cn

JS:   arr.join(", ")
来源：http://nx.lnxyls.cn

TS:   arr.join(", ")
来源：http://sv.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://wk.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://hm.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://gc.nicolike.cn

C#:   string.Join(", ", list)
来源：http://bp.shxzskj.cn

================================================================================
来源：http://lf.nszjky.cn

E. 字符串处理
来源：http://wn.bookmarksfly.cn

================================================================================
来源：http://pr.shxzskj.cn

[E01] 拼接字符串
来源：http://wf.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pe.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ke.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gz.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hl.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dm.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rs.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xm.521024.cn

[E02] 重复字符串
来源：http://xm.jctech888.com.cn

Py:   "ab" * 3
来源：http://gt.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://qd.nszjky.cn

JS:   "ab".repeat(3)
来源：http://eu.nicolike.cn

TS:   "ab".repeat(3)
来源：http://hv.colortex.cn

Java: "ab".repeat(3)
来源：http://fg.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://al.asd995.cn

Ruby: "ab" * 3
来源：http://zt.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://us.nicolike.cn

[E03] 截取子串
来源：http://md.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yh.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uh.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://la.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://uc.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://wz.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oy.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wh.colortex.cn

C#:   s.Substring(1, 3)
来源：http://mi.yuexingan06.cn

[E04] 查找子串位置
来源：http://ce.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://xn.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://cg.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zn.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ky.hahajie.cn

Java: s.indexOf("x")
来源：http://mu.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://bn.shxzskj.cn

Ruby: s.index("x")
来源：http://we.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ml.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uu.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fx.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ce.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lv.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://am.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yv.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uk.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jz.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wh.hahajie.cn

[E06] 替换子串
来源：http://yr.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kj.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://cq.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gk.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://sj.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uy.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ra.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yg.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://qr.newstarts.cn

[E07] 按分隔符拆分
来源：http://xg.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cw.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ax.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bd.haigaiapp.cn

TS:   s.split(",")
来源：http://gt.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fj.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wr.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://da.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fx.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://lx.gzmigu.cn

Py:   ",".join(items)
来源：http://mx.huanxung.cn

PHP:  implode(",", $items);
来源：http://ay.shxzukj.cn

JS:   items.join(",")
来源：http://tm.hnjuh.cn

TS:   items.join(",")
来源：http://vb.asd995.cn

Java: String.join(",", items)
来源：http://ec.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://lc.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://eh.shxzskj.cn

C#:   string.Join(",", items)
来源：http://rq.521024.cn

[E09] 去除所有空白字符
来源：http://sm.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pj.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qw.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://pe.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://fu.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://ih.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dl.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cd.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yw.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ub.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hy.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://df.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://we.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://gw.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://ca.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gq.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rj.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xg.lnxyls.cn

[E11] 反转字符串
来源：http://pi.bjjhwx.cn

Py:   s[::-1]
来源：http://eu.panjiajie.cn

PHP:  strrev($s);
来源：http://it.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://mh.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://ls.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bd.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://by.bookmarksfly.cn

Ruby: s.reverse
来源：http://ga.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qz.nszjky.cn

[E12] 统计某字符出现次数
来源：http://ml.newstarts.cn

Py:   s.count("a")
来源：http://pd.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://nh.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://co.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://vw.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kt.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://it.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://rw.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://lw.colortex.cn

[E13] 逐字符遍历
来源：http://as.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://hr.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mv.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://id.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ft.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nx.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ps.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://om.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://px.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://ex.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://el.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nw.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://za.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://av.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gv.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://al.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sy.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jd.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://rh.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nu.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qb.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lo.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qr.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://il.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eb.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ue.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ls.hnjuh.cn

[E16] 数字千分位
来源：http://cf.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://ve.asd995.cn

PHP:  number_format(1234567);
来源：http://nf.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tj.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qu.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://th.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vk.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qj.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://fp.lnxyls.cn

[E17] 首字母大写
来源：http://ww.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ec.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jb.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xt.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xe.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://so.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ji.newstarts.cn

Ruby: s.capitalize
来源：http://cr.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tf.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://xs.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cz.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yg.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ir.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uy.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lv.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zh.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ay.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wl.newstarts.cn

[E19] 多行文本按行拆分
来源：http://kj.huixiangedu.cn

Py:   s.splitlines()
来源：http://wa.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://al.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://sv.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://ud.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ro.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ew.huixinmuqiang.cn

Ruby: s.lines
来源：http://xk.shxzukj.cn

C#:   s.Split('\n')
来源：http://zm.521024.cn

[E20] 判断字符串是否为空
来源：http://kb.panjiajie.cn

Py:   if not s:
来源：http://ax.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hq.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ci.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://xk.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://zq.gzmigu.cn

Go:   if s == "" {}
来源：http://pt.haigaiapp.cn

Ruby: if s.empty?
来源：http://zx.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mb.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://gg.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bd.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wn.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vs.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ei.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jj.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://qs.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tx.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://il.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://xd.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yg.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pt.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uw.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bg.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ug.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dk.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://vb.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uz.panjiajie.cn

================================================================================
来源：http://ll.nszjky.cn

F. 文件与目录
来源：http://yu.hahajie.cn

================================================================================
来源：http://vf.szsharing.cn

[F01] 读取整个文件
来源：http://ow.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cs.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://yl.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uc.yuntaijiaju.cn


<!-- 参考信息 -->