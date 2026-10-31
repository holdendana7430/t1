代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eh.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bv.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vd.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ii.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sp.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://kw.huanxung.cn

[D17] 最大值与最小值
来源：http://lj.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://xf.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://zx.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://az.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ee.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jf.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://me.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://yj.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://cv.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://ul.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://po.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://zg.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ke.nszjky.cn

TS:   nested.flat();
来源：http://dr.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xg.521024.cn

Go:   // 手写双层循环
来源：http://mp.newstarts.cn

Ruby: nested.flatten
来源：http://ql.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://we.yuexingan06.cn

[D19] 按字段分组
来源：http://ka.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ll.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://di.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bj.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rj.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ea.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ib.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aw.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ad.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://zr.gzmigu.cn

Py:   Counter(arr)
来源：http://bu.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://hk.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bp.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yu.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tz.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://wt.gzmigu.cn

Ruby: arr.tally
来源：http://yv.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ug.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://qh.bjjhwx.cn

Py:   x in arr
来源：http://cp.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://oj.hahajie.cn

JS:   arr.includes(x)
来源：http://lu.521024.cn

TS:   arr.includes(x)
来源：http://ok.huixiangedu.cn

Java: list.contains(x)
来源：http://ln.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://gd.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://ew.huixiangedu.cn

C#:   list.Contains(x)
来源：http://xz.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://xj.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ye.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pp.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gw.huixiangedu.cn

TS:   [...arr];
来源：http://kn.nicolike.cn

Java: new ArrayList<>(list);
来源：http://ua.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sm.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://lc.hahajie.cn

C#:   new List<int>(list);
来源：http://lp.gzmigu.cn

[D23] reduce 累积计算
来源：http://ph.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qg.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xc.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cs.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jw.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sd.haigaiapp.cn

Go:   // 手写循环
来源：http://th.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qm.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ia.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://rr.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ul.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://co.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pv.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qa.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rj.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aw.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hs.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fn.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://qt.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lh.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kd.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ma.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kp.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ta.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rn.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pv.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pj.shtwfgs.cn

[D26] 数组转字符串
来源：http://jj.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ou.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://bd.9csxet.cn

JS:   arr.join(", ")
来源：http://jb.hnjuh.cn

TS:   arr.join(", ")
来源：http://fv.nicolike.cn

Java: String.join(", ", list)
来源：http://vg.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://vj.huanxung.cn

Ruby: arr.join(", ")
来源：http://tv.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://zi.asd995.cn

================================================================================
来源：http://nq.hnjuh.cn

E. 字符串处理
来源：http://fe.gzmigu.cn

================================================================================
来源：http://bf.shxzskj.cn

[E01] 拼接字符串
来源：http://op.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://td.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cd.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lt.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vf.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zk.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zv.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jp.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://om.hnjuh.cn

[E02] 重复字符串
来源：http://tb.haigaiapp.cn

Py:   "ab" * 3
来源：http://hv.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ik.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://on.colortex.cn

TS:   "ab".repeat(3)
来源：http://oc.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://mi.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://dv.lnxyls.cn

Ruby: "ab" * 3
来源：http://fm.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lt.lnxyls.cn

[E03] 截取子串
来源：http://bv.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pc.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ih.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wc.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ed.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://kc.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ja.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ls.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://bw.gzmigu.cn

[E04] 查找子串位置
来源：http://do.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://cl.hahajie.cn

PHP:  strpos($s, "x");
来源：http://go.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ni.hahajie.cn

TS:   s.indexOf("x")
来源：http://zu.asd995.cn

Java: s.indexOf("x")
来源：http://vn.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://kr.colortex.cn

Ruby: s.index("x")
来源：http://yn.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://yy.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bz.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xb.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://po.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zv.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://az.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ei.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gs.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gr.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fx.nicolike.cn

[E06] 替换子串
来源：http://mt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mu.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://tq.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://er.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ex.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://si.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://er.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://lx.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://ml.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qe.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pn.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mk.hahajie.cn

TS:   s.split(",")
来源：http://tx.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kr.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gs.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://ry.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oe.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://rq.colortex.cn

Py:   ",".join(items)
来源：http://eg.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://vv.nszjky.cn

JS:   items.join(",")
来源：http://tw.shtwfgs.cn

TS:   items.join(",")
来源：http://ws.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://zv.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://oa.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://us.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://rq.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://ym.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aw.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ir.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wm.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://im.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://oz.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cf.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ou.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zh.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://pr.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://au.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cf.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://na.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://ug.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://nu.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://id.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ey.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://si.bjjhwx.cn

[E11] 反转字符串
来源：http://pu.szxytkj.cn

Py:   s[::-1]
来源：http://lo.bookmarksfly.cn

PHP:  strrev($s);
来源：http://or.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://ev.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://rj.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rb.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zq.wgjwhj.cn

Ruby: s.reverse
来源：http://mk.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qb.huanxung.cn

[E12] 统计某字符出现次数
来源：http://tk.shtwfgs.cn

Py:   s.count("a")
来源：http://pq.colortex.cn

PHP:  substr_count($s, "a");
来源：http://jv.asd995.cn

JS:   s.split("a").length - 1
来源：http://qh.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://gy.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bu.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://kt.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://pm.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://cu.shtwfgs.cn

[E13] 逐字符遍历
来源：http://hu.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://di.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://va.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yl.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lc.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ag.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zq.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yx.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qo.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://vs.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pb.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ju.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hw.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fe.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://be.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://av.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ld.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://cy.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xt.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fi.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ao.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vc.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cg.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ap.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ej.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iq.haigaiapp.cn

[E16] 数字千分位
来源：http://vp.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://xq.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://dj.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kh.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wj.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yv.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ql.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ua.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://eu.hnjuh.cn

[E17] 首字母大写
来源：http://ug.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hr.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ie.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vm.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ww.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fy.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fp.szsharing.cn

Ruby: s.capitalize
来源：http://po.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xj.huanxung.cn

[E18] 模板占位符替换
来源：http://cq.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://do.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ej.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ab.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rb.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qg.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vf.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ci.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fe.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://cz.szsharing.cn

Py:   s.splitlines()
来源：http://fp.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gz.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://xm.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://kl.szxytkj.cn

Java: s.lines().toList()
来源：http://yw.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://tj.jctech888.com.cn

Ruby: s.lines
来源：http://ug.gzmigu.cn

C#:   s.Split('\n')
来源：http://gl.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://cv.huanxung.cn

Py:   if not s:
来源：http://tw.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wy.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gm.bjjhwx.cn

TS:   if (s === "") {}
来源：http://oo.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://sd.colortex.cn

Go:   if s == "" {}
来源：http://db.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://ok.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pt.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://fi.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kv.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://li.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ce.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xo.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tv.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://pm.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://se.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dm.hahajie.cn

[E22] 字节长度与字符长度
来源：http://zg.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sm.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mm.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://al.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rk.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iq.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oh.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://iu.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wi.9csxet.cn

================================================================================
来源：http://ck.shxzukj.cn

F. 文件与目录
来源：http://nd.bjjhwx.cn

================================================================================
来源：http://ts.shtwfgs.cn


<!-- 参考信息 -->