代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wp.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://hj.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ui.521024.cn

[D18] 扁平化嵌套数组
来源：http://hp.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gr.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://cw.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ou.muxihuayi.cn

TS:   nested.flat();
来源：http://ov.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tj.huanxung.cn

Go:   // 手写双层循环
来源：http://ys.shxzskj.cn

Ruby: nested.flatten
来源：http://ga.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rk.huixinmuqiang.cn

[D19] 按字段分组
来源：http://hd.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://st.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ew.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gb.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kt.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://si.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://ww.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wo.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ey.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://pr.9csxet.cn

Py:   Counter(arr)
来源：http://qk.newstarts.cn

PHP:  array_count_values($arr);
来源：http://to.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wx.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gw.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qo.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://up.521024.cn

Ruby: arr.tally
来源：http://ou.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xd.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://jf.haigaiapp.cn

Py:   x in arr
来源：http://hz.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://nj.shtwfgs.cn

JS:   arr.includes(x)
来源：http://ee.muxihuayi.cn

TS:   arr.includes(x)
来源：http://ti.huixiangedu.cn

Java: list.contains(x)
来源：http://de.521024.cn

Go:   slices.Contains(arr, x)
来源：http://wv.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://qa.newstarts.cn

C#:   list.Contains(x)
来源：http://ij.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://um.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ae.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bn.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ch.newstarts.cn

TS:   [...arr];
来源：http://xh.szsharing.cn

Java: new ArrayList<>(list);
来源：http://bs.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zo.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://wk.asd995.cn

C#:   new List<int>(list);
来源：http://wh.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ns.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vh.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://om.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://we.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tr.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yt.jctech888.com.cn

Go:   // 手写循环
来源：http://ep.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ux.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pg.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://yd.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bc.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hy.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gw.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fh.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yg.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dm.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eb.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bt.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://wg.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tx.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wv.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gr.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gy.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sv.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://as.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wl.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://za.bjjhwx.cn

[D26] 数组转字符串
来源：http://ah.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://ix.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://ry.asd995.cn

JS:   arr.join(", ")
来源：http://hi.lnxyls.cn

TS:   arr.join(", ")
来源：http://dc.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ts.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://om.hahajie.cn

Ruby: arr.join(", ")
来源：http://ws.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://jn.huixinmuqiang.cn

================================================================================
来源：http://bv.hahajie.cn

E. 字符串处理
来源：http://px.szxytkj.cn

================================================================================
来源：http://jw.shxzukj.cn

[E01] 拼接字符串
来源：http://ug.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tu.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dw.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zh.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kl.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ui.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eo.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://re.lnxyls.cn

[E02] 重复字符串
来源：http://xc.wgjwhj.cn

Py:   "ab" * 3
来源：http://ol.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://zl.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://sk.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://ko.9csxet.cn

Java: "ab".repeat(3)
来源：http://ah.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://vw.shxzukj.cn

Ruby: "ab" * 3
来源：http://pq.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mo.9csxet.cn

[E03] 截取子串
来源：http://oh.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nc.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dr.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kl.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://gx.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://qe.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jn.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kf.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://qh.haigaiapp.cn

[E04] 查找子串位置
来源：http://fx.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://gm.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://er.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qo.szxytkj.cn

TS:   s.indexOf("x")
来源：http://cu.hahajie.cn

Java: s.indexOf("x")
来源：http://zh.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://pp.yuexingan06.cn

Ruby: s.index("x")
来源：http://zi.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://dm.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rn.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yv.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://my.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ud.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://os.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pm.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pv.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gq.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nq.szxytkj.cn

[E06] 替换子串
来源：http://gt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nz.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://fw.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dq.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://yd.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ib.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pn.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xi.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://nc.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://oi.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kp.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fj.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iq.panjiajie.cn

TS:   s.split(",")
来源：http://ty.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bo.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jh.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://fb.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ch.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ja.shxzukj.cn

