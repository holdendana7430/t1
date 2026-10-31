代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gs.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ic.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://sq.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ye.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sl.colortex.cn

PHP:  array_merge(...$nested);
来源：http://gf.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oi.9csxet.cn

TS:   nested.flat();
来源：http://la.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mm.panjiajie.cn

Go:   // 手写双层循环
来源：http://pa.jctech888.com.cn

Ruby: nested.flatten
来源：http://ri.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bv.lnxyls.cn

[D19] 按字段分组
来源：http://qm.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rl.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ib.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cb.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://px.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://si.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ov.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cw.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fb.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://zz.muxihuayi.cn

Py:   Counter(arr)
来源：http://sv.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://oy.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fo.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ee.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://rn.jctech888.com.cn

Ruby: arr.tally
来源：http://is.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nm.szsharing.cn

[D21] 判断是否包含某元素
来源：http://rr.yuntaijiaju.cn

Py:   x in arr
来源：http://vi.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://hf.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://gg.chemitech.net.cn

TS:   arr.includes(x)
来源：http://dx.panjiajie.cn

Java: list.contains(x)
来源：http://hq.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://jk.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://gu.huanxung.cn

C#:   list.Contains(x)
来源：http://hu.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://yc.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wf.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oz.yuntaijiaju.cn

TS:   [...arr];
来源：http://lp.nszjky.cn

Java: new ArrayList<>(list);
来源：http://gk.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jc.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://xg.newstarts.cn

C#:   new List<int>(list);
来源：http://gb.hnjuh.cn

[D23] reduce 累积计算
来源：http://zx.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jv.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ze.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dc.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hq.panjiajie.cn

Go:   // 手写循环
来源：http://we.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oy.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zh.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://gr.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qi.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yx.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wc.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ly.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ut.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dh.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kc.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ev.colortex.cn

[D25] Set 集合去重与交并差
来源：http://ik.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uc.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hi.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ov.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xf.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uq.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wh.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yq.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sy.bjjhwx.cn

[D26] 数组转字符串
来源：http://jl.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://kd.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://le.haigaiapp.cn

JS:   arr.join(", ")
来源：http://dn.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ib.huanxung.cn

Java: String.join(", ", list)
来源：http://hb.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://qa.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://jn.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://cm.bjjhwx.cn

================================================================================
来源：http://jl.nicolike.cn

E. 字符串处理
来源：http://xv.hnjuh.cn

================================================================================
来源：http://ng.9csxet.cn

[E01] 拼接字符串
来源：http://mn.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://th.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sq.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tb.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fa.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://de.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xj.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xe.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wr.lnxyls.cn

[E02] 重复字符串
来源：http://vd.colortex.cn

Py:   "ab" * 3
来源：http://ky.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://ng.szsharing.cn

JS:   "ab".repeat(3)
来源：http://uj.hahajie.cn

TS:   "ab".repeat(3)
来源：http://vh.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://co.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://gu.huixiangedu.cn

Ruby: "ab" * 3
来源：http://zh.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://so.colortex.cn

[E03] 截取子串
来源：http://ju.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lf.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ra.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wt.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ru.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://fc.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ku.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sb.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://fc.lnxyls.cn

[E04] 查找子串位置
来源：http://bg.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://lq.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://kf.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fz.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ib.hahajie.cn

Java: s.indexOf("x")
来源：http://sd.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://ta.gzmigu.cn

Ruby: s.index("x")
来源：http://fs.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://eq.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ad.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pw.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cr.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://of.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qo.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://od.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ze.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ae.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xk.chemitech.net.cn

[E06] 替换子串
来源：http://th.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kr.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dw.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://lf.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nn.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pz.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gr.521024.cn

C#:   s.Replace("a", "b")
来源：http://yh.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://rw.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xc.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hn.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xj.szsharing.cn

TS:   s.split(",")
来源：http://vf.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rr.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yn.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://dh.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hx.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://vq.wgjwhj.cn

Py:   ",".join(items)
来源：http://qj.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://nb.wgjwhj.cn

JS:   items.join(",")
来源：http://mv.nszjky.cn

TS:   items.join(",")
来源：http://ro.yuexingan06.cn

Java: String.join(",", items)
来源：http://dz.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://qo.wgjwhj.cn

Ruby: items.join(",")
来源：http://ct.hahajie.cn

C#:   string.Join(",", items)
来源：http://gh.huanxung.cn

[E09] 去除所有空白字符
来源：http://zp.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gx.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jt.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zf.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://na.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://fg.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zs.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hz.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tz.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://yr.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kw.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ff.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://iu.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://vb.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://pd.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hr.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kp.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fl.haigaiapp.cn

[E11] 反转字符串
来源：http://yc.huixiangedu.cn

Py:   s[::-1]
来源：http://az.panjiajie.cn

PHP:  strrev($s);
来源：http://tg.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://we.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://uu.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ku.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kn.yuexingan06.cn

Ruby: s.reverse
来源：http://jd.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pt.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://jb.huanxung.cn

Py:   s.count("a")
来源：http://jr.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://qi.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://yq.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://hn.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ke.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://vf.muxihuayi.cn

Ruby: s.count("a")
来源：http://xb.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://qx.colortex.cn

[E13] 逐字符遍历
来源：http://xt.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://gu.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sf.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fe.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://az.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qd.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uh.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://od.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://as.nicolike.cn

[E14] URL 编码与 Base64
来源：http://kq.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hh.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mj.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fg.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ok.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ez.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zt.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dg.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sm.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://yc.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nk.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sb.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ls.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ke.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://js.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://do.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qh.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pt.asd995.cn

[E16] 数字千分位
来源：http://ge.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://sg.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ba.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uy.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pj.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wm.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ll.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zs.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://sk.newstarts.cn

[E17] 首字母大写
来源：http://yk.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yo.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://im.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jc.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bl.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fr.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pt.newstarts.cn

Ruby: s.capitalize
来源：http://bc.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://js.shxzskj.cn

[E18] 模板占位符替换
来源：http://fh.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pd.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bh.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bo.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nf.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qm.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sv.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ed.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pp.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://dp.yuexingan06.cn

Py:   s.splitlines()
来源：http://ae.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dk.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://kr.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://ru.yuexingan06.cn

Java: s.lines().toList()
来源：http://pm.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://aq.yuntaijiaju.cn

Ruby: s.lines
来源：http://wb.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ng.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://qu.hahajie.cn

Py:   if not s:
来源：http://kh.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uw.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yj.jctech888.com.cn

TS:   if (s === "") {}
来源：http://wj.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://ud.hahajie.cn

Go:   if s == "" {}
来源：http://kz.521024.cn

Ruby: if s.empty?
来源：http://ft.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ga.panjiajie.cn

[E21] 超长截断加省略号
来源：http://of.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ip.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ht.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bx.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yt.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vg.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ey.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ri.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mr.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://eu.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ac.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ji.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qm.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bh.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://um.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uh.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://me.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eb.gzmigu.cn

================================================================================
来源：http://km.chemitech.net.cn

F. 文件与目录
来源：http://wj.9csxet.cn

================================================================================
来源：http://qw.szsharing.cn

[F01] 读取整个文件
来源：http://ea.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wr.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://sv.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zf.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xn.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sr.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ts.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://uo.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://xa.colortex.cn

[F02] 逐行读取文件
来源：http://ls.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vo.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tz.hahajie.cn


<!-- 参考信息 -->