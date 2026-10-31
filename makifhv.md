代发 wailian999

TS:   [...new Set(arr)]
来源：http://pe.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ex.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wm.shtwfgs.cn

Ruby: arr.uniq
来源：http://cd.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://la.jctech888.com.cn

[D16] 求和与平均值
来源：http://hq.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qk.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://li.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://px.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fe.huanxung.cn

Go:   // 手写循环累加
来源：http://eb.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://he.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://uk.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://fc.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://fy.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://tv.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://of.nszjky.cn

TS:   Math.max(...arr);
来源：http://cs.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aa.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ww.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://qd.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://eo.521024.cn

[D18] 扁平化嵌套数组
来源：http://py.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://me.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://yg.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eg.shtwfgs.cn

TS:   nested.flat();
来源：http://zq.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hu.haigaiapp.cn

Go:   // 手写双层循环
来源：http://fe.hnjuh.cn

Ruby: nested.flatten
来源：http://bt.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tm.bjjhwx.cn

[D19] 按字段分组
来源：http://ev.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qv.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mu.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mo.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mw.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ae.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://qh.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gi.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yk.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ky.shtwfgs.cn

Py:   Counter(arr)
来源：http://ow.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://ll.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ps.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dz.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uf.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://hq.hahajie.cn

Ruby: arr.tally
来源：http://ow.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ev.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://xq.hahajie.cn

Py:   x in arr
来源：http://oc.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://pf.nicolike.cn

JS:   arr.includes(x)
来源：http://aa.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ad.wgjwhj.cn

Java: list.contains(x)
来源：http://jh.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://ly.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://na.gzmigu.cn

C#:   list.Contains(x)
来源：http://yu.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ft.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lb.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dd.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bi.szxytkj.cn

TS:   [...arr];
来源：http://gu.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://go.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qu.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://ol.szsharing.cn

C#:   new List<int>(list);
来源：http://nb.shtwfgs.cn

[D23] reduce 累积计算
来源：http://rc.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gi.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ia.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pn.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nj.haigaiapp.cn

Go:   // 手写循环
来源：http://bu.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wf.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ra.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ec.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ap.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gv.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ok.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rm.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wq.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qn.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sr.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://id.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ow.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kl.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mx.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ka.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zk.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vp.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pd.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tv.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ka.gzmigu.cn

[D26] 数组转字符串
来源：http://op.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://br.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://qr.newstarts.cn

JS:   arr.join(", ")
来源：http://nr.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://mb.szxytkj.cn

Java: String.join(", ", list)
来源：http://lt.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://ln.shxzskj.cn

Ruby: arr.join(", ")
来源：http://tg.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://el.wgjwhj.cn

================================================================================
来源：http://gr.jianghongdianzi.cn

E. 字符串处理
来源：http://hn.szxytkj.cn

================================================================================
来源：http://cn.521024.cn

[E01] 拼接字符串
来源：http://dm.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lc.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bz.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lg.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pw.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xo.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fu.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://or.muxihuayi.cn

[E02] 重复字符串
来源：http://bv.bookmarksfly.cn

Py:   "ab" * 3
来源：http://xj.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://vf.colortex.cn

JS:   "ab".repeat(3)
来源：http://lu.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://tp.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ho.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://np.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://rm.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vm.haigaiapp.cn

[E03] 截取子串
来源：http://rd.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hs.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hj.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gg.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ot.hnjuh.cn

Java: s.substring(1, 4)
来源：http://yb.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aj.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pw.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://so.panjiajie.cn

[E04] 查找子串位置
来源：http://na.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://oy.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://ix.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sz.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://wr.asd995.cn

Java: s.indexOf("x")
来源：http://nq.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://er.newstarts.cn

Ruby: s.index("x")
来源：http://jr.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ze.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://op.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qt.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cs.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ak.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lj.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dt.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rw.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tm.huixiangedu.cn

[E06] 替换子串
来源：http://fc.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://py.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://gx.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fz.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://eg.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nb.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gx.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sf.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://gn.shxzskj.cn

[E07] 按分隔符拆分
来源：http://la.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://as.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ki.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oq.nicolike.cn

TS:   s.split(",")
来源：http://bq.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nd.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kn.521024.cn

Ruby: s.split(",");  s.split
来源：http://jx.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://og.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ju.chemitech.net.cn

Py:   ",".join(items)
来源：http://td.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://nb.bookmarksfly.cn

JS:   items.join(",")
来源：http://ld.bookmarksfly.cn

TS:   items.join(",")
来源：http://ke.newstarts.cn

Java: String.join(",", items)
来源：http://gl.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://qu.nszjky.cn

Ruby: items.join(",")
来源：http://kl.szsharing.cn

C#:   string.Join(",", items)
来源：http://og.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://qi.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wa.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nu.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://rj.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://tg.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://xv.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://he.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qs.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wm.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://aw.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ih.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xc.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://up.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://to.hahajie.cn

Java: String.format("%03d", 7)
来源：http://df.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://va.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mk.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://id.wgjwhj.cn

[E11] 反转字符串
来源：http://tq.yuexingan06.cn

Py:   s[::-1]
来源：http://ot.shtwfgs.cn

PHP:  strrev($s);
来源：http://fm.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://lf.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://tq.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ns.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lo.jianghongdianzi.cn

Ruby: s.reverse
来源：http://dq.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ym.hahajie.cn

[E12] 统计某字符出现次数
来源：http://hg.9csxet.cn

Py:   s.count("a")
来源：http://wz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://ga.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://mm.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://qn.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ms.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://qt.9csxet.cn

Ruby: s.count("a")
来源：http://ui.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://xv.szsharing.cn

[E13] 逐字符遍历
来源：http://nl.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://zn.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hn.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tv.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ez.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dg.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ug.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ko.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hj.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://we.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bx.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eh.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vs.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iq.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oq.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vz.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pj.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mh.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://xg.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ur.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://az.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uu.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fn.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hn.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://at.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zx.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qq.szxytkj.cn

[E16] 数字千分位
来源：http://yl.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://cv.huanxung.cn

PHP:  number_format(1234567);
来源：http://sp.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://km.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ac.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ef.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rg.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://st.colortex.cn

C#:   1234567.ToString("N0")
来源：http://gt.huanxung.cn

[E17] 首字母大写
来源：http://au.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uy.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ly.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://it.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ck.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qy.lnxyls.cn

Ruby: s.capitalize
来源：http://ym.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bc.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://hn.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sj.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bl.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cz.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qc.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wl.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ai.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nm.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kp.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://gg.muxihuayi.cn

Py:   s.splitlines()
来源：http://gl.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ut.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://lv.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://ew.shtwfgs.cn

Java: s.lines().toList()
来源：http://lm.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://bo.hahajie.cn

Ruby: s.lines
来源：http://rk.shtwfgs.cn

C#:   s.Split('\n')
来源：http://id.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://cu.panjiajie.cn

Py:   if not s:
来源：http://la.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fi.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yl.colortex.cn

TS:   if (s === "") {}
来源：http://sx.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://pd.bookmarksfly.cn

Go:   if s == "" {}
来源：http://sb.9csxet.cn

Ruby: if s.empty?
来源：http://mq.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ac.nszjky.cn

[E21] 超长截断加省略号
来源：http://nb.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tr.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ek.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gf.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lu.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mq.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://df.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nw.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fn.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://na.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://il.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qa.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zp.nszjky.cn


<!-- 参考信息 -->