代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gb.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vs.huanxung.cn

Go:   // 手写循环累加
来源：http://vh.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lj.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://dc.jctech888.com.cn

[D17] 最大值与最小值
来源：http://pd.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://qz.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ee.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fq.shxzukj.cn

TS:   Math.max(...arr);
来源：http://np.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bg.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bf.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://kj.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://me.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://we.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xo.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://vl.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pn.gzmigu.cn

TS:   nested.flat();
来源：http://jt.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tt.wgjwhj.cn

Go:   // 手写双层循环
来源：http://nw.shtwfgs.cn

Ruby: nested.flatten
来源：http://um.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fj.shxzskj.cn

[D19] 按字段分组
来源：http://rx.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gc.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ve.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sa.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nm.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fb.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://mi.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://in.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://na.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://to.shxzskj.cn

Py:   Counter(arr)
来源：http://em.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://lm.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hg.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sv.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fm.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ek.haigaiapp.cn

Ruby: arr.tally
来源：http://cf.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rg.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://mp.szxytkj.cn

Py:   x in arr
来源：http://ui.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://rv.hnjuh.cn

JS:   arr.includes(x)
来源：http://yd.muxihuayi.cn

TS:   arr.includes(x)
来源：http://zo.gzmigu.cn

Java: list.contains(x)
来源：http://yh.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://we.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://cm.haigaiapp.cn

C#:   list.Contains(x)
来源：http://oj.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://yb.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aj.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lu.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sy.yuexingan06.cn

TS:   [...arr];
来源：http://xg.9csxet.cn

Java: new ArrayList<>(list);
来源：http://ui.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lr.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://tg.bjjhwx.cn

C#:   new List<int>(list);
来源：http://or.521024.cn

[D23] reduce 累积计算
来源：http://ky.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tu.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xj.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://op.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ca.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sn.shtwfgs.cn

Go:   // 手写循环
来源：http://hy.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bx.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cc.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://cr.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iq.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cp.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ks.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://er.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gj.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hf.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jq.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gy.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://kr.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hr.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ma.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tf.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ff.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sn.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lw.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://go.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ix.asd995.cn

[D26] 数组转字符串
来源：http://rk.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://cg.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://bl.chemitech.net.cn

JS:   arr.join(", ")
来源：http://wx.nszjky.cn

TS:   arr.join(", ")
来源：http://ts.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://tn.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://wx.newstarts.cn

Ruby: arr.join(", ")
来源：http://fv.colortex.cn

C#:   string.Join(", ", list)
来源：http://bl.shtwfgs.cn

================================================================================
来源：http://nu.hahajie.cn

E. 字符串处理
来源：http://fu.shxzskj.cn

================================================================================
来源：http://hm.szxytkj.cn

[E01] 拼接字符串
来源：http://km.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oc.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ki.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aw.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qj.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pe.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cj.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eh.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eu.lnxyls.cn

[E02] 重复字符串
来源：http://sd.bjjhwx.cn

Py:   "ab" * 3
来源：http://ok.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://bq.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://nl.newstarts.cn

TS:   "ab".repeat(3)
来源：http://qg.colortex.cn

Java: "ab".repeat(3)
来源：http://hc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://hy.nicolike.cn

Ruby: "ab" * 3
来源：http://by.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kj.nszjky.cn

[E03] 截取子串
来源：http://pw.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mc.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bn.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mv.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://ls.panjiajie.cn

Java: s.substring(1, 4)
来源：http://xk.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sv.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yo.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://kc.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://cb.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://iz.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://fi.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ke.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://vz.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://bh.521024.cn

Go:   strings.Index(s, "x")
来源：http://fk.shxzskj.cn

Ruby: s.index("x")
来源：http://aq.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://pw.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dz.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wr.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nk.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mx.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rr.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wd.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://op.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wo.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ha.huixinmuqiang.cn

