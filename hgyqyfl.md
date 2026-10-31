代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gj.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://vl.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://ri.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://jj.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vy.colortex.cn

PHP:  array_merge(...$nested);
来源：http://wh.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://de.huixiangedu.cn

TS:   nested.flat();
来源：http://sz.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qj.asd995.cn

Go:   // 手写双层循环
来源：http://ii.gzmigu.cn

Ruby: nested.flatten
来源：http://bt.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wp.hnjuh.cn

[D19] 按字段分组
来源：http://fw.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rn.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xl.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qj.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vo.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ka.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://nx.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kr.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eq.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://xn.gzmigu.cn

Py:   Counter(arr)
来源：http://pa.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://fb.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ht.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://df.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gl.hahajie.cn

Go:   // 手写 map[T]int
来源：http://jw.yuntaijiaju.cn

Ruby: arr.tally
来源：http://fj.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kj.9csxet.cn

[D21] 判断是否包含某元素
来源：http://pk.colortex.cn

Py:   x in arr
来源：http://wj.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://rr.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://kt.hahajie.cn

TS:   arr.includes(x)
来源：http://ed.hahajie.cn

Java: list.contains(x)
来源：http://fn.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://jk.gzmigu.cn

Ruby: arr.include?(x)
来源：http://fx.lnxyls.cn

C#:   list.Contains(x)
来源：http://en.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://qk.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lz.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ph.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iw.shxzukj.cn

TS:   [...arr];
来源：http://df.9csxet.cn

Java: new ArrayList<>(list);
来源：http://kv.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wf.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://qj.szxytkj.cn

C#:   new List<int>(list);
来源：http://wz.yuexingan06.cn

[D23] reduce 累积计算
来源：http://xo.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gf.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bb.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fd.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ss.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xe.huixiangedu.cn

Go:   // 手写循环
来源：http://dg.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qp.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xl.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://gg.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kw.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aq.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ty.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ju.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://le.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ct.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ry.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pt.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://ro.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wt.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ih.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dk.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ls.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wr.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xt.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iq.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ry.szxytkj.cn

[D26] 数组转字符串
来源：http://on.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://zz.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://af.lnxyls.cn

JS:   arr.join(", ")
来源：http://eo.nszjky.cn

TS:   arr.join(", ")
来源：http://jr.gzmigu.cn

Java: String.join(", ", list)
来源：http://nv.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://ms.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://fp.hahajie.cn

C#:   string.Join(", ", list)
来源：http://pq.hnjuh.cn

================================================================================
来源：http://fa.521024.cn

E. 字符串处理
来源：http://vd.jianghongdianzi.cn

================================================================================
来源：http://ly.nicolike.cn

[E01] 拼接字符串
来源：http://zh.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rv.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hx.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kw.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wj.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zr.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ze.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gd.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dv.shxzukj.cn

[E02] 重复字符串
来源：http://gl.9csxet.cn

Py:   "ab" * 3
来源：http://ox.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://qc.newstarts.cn

JS:   "ab".repeat(3)
来源：http://il.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://og.shxzukj.cn

Java: "ab".repeat(3)
来源：http://bj.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://kg.yuexingan06.cn

Ruby: "ab" * 3
来源：http://qa.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vs.gzmigu.cn

[E03] 截取子串
来源：http://gv.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vk.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fj.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xr.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://bm.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://sx.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rm.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lr.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://vz.jctech888.com.cn

[E04] 查找子串位置
来源：http://rj.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://ti.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://ol.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ka.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://jp.szxytkj.cn

Java: s.indexOf("x")
来源：http://ku.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://ef.nicolike.cn

Ruby: s.index("x")
来源：http://yw.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://dk.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xa.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yr.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dr.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kq.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://de.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sz.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bk.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kj.panjiajie.cn

[E06] 替换子串
来源：http://zy.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xg.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://sx.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ik.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://mn.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vv.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qn.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://mr.nszjky.cn

