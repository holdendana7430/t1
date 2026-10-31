代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zb.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gl.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mf.shxzukj.cn

Go:   // 手写循环累加
来源：http://zg.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pn.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://uc.newstarts.cn

[D17] 最大值与最小值
来源：http://hj.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://sh.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ha.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qp.nicolike.cn

TS:   Math.max(...arr);
来源：http://mu.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yw.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nz.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://wp.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://gr.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://gq.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sj.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://vi.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ja.jianghongdianzi.cn

TS:   nested.flat();
来源：http://mf.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xu.nicolike.cn

Go:   // 手写双层循环
来源：http://rc.gzmigu.cn

Ruby: nested.flatten
来源：http://jt.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tj.nicolike.cn

[D19] 按字段分组
来源：http://hu.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zh.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ww.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sd.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pz.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wa.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://dn.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qk.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eh.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://cn.bjjhwx.cn

Py:   Counter(arr)
来源：http://bv.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://zr.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bc.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://we.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://us.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ap.szxytkj.cn

Ruby: arr.tally
来源：http://pv.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nc.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://se.colortex.cn

Py:   x in arr
来源：http://wp.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://zj.nicolike.cn

JS:   arr.includes(x)
来源：http://xx.asd995.cn

TS:   arr.includes(x)
来源：http://mx.chemitech.net.cn

Java: list.contains(x)
来源：http://kl.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://qk.nszjky.cn

Ruby: arr.include?(x)
来源：http://op.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://ht.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://wf.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dl.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xk.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://or.521024.cn

TS:   [...arr];
来源：http://hc.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://wq.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hf.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://aw.shxzskj.cn

C#:   new List<int>(list);
来源：http://uv.chemitech.net.cn

[D23] reduce 累积计算
来源：http://hb.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ua.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cs.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qe.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ad.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ta.colortex.cn

Go:   // 手写循环
来源：http://qh.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://da.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vo.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://ly.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dv.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vv.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yj.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wk.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://df.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eg.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jl.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://cm.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wh.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eu.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eo.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eu.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aw.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rl.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://an.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://om.asd995.cn

[D26] 数组转字符串
来源：http://to.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://kg.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://du.nszjky.cn

JS:   arr.join(", ")
来源：http://ii.colortex.cn

TS:   arr.join(", ")
来源：http://hg.huanxung.cn

Java: String.join(", ", list)
来源：http://nu.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://as.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://yu.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://zq.huanxung.cn

================================================================================
来源：http://lt.huixiangedu.cn

E. 字符串处理
来源：http://gl.nszjky.cn

================================================================================
来源：http://lz.szxytkj.cn

[E01] 拼接字符串
来源：http://yb.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dk.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sp.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bm.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sc.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qy.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oq.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qh.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ub.chemitech.net.cn

[E02] 重复字符串
来源：http://nm.muxihuayi.cn

Py:   "ab" * 3
来源：http://ro.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://by.521024.cn

JS:   "ab".repeat(3)
来源：http://uh.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://uf.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://sp.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://je.hahajie.cn

Ruby: "ab" * 3
来源：http://zj.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bd.bjjhwx.cn

[E03] 截取子串
来源：http://dv.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pu.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mc.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://co.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ga.newstarts.cn

Java: s.substring(1, 4)
来源：http://pr.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://px.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pj.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://un.nicolike.cn

[E04] 查找子串位置
来源：http://cw.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://ff.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ec.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://et.colortex.cn

TS:   s.indexOf("x")
来源：http://lv.bjjhwx.cn

Java: s.indexOf("x")
来源：http://jf.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://jd.panjiajie.cn

Ruby: s.index("x")
来源：http://xd.nszjky.cn

C#:   s.IndexOf("x")
来源：http://fv.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mr.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hg.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tt.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vq.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tz.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xj.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ar.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ty.szsharing.cn

[E06] 替换子串
来源：http://te.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zy.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://hx.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://up.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://za.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://om.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vu.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tf.colortex.cn

