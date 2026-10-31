代发 wailian999

TS:   [...new Set(arr)]
来源：http://vm.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hu.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ap.yuexingan06.cn

Ruby: arr.uniq
来源：http://re.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://ye.gzmigu.cn

[D16] 求和与平均值
来源：http://ck.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://im.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://km.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xo.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xj.huixiangedu.cn

Go:   // 手写循环累加
来源：http://eu.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vt.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://wr.haigaiapp.cn

[D17] 最大值与最小值
来源：http://rc.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://te.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://he.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dz.hahajie.cn

TS:   Math.max(...arr);
来源：http://ln.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oc.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nv.521024.cn

Ruby: arr.max;  arr.min
来源：http://ej.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://vr.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://bi.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zq.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://sz.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ha.521024.cn

TS:   nested.flat();
来源：http://um.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://to.gzmigu.cn

Go:   // 手写双层循环
来源：http://ds.nicolike.cn

Ruby: nested.flatten
来源：http://zw.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kb.gzmigu.cn

[D19] 按字段分组
来源：http://ft.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gh.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pi.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ps.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nm.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tr.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://jn.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pl.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nz.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://rz.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://lq.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ij.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bd.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://us.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zi.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://se.muxihuayi.cn

Ruby: arr.tally
来源：http://py.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fl.colortex.cn

[D21] 判断是否包含某元素
来源：http://ps.lnxyls.cn

Py:   x in arr
来源：http://fp.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://yc.shxzskj.cn

JS:   arr.includes(x)
来源：http://nu.shxzskj.cn

TS:   arr.includes(x)
来源：http://yc.hahajie.cn

Java: list.contains(x)
来源：http://up.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://ee.hahajie.cn

Ruby: arr.include?(x)
来源：http://zb.yuexingan06.cn

C#:   list.Contains(x)
来源：http://ks.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://tt.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mp.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fr.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lb.lnxyls.cn

TS:   [...arr];
来源：http://jm.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://yd.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yk.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://bt.jctech888.com.cn

C#:   new List<int>(list);
来源：http://we.chemitech.net.cn

[D23] reduce 累积计算
来源：http://es.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bb.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jl.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uq.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vm.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zm.hnjuh.cn

Go:   // 手写循环
来源：http://vv.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://el.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ed.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://xp.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ay.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kf.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qv.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bl.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kb.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://if.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sj.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wi.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://qe.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wb.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yb.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kp.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zd.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rm.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://op.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cs.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aq.bookmarksfly.cn

[D26] 数组转字符串
来源：http://tq.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ss.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://va.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://oi.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ql.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://kt.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://cv.gzmigu.cn

Ruby: arr.join(", ")
来源：http://ue.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://cd.yuntaijiaju.cn

================================================================================
来源：http://zt.yuexingan06.cn

E. 字符串处理
来源：http://xk.jianghongdianzi.cn

================================================================================
来源：http://no.nicolike.cn

[E01] 拼接字符串
来源：http://tb.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sj.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rl.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tx.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tp.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qa.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hq.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.muxihuayi.cn

[E02] 重复字符串
来源：http://kb.wgjwhj.cn

Py:   "ab" * 3
来源：http://po.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://pw.colortex.cn

JS:   "ab".repeat(3)
来源：http://na.asd995.cn

TS:   "ab".repeat(3)
来源：http://ib.nszjky.cn

Java: "ab".repeat(3)
来源：http://zy.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://rw.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://oy.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://im.yuntaijiaju.cn

[E03] 截取子串
来源：http://ne.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xe.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vd.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lt.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://qp.nszjky.cn

Java: s.substring(1, 4)
来源：http://ny.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tr.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yd.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://lx.shxzskj.cn

[E04] 查找子串位置
来源：http://pi.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://om.asd995.cn

PHP:  strpos($s, "x");
来源：http://sx.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xf.newstarts.cn

TS:   s.indexOf("x")
来源：http://mt.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ku.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://aj.bookmarksfly.cn

Ruby: s.index("x")
来源：http://by.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://zc.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fy.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nv.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cp.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aw.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mw.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ky.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ys.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qp.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hj.nicolike.cn

[E06] 替换子串
来源：http://xi.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bw.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://sw.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://ct.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aq.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qi.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vi.asd995.cn

C#:   s.Replace("a", "b")
来源：http://jt.hnjuh.cn

[E07] 按分隔符拆分
来源：http://qa.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yo.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ra.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sg.panjiajie.cn

TS:   s.split(",")
来源：http://gg.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ts.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eg.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://rm.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mk.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://wv.huixiangedu.cn

Py:   ",".join(items)
来源：http://xt.szsharing.cn

PHP:  implode(",", $items);
来源：http://ow.szsharing.cn

JS:   items.join(",")
来源：http://wb.gzmigu.cn

TS:   items.join(",")
来源：http://mt.wgjwhj.cn

Java: String.join(",", items)
来源：http://ii.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://fy.521024.cn

Ruby: items.join(",")
来源：http://bo.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://lf.colortex.cn

[E09] 去除所有空白字符
来源：http://cw.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yl.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xy.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://zn.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://um.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://qx.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ip.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vh.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fz.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://oe.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kc.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bk.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://zo.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://pd.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://vp.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ct.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rm.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ma.asd995.cn

[E11] 反转字符串
来源：http://qv.shxzskj.cn

Py:   s[::-1]
来源：http://pc.hnjuh.cn

PHP:  strrev($s);
来源：http://xf.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://ok.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://tq.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pd.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://by.nszjky.cn

Ruby: s.reverse
来源：http://fv.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rh.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://qp.nszjky.cn

Py:   s.count("a")
来源：http://up.521024.cn

PHP:  substr_count($s, "a");
来源：http://vt.hahajie.cn

JS:   s.split("a").length - 1
来源：http://vs.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://xw.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ye.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://vx.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://jy.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://ay.huixiangedu.cn

[E13] 逐字符遍历
来源：http://hp.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://fn.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sn.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yi.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bb.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://da.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gm.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sm.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sd.newstarts.cn

[E14] URL 编码与 Base64
来源：http://rs.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://du.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ym.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://es.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ty.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qg.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zd.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tq.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dt.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ef.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ma.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://si.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ym.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vl.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wf.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gn.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://va.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kk.asd995.cn

[E16] 数字千分位
来源：http://pd.nicolike.cn

Py:   f"{1234567:,}"
来源：http://qh.nicolike.cn

PHP:  number_format(1234567);
来源：http://oy.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qc.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fw.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ub.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://je.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ij.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://ij.hahajie.cn

[E17] 首字母大写
来源：http://ey.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ts.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kq.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nu.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mn.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kf.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vh.hahajie.cn

Ruby: s.capitalize
来源：http://ia.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mo.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://be.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cg.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ya.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mz.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kv.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mb.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uy.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ed.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ja.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ar.521024.cn

Py:   s.splitlines()
来源：http://ff.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ry.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://vc.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ge.hahajie.cn

Java: s.lines().toList()
来源：http://qd.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://xu.shxzukj.cn

Ruby: s.lines
来源：http://bn.nszjky.cn

C#:   s.Split('\n')
来源：http://tj.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://il.huixinmuqiang.cn

Py:   if not s:
来源：http://hp.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ff.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ms.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ls.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://kh.lnxyls.cn

Go:   if s == "" {}
来源：http://fw.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://zl.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ai.gzmigu.cn

[E21] 超长截断加省略号
来源：http://pt.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://on.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://of.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xc.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cy.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ra.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://bx.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uz.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kx.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://vv.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sc.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gz.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ue.jctech888.com.cn


<!-- 参考信息 -->