[E06] 替换子串
来源：http://cc.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wq.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://lb.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://la.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://te.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tc.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rb.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hq.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://yu.hnjuh.cn

[E07] 按分隔符拆分
来源：http://tq.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aj.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fs.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ua.shxzukj.cn

TS:   s.split(",")
来源：http://kr.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fa.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jt.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://on.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qs.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ww.shxzukj.cn

Py:   ",".join(items)
来源：http://zx.hnjuh.cn

PHP:  implode(",", $items);
来源：http://yv.bookmarksfly.cn

JS:   items.join(",")
来源：http://ay.521024.cn

TS:   items.join(",")
来源：http://kw.colortex.cn

Java: String.join(",", items)
来源：http://bh.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://kk.shxzskj.cn

Ruby: items.join(",")
来源：http://qn.nszjky.cn

C#:   string.Join(",", items)
来源：http://zg.colortex.cn

[E09] 去除所有空白字符
来源：http://he.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://du.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pk.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://cc.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://id.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://fa.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cx.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://it.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gs.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://md.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tv.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wg.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://gx.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://vd.newstarts.cn

Java: String.format("%03d", 7)
来源：http://kx.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vs.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://db.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://is.nicolike.cn

[E11] 反转字符串
来源：http://qh.gzmigu.cn

Py:   s[::-1]
来源：http://sn.szsharing.cn

PHP:  strrev($s);
来源：http://qu.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ui.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://yb.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://il.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ww.chemitech.net.cn

Ruby: s.reverse
来源：http://el.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sv.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://tg.huixiangedu.cn

Py:   s.count("a")
来源：http://vj.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://bu.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://ny.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://ic.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://el.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://tn.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://ra.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://te.huixiangedu.cn

[E13] 逐字符遍历
来源：http://hk.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://bd.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rj.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://va.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wk.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ld.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tq.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kw.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jv.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://sx.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gx.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hk.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dp.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fr.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jj.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nr.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sp.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ze.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://hg.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://un.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yy.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xe.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qd.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iv.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vy.asd995.cn

[E16] 数字千分位
来源：http://da.nszjky.cn

Py:   f"{1234567:,}"
来源：http://hy.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://yt.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ti.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tl.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cp.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wp.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xx.asd995.cn

C#:   1234567.ToString("N0")
来源：http://kv.nszjky.cn

[E17] 首字母大写
来源：http://wn.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ux.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pn.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lk.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xp.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vg.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dh.shxzskj.cn

Ruby: s.capitalize
来源：http://gs.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zc.newstarts.cn

[E18] 模板占位符替换
来源：http://qu.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sq.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nu.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://na.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cd.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nj.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xz.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xp.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tt.colortex.cn

[E19] 多行文本按行拆分
来源：http://cs.bjjhwx.cn

Py:   s.splitlines()
来源：http://yl.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hv.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://op.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://dn.gzmigu.cn

Java: s.lines().toList()
来源：http://jn.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://kl.jctech888.com.cn

Ruby: s.lines
来源：http://pb.9csxet.cn

C#:   s.Split('\n')
来源：http://lv.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://gh.shtwfgs.cn

Py:   if not s:
来源：http://vs.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qo.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ro.shxzskj.cn

TS:   if (s === "") {}
来源：http://ou.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://hy.bjjhwx.cn

Go:   if s == "" {}
来源：http://ld.szxytkj.cn

Ruby: if s.empty?
来源：http://qb.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ve.lnxyls.cn

[E21] 超长截断加省略号
来源：http://ps.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zl.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bu.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cc.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vs.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ie.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ej.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ak.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gi.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://kw.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eo.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fz.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fm.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vs.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vh.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jd.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://vm.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://og.bjjhwx.cn

================================================================================
来源：http://kq.huanxung.cn

F. 文件与目录
来源：http://iv.muxihuayi.cn

================================================================================
来源：http://vv.chemitech.net.cn


<!-- 参考信息 -->