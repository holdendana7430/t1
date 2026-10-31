代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hv.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rm.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://of.shtwfgs.cn

Go:   // 手写循环累加
来源：http://wy.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tg.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://wb.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://ip.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://ex.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ux.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ad.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://hg.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mf.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jc.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ak.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://fw.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ky.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jq.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ol.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://di.wgjwhj.cn

TS:   nested.flat();
来源：http://nl.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ne.szsharing.cn

Go:   // 手写双层循环
来源：http://pk.bookmarksfly.cn

Ruby: nested.flatten
来源：http://vo.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sd.gzmigu.cn

[D19] 按字段分组
来源：http://rr.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uk.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fu.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kn.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rp.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ek.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://hg.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lw.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://de.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ic.9csxet.cn

Py:   Counter(arr)
来源：http://et.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://qg.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bs.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vj.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sb.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://tm.yuexingan06.cn

Ruby: arr.tally
来源：http://ng.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tz.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://rd.shxzskj.cn

Py:   x in arr
来源：http://sf.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://ly.jctech888.com.cn

JS:   arr.includes(x)
来源：http://cv.lnxyls.cn

TS:   arr.includes(x)
来源：http://hn.521024.cn

Java: list.contains(x)
来源：http://ho.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://bn.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://py.nszjky.cn

C#:   list.Contains(x)
来源：http://ph.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ok.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mh.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wf.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ac.nszjky.cn

TS:   [...arr];
来源：http://vn.colortex.cn

Java: new ArrayList<>(list);
来源：http://wf.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ol.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://by.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://dq.521024.cn

[D23] reduce 累积计算
来源：http://wj.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lx.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://op.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lo.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hs.hnjuh.cn

Go:   // 手写循环
来源：http://vq.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://za.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mw.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://wr.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sp.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ww.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bh.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sd.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xh.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dk.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kr.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://un.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ap.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nq.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ae.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ju.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iw.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qz.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gk.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yp.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qf.haigaiapp.cn

[D26] 数组转字符串
来源：http://az.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://ze.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://de.wgjwhj.cn

JS:   arr.join(", ")
来源：http://kt.wgjwhj.cn

TS:   arr.join(", ")
来源：http://ul.yuexingan06.cn

Java: String.join(", ", list)
来源：http://kw.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://hs.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://bs.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://pj.jianghongdianzi.cn

================================================================================
来源：http://zr.shxzskj.cn

E. 字符串处理
来源：http://py.bjjhwx.cn

================================================================================
来源：http://er.yuexingan06.cn

[E01] 拼接字符串
来源：http://pk.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ut.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tw.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ol.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fa.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ne.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ad.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yx.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ex.hahajie.cn

[E02] 重复字符串
来源：http://pw.nicolike.cn

Py:   "ab" * 3
来源：http://yb.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://am.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://oa.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://qb.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://tn.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://sm.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://zw.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qp.hahajie.cn

[E03] 截取子串
来源：http://zt.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jk.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hn.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nh.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://kb.asd995.cn

Java: s.substring(1, 4)
来源：http://vr.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gc.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ny.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://mr.nszjky.cn

[E04] 查找子串位置
来源：http://vb.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://hl.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://xo.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hj.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://cl.asd995.cn

Java: s.indexOf("x")
来源：http://ij.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://wr.bjjhwx.cn

Ruby: s.index("x")
来源：http://pb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ai.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qm.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ce.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lj.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://po.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zp.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zs.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ck.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vr.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uy.bjjhwx.cn

[E06] 替换子串
来源：http://aa.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uc.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://he.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mp.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://zc.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uz.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gu.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uc.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://vl.521024.cn

[E07] 按分隔符拆分
来源：http://pz.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qj.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bs.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yx.jctech888.com.cn

TS:   s.split(",")
来源：http://iq.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yl.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://be.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ky.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wc.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://dz.haigaiapp.cn

Py:   ",".join(items)
来源：http://dx.szsharing.cn

PHP:  implode(",", $items);
来源：http://js.hahajie.cn

JS:   items.join(",")
来源：http://ht.gzmigu.cn

TS:   items.join(",")
来源：http://vx.hnjuh.cn

Java: String.join(",", items)
来源：http://ek.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://lo.lnxyls.cn

Ruby: items.join(",")
来源：http://bp.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://to.newstarts.cn

[E09] 去除所有空白字符
来源：http://wn.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vh.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ym.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://fo.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://op.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://sc.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jo.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bc.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://ka.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://co.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xe.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://oc.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://mg.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://os.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ej.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jg.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ga.jianghongdianzi.cn

[E11] 反转字符串
来源：http://jt.hahajie.cn

Py:   s[::-1]
来源：http://jg.521024.cn

PHP:  strrev($s);
来源：http://vd.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://vw.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://jv.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jt.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cu.szxytkj.cn

Ruby: s.reverse
来源：http://vv.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ar.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://zi.huixinmuqiang.cn

Py:   s.count("a")
来源：http://qk.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ew.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://we.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ev.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rp.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://ow.nicolike.cn

Ruby: s.count("a")
来源：http://hw.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://hx.asd995.cn

[E13] 逐字符遍历
来源：http://yu.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://td.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kv.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gu.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mg.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sd.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tr.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jf.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://il.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://db.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nh.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kc.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rm.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vt.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://js.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lc.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fi.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://br.521024.cn

[E15] HTML 转义 / 反转义
来源：http://tt.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://my.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mq.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mu.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zu.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uc.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://el.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://np.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zx.lnxyls.cn

[E16] 数字千分位
来源：http://lj.hahajie.cn

Py:   f"{1234567:,}"
来源：http://gk.newstarts.cn

PHP:  number_format(1234567);
来源：http://ct.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cg.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fz.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vs.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bm.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lz.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ep.lnxyls.cn

[E17] 首字母大写
来源：http://bf.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xe.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ln.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gy.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bn.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ha.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rn.bookmarksfly.cn

Ruby: s.capitalize
来源：http://qy.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ch.jctech888.com.cn

[E18] 模板占位符替换
来源：http://xf.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pc.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://po.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://he.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iy.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iy.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xo.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://je.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pl.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://nj.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://df.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gd.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://yr.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ku.jctech888.com.cn

Java: s.lines().toList()
来源：http://jn.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://dj.huixinmuqiang.cn

Ruby: s.lines
来源：http://md.muxihuayi.cn

C#:   s.Split('\n')
来源：http://mk.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://px.asd995.cn

Py:   if not s:
来源：http://yh.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dw.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://db.asd995.cn

TS:   if (s === "") {}
来源：http://oz.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://my.hnjuh.cn

Go:   if s == "" {}
来源：http://jz.chemitech.net.cn

Ruby: if s.empty?
来源：http://rr.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ms.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://nm.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vu.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ok.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://an.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pd.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vk.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://pn.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qe.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kc.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://wx.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ms.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ak.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://va.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tb.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ch.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eq.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://hs.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mk.szxytkj.cn

================================================================================
来源：http://xf.wgjwhj.cn

F. 文件与目录
来源：http://ca.nszjky.cn

================================================================================
来源：http://bb.huixinmuqiang.cn


<!-- 参考信息 -->