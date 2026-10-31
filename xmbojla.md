代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://yr.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gg.newstarts.cn

TS:   Math.max(...arr);
来源：http://ko.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mq.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ss.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://nj.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://mg.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://lu.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://su.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://jv.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ep.muxihuayi.cn

TS:   nested.flat();
来源：http://js.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mg.bjjhwx.cn

Go:   // 手写双层循环
来源：http://mo.521024.cn

Ruby: nested.flatten
来源：http://da.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fq.521024.cn

[D19] 按字段分组
来源：http://fk.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wh.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jm.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lu.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kg.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://er.521024.cn

Go:   // 手写 map[string][]T
来源：http://eo.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bt.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mt.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://ur.shxzskj.cn

Py:   Counter(arr)
来源：http://uo.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://dl.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://re.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ee.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eh.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://ej.huixiangedu.cn

Ruby: arr.tally
来源：http://ao.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://du.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://vq.panjiajie.cn

Py:   x in arr
来源：http://qg.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://uf.yuexingan06.cn

JS:   arr.includes(x)
来源：http://nj.gzmigu.cn

TS:   arr.includes(x)
来源：http://iw.yuexingan06.cn

Java: list.contains(x)
来源：http://vt.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://vz.panjiajie.cn

Ruby: arr.include?(x)
来源：http://qe.gzmigu.cn

C#:   list.Contains(x)
来源：http://kj.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://ez.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dh.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xt.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rl.chemitech.net.cn

TS:   [...arr];
来源：http://sb.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://ml.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xu.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://dw.bjjhwx.cn

C#:   new List<int>(list);
来源：http://hs.shxzukj.cn

[D23] reduce 累积计算
来源：http://pl.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://an.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cb.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://db.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://di.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kv.521024.cn

Go:   // 手写循环
来源：http://tw.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sq.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yw.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://fd.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qs.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nh.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ft.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iv.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kj.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wx.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nf.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mi.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://km.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pp.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dw.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ff.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xk.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zo.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fk.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yy.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qs.asd995.cn

[D26] 数组转字符串
来源：http://am.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://fh.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://pf.shtwfgs.cn

JS:   arr.join(", ")
来源：http://zn.huixiangedu.cn

TS:   arr.join(", ")
来源：http://is.9csxet.cn

Java: String.join(", ", list)
来源：http://sn.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://wx.shxzskj.cn

Ruby: arr.join(", ")
来源：http://yh.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://ww.huanxung.cn

================================================================================
来源：http://ow.shxzskj.cn

E. 字符串处理
来源：http://dv.hahajie.cn

================================================================================
来源：http://kl.newstarts.cn

[E01] 拼接字符串
来源：http://sn.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sx.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pv.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kz.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tk.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wv.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ba.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fn.huanxung.cn

[E02] 重复字符串
来源：http://ut.wgjwhj.cn

Py:   "ab" * 3
来源：http://ik.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ju.szsharing.cn

JS:   "ab".repeat(3)
来源：http://gl.szsharing.cn

TS:   "ab".repeat(3)
来源：http://qh.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://nf.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://cf.shxzskj.cn

Ruby: "ab" * 3
来源：http://ki.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vb.yuntaijiaju.cn

[E03] 截取子串
来源：http://nt.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bu.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://te.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ql.nicolike.cn

TS:   s.slice(1, 4)
来源：http://dy.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://ik.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cv.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gk.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://tn.nicolike.cn

[E04] 查找子串位置
来源：http://ya.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://ss.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ep.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sx.hnjuh.cn

TS:   s.indexOf("x")
来源：http://lp.hnjuh.cn

Java: s.indexOf("x")
来源：http://zd.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://cu.szsharing.cn

Ruby: s.index("x")
来源：http://by.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ie.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ck.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gg.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fa.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dj.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bb.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lk.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uu.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sz.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fo.hahajie.cn

[E06] 替换子串
来源：http://ri.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ms.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://xs.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://sa.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ff.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ug.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lx.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://yy.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ix.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yw.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ui.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vj.wgjwhj.cn

TS:   s.split(",")
来源：http://ei.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gq.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jo.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://am.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ph.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ml.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://bh.521024.cn

PHP:  implode(",", $items);
来源：http://tj.bjjhwx.cn

JS:   items.join(",")
来源：http://up.huixinmuqiang.cn

TS:   items.join(",")
来源：http://xk.muxihuayi.cn

Java: String.join(",", items)
来源：http://ge.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://dl.bookmarksfly.cn

Ruby: items.join(",")
来源：http://md.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://gx.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://qi.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://av.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zn.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://ko.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://la.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://xs.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://be.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kd.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sb.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://js.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rm.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tz.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://rk.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://co.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://vs.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uj.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jw.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dv.hnjuh.cn

[E11] 反转字符串
来源：http://am.huixinmuqiang.cn

Py:   s[::-1]
来源：http://it.bjjhwx.cn

PHP:  strrev($s);
来源：http://bp.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://fd.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://nl.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ev.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yc.szsharing.cn

Ruby: s.reverse
来源：http://mq.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://at.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://av.colortex.cn

Py:   s.count("a")
来源：http://ym.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://mb.9csxet.cn

JS:   s.split("a").length - 1
来源：http://mm.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://zx.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hi.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://fi.hahajie.cn

Ruby: s.count("a")
来源：http://ac.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://lt.newstarts.cn

[E13] 逐字符遍历
来源：http://ot.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ku.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://co.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ul.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hp.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oi.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eg.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fn.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ya.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://vi.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://it.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oh.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rt.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yx.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sj.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ek.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cs.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vu.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://zc.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nh.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jq.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mn.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sv.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://os.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ls.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://km.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mz.yuexingan06.cn

[E16] 数字千分位
来源：http://ms.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://bl.gzmigu.cn

PHP:  number_format(1234567);
来源：http://fh.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ia.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yo.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hg.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mf.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://va.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://fv.bjjhwx.cn

[E17] 首字母大写
来源：http://qs.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ny.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iu.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tb.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sp.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wt.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jf.muxihuayi.cn

Ruby: s.capitalize
来源：http://ys.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xk.gzmigu.cn

[E18] 模板占位符替换
来源：http://hp.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gb.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://of.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://an.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://as.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zk.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dy.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fg.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nd.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://ih.gzmigu.cn

Py:   s.splitlines()
来源：http://ka.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://id.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ov.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://vy.521024.cn

Java: s.lines().toList()
来源：http://ma.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://jq.nicolike.cn

Ruby: s.lines
来源：http://zv.szsharing.cn

C#:   s.Split('\n')
来源：http://gz.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://li.shxzskj.cn

Py:   if not s:
来源：http://cw.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jw.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oc.asd995.cn

TS:   if (s === "") {}
来源：http://xt.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://dm.shxzskj.cn

Go:   if s == "" {}
来源：http://im.shxzskj.cn

Ruby: if s.empty?
来源：http://mi.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fx.lnxyls.cn

[E21] 超长截断加省略号
来源：http://sy.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pp.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://na.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qn.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hu.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://in.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://zf.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mk.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://if.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://wl.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://as.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ln.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sf.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fn.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lz.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://un.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://lj.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://av.hahajie.cn

================================================================================
来源：http://vu.bjjhwx.cn

F. 文件与目录
来源：http://sr.gzmigu.cn

================================================================================
来源：http://ge.nicolike.cn

[F01] 读取整个文件
来源：http://pz.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vq.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://vg.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mm.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ip.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qj.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hg.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://cr.bookmarksfly.cn


<!-- 参考信息 -->