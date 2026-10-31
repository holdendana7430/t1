代发 wailian999

TS:   [...new Set(arr)]
来源：http://as.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mw.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zq.szxytkj.cn

Ruby: arr.uniq
来源：http://lp.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://en.shtwfgs.cn

[D16] 求和与平均值
来源：http://ya.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bd.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ll.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uk.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jg.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bj.haigaiapp.cn

Go:   // 手写循环累加
来源：http://oj.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sk.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://jv.nszjky.cn

[D17] 最大值与最小值
来源：http://vt.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://vr.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ok.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jc.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://wi.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kx.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bg.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://ut.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://jc.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://jo.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fz.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://ie.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ss.panjiajie.cn

TS:   nested.flat();
来源：http://ve.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://he.lnxyls.cn

Go:   // 手写双层循环
来源：http://py.yuexingan06.cn

Ruby: nested.flatten
来源：http://vr.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dx.huixiangedu.cn

[D19] 按字段分组
来源：http://zg.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pj.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ce.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ee.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://js.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hi.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://oz.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bi.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eg.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://ey.colortex.cn

Py:   Counter(arr)
来源：http://yc.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://cn.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://am.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bo.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kb.nszjky.cn

Go:   // 手写 map[T]int
来源：http://qi.lnxyls.cn

Ruby: arr.tally
来源：http://cy.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bm.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://il.nicolike.cn

Py:   x in arr
来源：http://pm.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ia.szxytkj.cn

JS:   arr.includes(x)
来源：http://rv.gzmigu.cn

TS:   arr.includes(x)
来源：http://hx.shtwfgs.cn

Java: list.contains(x)
来源：http://iv.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://pk.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://lj.nszjky.cn

C#:   list.Contains(x)
来源：http://me.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://jr.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://se.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ig.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://us.szxytkj.cn

TS:   [...arr];
来源：http://cc.newstarts.cn

Java: new ArrayList<>(list);
来源：http://cn.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ep.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://qe.shxzukj.cn

C#:   new List<int>(list);
来源：http://uf.nicolike.cn

[D23] reduce 累积计算
来源：http://bs.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qy.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cq.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://na.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://en.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eq.9csxet.cn

Go:   // 手写循环
来源：http://qp.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yc.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://em.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://sb.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eu.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ni.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rv.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ms.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fs.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ms.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rh.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cn.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://yl.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zb.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jp.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tc.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hl.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://al.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://co.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dy.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pl.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://ap.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://qw.colortex.cn

PHP:  implode(", ", $arr);
来源：http://hd.szsharing.cn

JS:   arr.join(", ")
来源：http://yv.newstarts.cn

TS:   arr.join(", ")
来源：http://wa.asd995.cn

Java: String.join(", ", list)
来源：http://kl.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://rh.colortex.cn

Ruby: arr.join(", ")
来源：http://ll.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ig.colortex.cn

================================================================================
来源：http://tt.huixiangedu.cn

E. 字符串处理
来源：http://vu.jctech888.com.cn

================================================================================
来源：http://rv.521024.cn

[E01] 拼接字符串
来源：http://gv.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ky.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cp.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://me.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zl.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ks.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sm.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://si.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ml.hnjuh.cn

[E02] 重复字符串
来源：http://bz.yuexingan06.cn

Py:   "ab" * 3
来源：http://yl.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://yb.asd995.cn

JS:   "ab".repeat(3)
来源：http://rb.hahajie.cn

TS:   "ab".repeat(3)
来源：http://bv.colortex.cn

Java: "ab".repeat(3)
来源：http://oa.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ic.jctech888.com.cn

Ruby: "ab" * 3
来源：http://mz.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fk.yuexingan06.cn

[E03] 截取子串
来源：http://tr.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ai.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fz.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dn.huanxung.cn

TS:   s.slice(1, 4)
来源：http://zh.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://ut.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ve.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cy.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://cm.huixiangedu.cn

[E04] 查找子串位置
来源：http://jx.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://nh.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://yl.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://em.colortex.cn

TS:   s.indexOf("x")
来源：http://rm.shtwfgs.cn

