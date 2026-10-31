代发 wailian999

C#:   list.Distinct().ToList()
来源：http://su.asd995.cn

[D16] 求和与平均值
来源：http://zk.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vr.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zn.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iv.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bd.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://et.lnxyls.cn

Go:   // 手写循环累加
来源：http://cj.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vu.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://jv.szxytkj.cn

[D17] 最大值与最小值
来源：http://ay.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://gt.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://ur.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pk.panjiajie.cn

TS:   Math.max(...arr);
来源：http://pa.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jm.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yc.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://yn.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://wb.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://xz.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ng.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://eh.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fp.bookmarksfly.cn

TS:   nested.flat();
来源：http://xh.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mq.nicolike.cn

Go:   // 手写双层循环
来源：http://va.jctech888.com.cn

Ruby: nested.flatten
来源：http://zo.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xf.colortex.cn

[D19] 按字段分组
来源：http://vj.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://df.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vh.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hn.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hv.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ch.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://fu.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qg.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cp.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://mh.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://xk.huanxung.cn

PHP:  array_count_values($arr);
来源：http://vb.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wl.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sr.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jy.szsharing.cn

Go:   // 手写 map[T]int
来源：http://vu.newstarts.cn

Ruby: arr.tally
来源：http://bl.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://si.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://vf.9csxet.cn

Py:   x in arr
来源：http://re.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://jr.nszjky.cn

JS:   arr.includes(x)
来源：http://mf.panjiajie.cn

TS:   arr.includes(x)
来源：http://ey.shxzukj.cn

Java: list.contains(x)
来源：http://zi.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://mz.nicolike.cn

Ruby: arr.include?(x)
来源：http://vw.nszjky.cn

C#:   list.Contains(x)
来源：http://bj.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://wd.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rn.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rs.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://on.colortex.cn

TS:   [...arr];
来源：http://gm.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ue.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ye.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://pe.szxytkj.cn

C#:   new List<int>(list);
来源：http://hy.shxzskj.cn

[D23] reduce 累积计算
来源：http://hl.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ov.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xf.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ei.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tt.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oo.bookmarksfly.cn

Go:   // 手写循环
来源：http://ol.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yq.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mx.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://yz.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pw.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ih.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qx.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mb.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qa.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gs.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pr.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qf.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://lh.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ig.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vf.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wx.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://km.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xh.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nk.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eb.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mk.shxzukj.cn

[D26] 数组转字符串
来源：http://ex.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://nt.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ip.shxzukj.cn

JS:   arr.join(", ")
来源：http://se.panjiajie.cn

TS:   arr.join(", ")
来源：http://dn.nszjky.cn

Java: String.join(", ", list)
来源：http://tj.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://oi.asd995.cn

Ruby: arr.join(", ")
来源：http://ut.asd995.cn

C#:   string.Join(", ", list)
来源：http://oj.muxihuayi.cn

================================================================================
来源：http://ql.shxzukj.cn

E. 字符串处理
来源：http://ul.huixiangedu.cn

================================================================================
来源：http://ug.szxytkj.cn

[E01] 拼接字符串
来源：http://an.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dd.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rk.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cv.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://st.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://on.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rd.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ih.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://me.yuntaijiaju.cn

[E02] 重复字符串
来源：http://be.haigaiapp.cn

Py:   "ab" * 3
来源：http://rb.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://th.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://ce.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://eu.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://hm.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://jd.shxzskj.cn

Ruby: "ab" * 3
来源：http://qr.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gi.hnjuh.cn

[E03] 截取子串
来源：http://wh.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eo.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ik.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lp.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://sh.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://fp.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sv.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ns.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://rg.huanxung.cn

[E04] 查找子串位置
来源：http://kq.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://wd.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://gj.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oa.hnjuh.cn

TS:   s.indexOf("x")
来源：http://rx.yuexingan06.cn

Java: s.indexOf("x")
来源：http://cs.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://rb.asd995.cn

Ruby: s.index("x")
来源：http://aq.521024.cn

C#:   s.IndexOf("x")
来源：http://wz.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oo.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fm.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ad.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ya.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wq.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fn.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oq.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gv.haigaiapp.cn

[E06] 替换子串
来源：http://zv.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lp.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://be.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fx.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://tm.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ns.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://se.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vc.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://zx.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://dl.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://me.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://va.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zx.szsharing.cn

TS:   s.split(",")
来源：http://rg.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nt.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://po.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://im.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iu.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://eq.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://wd.nszjky.cn

PHP:  implode(",", $items);
来源：http://mt.gzmigu.cn

JS:   items.join(",")
来源：http://tt.shtwfgs.cn

TS:   items.join(",")
来源：http://ul.colortex.cn

Java: String.join(",", items)
来源：http://tk.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ck.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://xq.hahajie.cn

C#:   string.Join(",", items)
来源：http://ia.newstarts.cn

[E09] 去除所有空白字符
来源：http://fa.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pu.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://av.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://cg.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ef.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://yh.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ok.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bp.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ph.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://ef.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bz.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vt.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://yj.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://zf.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://pr.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lw.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zy.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://os.asd995.cn

[E11] 反转字符串
来源：http://pv.hnjuh.cn

Py:   s[::-1]
来源：http://fl.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://jr.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://cy.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://eo.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fh.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zu.szsharing.cn

Ruby: s.reverse
来源：http://hz.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://th.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://zh.jctech888.com.cn

Py:   s.count("a")
来源：http://dn.521024.cn

PHP:  substr_count($s, "a");
来源：http://so.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://qk.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://ap.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xn.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://ga.szxytkj.cn

Ruby: s.count("a")
来源：http://gw.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://xn.bjjhwx.cn

[E13] 逐字符遍历
来源：http://wq.colortex.cn

Py:   for ch in s: print(ch)
来源：http://bl.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yo.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ut.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hj.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kv.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kj.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ju.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yi.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://ub.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xh.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rx.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wq.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cn.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hr.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xs.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kn.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wv.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://hw.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rd.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kv.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ud.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ud.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qr.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ps.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://go.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dr.panjiajie.cn

[E16] 数字千分位
来源：http://jo.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://qg.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://uf.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ga.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ia.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hn.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bd.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hi.colortex.cn

C#:   1234567.ToString("N0")
来源：http://jy.bjjhwx.cn

[E17] 首字母大写
来源：http://ox.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cf.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yo.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rn.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://do.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vc.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yl.nszjky.cn

Ruby: s.capitalize
来源：http://ry.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qj.newstarts.cn

[E18] 模板占位符替换
来源：http://lq.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fc.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gf.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yz.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nf.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kv.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zx.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jf.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://er.nszjky.cn

[E19] 多行文本按行拆分
来源：http://lb.nszjky.cn

Py:   s.splitlines()
来源：http://yx.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lf.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://bp.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://od.newstarts.cn

Java: s.lines().toList()
来源：http://sw.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://zt.nicolike.cn

Ruby: s.lines
来源：http://nd.lnxyls.cn

C#:   s.Split('\n')
来源：http://uc.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://vg.szsharing.cn

Py:   if not s:
来源：http://bw.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jd.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bb.shxzskj.cn

TS:   if (s === "") {}
来源：http://kr.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ge.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://yl.bjjhwx.cn

Ruby: if s.empty?
来源：http://at.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tb.hahajie.cn

[E21] 超长截断加省略号
来源：http://xw.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mj.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://su.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://as.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cc.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qi.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ic.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vx.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sb.newstarts.cn

[E22] 字节长度与字符长度
来源：http://og.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cj.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zm.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gi.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qt.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gz.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kr.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://pb.shxzskj.cn


<!-- 参考信息 -->