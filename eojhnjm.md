代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ch.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://sp.521024.cn

C#:   list.Max();  list.Min()
来源：http://iw.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://wg.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qp.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://cl.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lk.hnjuh.cn

TS:   nested.flat();
来源：http://xv.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wj.shxzskj.cn

Go:   // 手写双层循环
来源：http://qp.nicolike.cn

Ruby: nested.flatten
来源：http://ct.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fd.huanxung.cn

[D19] 按字段分组
来源：http://wx.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cz.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ab.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ml.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ub.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kj.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://mg.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nd.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ze.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://an.bookmarksfly.cn

Py:   Counter(arr)
来源：http://gp.newstarts.cn

PHP:  array_count_values($arr);
来源：http://tn.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qt.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gr.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fi.huanxung.cn

Go:   // 手写 map[T]int
来源：http://bl.haigaiapp.cn

Ruby: arr.tally
来源：http://ff.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ft.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://yu.521024.cn

Py:   x in arr
来源：http://vj.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://zt.huanxung.cn

JS:   arr.includes(x)
来源：http://ev.jctech888.com.cn

TS:   arr.includes(x)
来源：http://gw.lnxyls.cn

Java: list.contains(x)
来源：http://os.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://nw.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://je.lnxyls.cn

C#:   list.Contains(x)
来源：http://ah.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://jy.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yp.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xp.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ls.9csxet.cn

TS:   [...arr];
来源：http://jd.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://cr.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zr.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://gx.asd995.cn

C#:   new List<int>(list);
来源：http://br.huixiangedu.cn

[D23] reduce 累积计算
来源：http://nq.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qg.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uv.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wf.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zw.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://am.yuexingan06.cn

Go:   // 手写循环
来源：http://rd.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xh.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kz.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://aa.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ls.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eg.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lc.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tk.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pu.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ad.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ay.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mv.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://zf.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yu.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://km.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dc.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ck.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://un.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ud.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uo.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dh.huanxung.cn

[D26] 数组转字符串
来源：http://fk.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://xl.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ty.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://bj.gzmigu.cn

TS:   arr.join(", ")
来源：http://gr.jctech888.com.cn

Java: String.join(", ", list)
来源：http://el.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://vl.szxytkj.cn

Ruby: arr.join(", ")
来源：http://zm.szsharing.cn

C#:   string.Join(", ", list)
来源：http://bd.9csxet.cn

================================================================================
来源：http://bt.yuexingan06.cn

E. 字符串处理
来源：http://vx.huixinmuqiang.cn

================================================================================
来源：http://fg.panjiajie.cn

[E01] 拼接字符串
来源：http://jm.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sf.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yk.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sv.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aw.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gq.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ds.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rn.szxytkj.cn

[E02] 重复字符串
来源：http://wi.panjiajie.cn

Py:   "ab" * 3
来源：http://rj.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://ex.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://sb.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://lz.gzmigu.cn

Java: "ab".repeat(3)
来源：http://pe.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://vh.shxzukj.cn

Ruby: "ab" * 3
来源：http://uu.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vw.hahajie.cn

[E03] 截取子串
来源：http://ce.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bp.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://no.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qo.colortex.cn

TS:   s.slice(1, 4)
来源：http://jp.newstarts.cn

Java: s.substring(1, 4)
来源：http://ga.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://np.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ca.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ze.haigaiapp.cn

[E04] 查找子串位置
来源：http://qu.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://cp.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ud.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vn.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://de.nicolike.cn

Java: s.indexOf("x")
来源：http://ge.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://xc.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://im.asd995.cn

C#:   s.IndexOf("x")
来源：http://mc.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ku.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oe.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tp.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sq.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cs.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pp.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://na.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aj.newstarts.cn

[E06] 替换子串
来源：http://gy.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://my.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://xn.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yi.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://kb.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jn.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ps.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ib.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://ud.colortex.cn

