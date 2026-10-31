代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wl.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://ti.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://zk.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://kq.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://tj.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://av.szxytkj.cn

TS:   Math.max(...arr);
来源：http://yg.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ky.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bz.colortex.cn

Ruby: arr.max;  arr.min
来源：http://hp.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://oq.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://cj.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jz.asd995.cn

PHP:  array_merge(...$nested);
来源：http://gb.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ev.yuntaijiaju.cn

TS:   nested.flat();
来源：http://nj.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uf.shxzukj.cn

Go:   // 手写双层循环
来源：http://fy.huanxung.cn

Ruby: nested.flatten
来源：http://nw.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cu.szxytkj.cn

[D19] 按字段分组
来源：http://gt.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ga.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bv.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yv.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xw.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zi.asd995.cn

Go:   // 手写 map[string][]T
来源：http://vb.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cd.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rv.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://tg.szsharing.cn

Py:   Counter(arr)
来源：http://tz.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://de.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fl.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bi.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://ib.9csxet.cn

Ruby: arr.tally
来源：http://if.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://il.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://lh.haigaiapp.cn

Py:   x in arr
来源：http://mj.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ra.hnjuh.cn

JS:   arr.includes(x)
来源：http://gg.shtwfgs.cn

TS:   arr.includes(x)
来源：http://tc.shxzskj.cn

Java: list.contains(x)
来源：http://jo.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://sq.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://sd.haigaiapp.cn

C#:   list.Contains(x)
来源：http://yw.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://ek.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wa.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gx.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aw.shxzskj.cn

TS:   [...arr];
来源：http://xq.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://wk.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://al.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://wa.hahajie.cn

C#:   new List<int>(list);
来源：http://xy.yuexingan06.cn

[D23] reduce 累积计算
来源：http://yy.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sm.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eb.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mm.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ca.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tr.9csxet.cn

Go:   // 手写循环
来源：http://mr.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sz.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ko.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://od.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oi.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nu.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kp.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bh.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oa.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eu.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fn.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ze.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://kj.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nq.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vc.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pj.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bs.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mx.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ux.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fo.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://im.bookmarksfly.cn

[D26] 数组转字符串
来源：http://mw.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://my.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://ho.szxytkj.cn

JS:   arr.join(", ")
来源：http://fs.nszjky.cn

TS:   arr.join(", ")
来源：http://il.huanxung.cn

Java: String.join(", ", list)
来源：http://ex.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://bx.gzmigu.cn

Ruby: arr.join(", ")
来源：http://je.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://va.shtwfgs.cn

================================================================================
来源：http://yk.bookmarksfly.cn

E. 字符串处理
来源：http://kk.hnjuh.cn

================================================================================
来源：http://ez.muxihuayi.cn

[E01] 拼接字符串
来源：http://zh.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ni.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mh.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ut.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://py.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ej.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wr.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ct.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bo.bjjhwx.cn

[E02] 重复字符串
来源：http://mr.colortex.cn

Py:   "ab" * 3
来源：http://ne.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://gb.hahajie.cn

JS:   "ab".repeat(3)
来源：http://lf.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://db.panjiajie.cn

Java: "ab".repeat(3)
来源：http://aw.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rd.521024.cn

Ruby: "ab" * 3
来源：http://aw.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gk.lnxyls.cn

[E03] 截取子串
来源：http://dv.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rr.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ae.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hf.hahajie.cn

TS:   s.slice(1, 4)
来源：http://ew.hahajie.cn

Java: s.substring(1, 4)
来源：http://ew.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ob.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://it.521024.cn

C#:   s.Substring(1, 3)
来源：http://ig.gzmigu.cn

[E04] 查找子串位置
来源：http://gp.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://hm.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://ce.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://df.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ul.521024.cn

Java: s.indexOf("x")
来源：http://le.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://zu.lnxyls.cn

Ruby: s.index("x")
来源：http://lr.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://hy.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mu.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://he.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uq.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hl.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pb.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uw.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hp.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qn.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hv.gzmigu.cn

