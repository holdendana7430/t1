代发 wailian999

TS:   [...new Set(arr)]
来源：http://yh.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kk.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lk.chemitech.net.cn

Ruby: arr.uniq
来源：http://wq.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://zg.bookmarksfly.cn

[D16] 求和与平均值
来源：http://xs.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nk.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ey.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bv.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pj.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjjhwx.cn

Go:   // 手写循环累加
来源：http://rt.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yu.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://tv.bjjhwx.cn

[D17] 最大值与最小值
来源：http://fu.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://hy.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://fl.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eq.szsharing.cn

TS:   Math.max(...arr);
来源：http://az.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yk.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ik.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://lg.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://sq.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://zo.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iu.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://bw.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://my.bookmarksfly.cn

TS:   nested.flat();
来源：http://rj.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ga.521024.cn

Go:   // 手写双层循环
来源：http://jc.wgjwhj.cn

Ruby: nested.flatten
来源：http://sf.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sy.szsharing.cn

[D19] 按字段分组
来源：http://kd.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://do.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bt.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ja.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mj.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qk.521024.cn

Go:   // 手写 map[string][]T
来源：http://yr.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tc.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nm.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://xy.hahajie.cn

Py:   Counter(arr)
来源：http://ij.9csxet.cn

PHP:  array_count_values($arr);
来源：http://st.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oa.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zp.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ab.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ob.521024.cn

Ruby: arr.tally
来源：http://bx.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zu.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://cg.hahajie.cn

Py:   x in arr
来源：http://gq.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://io.bjjhwx.cn

JS:   arr.includes(x)
来源：http://po.9csxet.cn

TS:   arr.includes(x)
来源：http://zi.huanxung.cn

Java: list.contains(x)
来源：http://lx.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ph.newstarts.cn

Ruby: arr.include?(x)
来源：http://te.jctech888.com.cn

C#:   list.Contains(x)
来源：http://qd.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://tl.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vl.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nk.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fm.521024.cn

TS:   [...arr];
来源：http://fk.9csxet.cn

Java: new ArrayList<>(list);
来源：http://hd.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fm.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://hb.bjjhwx.cn

C#:   new List<int>(list);
来源：http://yz.colortex.cn

[D23] reduce 累积计算
来源：http://ya.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ur.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ck.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eu.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hc.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gj.gzmigu.cn

Go:   // 手写循环
来源：http://ez.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tq.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ig.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://mj.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vs.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gh.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kc.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vx.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bf.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qd.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uv.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oa.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://cp.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tp.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://za.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lk.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eb.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zg.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xu.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://el.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yw.9csxet.cn

[D26] 数组转字符串
来源：http://hw.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://cs.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://cn.yuexingan06.cn

JS:   arr.join(", ")
来源：http://xg.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://sl.wgjwhj.cn

Java: String.join(", ", list)
来源：http://mx.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://rj.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://lk.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://pb.huixinmuqiang.cn

================================================================================
来源：http://zn.chemitech.net.cn

E. 字符串处理
来源：http://ye.hnjuh.cn

================================================================================
来源：http://vj.shxzskj.cn

[E01] 拼接字符串
来源：http://pi.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cr.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qn.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rb.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ce.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wa.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://av.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nw.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yx.huixiangedu.cn

[E02] 重复字符串
来源：http://pz.bookmarksfly.cn

Py:   "ab" * 3
来源：http://to.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://as.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://np.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://vb.9csxet.cn

Java: "ab".repeat(3)
来源：http://th.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://tt.asd995.cn

Ruby: "ab" * 3
来源：http://cr.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zp.haigaiapp.cn

[E03] 截取子串
来源：http://fx.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bu.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wz.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dm.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://lz.colortex.cn

Java: s.substring(1, 4)
来源：http://ww.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rg.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zz.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://aa.shxzukj.cn

[E04] 查找子串位置
来源：http://gt.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://mc.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://sn.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://in.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://na.lnxyls.cn

Java: s.indexOf("x")
来源：http://gk.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://cg.asd995.cn

Ruby: s.index("x")
来源：http://ur.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://pk.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wc.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://br.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tj.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vu.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zc.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ye.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wp.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jp.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xg.asd995.cn

[E06] 替换子串
来源：http://mc.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gv.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://tf.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bn.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://sk.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tq.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ec.521024.cn

C#:   s.Replace("a", "b")
来源：http://da.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ar.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lc.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fe.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cs.shxzskj.cn

TS:   s.split(",")
来源：http://ud.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hb.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hy.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://jh.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ac.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://iy.colortex.cn

Py:   ",".join(items)
来源：http://xa.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://hw.szsharing.cn

JS:   items.join(",")
来源：http://th.panjiajie.cn

TS:   items.join(",")
来源：http://ht.9csxet.cn

Java: String.join(",", items)
来源：http://xf.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://dx.huixiangedu.cn

Ruby: items.join(",")
来源：http://zt.shxzskj.cn

C#:   string.Join(",", items)
来源：http://vq.panjiajie.cn

[E09] 去除所有空白字符
来源：http://qr.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://it.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ct.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://wj.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://cj.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ai.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zx.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://en.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pb.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://bn.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://he.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://co.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://vo.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://lx.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://yp.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ob.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wz.gzmigu.cn

[E11] 反转字符串
来源：http://oz.yuexingan06.cn

Py:   s[::-1]
来源：http://wb.asd995.cn

PHP:  strrev($s);
来源：http://ax.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://so.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://qy.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oa.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wv.lnxyls.cn

Ruby: s.reverse
来源：http://dz.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nt.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://my.newstarts.cn

Py:   s.count("a")
来源：http://ct.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://tj.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://bd.nicolike.cn

TS:   s.split("a").length - 1
来源：http://fx.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nv.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://nb.panjiajie.cn

Ruby: s.count("a")
来源：http://km.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://on.chemitech.net.cn

[E13] 逐字符遍历
来源：http://vm.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://hi.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zz.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gb.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vu.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cm.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jx.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ig.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://en.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://oq.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rb.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bj.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jb.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hh.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://af.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hk.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://et.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://np.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://yb.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dz.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mf.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://di.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pp.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ol.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qi.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sl.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ni.yuexingan06.cn

[E16] 数字千分位
来源：http://ob.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://gs.hnjuh.cn

PHP:  number_format(1234567);
来源：http://of.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qs.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ql.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kw.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://in.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fh.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://av.shxzskj.cn

[E17] 首字母大写
来源：http://ay.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eu.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sn.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cd.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bz.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tj.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ri.hnjuh.cn

Ruby: s.capitalize
来源：http://tx.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://st.huanxung.cn

[E18] 模板占位符替换
来源：http://ei.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fe.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pq.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bg.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gd.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wf.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mv.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yr.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wb.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://aj.muxihuayi.cn

Py:   s.splitlines()
来源：http://tz.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vp.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://zg.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://fe.gzmigu.cn

Java: s.lines().toList()
来源：http://jn.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://qh.bookmarksfly.cn

Ruby: s.lines
来源：http://pr.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://kx.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://xq.lnxyls.cn

Py:   if not s:
来源：http://fg.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nk.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zn.haigaiapp.cn

TS:   if (s === "") {}
来源：http://od.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://yu.bjjhwx.cn

Go:   if s == "" {}
来源：http://ul.nicolike.cn

Ruby: if s.empty?
来源：http://qs.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://is.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://tq.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lm.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lq.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wm.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hp.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pv.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://qa.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eb.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hi.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://rr.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wj.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hs.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ke.bjjhwx.cn


<!-- 参考信息 -->