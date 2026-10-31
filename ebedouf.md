代发 wailian999

[D15] 去重
来源：http://cb.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jx.hahajie.cn

PHP:  array_unique($arr);
来源：http://ml.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://ku.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://um.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fr.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ai.nszjky.cn

Ruby: arr.uniq
来源：http://ng.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://hm.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://yl.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yf.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://su.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ks.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qi.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pu.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://yu.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xn.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://xg.chemitech.net.cn

[D17] 最大值与最小值
来源：http://wr.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://lt.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://cd.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hr.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://ia.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cn.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kp.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://gz.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://sg.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ng.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nu.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://vb.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bv.huixiangedu.cn

TS:   nested.flat();
来源：http://rh.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fu.bjjhwx.cn

Go:   // 手写双层循环
来源：http://nc.huixiangedu.cn

Ruby: nested.flatten
来源：http://ek.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hp.gzmigu.cn

[D19] 按字段分组
来源：http://eu.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ht.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nk.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vr.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bc.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eo.521024.cn

Go:   // 手写 map[string][]T
来源：http://tz.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jw.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ux.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://fx.jctech888.com.cn

Py:   Counter(arr)
来源：http://gj.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://gn.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hv.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://no.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hf.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ay.bookmarksfly.cn

Ruby: arr.tally
来源：http://nn.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rl.huanxung.cn

[D21] 判断是否包含某元素
来源：http://gb.nszjky.cn

Py:   x in arr
来源：http://yw.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://it.huixiangedu.cn

JS:   arr.includes(x)
来源：http://em.colortex.cn

TS:   arr.includes(x)
来源：http://nt.wgjwhj.cn

Java: list.contains(x)
来源：http://in.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ua.szsharing.cn

Ruby: arr.include?(x)
来源：http://an.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://tw.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://lz.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ay.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://in.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hc.jctech888.com.cn

TS:   [...arr];
来源：http://xy.hahajie.cn

Java: new ArrayList<>(list);
来源：http://ri.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kk.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ip.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://qr.chemitech.net.cn

[D23] reduce 累积计算
来源：http://mt.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nv.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vb.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mp.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zd.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hk.colortex.cn

Go:   // 手写循环
来源：http://ub.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ak.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yp.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://bp.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://re.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tp.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://na.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ui.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ur.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tb.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://do.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bw.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://rk.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yx.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sb.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ha.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ej.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qo.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wg.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://en.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ra.hahajie.cn

[D26] 数组转字符串
来源：http://vk.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://nq.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://tn.shxzukj.cn

JS:   arr.join(", ")
来源：http://is.colortex.cn

TS:   arr.join(", ")
来源：http://hj.shxzukj.cn

Java: String.join(", ", list)
来源：http://mx.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://wu.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://ls.asd995.cn

C#:   string.Join(", ", list)
来源：http://hg.szsharing.cn

================================================================================
来源：http://my.lnxyls.cn

E. 字符串处理
来源：http://pv.shxzukj.cn

================================================================================
来源：http://le.muxihuayi.cn

[E01] 拼接字符串
来源：http://tz.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ny.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pj.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xf.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rr.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zp.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kx.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hn.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zt.bookmarksfly.cn

[E02] 重复字符串
来源：http://iy.bjjhwx.cn

Py:   "ab" * 3
来源：http://kc.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://kw.hahajie.cn

JS:   "ab".repeat(3)
来源：http://bw.colortex.cn

TS:   "ab".repeat(3)
来源：http://cr.szxytkj.cn

Java: "ab".repeat(3)
来源：http://an.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://iy.9csxet.cn

Ruby: "ab" * 3
来源：http://mx.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ug.nicolike.cn

[E03] 截取子串
来源：http://sp.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bd.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gf.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lc.nicolike.cn

TS:   s.slice(1, 4)
来源：http://ao.hnjuh.cn

Java: s.substring(1, 4)
来源：http://lg.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sj.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nl.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ge.shxzukj.cn

[E04] 查找子串位置
来源：http://qt.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://it.9csxet.cn