Py:   ",".join(items)
来源：http://jz.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://dz.chemitech.net.cn

JS:   items.join(",")
来源：http://hh.muxihuayi.cn

TS:   items.join(",")
来源：http://dl.nicolike.cn

Java: String.join(",", items)
来源：http://mu.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://ca.shxzukj.cn

Ruby: items.join(",")
来源：http://li.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://st.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://kf.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://el.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nw.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mt.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://bo.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://tg.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xn.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qq.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zm.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://pj.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mk.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ld.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://qn.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://zx.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://cl.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sm.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zj.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ue.szxytkj.cn

[E11] 反转字符串
来源：http://co.asd995.cn

Py:   s[::-1]
来源：http://tw.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://ab.asd995.cn

JS:   [...s].reverse().join("")
来源：http://tq.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://hf.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yu.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ga.hnjuh.cn

Ruby: s.reverse
来源：http://yf.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://it.asd995.cn

[E12] 统计某字符出现次数
来源：http://yn.shxzskj.cn

Py:   s.count("a")
来源：http://nz.521024.cn

PHP:  substr_count($s, "a");
来源：http://xw.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://cp.9csxet.cn

TS:   s.split("a").length - 1
来源：http://rf.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hb.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://aj.nicolike.cn

Ruby: s.count("a")
来源：http://sz.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://hz.shxzukj.cn

[E13] 逐字符遍历
来源：http://ev.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://wx.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kw.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mm.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jt.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://in.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yk.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gu.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ex.huanxung.cn

[E14] URL 编码与 Base64
来源：http://tb.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zj.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://og.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://os.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vp.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bw.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jq.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://co.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yp.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://ry.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zd.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dm.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mb.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ds.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iz.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ia.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vx.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nr.huanxung.cn

[E16] 数字千分位
来源：http://yn.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://jr.szxytkj.cn

PHP:  number_format(1234567);
来源：http://vk.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pp.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lh.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gl.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zk.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zv.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ig.jianghongdianzi.cn

[E17] 首字母大写
来源：http://tk.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dl.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rz.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wz.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pg.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bb.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ia.gzmigu.cn

Ruby: s.capitalize
来源：http://tt.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wh.haigaiapp.cn

[E18] 模板占位符替换
来源：http://he.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yd.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ex.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lw.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rl.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pg.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://an.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ur.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://is.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://kw.haigaiapp.cn

Py:   s.splitlines()
来源：http://xt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ac.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://zl.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://id.shxzskj.cn

Java: s.lines().toList()
来源：http://ty.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://ww.hnjuh.cn

Ruby: s.lines
来源：http://bw.yuexingan06.cn

C#:   s.Split('\n')
来源：http://cz.colortex.cn

[E20] 判断字符串是否为空
来源：http://rv.colortex.cn

Py:   if not s:
来源：http://cz.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://td.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pz.lnxyls.cn

TS:   if (s === "") {}
来源：http://rg.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://zt.shtwfgs.cn

Go:   if s == "" {}
来源：http://vz.bjjhwx.cn

Ruby: if s.empty?
来源：http://kk.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qf.hahajie.cn

[E21] 超长截断加省略号
来源：http://tt.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rf.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jj.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hk.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ma.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://cd.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qm.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cu.hahajie.cn

[E22] 字节长度与字符长度
来源：http://sc.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tj.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://km.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gp.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rv.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sg.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ot.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://nq.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yv.521024.cn

================================================================================
来源：http://pr.hahajie.cn

F. 文件与目录
来源：http://cy.yuntaijiaju.cn

================================================================================
来源：http://ff.hnjuh.cn

[F01] 读取整个文件
来源：http://hb.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cl.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://ab.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zt.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ov.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xh.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ya.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://ok.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://kl.huanxung.cn

[F02] 逐行读取文件
来源：http://zq.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cy.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ks.lnxyls.cn


<!-- 参考信息 -->