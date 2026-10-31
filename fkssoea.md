代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wm.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qn.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wn.huixiangedu.cn

Go:   // 手写循环累加
来源：http://nh.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://in.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://xb.huixiangedu.cn

[D17] 最大值与最小值
来源：http://uv.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://pt.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://ds.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ka.szsharing.cn

TS:   Math.max(...arr);
来源：http://ej.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ux.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vm.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://lz.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://kq.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://nu.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ng.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://en.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fj.nszjky.cn

TS:   nested.flat();
来源：http://ef.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pp.hahajie.cn

Go:   // 手写双层循环
来源：http://ib.huixiangedu.cn

Ruby: nested.flatten
来源：http://hd.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ux.yuexingan06.cn

[D19] 按字段分组
来源：http://mu.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ix.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qq.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ja.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ya.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ya.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://cq.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rp.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lq.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://vm.bookmarksfly.cn

Py:   Counter(arr)
来源：http://wi.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://lq.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ft.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://re.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wo.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://uu.shxzskj.cn

Ruby: arr.tally
来源：http://vm.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xx.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://cl.huixinmuqiang.cn

Py:   x in arr
来源：http://dd.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://vb.jctech888.com.cn

JS:   arr.includes(x)
来源：http://se.huanxung.cn

TS:   arr.includes(x)
来源：http://hd.521024.cn

Java: list.contains(x)
来源：http://eb.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ve.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://ha.bjjhwx.cn

C#:   list.Contains(x)
来源：http://ro.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://dp.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sv.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aa.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gn.jianghongdianzi.cn

TS:   [...arr];
来源：http://fw.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://dl.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xh.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://mk.szxytkj.cn

C#:   new List<int>(list);
来源：http://ni.shxzskj.cn

[D23] reduce 累积计算
来源：http://fh.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lq.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hs.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jb.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nr.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wa.wgjwhj.cn

Go:   // 手写循环
来源：http://ih.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nx.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zt.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://wf.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ef.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qj.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://km.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ti.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uj.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bv.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://up.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xv.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://hc.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sy.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hb.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wn.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ki.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dl.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rg.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gc.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zn.newstarts.cn

[D26] 数组转字符串
来源：http://yp.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://mx.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://xa.jctech888.com.cn

JS:   arr.join(", ")
来源：http://dq.hnjuh.cn

TS:   arr.join(", ")
来源：http://qm.hnjuh.cn

Java: String.join(", ", list)
来源：http://kb.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://hj.shxzskj.cn

Ruby: arr.join(", ")
来源：http://eo.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://uc.yuntaijiaju.cn

================================================================================
来源：http://do.521024.cn

E. 字符串处理
来源：http://xp.chemitech.net.cn

================================================================================
来源：http://gi.haigaiapp.cn

[E01] 拼接字符串
来源：http://bd.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ed.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zc.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gf.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lp.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ho.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qb.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qd.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fr.panjiajie.cn

[E02] 重复字符串
来源：http://dx.9csxet.cn

Py:   "ab" * 3
来源：http://nb.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://vp.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://js.huanxung.cn

TS:   "ab".repeat(3)
来源：http://tq.nszjky.cn

Java: "ab".repeat(3)
来源：http://ex.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://qw.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://vq.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nr.yuntaijiaju.cn

[E03] 截取子串
来源：http://mr.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bc.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://op.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ow.shxzukj.cn

Java: s.substring(1, 4)
来源：http://uw.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ch.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uz.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://zh.wgjwhj.cn

[E04] 查找子串位置
来源：http://xe.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://dw.colortex.cn

PHP:  strpos($s, "x");
来源：http://ch.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sn.szxytkj.cn

TS:   s.indexOf("x")
来源：http://iy.huanxung.cn

Java: s.indexOf("x")
来源：http://fj.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://rm.muxihuayi.cn

Ruby: s.index("x")
来源：http://tf.huanxung.cn

