代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ls.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://kf.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://es.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://ko.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ji.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://mo.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vp.huixiangedu.cn

TS:   nested.flat();
来源：http://xz.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wx.szxytkj.cn

Go:   // 手写双层循环
来源：http://xl.bookmarksfly.cn

Ruby: nested.flatten
来源：http://cb.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nh.lnxyls.cn

[D19] 按字段分组
来源：http://ph.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ph.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fe.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sj.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cp.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gc.521024.cn

Go:   // 手写 map[string][]T
来源：http://fy.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oi.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://my.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://ar.huixiangedu.cn

Py:   Counter(arr)
来源：http://mt.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://pr.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://na.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mk.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://la.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ws.shxzukj.cn

Ruby: arr.tally
来源：http://fh.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zo.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://ge.shxzskj.cn

Py:   x in arr
来源：http://cf.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://tu.asd995.cn

JS:   arr.includes(x)
来源：http://en.9csxet.cn

TS:   arr.includes(x)
来源：http://xf.szxytkj.cn

Java: list.contains(x)
来源：http://cu.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://ty.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://tx.shxzukj.cn

C#:   list.Contains(x)
来源：http://pj.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://qi.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://og.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jr.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zk.hnjuh.cn

TS:   [...arr];
来源：http://gn.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ux.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fg.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://vh.shxzukj.cn

C#:   new List<int>(list);
来源：http://wl.521024.cn

[D23] reduce 累积计算
来源：http://yw.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ds.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zz.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://es.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rt.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ib.colortex.cn

Go:   // 手写循环
来源：http://ti.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://es.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://td.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://bh.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ri.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ux.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bf.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xf.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zq.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zi.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qm.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jl.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://cb.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cg.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nf.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lb.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wh.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hm.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qq.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mx.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vm.shxzskj.cn

[D26] 数组转字符串
来源：http://tp.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://ld.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://da.yuexingan06.cn

JS:   arr.join(", ")
来源：http://cj.panjiajie.cn

TS:   arr.join(", ")
来源：http://ye.asd995.cn

Java: String.join(", ", list)
来源：http://jx.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://sj.hahajie.cn

Ruby: arr.join(", ")
来源：http://hx.huanxung.cn

C#:   string.Join(", ", list)
来源：http://ea.chemitech.net.cn

================================================================================
来源：http://zk.bookmarksfly.cn

E. 字符串处理
来源：http://uj.huixinmuqiang.cn

================================================================================
来源：http://yc.bookmarksfly.cn

[E01] 拼接字符串
来源：http://an.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ne.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://re.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zc.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yt.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yi.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dk.huixiangedu.cn

[E02] 重复字符串
来源：http://yn.newstarts.cn

Py:   "ab" * 3
来源：http://ir.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://mx.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://hz.521024.cn

TS:   "ab".repeat(3)
来源：http://na.hnjuh.cn

Java: "ab".repeat(3)
来源：http://bi.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://pn.newstarts.cn

Ruby: "ab" * 3
来源：http://xy.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iw.haigaiapp.cn

[E03] 截取子串
来源：http://es.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wi.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fa.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zk.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://gb.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://dl.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xg.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ft.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://ml.szxytkj.cn

[E04] 查找子串位置
来源：http://yp.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bu.521024.cn

PHP:  strpos($s, "x");
来源：http://nq.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ma.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://wd.shtwfgs.cn

Java: s.indexOf("x")
来源：http://kf.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://dv.lnxyls.cn

Ruby: s.index("x")
来源：http://ls.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://ph.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oy.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://km.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://po.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://la.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mz.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dx.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eb.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yc.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hf.gzmigu.cn

[E06] 替换子串
来源：http://da.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cm.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://qd.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mz.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://px.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wf.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sr.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kt.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://vm.shxzukj.cn

[E07] 按分隔符拆分
来源：http://jp.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ga.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sx.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wz.shxzskj.cn

