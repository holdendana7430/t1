代发 wailian999

C#:   list.Distinct().ToList()
来源：http://pz.newstarts.cn

[D16] 求和与平均值
来源：http://oh.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jn.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xq.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ua.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eu.haigaiapp.cn

Go:   // 手写循环累加
来源：http://xb.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mf.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ny.jctech888.com.cn

[D17] 最大值与最小值
来源：http://aj.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://dk.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://es.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mc.colortex.cn

TS:   Math.max(...arr);
来源：http://vr.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qc.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mb.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://qb.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://pr.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://up.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mp.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://nz.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ww.521024.cn

TS:   nested.flat();
来源：http://jw.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://df.huixiangedu.cn

Go:   // 手写双层循环
来源：http://uy.shxzskj.cn

Ruby: nested.flatten
来源：http://gg.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://as.nicolike.cn

[D19] 按字段分组
来源：http://un.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kb.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ij.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sd.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uw.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ho.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://um.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bl.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jb.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://wc.colortex.cn

Py:   Counter(arr)
来源：http://ug.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://yp.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rk.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zr.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://th.9csxet.cn

Go:   // 手写 map[T]int
来源：http://pg.colortex.cn

Ruby: arr.tally
来源：http://tg.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qa.szsharing.cn

[D21] 判断是否包含某元素
来源：http://oz.jianghongdianzi.cn

Py:   x in arr
来源：http://bh.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://md.szxytkj.cn

JS:   arr.includes(x)
来源：http://ou.huanxung.cn

TS:   arr.includes(x)
来源：http://cq.shtwfgs.cn

Java: list.contains(x)
来源：http://qo.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://et.lnxyls.cn

Ruby: arr.include?(x)
来源：http://rf.gzmigu.cn

C#:   list.Contains(x)
来源：http://vo.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://au.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pa.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lb.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://in.asd995.cn

TS:   [...arr];
来源：http://dt.newstarts.cn

Java: new ArrayList<>(list);
来源：http://sq.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eh.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://tv.szxytkj.cn

C#:   new List<int>(list);
来源：http://wy.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://hm.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kh.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mk.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fz.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://up.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uq.nszjky.cn

Go:   // 手写循环
来源：http://od.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://il.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oo.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://no.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hy.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kl.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://si.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://py.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yi.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fi.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fn.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://go.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://wl.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ee.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wr.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wq.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ts.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pj.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://re.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zi.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://he.bjjhwx.cn

[D26] 数组转字符串
来源：http://lu.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://ac.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://ev.nicolike.cn

JS:   arr.join(", ")
来源：http://wc.bjjhwx.cn

TS:   arr.join(", ")
来源：http://kz.shxzskj.cn

Java: String.join(", ", list)
来源：http://sc.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://xq.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://lo.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://oa.hnjuh.cn

================================================================================
来源：http://wi.newstarts.cn

E. 字符串处理
来源：http://yx.muxihuayi.cn

================================================================================
来源：http://xi.bjjhwx.cn

[E01] 拼接字符串
来源：http://tv.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ft.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mv.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dj.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tm.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://te.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xw.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ce.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jd.shxzskj.cn

[E02] 重复字符串
来源：http://ph.bjjhwx.cn

Py:   "ab" * 3
来源：http://ch.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://ij.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://fv.521024.cn

TS:   "ab".repeat(3)
来源：http://rg.nszjky.cn

Java: "ab".repeat(3)
来源：http://fe.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://fy.9csxet.cn

Ruby: "ab" * 3
来源：http://qg.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qt.shxzskj.cn

[E03] 截取子串
来源：http://dk.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fa.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eh.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qy.nicolike.cn

TS:   s.slice(1, 4)
来源：http://to.9csxet.cn

Java: s.substring(1, 4)
来源：http://aa.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vt.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cs.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://ao.nszjky.cn

[E04] 查找子串位置
来源：http://ab.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://ag.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://zc.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qo.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://vc.hahajie.cn

Java: s.indexOf("x")
来源：http://ri.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://hq.colortex.cn