C#:   s.IndexOf("x")
来源：http://bp.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kk.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tu.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eu.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mx.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sr.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gj.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ek.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rb.lnxyls.cn

[E06] 替换子串
来源：http://em.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bi.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://gu.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ms.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://xo.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gu.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uj.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xg.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://oa.nszjky.cn

[E07] 按分隔符拆分
来源：http://sz.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sp.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ru.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qv.szsharing.cn

TS:   s.split(",")
来源：http://mh.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xi.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fj.asd995.cn

Ruby: s.split(",");  s.split
来源：http://th.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://in.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://vx.521024.cn

Py:   ",".join(items)
来源：http://oz.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://hc.szsharing.cn

JS:   items.join(",")
来源：http://pt.szsharing.cn

TS:   items.join(",")
来源：http://vd.shxzukj.cn

Java: String.join(",", items)
来源：http://ps.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://ut.newstarts.cn

Ruby: items.join(",")
来源：http://pb.nszjky.cn

C#:   string.Join(",", items)
来源：http://ai.asd995.cn

[E09] 去除所有空白字符
来源：http://ba.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bm.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ro.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://zg.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://sp.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://lb.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wd.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dy.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cc.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://hr.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rc.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uo.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://lz.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ni.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://bi.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sw.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rx.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wb.wgjwhj.cn

[E11] 反转字符串
来源：http://bf.szsharing.cn

Py:   s[::-1]
来源：http://jb.hahajie.cn

PHP:  strrev($s);
来源：http://tb.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://wp.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://js.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zv.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://no.9csxet.cn

Ruby: s.reverse
来源：http://ts.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://av.hahajie.cn

[E12] 统计某字符出现次数
来源：http://cm.shtwfgs.cn

Py:   s.count("a")
来源：http://yf.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://el.asd995.cn

JS:   s.split("a").length - 1
来源：http://qp.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://ob.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gc.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://jh.gzmigu.cn

Ruby: s.count("a")
来源：http://dp.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://hu.shxzskj.cn

[E13] 逐字符遍历
来源：http://su.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://su.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zc.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jg.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ln.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oj.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oi.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ok.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xf.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://uh.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nq.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rb.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://of.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vv.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ak.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://el.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wg.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xj.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://om.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ha.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kq.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cc.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jh.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dj.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yz.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xe.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wt.jianghongdianzi.cn

[E16] 数字千分位
来源：http://ie.nicolike.cn

Py:   f"{1234567:,}"
来源：http://sp.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ob.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sj.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ud.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ir.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wr.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eb.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://qg.hahajie.cn

[E17] 首字母大写
来源：http://eo.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dl.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wg.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mq.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://du.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kg.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cg.9csxet.cn

Ruby: s.capitalize
来源：http://kv.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fv.hahajie.cn

[E18] 模板占位符替换
来源：http://at.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mz.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kb.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gg.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yz.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ou.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jm.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zh.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yv.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://yn.lnxyls.cn

Py:   s.splitlines()
来源：http://ld.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://us.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://qz.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://nv.nszjky.cn

Java: s.lines().toList()
来源：http://ji.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ra.hahajie.cn

Ruby: s.lines
来源：http://zb.yuexingan06.cn

C#:   s.Split('\n')
来源：http://az.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://sc.colortex.cn

Py:   if not s:
来源：http://hc.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://br.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dc.muxihuayi.cn

TS:   if (s === "") {}
来源：http://qw.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://ua.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://cd.gzmigu.cn

Ruby: if s.empty?
来源：http://bz.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lv.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://no.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ou.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rl.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ru.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hu.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ek.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://fw.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ah.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cn.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://xi.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wj.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uo.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vq.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://st.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://al.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jj.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://gl.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ut.chemitech.net.cn

================================================================================
来源：http://ya.shtwfgs.cn

F. 文件与目录
来源：http://eg.huanxung.cn

================================================================================
来源：http://ag.haigaiapp.cn


<!-- 参考信息 -->