[E06] 替换子串
来源：http://qj.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fy.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://di.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xg.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://wm.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ks.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ll.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wi.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://wp.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://lh.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oe.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ec.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bd.colortex.cn

TS:   s.split(",")
来源：http://kh.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mc.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://js.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://rv.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ly.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://fy.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://ih.huanxung.cn

PHP:  implode(",", $items);
来源：http://sw.haigaiapp.cn

JS:   items.join(",")
来源：http://io.huixiangedu.cn

TS:   items.join(",")
来源：http://sr.shxzskj.cn

Java: String.join(",", items)
来源：http://bv.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://bu.bookmarksfly.cn

Ruby: items.join(",")
来源：http://gx.asd995.cn

C#:   string.Join(",", items)
来源：http://gm.panjiajie.cn

[E09] 去除所有空白字符
来源：http://bn.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vv.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hj.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://bn.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://xu.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ij.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ww.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ix.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bm.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://mh.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nl.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ua.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://nc.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://ns.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://bp.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://up.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://em.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xy.nicolike.cn

[E11] 反转字符串
来源：http://xx.colortex.cn

Py:   s[::-1]
来源：http://xj.haigaiapp.cn

PHP:  strrev($s);
来源：http://ea.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ut.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://vi.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cd.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://az.haigaiapp.cn

Ruby: s.reverse
来源：http://ed.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ua.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://sg.jianghongdianzi.cn

Py:   s.count("a")
来源：http://cw.colortex.cn

PHP:  substr_count($s, "a");
来源：http://qf.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://af.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://rd.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ef.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://av.szxytkj.cn

Ruby: s.count("a")
来源：http://po.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://mx.szsharing.cn

[E13] 逐字符遍历
来源：http://fw.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://ig.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qk.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xl.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://we.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bf.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ky.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jo.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sw.newstarts.cn

[E14] URL 编码与 Base64
来源：http://xk.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cd.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nc.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sl.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ee.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cw.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eb.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hh.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bd.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ge.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vw.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ux.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nn.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://um.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rg.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pm.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nd.shxzukj.cn

[E16] 数字千分位
来源：http://ij.newstarts.cn

Py:   f"{1234567:,}"
来源：http://af.newstarts.cn

PHP:  number_format(1234567);
来源：http://tj.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bw.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dk.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bj.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tl.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ng.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://hw.asd995.cn

[E17] 首字母大写
来源：http://vt.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lb.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fd.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hp.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fl.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jj.colortex.cn

Ruby: s.capitalize
来源：http://mr.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dz.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://gy.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wo.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://am.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ym.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ez.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://af.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ui.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kb.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fm.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://kr.asd995.cn

Py:   s.splitlines()
来源：http://ef.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vh.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://ky.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://rs.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://tp.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://bl.chemitech.net.cn

Ruby: s.lines
来源：http://rc.huanxung.cn

C#:   s.Split('\n')
来源：http://co.9csxet.cn

[E20] 判断字符串是否为空
来源：http://qj.shxzskj.cn

Py:   if not s:
来源：http://sr.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zt.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kw.szxytkj.cn

TS:   if (s === "") {}
来源：http://bi.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://mb.shxzskj.cn

Go:   if s == "" {}
来源：http://fv.wgjwhj.cn

Ruby: if s.empty?
来源：http://dk.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ud.szxytkj.cn

[E21] 超长截断加省略号
来源：http://fw.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vf.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dx.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zs.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jp.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jw.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://go.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yq.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ae.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://zs.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ii.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jx.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mv.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vf.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kw.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oe.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://gg.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oq.jctech888.com.cn

================================================================================
来源：http://ia.wgjwhj.cn

F. 文件与目录
来源：http://kj.hnjuh.cn

================================================================================
来源：http://zu.muxihuayi.cn

[F01] 读取整个文件
来源：http://ku.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qz.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://fu.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jc.newstarts.cn


<!-- 参考信息 -->