TS:   s.split(",")
来源：http://ki.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rt.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vv.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://yx.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tj.newstarts.cn

[E08] 数组按分隔符合并
来源：http://kr.bookmarksfly.cn

Py:   ",".join(items)
来源：http://el.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://ph.szsharing.cn

JS:   items.join(",")
来源：http://lg.muxihuayi.cn

TS:   items.join(",")
来源：http://bl.szsharing.cn

Java: String.join(",", items)
来源：http://vc.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://yg.wgjwhj.cn

Ruby: items.join(",")
来源：http://js.hahajie.cn

C#:   string.Join(",", items)
来源：http://xz.lnxyls.cn

[E09] 去除所有空白字符
来源：http://yl.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://it.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gq.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wq.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://xo.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://wv.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rz.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gf.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wd.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://kx.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tz.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cx.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://zl.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://qw.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://am.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bl.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lm.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gj.muxihuayi.cn

[E11] 反转字符串
来源：http://ti.yuntaijiaju.cn

Py:   s[::-1]
来源：http://xg.szsharing.cn

PHP:  strrev($s);
来源：http://ia.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://yh.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://mb.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xn.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zi.lnxyls.cn

Ruby: s.reverse
来源：http://oq.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pp.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://ie.asd995.cn

Py:   s.count("a")
来源：http://um.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://fc.colortex.cn

JS:   s.split("a").length - 1
来源：http://qt.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://st.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ve.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://eo.shxzukj.cn

Ruby: s.count("a")
来源：http://yj.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://mg.shtwfgs.cn

[E13] 逐字符遍历
来源：http://mn.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://zo.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fv.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pr.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ge.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kg.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jk.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://al.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hj.nszjky.cn

[E14] URL 编码与 Base64
来源：http://fi.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qr.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ca.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nk.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jp.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eg.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ye.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://es.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fc.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://ke.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mu.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nf.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oj.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://id.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oz.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ac.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tc.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fn.hnjuh.cn

[E16] 数字千分位
来源：http://rd.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://hh.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://vi.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ud.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nq.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sp.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lc.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ly.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://nu.wgjwhj.cn

[E17] 首字母大写
来源：http://yp.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oi.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pp.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ll.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mu.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bg.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ki.jctech888.com.cn

Ruby: s.capitalize
来源：http://qn.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zl.9csxet.cn

[E18] 模板占位符替换
来源：http://oj.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jv.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yr.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://og.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ci.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ad.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zf.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jx.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xl.9csxet.cn

[E19] 多行文本按行拆分
来源：http://gg.szxytkj.cn

Py:   s.splitlines()
来源：http://jn.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dk.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://uw.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://yf.hahajie.cn

Java: s.lines().toList()
来源：http://tb.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://nh.jianghongdianzi.cn

Ruby: s.lines
来源：http://yg.shtwfgs.cn

C#:   s.Split('\n')
来源：http://dg.nszjky.cn

[E20] 判断字符串是否为空
来源：http://ep.newstarts.cn

Py:   if not s:
来源：http://lw.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nr.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uv.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://xn.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://oe.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://em.nicolike.cn

Ruby: if s.empty?
来源：http://nv.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sd.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://ai.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kz.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bz.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vx.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jv.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dv.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ou.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tk.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qb.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://rp.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://km.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wz.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qc.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lg.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ef.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ev.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ls.shxzskj.cn

================================================================================
来源：http://mg.521024.cn

F. 文件与目录
来源：http://fh.wgjwhj.cn

================================================================================
来源：http://pf.shxzukj.cn

[F01] 读取整个文件
来源：http://ap.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zt.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yh.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ot.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qf.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sg.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sn.huanxung.cn

Ruby: File.read("a.txt")
来源：http://yk.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vx.wgjwhj.cn

[F02] 逐行读取文件
来源：http://vl.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gi.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sf.nszjky.cn


<!-- 参考信息 -->