C#:   s.Replace("a", "b")
来源：http://zz.newstarts.cn

[E07] 按分隔符拆分
来源：http://ni.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://or.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cw.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gn.colortex.cn

TS:   s.split(",")
来源：http://re.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kx.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dz.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://hp.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ip.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://ol.asd995.cn

Py:   ",".join(items)
来源：http://td.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://ae.shxzukj.cn

JS:   items.join(",")
来源：http://rg.yuntaijiaju.cn

TS:   items.join(",")
来源：http://bn.chemitech.net.cn

Java: String.join(",", items)
来源：http://cj.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://qm.szsharing.cn

Ruby: items.join(",")
来源：http://gb.szsharing.cn

C#:   string.Join(",", items)
来源：http://gb.newstarts.cn

[E09] 去除所有空白字符
来源：http://mz.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://he.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ru.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://nt.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://ds.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://yi.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vp.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ji.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://km.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://bw.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tx.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zi.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://sw.521024.cn

TS:   "7".padStart(3, "0")
来源：http://oy.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://lu.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bp.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fo.bjjhwx.cn

[E11] 反转字符串
来源：http://ov.haigaiapp.cn

Py:   s[::-1]
来源：http://ok.colortex.cn

PHP:  strrev($s);
来源：http://sd.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://gk.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ko.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ss.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vp.haigaiapp.cn

Ruby: s.reverse
来源：http://cm.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ot.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://sg.huanxung.cn

Py:   s.count("a")
来源：http://ie.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://kh.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://jj.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://fe.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ip.colortex.cn

Go:   strings.Count(s, "a")
来源：http://rc.colortex.cn

Ruby: s.count("a")
来源：http://id.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://sl.gzmigu.cn

[E13] 逐字符遍历
来源：http://hs.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://um.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uz.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mq.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cn.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fx.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uo.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cl.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bu.hahajie.cn

[E14] URL 编码与 Base64
来源：http://kh.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qn.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rt.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qa.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xy.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dw.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fl.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dt.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dw.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://on.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fn.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dm.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rd.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xr.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://js.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oo.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lt.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yx.szsharing.cn

[E16] 数字千分位
来源：http://hk.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://qp.shxzskj.cn

PHP:  number_format(1234567);
来源：http://yu.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ax.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hh.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lh.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ln.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cp.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://kg.hahajie.cn

[E17] 首字母大写
来源：http://yw.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yn.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oo.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aq.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nh.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hx.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qg.huixiangedu.cn

Ruby: s.capitalize
来源：http://zs.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dm.muxihuayi.cn

[E18] 模板占位符替换
来源：http://sf.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ui.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kq.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ul.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ks.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tn.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bx.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nu.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pc.newstarts.cn

[E19] 多行文本按行拆分
来源：http://xu.newstarts.cn

Py:   s.splitlines()
来源：http://vq.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ga.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://bl.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://tr.hahajie.cn

Java: s.lines().toList()
来源：http://sq.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://yl.huixinmuqiang.cn

Ruby: s.lines
来源：http://wc.yuexingan06.cn

C#:   s.Split('\n')
来源：http://zk.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://ev.shxzskj.cn

Py:   if not s:
来源：http://jn.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vc.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ky.huanxung.cn

TS:   if (s === "") {}
来源：http://ge.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://wg.lnxyls.cn

Go:   if s == "" {}
来源：http://ci.nszjky.cn

Ruby: if s.empty?
来源：http://gv.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ux.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://nb.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qm.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cb.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cp.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lh.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rs.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://hs.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ox.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ap.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://yz.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://di.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fy.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ld.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ji.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cp.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://af.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://hb.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://th.szxytkj.cn

================================================================================
来源：http://pp.asd995.cn

F. 文件与目录
来源：http://rc.9csxet.cn

================================================================================
来源：http://nb.hnjuh.cn


<!-- 参考信息 -->