Ruby: s.index("x")
来源：http://gn.huanxung.cn

C#:   s.IndexOf("x")
来源：http://wh.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ss.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ty.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fk.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cq.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ou.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xr.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ln.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wi.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fc.szxytkj.cn

[E06] 替换子串
来源：http://th.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qs.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://wh.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qg.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://if.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ha.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jx.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lu.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://ip.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://gc.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ue.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ya.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sd.hnjuh.cn

TS:   s.split(",")
来源：http://yb.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gc.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xd.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://da.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bi.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://my.jctech888.com.cn

Py:   ",".join(items)
来源：http://dq.shxzskj.cn

PHP:  implode(",", $items);
来源：http://xt.jctech888.com.cn

JS:   items.join(",")
来源：http://bd.wgjwhj.cn

TS:   items.join(",")
来源：http://yz.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://ct.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://zd.haigaiapp.cn

Ruby: items.join(",")
来源：http://eg.lnxyls.cn

C#:   string.Join(",", items)
来源：http://gk.nszjky.cn

[E09] 去除所有空白字符
来源：http://to.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tg.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://or.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://eq.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://kr.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://up.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ep.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pi.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kp.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://zn.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lp.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tc.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://xt.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://dn.asd995.cn

Java: String.format("%03d", 7)
来源：http://vl.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jy.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://by.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nl.shtwfgs.cn

[E11] 反转字符串
来源：http://oa.wgjwhj.cn

Py:   s[::-1]
来源：http://hm.haigaiapp.cn

PHP:  strrev($s);
来源：http://bz.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://wa.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://pf.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jm.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mo.nszjky.cn

Ruby: s.reverse
来源：http://ib.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vm.szsharing.cn

[E12] 统计某字符出现次数
来源：http://fp.yuntaijiaju.cn

Py:   s.count("a")
来源：http://gl.521024.cn

PHP:  substr_count($s, "a");
来源：http://ws.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://jh.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://jh.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qu.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://uc.huixiangedu.cn

Ruby: s.count("a")
来源：http://ig.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://ha.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://qy.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://vx.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fu.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bf.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://al.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://el.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://au.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://um.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pd.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://xt.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ek.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kt.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qs.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qz.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dy.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://up.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lg.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xd.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ri.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cd.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xj.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fw.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rt.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rf.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hk.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ym.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://al.yuntaijiaju.cn

[E16] 数字千分位
来源：http://vi.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://nt.szsharing.cn

PHP:  number_format(1234567);
来源：http://ni.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://np.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://og.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://su.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ou.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ga.521024.cn

C#:   1234567.ToString("N0")
来源：http://fh.jianghongdianzi.cn

[E17] 首字母大写
来源：http://zt.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oi.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yw.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xy.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xe.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://um.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wf.szxytkj.cn

Ruby: s.capitalize
来源：http://ic.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kh.jctech888.com.cn

[E18] 模板占位符替换
来源：http://fa.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xp.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qk.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ud.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fb.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wg.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sp.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ng.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://is.nicolike.cn

[E19] 多行文本按行拆分
来源：http://wa.hahajie.cn

Py:   s.splitlines()
来源：http://fj.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ed.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ql.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://rc.chemitech.net.cn

Java: s.lines().toList()
来源：http://dy.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://kk.nicolike.cn

Ruby: s.lines
来源：http://km.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://zg.asd995.cn

[E20] 判断字符串是否为空
来源：http://vg.9csxet.cn

Py:   if not s:
来源：http://bl.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ac.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jb.szsharing.cn

TS:   if (s === "") {}
来源：http://ak.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://od.521024.cn

Go:   if s == "" {}
来源：http://sf.haigaiapp.cn

Ruby: if s.empty?
来源：http://op.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fc.521024.cn

[E21] 超长截断加省略号
来源：http://hi.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hm.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cx.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qj.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://la.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ld.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://xy.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uh.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ty.huanxung.cn

[E22] 字节长度与字符长度
来源：http://sq.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ih.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aq.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://el.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kj.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ns.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://qq.panjiajie.cn


<!-- 参考信息 -->