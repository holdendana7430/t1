代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://vn.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nn.huanxung.cn

TS:   Math.max(...arr);
来源：http://od.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rc.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sn.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://lp.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://vt.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://zi.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ei.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://lc.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uw.bookmarksfly.cn

TS:   nested.flat();
来源：http://jp.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ni.nszjky.cn

Go:   // 手写双层循环
来源：http://aq.wgjwhj.cn

Ruby: nested.flatten
来源：http://te.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kn.shxzskj.cn

[D19] 按字段分组
来源：http://um.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yi.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qu.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pc.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wm.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ze.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://td.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://of.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://px.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://we.hahajie.cn

Py:   Counter(arr)
来源：http://ki.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://cu.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lg.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eq.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qk.asd995.cn

Go:   // 手写 map[T]int
来源：http://mz.yuexingan06.cn

Ruby: arr.tally
来源：http://rs.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sg.521024.cn

[D21] 判断是否包含某元素
来源：http://cu.huixinmuqiang.cn

Py:   x in arr
来源：http://gn.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://vq.colortex.cn

JS:   arr.includes(x)
来源：http://ow.huixiangedu.cn

TS:   arr.includes(x)
来源：http://pp.gzmigu.cn

Java: list.contains(x)
来源：http://sz.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://yo.asd995.cn

Ruby: arr.include?(x)
来源：http://ef.haigaiapp.cn

C#:   list.Contains(x)
来源：http://ax.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://nd.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yt.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iq.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xl.muxihuayi.cn

TS:   [...arr];
来源：http://sv.nszjky.cn

Java: new ArrayList<>(list);
来源：http://bo.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gx.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://zg.hnjuh.cn

C#:   new List<int>(list);
来源：http://jk.shtwfgs.cn

[D23] reduce 累积计算
来源：http://zf.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eu.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://at.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gd.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dg.panjiajie.cn

Go:   // 手写循环
来源：http://ok.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uw.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fs.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://hp.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gg.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ph.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jd.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iw.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kx.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mk.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hq.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tj.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://tr.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ev.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xi.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zt.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rd.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ks.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cb.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rf.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uq.9csxet.cn

[D26] 数组转字符串
来源：http://of.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://oh.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://nu.hahajie.cn

JS:   arr.join(", ")
来源：http://kl.huixiangedu.cn

TS:   arr.join(", ")
来源：http://fk.yuexingan06.cn

Java: String.join(", ", list)
来源：http://hl.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://lo.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://fz.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://od.nicolike.cn

================================================================================
来源：http://jg.lnxyls.cn

E. 字符串处理
来源：http://zv.shtwfgs.cn

================================================================================
来源：http://qo.newstarts.cn

[E01] 拼接字符串
来源：http://zw.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qj.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vo.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vc.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://js.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://me.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qp.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yx.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hs.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ed.9csxet.cn

Py:   "ab" * 3
来源：http://wo.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://mz.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ig.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://vd.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ba.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://jt.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://lh.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qg.colortex.cn

[E03] 截取子串
来源：http://ns.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dc.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kc.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oo.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://wp.521024.cn

Java: s.substring(1, 4)
来源：http://pg.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gv.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ux.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ng.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://mf.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://rg.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://fm.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oe.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://oz.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://gy.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://po.521024.cn

Ruby: s.index("x")
来源：http://we.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://en.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qu.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rj.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xe.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kh.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://am.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ad.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pk.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fq.panjiajie.cn

[E06] 替换子串
来源：http://ho.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://od.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vr.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hf.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://el.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ss.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ai.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uc.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://qe.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://zw.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gb.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ba.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lq.yuexingan06.cn

TS:   s.split(",")
来源：http://gt.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nk.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bc.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://ug.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rm.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://yg.yuexingan06.cn

Py:   ",".join(items)
来源：http://fn.huanxung.cn

PHP:  implode(",", $items);
来源：http://aq.shxzskj.cn

JS:   items.join(",")
来源：http://ds.huixiangedu.cn

TS:   items.join(",")
来源：http://gr.newstarts.cn

Java: String.join(",", items)
来源：http://eu.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://gc.haigaiapp.cn

Ruby: items.join(",")
来源：http://qa.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://lj.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://ek.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://go.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vv.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://cq.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://vg.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://su.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jn.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://al.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ce.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://zs.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iw.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pq.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://ir.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://nu.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://ue.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wd.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pl.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ig.shtwfgs.cn

[E11] 反转字符串
来源：http://op.panjiajie.cn

Py:   s[::-1]
来源：http://yq.jctech888.com.cn

PHP:  strrev($s);
来源：http://kh.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://jf.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://dp.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wb.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gu.nszjky.cn

Ruby: s.reverse
来源：http://le.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ic.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://xr.9csxet.cn

Py:   s.count("a")
来源：http://gg.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://uo.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://xr.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ou.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gp.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://sy.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://qv.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://ls.nicolike.cn

[E13] 逐字符遍历
来源：http://bv.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ub.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hi.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kv.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kq.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ec.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://em.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cu.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aa.nicolike.cn

[E14] URL 编码与 Base64
来源：http://mv.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mr.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://go.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ab.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dc.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mn.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ep.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lf.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yr.521024.cn

[E15] HTML 转义 / 反转义
来源：http://zw.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ws.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wz.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oq.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fh.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kc.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hq.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lf.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gy.nszjky.cn

[E16] 数字千分位
来源：http://if.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://yd.9csxet.cn

PHP:  number_format(1234567);
来源：http://tk.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jx.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tk.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zb.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yk.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tp.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://zs.muxihuayi.cn

[E17] 首字母大写
来源：http://yy.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ye.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ec.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cz.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fn.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ja.szxytkj.cn

Ruby: s.capitalize
来源：http://pd.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zp.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://qb.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fg.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bu.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ts.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ny.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lt.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hm.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pb.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ur.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://ep.nicolike.cn

Py:   s.splitlines()
来源：http://er.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ax.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://ma.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://gt.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://rn.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://we.hahajie.cn

Ruby: s.lines
来源：http://ez.521024.cn

C#:   s.Split('\n')
来源：http://dd.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://un.shtwfgs.cn

Py:   if not s:
来源：http://gn.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jf.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://by.9csxet.cn

TS:   if (s === "") {}
来源：http://tk.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://zi.bookmarksfly.cn

Go:   if s == "" {}
来源：http://bm.bookmarksfly.cn

Ruby: if s.empty?
来源：http://es.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ft.shxzukj.cn

[E21] 超长截断加省略号
来源：http://bc.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wp.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oe.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tt.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cv.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://jd.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rk.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://us.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://jh.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kn.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xu.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fp.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://up.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ml.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pe.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://uj.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aq.gzmigu.cn

================================================================================
来源：http://gb.wgjwhj.cn

F. 文件与目录
来源：http://po.haigaiapp.cn

================================================================================
来源：http://rn.521024.cn

[F01] 读取整个文件
来源：http://hb.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://us.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://db.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sj.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kg.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wm.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ht.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ib.hnjuh.cn


<!-- 参考信息 -->