[E07] 按分隔符拆分
来源：http://tf.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bp.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zd.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ey.shtwfgs.cn

TS:   s.split(",")
来源：http://dy.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pq.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fa.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://gy.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gi.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://vp.yuexingan06.cn

Py:   ",".join(items)
来源：http://li.hnjuh.cn

PHP:  implode(",", $items);
来源：http://vq.bookmarksfly.cn

JS:   items.join(",")
来源：http://rz.panjiajie.cn

TS:   items.join(",")
来源：http://uw.huixiangedu.cn

Java: String.join(",", items)
来源：http://ve.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://hq.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://zv.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://th.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://yc.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hh.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lu.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ff.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://ql.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://bu.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ni.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sd.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jj.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://hf.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pj.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oz.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://lb.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://eq.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://oc.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xv.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://at.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pc.521024.cn

[E11] 反转字符串
来源：http://io.szxytkj.cn

Py:   s[::-1]
来源：http://lp.bjjhwx.cn

PHP:  strrev($s);
来源：http://ql.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ya.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://zk.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://da.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ki.lnxyls.cn

Ruby: s.reverse
来源：http://fe.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nu.colortex.cn

[E12] 统计某字符出现次数
来源：http://eg.bookmarksfly.cn

Py:   s.count("a")
来源：http://hy.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://st.newstarts.cn

JS:   s.split("a").length - 1
来源：http://iu.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://dg.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nu.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://vt.lnxyls.cn

Ruby: s.count("a")
来源：http://gn.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://po.szxytkj.cn

[E13] 逐字符遍历
来源：http://hw.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://xo.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://db.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zd.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ug.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://io.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mk.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ki.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uo.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://xs.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fi.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xx.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qa.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vi.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jy.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pj.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rq.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cm.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://tz.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gl.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qg.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iy.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pf.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://px.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vu.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zw.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yg.yuntaijiaju.cn

[E16] 数字千分位
来源：http://oy.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://zo.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://fn.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rm.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mf.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lc.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zz.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ky.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://ro.huixinmuqiang.cn

[E17] 首字母大写
来源：http://cu.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ys.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pr.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kp.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yg.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zv.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ng.szxytkj.cn

Ruby: s.capitalize
来源：http://gs.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gu.yuexingan06.cn

[E18] 模板占位符替换
来源：http://jy.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://in.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wu.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qv.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://in.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nc.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sl.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yu.521024.cn

[E19] 多行文本按行拆分
来源：http://cs.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ch.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qu.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://vr.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://fs.bjjhwx.cn

Java: s.lines().toList()
来源：http://oe.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://fe.jianghongdianzi.cn

Ruby: s.lines
来源：http://uj.panjiajie.cn

C#:   s.Split('\n')
来源：http://qf.521024.cn

[E20] 判断字符串是否为空
来源：http://kf.521024.cn

Py:   if not s:
来源：http://sg.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hg.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rj.szxytkj.cn

TS:   if (s === "") {}
来源：http://cg.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://fe.wgjwhj.cn

Go:   if s == "" {}
来源：http://td.shtwfgs.cn

Ruby: if s.empty?
来源：http://zn.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lw.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://us.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jy.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kv.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ke.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vp.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ji.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://uk.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kq.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gx.huanxung.cn

[E22] 字节长度与字符长度
来源：http://cl.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hv.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://un.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jy.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ui.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jb.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ur.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://yg.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eu.bookmarksfly.cn

================================================================================
来源：http://kr.huanxung.cn

F. 文件与目录
来源：http://ru.bjjhwx.cn

================================================================================
来源：http://ud.yuexingan06.cn

[F01] 读取整个文件
来源：http://lq.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nh.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://uj.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hf.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mx.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ga.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kg.521024.cn

Ruby: File.read("a.txt")
来源：http://wy.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://ad.bjjhwx.cn

[F02] 逐行读取文件
来源：http://bo.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://op.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ge.wgjwhj.cn


<!-- 参考信息 -->