PHP:  strpos($s, "x");
来源：http://hh.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nd.9csxet.cn

TS:   s.indexOf("x")
来源：http://pt.szsharing.cn

Java: s.indexOf("x")
来源：http://pn.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ap.bookmarksfly.cn

Ruby: s.index("x")
来源：http://oy.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://ua.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ow.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tr.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mv.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cg.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ep.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oj.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sg.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yw.jianghongdianzi.cn

[E06] 替换子串
来源：http://va.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pa.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ne.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wj.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://qj.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jm.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xn.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lb.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://fx.shxzukj.cn

[E07] 按分隔符拆分
来源：http://tk.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ay.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://um.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zt.shxzskj.cn

TS:   s.split(",")
来源：http://hk.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gy.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ce.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://ld.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ys.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://yy.panjiajie.cn

Py:   ",".join(items)
来源：http://el.nicolike.cn

PHP:  implode(",", $items);
来源：http://kg.bjjhwx.cn

JS:   items.join(",")
来源：http://zf.huixiangedu.cn

TS:   items.join(",")
来源：http://yd.9csxet.cn

Java: String.join(",", items)
来源：http://jx.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://rn.lnxyls.cn

Ruby: items.join(",")
来源：http://ag.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://pw.colortex.cn

[E09] 去除所有空白字符
来源：http://hv.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fr.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uq.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://mz.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://ir.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://uf.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pz.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pc.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ti.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://ad.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qs.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bm.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://zd.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://ak.nicolike.cn

Java: String.format("%03d", 7)
来源：http://sh.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yy.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dz.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cf.chemitech.net.cn

[E11] 反转字符串
来源：http://ie.chemitech.net.cn

Py:   s[::-1]
来源：http://zm.9csxet.cn

PHP:  strrev($s);
来源：http://rt.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://ja.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://ln.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bo.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xd.chemitech.net.cn

Ruby: s.reverse
来源：http://as.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pe.szsharing.cn

[E12] 统计某字符出现次数
来源：http://du.shtwfgs.cn

Py:   s.count("a")
来源：http://js.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://en.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://hw.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://rm.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fp.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://ee.szxytkj.cn

Ruby: s.count("a")
来源：http://rd.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://er.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://il.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://le.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vm.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ll.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ql.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nx.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qn.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://it.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pu.asd995.cn

[E14] URL 编码与 Base64
来源：http://ra.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xy.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qd.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ln.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qv.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qk.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tw.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ds.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://vn.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sz.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wm.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qq.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vl.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jo.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bx.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lu.9csxet.cn

[E16] 数字千分位
来源：http://df.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://sg.colortex.cn

PHP:  number_format(1234567);
来源：http://ne.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://om.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bx.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lx.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sl.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lb.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://wz.hnjuh.cn

[E17] 首字母大写
来源：http://bb.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yy.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cd.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gz.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hr.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wu.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.521024.cn

Ruby: s.capitalize
来源：http://oc.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gi.shxzskj.cn

[E18] 模板占位符替换
来源：http://kw.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vb.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aa.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://md.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fu.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bb.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dx.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xw.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eq.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://jq.chemitech.net.cn

Py:   s.splitlines()
来源：http://xr.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jp.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://gq.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://yo.colortex.cn

Java: s.lines().toList()
来源：http://lt.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://va.muxihuayi.cn

Ruby: s.lines
来源：http://td.newstarts.cn

C#:   s.Split('\n')
来源：http://us.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://sg.panjiajie.cn

Py:   if not s:
来源：http://af.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wr.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sp.521024.cn

TS:   if (s === "") {}
来源：http://dp.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://rf.szxytkj.cn

Go:   if s == "" {}
来源：http://uk.huixiangedu.cn

Ruby: if s.empty?
来源：http://uv.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rj.nszjky.cn

[E21] 超长截断加省略号
来源：http://on.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zr.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://df.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ud.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://po.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ra.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://jg.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kj.bookmarksfly.cn


<!-- 参考信息 -->