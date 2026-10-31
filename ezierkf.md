代发 wailian999

[D15] 去重
来源：http://tt.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kz.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://wj.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://qq.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://pa.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cw.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hw.asd995.cn

Ruby: arr.uniq
来源：http://pn.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ap.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://yd.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xa.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rm.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rf.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ns.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sg.huanxung.cn

Go:   // 手写循环累加
来源：http://lv.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ue.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://eo.gzmigu.cn

[D17] 最大值与最小值
来源：http://am.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://xs.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ye.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wu.panjiajie.cn

TS:   Math.max(...arr);
来源：http://xz.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wv.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wg.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://rs.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://so.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://aa.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xj.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://ya.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ps.hahajie.cn

TS:   nested.flat();
来源：http://ut.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mv.asd995.cn

Go:   // 手写双层循环
来源：http://af.haigaiapp.cn

Ruby: nested.flatten
来源：http://wu.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oi.chemitech.net.cn

[D19] 按字段分组
来源：http://iq.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zi.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rc.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://is.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fn.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ru.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://xu.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ml.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dw.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ao.shtwfgs.cn

Py:   Counter(arr)
来源：http://ct.newstarts.cn

PHP:  array_count_values($arr);
来源：http://iv.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mp.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://co.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jz.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://de.shxzukj.cn

Ruby: arr.tally
来源：http://of.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://md.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://pv.521024.cn

Py:   x in arr
来源：http://zb.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://gw.yuexingan06.cn

JS:   arr.includes(x)
来源：http://qj.nicolike.cn

TS:   arr.includes(x)
来源：http://op.yuntaijiaju.cn

Java: list.contains(x)
来源：http://la.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://bw.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://pi.shxzskj.cn

C#:   list.Contains(x)
来源：http://ve.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ds.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ae.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vv.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ds.nicolike.cn

TS:   [...arr];
来源：http://yo.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://id.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fb.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://gl.huixiangedu.cn

C#:   new List<int>(list);
来源：http://hx.colortex.cn

[D23] reduce 累积计算
来源：http://ip.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hb.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vq.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nj.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ot.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bs.shxzukj.cn

Go:   // 手写循环
来源：http://vq.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yp.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lq.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://sd.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pn.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sr.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wh.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qt.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sb.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hx.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mu.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ko.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://dn.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wo.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pu.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mu.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ph.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vz.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ro.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ib.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yg.shtwfgs.cn

[D26] 数组转字符串
来源：http://gs.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://zh.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://re.hahajie.cn

JS:   arr.join(", ")
来源：http://hk.shxzskj.cn

TS:   arr.join(", ")
来源：http://ri.huixiangedu.cn

Java: String.join(", ", list)
来源：http://xr.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://fe.colortex.cn

Ruby: arr.join(", ")
来源：http://dh.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://rq.huanxung.cn

================================================================================
来源：http://bn.szxytkj.cn

E. 字符串处理
来源：http://wm.newstarts.cn

================================================================================
来源：http://dc.bookmarksfly.cn

[E01] 拼接字符串
来源：http://wc.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ys.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ez.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fn.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pg.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dq.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ii.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ni.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sc.521024.cn

[E02] 重复字符串
来源：http://xx.521024.cn

Py:   "ab" * 3
来源：http://rw.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://yx.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://qh.asd995.cn

TS:   "ab".repeat(3)
来源：http://pc.nszjky.cn

Java: "ab".repeat(3)
来源：http://ks.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://jv.newstarts.cn

Ruby: "ab" * 3
来源：http://bp.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gb.asd995.cn

[E03] 截取子串
来源：http://es.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ub.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nm.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oo.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://gg.lnxyls.cn

Java: s.substring(1, 4)
来源：http://sv.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fz.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wy.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://no.9csxet.cn

[E04] 查找子串位置
来源：http://ln.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://km.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://uh.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tm.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://lr.gzmigu.cn

Java: s.indexOf("x")
来源：http://cl.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ej.nszjky.cn

