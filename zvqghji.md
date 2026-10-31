代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dd.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://ui.asd995.cn

C#:   list.Max();  list.Min()
来源：http://oy.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://vp.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ep.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://nf.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bx.nicolike.cn

TS:   nested.flat();
来源：http://vb.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fb.9csxet.cn

Go:   // 手写双层循环
来源：http://gb.chemitech.net.cn

Ruby: nested.flatten
来源：http://cz.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ec.huanxung.cn

[D19] 按字段分组
来源：http://vg.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lb.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aw.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ut.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oz.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ya.521024.cn

Go:   // 手写 map[string][]T
来源：http://ah.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://us.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ms.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://hg.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://zz.colortex.cn

PHP:  array_count_values($arr);
来源：http://vt.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ui.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://is.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gb.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vu.shxzskj.cn

Ruby: arr.tally
来源：http://au.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://my.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://dl.yuexingan06.cn

Py:   x in arr
来源：http://zk.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://xc.521024.cn

JS:   arr.includes(x)
来源：http://jd.shxzukj.cn

TS:   arr.includes(x)
来源：http://ao.huanxung.cn

Java: list.contains(x)
来源：http://tv.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://ab.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://qq.nicolike.cn

C#:   list.Contains(x)
来源：http://xe.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://mh.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ub.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rg.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cr.huanxung.cn

TS:   [...arr];
来源：http://vu.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://oj.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kg.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://it.nszjky.cn

C#:   new List<int>(list);
来源：http://er.lnxyls.cn

[D23] reduce 累积计算
来源：http://ws.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://df.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://up.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qa.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wj.wgjwhj.cn

Go:   // 手写循环
来源：http://ux.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ap.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tn.521024.cn

[D24] 字典 / Map 基本操作
来源：http://cp.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bt.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nr.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aa.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ha.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sw.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ft.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pp.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fn.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://fu.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pn.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ji.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://om.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mn.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://er.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ek.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ei.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zi.nszjky.cn

[D26] 数组转字符串
来源：http://xr.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://yz.521024.cn

PHP:  implode(", ", $arr);
来源：http://et.muxihuayi.cn

JS:   arr.join(", ")
来源：http://eq.chemitech.net.cn

TS:   arr.join(", ")
来源：http://ow.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://th.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://mu.shxzskj.cn

Ruby: arr.join(", ")
来源：http://fl.nicolike.cn

C#:   string.Join(", ", list)
来源：http://jr.hnjuh.cn

================================================================================
来源：http://es.521024.cn

E. 字符串处理
来源：http://yc.chemitech.net.cn

================================================================================
来源：http://ky.newstarts.cn

[E01] 拼接字符串
来源：http://sm.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ed.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qs.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tj.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pm.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://su.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jb.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tb.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sj.colortex.cn

[E02] 重复字符串
来源：http://vq.hahajie.cn

Py:   "ab" * 3
来源：http://dm.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://nl.9csxet.cn

JS:   "ab".repeat(3)
来源：http://ae.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://mo.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://gl.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://qe.shxzukj.cn

Ruby: "ab" * 3
来源：http://yz.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hm.bjjhwx.cn

[E03] 截取子串
来源：http://iw.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ll.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ws.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sj.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://hv.nicolike.cn

Java: s.substring(1, 4)
来源：http://jb.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wv.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bv.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://nv.panjiajie.cn

[E04] 查找子串位置
来源：http://zn.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://xy.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://ek.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kn.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://sd.newstarts.cn

Java: s.indexOf("x")
来源：http://gc.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://xa.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://aj.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://ns.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vi.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bl.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wc.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://za.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vk.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fy.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nr.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vk.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ee.521024.cn

[E06] 替换子串
来源：http://xi.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mw.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://ob.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ju.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://st.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ez.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ev.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ht.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://uf.newstarts.cn

[E07] 按分隔符拆分
来源：http://ma.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hr.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://os.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cq.huixiangedu.cn

TS:   s.split(",")
来源：http://vf.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mh.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cz.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://af.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qj.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://tf.nicolike.cn

Py:   ",".join(items)
来源：http://mn.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ag.yuexingan06.cn

JS:   items.join(",")
来源：http://ie.bookmarksfly.cn

TS:   items.join(",")
来源：http://zz.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ky.asd995.cn

Go:   strings.Join(items, ",")
来源：http://eb.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://nc.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://za.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://sh.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oz.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xx.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://uq.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://gh.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://bf.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gb.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vj.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ug.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://jq.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jr.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ua.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://ag.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://zy.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://ph.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://es.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jb.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://at.huixinmuqiang.cn

[E11] 反转字符串
来源：http://no.colortex.cn

Py:   s[::-1]
来源：http://fj.wgjwhj.cn

PHP:  strrev($s);
来源：http://ku.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://ff.colortex.cn

TS:   [...s].reverse().join("")
来源：http://pj.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sr.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sx.huixinmuqiang.cn

Ruby: s.reverse
来源：http://nz.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://io.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://dj.nicolike.cn

Py:   s.count("a")
来源：http://fw.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://mo.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://di.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://md.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bx.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://iq.9csxet.cn

Ruby: s.count("a")
来源：http://ie.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://fe.9csxet.cn

[E13] 逐字符遍历
来源：http://fx.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://pw.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yf.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ur.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eh.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ip.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xk.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yp.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tp.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://wi.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sa.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bn.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bf.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xn.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wb.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yg.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sy.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gn.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://dq.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eg.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://os.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tb.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bs.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fs.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hp.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ig.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fq.jctech888.com.cn

[E16] 数字千分位
来源：http://sv.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://cb.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://ol.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dp.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sg.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ne.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wb.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lp.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://zg.521024.cn

[E17] 首字母大写
来源：http://qe.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uv.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xw.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aj.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.521024.cn

Ruby: s.capitalize
来源：http://sp.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kv.9csxet.cn

[E18] 模板占位符替换
来源：http://aa.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hk.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rj.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mm.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jp.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hr.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gu.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bm.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lt.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://xj.colortex.cn

Py:   s.splitlines()
来源：http://no.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vf.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://ce.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://xs.bjjhwx.cn

Java: s.lines().toList()
来源：http://dq.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://nu.szsharing.cn

Ruby: s.lines
来源：http://ky.lnxyls.cn

C#:   s.Split('\n')
来源：http://np.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ts.panjiajie.cn

Py:   if not s:
来源：http://jc.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rk.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rl.9csxet.cn

TS:   if (s === "") {}
来源：http://pd.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://iq.wgjwhj.cn

Go:   if s == "" {}
来源：http://lz.521024.cn

Ruby: if s.empty?
来源：http://mm.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://em.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ve.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lg.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bo.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gg.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ti.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://yh.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xr.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mt.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://mh.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jf.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wt.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ju.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rp.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://os.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nd.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://xt.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dq.szsharing.cn

================================================================================
来源：http://yb.szsharing.cn

F. 文件与目录
来源：http://br.lnxyls.cn

================================================================================
来源：http://ep.bookmarksfly.cn

[F01] 读取整个文件
来源：http://nq.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qg.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://hc.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dy.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xd.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ri.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zb.colortex.cn

Ruby: File.read("a.txt")
来源：http://ho.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://lx.lnxyls.cn

[F02] 逐行读取文件
来源：http://ce.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mr.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sr.yuntaijiaju.cn


<!-- 参考信息 -->