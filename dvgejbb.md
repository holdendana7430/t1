代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://pq.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ck.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://wv.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://le.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pz.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://oe.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://oi.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://lt.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hw.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://nj.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ww.szsharing.cn

TS:   nested.flat();
来源：http://ok.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ry.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ug.nicolike.cn

Ruby: nested.flatten
来源：http://qe.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ky.szsharing.cn

[D19] 按字段分组
来源：http://ic.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://co.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ip.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iy.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nc.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wc.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://nw.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ev.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gp.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://io.huixiangedu.cn

Py:   Counter(arr)
来源：http://gg.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://ot.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uj.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xy.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ky.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://tt.521024.cn

Ruby: arr.tally
来源：http://nq.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cs.9csxet.cn

[D21] 判断是否包含某元素
来源：http://hg.gzmigu.cn

Py:   x in arr
来源：http://xe.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://sk.shxzukj.cn

JS:   arr.includes(x)
来源：http://id.521024.cn

TS:   arr.includes(x)
来源：http://xp.jianghongdianzi.cn

Java: list.contains(x)
来源：http://lk.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://gj.gzmigu.cn

Ruby: arr.include?(x)
来源：http://zp.shtwfgs.cn

C#:   list.Contains(x)
来源：http://ve.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://cy.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ro.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gg.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pv.bookmarksfly.cn

TS:   [...arr];
来源：http://gh.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://bz.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hy.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://oe.huixiangedu.cn

C#:   new List<int>(list);
来源：http://ue.9csxet.cn

[D23] reduce 累积计算
来源：http://uy.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nu.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wt.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://do.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tf.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yi.hnjuh.cn

Go:   // 手写循环
来源：http://zq.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mp.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tk.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://io.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zd.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ni.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lt.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vd.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://at.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://la.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uw.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nq.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://bm.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jz.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iz.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iq.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jl.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wu.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sd.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ws.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://db.asd995.cn

[D26] 数组转字符串
来源：http://nz.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://xp.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://hg.haigaiapp.cn

JS:   arr.join(", ")
来源：http://jm.newstarts.cn

TS:   arr.join(", ")
来源：http://nt.nszjky.cn

Java: String.join(", ", list)
来源：http://mq.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://el.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://ji.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://fa.bjjhwx.cn

================================================================================
来源：http://ed.szsharing.cn

E. 字符串处理
来源：http://ri.muxihuayi.cn

================================================================================
来源：http://hk.huanxung.cn

[E01] 拼接字符串
来源：http://jw.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hd.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ey.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tr.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jq.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xz.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dt.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zh.yuntaijiaju.cn

[E02] 重复字符串
来源：http://xh.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://yw.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://sn.521024.cn

JS:   "ab".repeat(3)
来源：http://da.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://zl.shxzukj.cn

Java: "ab".repeat(3)
来源：http://li.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ho.asd995.cn

Ruby: "ab" * 3
来源：http://cd.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ta.szsharing.cn

[E03] 截取子串
来源：http://hy.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jq.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cy.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mk.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://ma.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ww.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lt.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zx.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://im.asd995.cn

[E04] 查找子串位置
来源：http://mf.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ef.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://kf.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sv.colortex.cn

TS:   s.indexOf("x")
来源：http://nn.panjiajie.cn

Java: s.indexOf("x")
来源：http://ze.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://kn.huixiangedu.cn

Ruby: s.index("x")
来源：http://ha.huanxung.cn

C#:   s.IndexOf("x")
来源：http://ls.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fj.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nf.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uz.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uw.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://it.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nl.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://af.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jo.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cs.lnxyls.cn

[E06] 替换子串
来源：http://dr.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kg.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://og.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qe.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://go.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pd.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gn.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bo.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://zi.521024.cn

[E07] 按分隔符拆分
来源：http://ol.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lu.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ai.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ni.shtwfgs.cn

TS:   s.split(",")
来源：http://lb.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jg.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ky.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ro.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hf.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://mn.521024.cn

Py:   ",".join(items)
来源：http://au.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://nk.shtwfgs.cn

JS:   items.join(",")
来源：http://hz.jianghongdianzi.cn

TS:   items.join(",")
来源：http://mq.hnjuh.cn

Java: String.join(",", items)
来源：http://fk.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ms.hahajie.cn

Ruby: items.join(",")
来源：http://me.szxytkj.cn

C#:   string.Join(",", items)
来源：http://ct.nszjky.cn

[E09] 去除所有空白字符
来源：http://gq.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jd.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kr.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ra.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://qu.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://qa.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uy.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fq.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ab.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://pr.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dr.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gi.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://dy.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://co.colortex.cn

Java: String.format("%03d", 7)
来源：http://jj.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xn.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ke.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ng.9csxet.cn

[E11] 反转字符串
来源：http://fg.huixinmuqiang.cn

Py:   s[::-1]
来源：http://bi.asd995.cn

PHP:  strrev($s);
来源：http://pp.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://cf.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://fu.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qe.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nv.shxzskj.cn

Ruby: s.reverse
来源：http://ou.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://se.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://ql.gzmigu.cn

Py:   s.count("a")
来源：http://po.521024.cn

PHP:  substr_count($s, "a");
来源：http://fc.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ts.newstarts.cn

TS:   s.split("a").length - 1
来源：http://zx.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nc.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://ad.jctech888.com.cn

Ruby: s.count("a")
来源：http://cw.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://vr.nicolike.cn

[E13] 逐字符遍历
来源：http://dx.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://mn.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wc.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fa.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sg.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://et.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bt.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vm.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rs.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://lu.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mi.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dh.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wq.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ul.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://av.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://he.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kq.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bo.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://am.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ye.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ac.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kt.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hl.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ei.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lu.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qf.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ft.chemitech.net.cn

[E16] 数字千分位
来源：http://zv.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://sh.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://fl.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://he.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://st.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://li.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aj.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mv.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://tb.yuntaijiaju.cn

[E17] 首字母大写
来源：http://ea.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zl.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oe.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ko.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sh.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zg.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ud.szxytkj.cn

Ruby: s.capitalize
来源：http://ze.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ha.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://oa.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ir.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lc.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sd.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vw.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oi.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://im.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dv.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ww.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://pz.hahajie.cn

Py:   s.splitlines()
来源：http://kr.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cq.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://lc.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://re.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ot.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://jb.bjjhwx.cn

Ruby: s.lines
来源：http://iw.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ww.asd995.cn

[E20] 判断字符串是否为空
来源：http://ra.yuntaijiaju.cn

Py:   if not s:
来源：http://wz.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tn.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vv.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ds.521024.cn

Java: if (s.isEmpty()) {}
来源：http://op.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://oq.nszjky.cn

Ruby: if s.empty?
来源：http://wo.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ji.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://yx.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tc.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pn.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kt.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://re.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qt.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://ln.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hn.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ix.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://yn.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kp.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uh.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dr.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ku.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://su.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ol.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pg.newstarts.cn

================================================================================
来源：http://sw.nicolike.cn

F. 文件与目录
来源：http://hp.jctech888.com.cn

================================================================================
来源：http://bt.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://av.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ax.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://gp.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hn.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wf.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rq.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hx.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://tf.panjiajie.cn


<!-- 参考信息 -->