[E07] 按分隔符拆分
来源：http://xx.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uu.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ga.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lg.panjiajie.cn

TS:   s.split(",")
来源：http://qg.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rx.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ki.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://gh.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bd.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://yj.shxzskj.cn

Py:   ",".join(items)
来源：http://go.colortex.cn

PHP:  implode(",", $items);
来源：http://ja.gzmigu.cn

JS:   items.join(",")
来源：http://ww.newstarts.cn

TS:   items.join(",")
来源：http://kh.wgjwhj.cn

Java: String.join(",", items)
来源：http://xa.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://xj.huixiangedu.cn

Ruby: items.join(",")
来源：http://iv.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://hs.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://yk.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gf.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hv.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://pn.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://we.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://kx.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vq.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qu.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gn.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://sl.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rx.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kf.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://oi.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://db.huanxung.cn

Java: String.format("%03d", 7)
来源：http://et.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eh.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rq.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yv.hnjuh.cn

[E11] 反转字符串
来源：http://vb.jctech888.com.cn

Py:   s[::-1]
来源：http://by.panjiajie.cn

PHP:  strrev($s);
来源：http://ok.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://gv.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://dc.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ng.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://an.lnxyls.cn

Ruby: s.reverse
来源：http://hi.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zn.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://cz.chemitech.net.cn

Py:   s.count("a")
来源：http://gr.colortex.cn

PHP:  substr_count($s, "a");
来源：http://iz.huanxung.cn

JS:   s.split("a").length - 1
来源：http://sr.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://sr.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uq.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://rc.nszjky.cn

Ruby: s.count("a")
来源：http://sg.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://pb.gzmigu.cn

[E13] 逐字符遍历
来源：http://pt.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://aj.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ne.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wv.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zf.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vv.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ro.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eg.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dy.9csxet.cn

[E14] URL 编码与 Base64
来源：http://na.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://el.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ou.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bu.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wr.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pd.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://no.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fz.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vg.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://vs.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wa.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://st.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pr.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eo.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fl.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xk.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wi.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ve.lnxyls.cn

[E16] 数字千分位
来源：http://iv.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ng.asd995.cn

PHP:  number_format(1234567);
来源：http://av.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qi.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lz.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zz.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pc.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mq.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://vf.lnxyls.cn

[E17] 首字母大写
来源：http://ir.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yf.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yt.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://el.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ai.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yi.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://pu.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ea.huanxung.cn

[E18] 模板占位符替换
来源：http://ww.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uq.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sn.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xx.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zw.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uv.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mk.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://py.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ka.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://tw.shxzukj.cn

Py:   s.splitlines()
来源：http://qg.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pt.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://yf.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://lh.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://mk.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://pc.huixinmuqiang.cn

Ruby: s.lines
来源：http://ir.shtwfgs.cn

C#:   s.Split('\n')
来源：http://uj.9csxet.cn

[E20] 判断字符串是否为空
来源：http://jy.hnjuh.cn

Py:   if not s:
来源：http://ef.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tp.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cv.colortex.cn

TS:   if (s === "") {}
来源：http://tt.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://jp.bjjhwx.cn

Go:   if s == "" {}
来源：http://xi.hnjuh.cn

Ruby: if s.empty?
来源：http://lc.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lm.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://en.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ec.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ok.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nn.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://je.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jv.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://wl.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tv.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://me.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://rt.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uf.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ek.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rc.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mo.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gp.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fh.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://us.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://by.gzmigu.cn

================================================================================
来源：http://ef.hahajie.cn

F. 文件与目录
来源：http://az.shxzukj.cn

================================================================================
来源：http://ys.shtwfgs.cn

[F01] 读取整个文件
来源：http://mr.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dl.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://hu.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ux.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xy.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bn.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iy.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://hq.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://do.hahajie.cn

[F02] 逐行读取文件
来源：http://lt.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yn.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://us.szxytkj.cn


<!-- 参考信息 -->