Ruby: s.index("x")
来源：http://yf.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://eh.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xx.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://od.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dd.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ru.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://un.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rm.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zi.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cr.hnjuh.cn

[E06] 替换子串
来源：http://mv.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xz.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://jb.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oj.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://xh.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ub.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fv.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fu.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://yd.nszjky.cn

[E07] 按分隔符拆分
来源：http://lq.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sl.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wt.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bs.hahajie.cn

TS:   s.split(",")
来源：http://bj.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zt.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zq.colortex.cn

Ruby: s.split(",");  s.split
来源：http://mq.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cx.colortex.cn

[E08] 数组按分隔符合并
来源：http://tt.wgjwhj.cn

Py:   ",".join(items)
来源：http://lv.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://xx.chemitech.net.cn

JS:   items.join(",")
来源：http://gd.muxihuayi.cn

TS:   items.join(",")
来源：http://ji.newstarts.cn

Java: String.join(",", items)
来源：http://so.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://rr.lnxyls.cn

Ruby: items.join(",")
来源：http://lb.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://or.nszjky.cn

[E09] 去除所有空白字符
来源：http://kd.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gu.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hy.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://sq.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://xz.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ba.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hx.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tq.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uq.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://nq.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://af.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://we.521024.cn

JS:   "7".padStart(3, "0")
来源：http://jj.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://jl.521024.cn

Java: String.format("%03d", 7)
来源：http://xs.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ao.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ns.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pq.shxzskj.cn

[E11] 反转字符串
来源：http://oj.521024.cn

Py:   s[::-1]
来源：http://xr.wgjwhj.cn

PHP:  strrev($s);
来源：http://ge.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://gq.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://pr.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jf.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bw.nszjky.cn

Ruby: s.reverse
来源：http://dv.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aj.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://rr.chemitech.net.cn

Py:   s.count("a")
来源：http://yn.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://db.hahajie.cn

JS:   s.split("a").length - 1
来源：http://jt.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ou.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wf.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://rp.muxihuayi.cn

Ruby: s.count("a")
来源：http://ue.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://wm.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ij.colortex.cn

Py:   for ch in s: print(ch)
来源：http://ev.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gq.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hx.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ei.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ja.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dl.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ry.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://jt.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ja.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ae.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://de.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lw.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hi.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ut.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uy.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ju.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ai.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qg.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://po.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cn.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pp.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ir.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ww.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ty.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ls.shtwfgs.cn

[E16] 数字千分位
来源：http://hy.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://jw.nszjky.cn

PHP:  number_format(1234567);
来源：http://hp.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jp.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gq.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pi.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ug.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qn.asd995.cn

C#:   1234567.ToString("N0")
来源：http://ym.huanxung.cn

[E17] 首字母大写
来源：http://yx.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qy.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wu.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://og.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hm.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qd.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ji.hahajie.cn

Ruby: s.capitalize
来源：http://ok.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nd.newstarts.cn

[E18] 模板占位符替换
来源：http://it.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sw.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://po.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iq.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ad.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vy.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gb.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sc.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sy.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://mi.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://yx.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pr.521024.cn

JS:   s.split(/\r?\n/)
来源：http://vl.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://qx.lnxyls.cn

Java: s.lines().toList()
来源：http://bh.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://tv.colortex.cn

Ruby: s.lines
来源：http://fc.yuexingan06.cn

C#:   s.Split('\n')
来源：http://si.nicolike.cn

[E20] 判断字符串是否为空
来源：http://qr.colortex.cn

Py:   if not s:
来源：http://ql.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kd.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oo.huanxung.cn

TS:   if (s === "") {}
来源：http://xf.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://lo.shxzukj.cn

Go:   if s == "" {}
来源：http://hx.nszjky.cn

Ruby: if s.empty?
来源：http://cf.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zl.nicolike.cn

[E21] 超长截断加省略号
来源：http://do.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ow.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uy.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ln.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nb.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xi.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://hj.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lk.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hi.panjiajie.cn


<!-- 参考信息 -->