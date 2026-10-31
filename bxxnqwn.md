代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://vf.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dm.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://lh.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mt.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://by.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ec.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://kq.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://tc.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jv.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://on.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fh.huanxung.cn

TS:   nested.flat();
来源：http://bq.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wq.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://cw.yuexingan06.cn

Ruby: nested.flatten
来源：http://wd.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ov.asd995.cn

[D19] 按字段分组
来源：http://ca.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://li.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bt.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ll.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://no.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iq.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://lc.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gr.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wp.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://sl.hnjuh.cn

Py:   Counter(arr)
来源：http://jd.szsharing.cn

PHP:  array_count_values($arr);
来源：http://wa.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nb.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lx.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://kc.szsharing.cn

Ruby: arr.tally
来源：http://np.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pf.9csxet.cn

[D21] 判断是否包含某元素
来源：http://xz.szxytkj.cn

Py:   x in arr
来源：http://yj.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://bc.shxzukj.cn

JS:   arr.includes(x)
来源：http://av.9csxet.cn

TS:   arr.includes(x)
来源：http://kk.haigaiapp.cn

Java: list.contains(x)
来源：http://dl.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://le.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://cw.shxzskj.cn

C#:   list.Contains(x)
来源：http://lw.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://gi.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wr.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fs.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.yuntaijiaju.cn

TS:   [...arr];
来源：http://po.huanxung.cn

Java: new ArrayList<>(list);
来源：http://sw.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bt.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://jk.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://tk.hahajie.cn

[D23] reduce 累积计算
来源：http://iv.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tp.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ji.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nx.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ch.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ff.bookmarksfly.cn

Go:   // 手写循环
来源：http://bp.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bs.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aj.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://xm.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jm.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://no.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pf.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aq.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://df.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rq.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vi.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gb.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://em.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hw.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ft.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gn.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zc.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wz.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mf.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mc.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sc.shtwfgs.cn

[D26] 数组转字符串
来源：http://nn.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ex.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://yb.gzmigu.cn

JS:   arr.join(", ")
来源：http://ft.szsharing.cn

TS:   arr.join(", ")
来源：http://dj.nszjky.cn

Java: String.join(", ", list)
来源：http://dm.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://yh.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://bz.huanxung.cn

C#:   string.Join(", ", list)
来源：http://va.yuexingan06.cn

================================================================================
来源：http://zy.shxzskj.cn

E. 字符串处理
来源：http://oh.huanxung.cn

================================================================================
来源：http://sd.shxzskj.cn

[E01] 拼接字符串
来源：http://as.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jf.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dm.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ep.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oz.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mi.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jf.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bg.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fq.521024.cn

[E02] 重复字符串
来源：http://ff.bookmarksfly.cn

Py:   "ab" * 3
来源：http://fl.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://rh.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://xr.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://xu.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ej.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://or.bjjhwx.cn

Ruby: "ab" * 3
来源：http://rp.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qa.nicolike.cn

[E03] 截取子串
来源：http://lm.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wo.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dh.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cz.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ks.9csxet.cn

Java: s.substring(1, 4)
来源：http://em.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fe.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eq.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://qs.colortex.cn

[E04] 查找子串位置
来源：http://jb.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://wx.nicolike.cn

PHP:  strpos($s, "x");
来源：http://cm.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ja.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://zh.9csxet.cn

Java: s.indexOf("x")
来源：http://rm.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://it.nicolike.cn

Ruby: s.index("x")
来源：http://lk.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://em.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ih.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iu.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wq.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wa.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bj.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zl.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qu.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lx.huanxung.cn

[E06] 替换子串
来源：http://cu.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://da.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://vt.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xn.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://wr.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dt.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nv.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qa.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://bq.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://dx.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nq.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eh.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ln.huixinmuqiang.cn

TS:   s.split(",")
来源：http://bf.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ke.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hl.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://xl.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fe.nszjky.cn

