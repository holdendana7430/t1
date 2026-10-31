代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://to.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://by.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://th.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://hr.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kz.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://pl.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tr.nicolike.cn

TS:   nested.flat();
来源：http://ko.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kx.lnxyls.cn

Go:   // 手写双层循环
来源：http://jl.panjiajie.cn

Ruby: nested.flatten
来源：http://sv.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wr.jianghongdianzi.cn

[D19] 按字段分组
来源：http://rm.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://af.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tb.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://do.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gr.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aj.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://gu.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ui.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fi.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://uc.huixiangedu.cn

Py:   Counter(arr)
来源：http://ws.nszjky.cn

PHP:  array_count_values($arr);
来源：http://ow.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gy.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zb.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dn.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vu.muxihuayi.cn

Ruby: arr.tally
来源：http://lm.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bm.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://dt.huixinmuqiang.cn

Py:   x in arr
来源：http://mz.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://ot.lnxyls.cn

JS:   arr.includes(x)
来源：http://hc.huanxung.cn

TS:   arr.includes(x)
来源：http://kj.muxihuayi.cn

Java: list.contains(x)
来源：http://py.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://fa.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://og.521024.cn

C#:   list.Contains(x)
来源：http://yc.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ji.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ex.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yz.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://du.haigaiapp.cn

TS:   [...arr];
来源：http://zo.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://tw.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sa.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://xp.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://ad.muxihuayi.cn

[D23] reduce 累积计算
来源：http://lm.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zf.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wx.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ak.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xh.panjiajie.cn

Go:   // 手写循环
来源：http://bc.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wd.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lv.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://tm.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jt.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yr.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sy.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ne.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rq.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gi.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rb.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dl.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://ma.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ru.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vg.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tk.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uw.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sx.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dp.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jd.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vo.yuexingan06.cn

[D26] 数组转字符串
来源：http://dr.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://tg.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://gl.muxihuayi.cn

JS:   arr.join(", ")
来源：http://ve.hnjuh.cn

TS:   arr.join(", ")
来源：http://ba.asd995.cn

Java: String.join(", ", list)
来源：http://nh.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://gm.szsharing.cn

Ruby: arr.join(", ")
来源：http://ye.9csxet.cn

C#:   string.Join(", ", list)
来源：http://nd.huixiangedu.cn

================================================================================
来源：http://hb.bjjhwx.cn

E. 字符串处理
来源：http://mw.wgjwhj.cn

================================================================================
来源：http://dx.huixiangedu.cn

[E01] 拼接字符串
来源：http://wj.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vn.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ab.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xt.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://se.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://js.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lc.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pj.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mh.szxytkj.cn

[E02] 重复字符串
来源：http://pv.yuexingan06.cn

Py:   "ab" * 3
来源：http://al.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ps.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://ch.szsharing.cn

TS:   "ab".repeat(3)
来源：http://uc.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ca.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ym.haigaiapp.cn

Ruby: "ab" * 3
来源：http://rx.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dr.shxzskj.cn

[E03] 截取子串
来源：http://ob.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mk.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dm.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hs.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ky.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://gi.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://py.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wa.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://qf.lnxyls.cn

[E04] 查找子串位置
来源：http://pb.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://pf.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://bw.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xe.lnxyls.cn

TS:   s.indexOf("x")
来源：http://dg.chemitech.net.cn

Java: s.indexOf("x")
来源：http://fc.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://pg.yuexingan06.cn

Ruby: s.index("x")
来源：http://mv.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://ug.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sw.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nz.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kr.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rb.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sx.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ym.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ch.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ex.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wt.asd995.cn

[E06] 替换子串
来源：http://qs.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tl.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://cz.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oh.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://el.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qi.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yi.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jf.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://tq.hnjuh.cn

[E07] 按分隔符拆分
来源：http://jh.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nc.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ti.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ys.nszjky.cn

TS:   s.split(",")
来源：http://xp.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ud.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ci.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://kz.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://my.hahajie.cn

[E08] 数组按分隔符合并
来源：http://hq.shxzukj.cn

Py:   ",".join(items)
来源：http://fw.newstarts.cn

PHP:  implode(",", $items);
来源：http://qq.muxihuayi.cn

JS:   items.join(",")
来源：http://od.huixiangedu.cn

TS:   items.join(",")
来源：http://ky.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://nj.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://mm.newstarts.cn

Ruby: items.join(",")
来源：http://hk.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://wi.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ui.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xj.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hk.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yn.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://op.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://nh.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cf.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mj.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oz.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://yl.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hv.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gm.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://vm.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://ls.nicolike.cn

Java: String.format("%03d", 7)
来源：http://yx.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tx.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ds.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yi.jctech888.com.cn

[E11] 反转字符串
来源：http://ou.nszjky.cn

Py:   s[::-1]
来源：http://sq.chemitech.net.cn

PHP:  strrev($s);
来源：http://qx.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://fa.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://ks.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cz.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yk.jianghongdianzi.cn

Ruby: s.reverse
来源：http://dn.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vy.hahajie.cn

[E12] 统计某字符出现次数
来源：http://jv.bjjhwx.cn

Py:   s.count("a")
来源：http://nh.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://va.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://ot.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://cu.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gb.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://et.nicolike.cn

Ruby: s.count("a")
来源：http://pn.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://rz.bjjhwx.cn

[E13] 逐字符遍历
来源：http://iz.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://nm.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://if.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yo.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pp.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bu.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bm.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xn.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hl.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://yt.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bu.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pt.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gs.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://im.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jf.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hw.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ns.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ji.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://hh.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wp.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wu.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rm.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://or.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vn.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mk.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zf.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kh.yuntaijiaju.cn

[E16] 数字千分位
来源：http://vz.nszjky.cn

Py:   f"{1234567:,}"
来源：http://yc.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://jq.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cu.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gf.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wg.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fn.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cz.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://bx.bookmarksfly.cn

[E17] 首字母大写
来源：http://ia.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rc.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kr.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ap.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vx.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mm.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wi.chemitech.net.cn

Ruby: s.capitalize
来源：http://fg.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ve.huixiangedu.cn

[E18] 模板占位符替换
来源：http://nr.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yg.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pr.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ub.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ua.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qi.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yh.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wj.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ch.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://vk.9csxet.cn

Py:   s.splitlines()
来源：http://rc.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ql.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://fj.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://uo.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://vk.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://qr.asd995.cn

Ruby: s.lines
来源：http://ag.9csxet.cn

C#:   s.Split('\n')
来源：http://da.521024.cn

[E20] 判断字符串是否为空
来源：http://gx.szxytkj.cn

Py:   if not s:
来源：http://gh.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hw.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bg.huanxung.cn

TS:   if (s === "") {}
来源：http://ca.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://sk.gzmigu.cn

Go:   if s == "" {}
来源：http://qj.colortex.cn

Ruby: if s.empty?
来源：http://bj.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://km.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://qh.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ox.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rc.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fp.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ty.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://um.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://wm.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ny.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://un.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://ed.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zz.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ij.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vb.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yo.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cq.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eo.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ru.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zv.nszjky.cn

================================================================================
来源：http://vd.jianghongdianzi.cn

F. 文件与目录
来源：http://sx.nszjky.cn

================================================================================
来源：http://wy.asd995.cn

[F01] 读取整个文件
来源：http://wv.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yo.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://ai.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yc.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://id.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yb.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zl.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://py.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://il.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ag.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gx.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hm.szsharing.cn


<!-- 参考信息 -->