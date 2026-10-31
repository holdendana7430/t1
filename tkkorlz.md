代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vc.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://bh.jctech888.com.cn

[D17] 最大值与最小值
来源：http://fm.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://cn.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://nt.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zp.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://un.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mu.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vf.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ub.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://kv.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://pm.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ox.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ff.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rg.huixinmuqiang.cn

TS:   nested.flat();
来源：http://hb.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sy.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://tx.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://rd.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uz.jctech888.com.cn

[D19] 按字段分组
来源：http://dt.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ff.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pj.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jr.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ws.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nu.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://zr.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ep.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xq.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://zf.yuexingan06.cn

Py:   Counter(arr)
来源：http://ki.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://dw.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ah.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xc.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pk.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://hh.szsharing.cn

Ruby: arr.tally
来源：http://zy.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sa.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://na.shxzukj.cn

Py:   x in arr
来源：http://kv.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://sh.hahajie.cn

JS:   arr.includes(x)
来源：http://mb.shtwfgs.cn

TS:   arr.includes(x)
来源：http://cv.colortex.cn

Java: list.contains(x)
来源：http://oz.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://vx.shxzskj.cn

Ruby: arr.include?(x)
来源：http://be.521024.cn

C#:   list.Contains(x)
来源：http://ot.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://cu.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xw.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ku.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xf.panjiajie.cn

TS:   [...arr];
来源：http://pr.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://me.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bf.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://bg.shxzskj.cn

C#:   new List<int>(list);
来源：http://mg.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://el.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ns.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bs.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rr.hahajie.cn

Go:   // 手写循环
来源：http://ot.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eg.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://od.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://lo.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jo.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zb.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kc.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fp.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gn.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://po.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aw.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hl.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://pp.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nu.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tn.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uz.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://en.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jy.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ca.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vs.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rk.521024.cn

[D26] 数组转字符串
来源：http://bn.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://fq.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://sz.nicolike.cn

JS:   arr.join(", ")
来源：http://wq.521024.cn

TS:   arr.join(", ")
来源：http://ee.panjiajie.cn

Java: String.join(", ", list)
来源：http://wn.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://vs.hahajie.cn

Ruby: arr.join(", ")
来源：http://nj.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://zk.colortex.cn

================================================================================
来源：http://bq.jctech888.com.cn

E. 字符串处理
来源：http://tt.hnjuh.cn

================================================================================
来源：http://nu.521024.cn

[E01] 拼接字符串
来源：http://oy.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yq.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dr.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bi.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qz.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mj.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ni.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wn.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ro.nszjky.cn

[E02] 重复字符串
来源：http://kn.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ex.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://nv.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://qh.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://wl.521024.cn

Java: "ab".repeat(3)
来源：http://bc.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://oa.asd995.cn

Ruby: "ab" * 3
来源：http://ln.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dm.9csxet.cn

[E03] 截取子串
来源：http://xi.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ne.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gr.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dw.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://pk.asd995.cn

Java: s.substring(1, 4)
来源：http://lu.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xb.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sx.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ks.bookmarksfly.cn

[E04] 查找子串位置
来源：http://un.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://fv.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://en.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://no.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://tn.gzmigu.cn

Java: s.indexOf("x")
来源：http://ib.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://gw.bjjhwx.cn

Ruby: s.index("x")
来源：http://jg.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://pn.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lx.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ol.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://te.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rt.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pq.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qa.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ni.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kj.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xr.huixinmuqiang.cn

[E06] 替换子串
来源：http://eb.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ge.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://ci.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qt.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://vb.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vk.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rr.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nf.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://aa.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ka.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mu.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fu.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://px.chemitech.net.cn

TS:   s.split(",")
来源：http://op.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mf.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dc.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://vr.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kq.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://st.wgjwhj.cn

Py:   ",".join(items)
来源：http://gw.shxzukj.cn

PHP:  implode(",", $items);
来源：http://qo.asd995.cn

JS:   items.join(",")
来源：http://my.521024.cn

TS:   items.join(",")
来源：http://gk.shxzskj.cn

Java: String.join(",", items)
来源：http://ll.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://qb.shxzukj.cn

Ruby: items.join(",")
来源：http://nw.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://hv.szsharing.cn

[E09] 去除所有空白字符
来源：http://lp.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jy.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oc.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://em.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://qd.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ws.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yt.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://by.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ce.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://fa.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gs.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ww.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://df.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://sj.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://mn.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dn.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ni.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://je.jctech888.com.cn

[E11] 反转字符串
来源：http://hs.hnjuh.cn

Py:   s[::-1]
来源：http://du.colortex.cn

PHP:  strrev($s);
来源：http://nh.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://bp.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://qa.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ju.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gp.szsharing.cn

Ruby: s.reverse
来源：http://wj.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://od.asd995.cn

[E12] 统计某字符出现次数
来源：http://ms.shtwfgs.cn

Py:   s.count("a")
来源：http://ft.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://gm.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://yh.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://xv.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dq.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://pf.wgjwhj.cn

Ruby: s.count("a")
来源：http://up.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://vv.huixiangedu.cn

[E13] 逐字符遍历
来源：http://fs.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://qr.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ea.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zr.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vc.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://de.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tl.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fp.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wu.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://qf.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pg.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qt.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ty.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pw.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rs.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kk.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jc.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ef.521024.cn

[E15] HTML 转义 / 反转义
来源：http://qm.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zw.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wg.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ic.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xc.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fk.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zm.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yw.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qm.muxihuayi.cn

[E16] 数字千分位
来源：http://xc.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://jc.9csxet.cn

PHP:  number_format(1234567);
来源：http://bp.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tn.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ij.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fg.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mf.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gc.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://nl.panjiajie.cn

[E17] 首字母大写
来源：http://xu.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yo.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wy.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oc.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sl.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bd.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nx.gzmigu.cn

Ruby: s.capitalize
来源：http://ro.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ev.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://tw.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jf.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ao.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ww.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://so.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xx.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://az.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cg.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oi.newstarts.cn

[E19] 多行文本按行拆分
来源：http://ar.jctech888.com.cn

Py:   s.splitlines()
来源：http://ot.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sf.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://yo.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://fu.huanxung.cn

Java: s.lines().toList()
来源：http://hf.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://jc.huixiangedu.cn

Ruby: s.lines
来源：http://md.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://io.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://uc.jctech888.com.cn

Py:   if not s:
来源：http://vo.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gg.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vn.hahajie.cn

TS:   if (s === "") {}
来源：http://st.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://lo.huixiangedu.cn

Go:   if s == "" {}
来源：http://sr.muxihuayi.cn

Ruby: if s.empty?
来源：http://it.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xv.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://we.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iz.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://db.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cz.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ox.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vq.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ki.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ki.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ut.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://az.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fh.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pu.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jt.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://py.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xw.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dg.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://vg.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qy.bjjhwx.cn

================================================================================
来源：http://up.wgjwhj.cn

F. 文件与目录
来源：http://xz.chemitech.net.cn

================================================================================
来源：http://vv.bjjhwx.cn

[F01] 读取整个文件
来源：http://zz.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vq.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://vq.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ts.haigaiapp.cn


<!-- 参考信息 -->