Java: s.indexOf("x")
来源：http://zw.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://sm.lnxyls.cn

Ruby: s.index("x")
来源：http://pc.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://pu.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zj.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fp.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mn.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yz.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yr.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yd.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uw.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ba.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dw.jctech888.com.cn

[E06] 替换子串
来源：http://ks.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xt.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://xt.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sj.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://er.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ck.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://od.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ta.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://zd.szxytkj.cn

[E07] 按分隔符拆分
来源：http://sp.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fl.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://za.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ms.chemitech.net.cn

TS:   s.split(",")
来源：http://pg.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vz.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qv.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://mv.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yo.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://sz.asd995.cn

Py:   ",".join(items)
来源：http://ga.newstarts.cn

PHP:  implode(",", $items);
来源：http://bw.nszjky.cn

JS:   items.join(",")
来源：http://mv.nszjky.cn

TS:   items.join(",")
来源：http://xn.jctech888.com.cn

Java: String.join(",", items)
来源：http://bv.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://xd.shtwfgs.cn

Ruby: items.join(",")
来源：http://mq.lnxyls.cn

C#:   string.Join(",", items)
来源：http://xd.huanxung.cn

[E09] 去除所有空白字符
来源：http://lo.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hg.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yx.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://nw.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ef.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ov.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://li.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sx.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fy.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://pu.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gk.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://we.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ul.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ez.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://ym.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://op.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cz.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ig.yuntaijiaju.cn

[E11] 反转字符串
来源：http://ya.hahajie.cn

Py:   s[::-1]
来源：http://or.chemitech.net.cn

PHP:  strrev($s);
来源：http://ek.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://ue.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://ah.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yk.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rc.521024.cn

Ruby: s.reverse
来源：http://ms.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ga.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://uo.panjiajie.cn

Py:   s.count("a")
来源：http://oy.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://oz.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://uv.szsharing.cn

TS:   s.split("a").length - 1
来源：http://nv.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ic.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://if.szxytkj.cn

Ruby: s.count("a")
来源：http://vf.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://pn.szsharing.cn

[E13] 逐字符遍历
来源：http://oh.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ls.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bi.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qu.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ya.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qi.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ir.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dq.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iz.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://cu.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mc.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gr.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zr.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iw.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://on.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ec.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kd.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qx.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://fg.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uz.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xn.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ep.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ty.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wk.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oa.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xi.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://so.yuntaijiaju.cn

[E16] 数字千分位
来源：http://lk.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://fz.asd995.cn

PHP:  number_format(1234567);
来源：http://xg.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://np.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ev.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ut.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eb.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sl.521024.cn

C#:   1234567.ToString("N0")
来源：http://la.muxihuayi.cn

[E17] 首字母大写
来源：http://pz.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rz.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zj.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hc.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bs.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bq.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ra.jctech888.com.cn

Ruby: s.capitalize
来源：http://vs.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iv.jctech888.com.cn

[E18] 模板占位符替换
来源：http://ns.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qa.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zb.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hu.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zt.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hu.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://au.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uk.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pv.hahajie.cn

[E19] 多行文本按行拆分
来源：http://de.chemitech.net.cn

Py:   s.splitlines()
来源：http://rf.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nd.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ph.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://ut.panjiajie.cn

Java: s.lines().toList()
来源：http://xc.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://wy.wgjwhj.cn

Ruby: s.lines
来源：http://oi.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ev.521024.cn

[E20] 判断字符串是否为空
来源：http://tq.chemitech.net.cn

Py:   if not s:
来源：http://fp.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://om.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rl.asd995.cn

TS:   if (s === "") {}
来源：http://qq.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://wu.asd995.cn

Go:   if s == "" {}
来源：http://qj.521024.cn

Ruby: if s.empty?
来源：http://fz.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bu.colortex.cn

[E21] 超长截断加省略号
来源：http://ge.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dy.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yq.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nb.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yv.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sa.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://ya.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ph.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pi.huanxung.cn

[E22] 字节长度与字符长度
来源：http://pn.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oo.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eh.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nj.shtwfgs.cn


<!-- 参考信息 -->