[E08] 数组按分隔符合并
来源：http://ie.9csxet.cn

Py:   ",".join(items)
来源：http://il.newstarts.cn

PHP:  implode(",", $items);
来源：http://fx.hahajie.cn

JS:   items.join(",")
来源：http://sg.bookmarksfly.cn

TS:   items.join(",")
来源：http://vr.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://ey.521024.cn

Go:   strings.Join(items, ",")
来源：http://ep.lnxyls.cn

Ruby: items.join(",")
来源：http://yc.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://rh.nszjky.cn

[E09] 去除所有空白字符
来源：http://yd.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ju.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ds.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://fr.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://bn.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://qb.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ip.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xn.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zi.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ka.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dj.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://je.521024.cn

JS:   "7".padStart(3, "0")
来源：http://mw.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://ci.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://iy.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wi.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bq.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fw.colortex.cn

[E11] 反转字符串
来源：http://xl.9csxet.cn

Py:   s[::-1]
来源：http://sb.shxzukj.cn

PHP:  strrev($s);
来源：http://ch.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://zt.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://pb.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gw.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jw.bjjhwx.cn

Ruby: s.reverse
来源：http://wh.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://of.huanxung.cn

[E12] 统计某字符出现次数
来源：http://fi.haigaiapp.cn

Py:   s.count("a")
来源：http://zy.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://gm.nicolike.cn

JS:   s.split("a").length - 1
来源：http://gj.asd995.cn

TS:   s.split("a").length - 1
来源：http://br.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://px.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://uh.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://qf.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://td.wgjwhj.cn

[E13] 逐字符遍历
来源：http://gq.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://zg.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rl.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nu.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tf.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tm.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://um.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kh.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://er.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://fm.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lw.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xp.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ds.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ve.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ri.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tr.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xn.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kx.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://xl.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://me.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zb.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://up.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ef.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nl.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xd.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rv.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://er.shtwfgs.cn

[E16] 数字千分位
来源：http://cx.9csxet.cn

Py:   f"{1234567:,}"
来源：http://nj.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://qz.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ai.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://af.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fo.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ak.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sj.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://pq.nszjky.cn

[E17] 首字母大写
来源：http://kf.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mj.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cu.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tp.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ic.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qa.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cw.asd995.cn

Ruby: s.capitalize
来源：http://pf.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://st.nicolike.cn

[E18] 模板占位符替换
来源：http://cp.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://am.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fn.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mu.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://si.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zv.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ru.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tw.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sd.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://dy.hahajie.cn

Py:   s.splitlines()
来源：http://wa.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://du.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://de.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://rb.gzmigu.cn

Java: s.lines().toList()
来源：http://an.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://jt.yuntaijiaju.cn

Ruby: s.lines
来源：http://cf.yuexingan06.cn

C#:   s.Split('\n')
来源：http://rj.521024.cn

[E20] 判断字符串是否为空
来源：http://zq.yuntaijiaju.cn

Py:   if not s:
来源：http://if.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dx.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ys.wgjwhj.cn

TS:   if (s === "") {}
来源：http://xy.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://sy.nszjky.cn

Go:   if s == "" {}
来源：http://ej.colortex.cn

Ruby: if s.empty?
来源：http://bg.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tm.hnjuh.cn

[E21] 超长截断加省略号
来源：http://hr.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://he.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ls.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rt.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zf.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tk.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://dw.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ao.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xh.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://vf.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gu.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ir.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nf.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lw.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wo.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wy.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://lk.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mr.9csxet.cn

================================================================================
来源：http://aw.gzmigu.cn

F. 文件与目录
来源：http://fl.bookmarksfly.cn

================================================================================
来源：http://mn.szxytkj.cn

[F01] 读取整个文件
来源：http://an.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zz.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://cj.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gm.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kh.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vm.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pm.hahajie.cn

Ruby: File.read("a.txt")
来源：http://te.hahajie.cn


<!-- 参考信息 -->