代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sc.521024.cn

Go:   // 手写双层循环
来源：http://zx.asd995.cn

Ruby: nested.flatten
来源：http://tq.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qv.jctech888.com.cn

[D19] 按字段分组
来源：http://bg.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eq.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pf.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mu.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dr.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jm.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://gm.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mo.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ms.asd995.cn

[D20] 统计每个元素出现次数
来源：http://dv.nicolike.cn

Py:   Counter(arr)
来源：http://hl.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://cu.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vg.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pg.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bm.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://rz.asd995.cn

Ruby: arr.tally
来源：http://na.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gb.9csxet.cn

[D21] 判断是否包含某元素
来源：http://to.haigaiapp.cn

Py:   x in arr
来源：http://me.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://cd.szsharing.cn

JS:   arr.includes(x)
来源：http://as.jctech888.com.cn

TS:   arr.includes(x)
来源：http://mc.gzmigu.cn

Java: list.contains(x)
来源：http://sq.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://lz.hnjuh.cn

Ruby: arr.include?(x)
来源：http://fb.9csxet.cn

C#:   list.Contains(x)
来源：http://ab.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://lj.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lw.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wd.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bm.hahajie.cn

TS:   [...arr];
来源：http://qc.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://yo.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://as.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://ej.jctech888.com.cn

C#:   new List<int>(list);
来源：http://mv.jctech888.com.cn

[D23] reduce 累积计算
来源：http://ee.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ky.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://se.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sp.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jd.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ud.9csxet.cn

Go:   // 手写循环
来源：http://og.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ra.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ww.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://se.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://in.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nc.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ij.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dg.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lh.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lk.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nw.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jw.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://jt.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pf.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ch.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ut.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wd.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://db.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ez.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ht.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pe.nszjky.cn

[D26] 数组转字符串
来源：http://ps.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://mg.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://ki.bjjhwx.cn

JS:   arr.join(", ")
来源：http://ne.gzmigu.cn

TS:   arr.join(", ")
来源：http://ne.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://zd.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://qg.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ru.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ll.newstarts.cn

================================================================================
来源：http://gk.yuexingan06.cn

E. 字符串处理
来源：http://ci.gzmigu.cn

================================================================================
来源：http://zp.yuexingan06.cn

[E01] 拼接字符串
来源：http://px.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lr.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hp.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://me.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tr.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xt.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fb.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jy.gzmigu.cn

[E02] 重复字符串
来源：http://cz.hahajie.cn

Py:   "ab" * 3
来源：http://jw.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://tm.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://zp.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://jd.huanxung.cn

Java: "ab".repeat(3)
来源：http://ve.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://qj.hahajie.cn

Ruby: "ab" * 3
来源：http://tz.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gg.yuexingan06.cn

[E03] 截取子串
来源：http://gt.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rs.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oq.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nv.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://yo.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://md.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://av.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zu.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://jh.bookmarksfly.cn

[E04] 查找子串位置
来源：http://eu.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://da.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ff.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tb.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ff.521024.cn

Java: s.indexOf("x")
来源：http://ve.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://oa.hnjuh.cn

Ruby: s.index("x")
来源：http://lj.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://bx.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hx.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kd.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ps.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kp.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gg.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hk.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ty.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cn.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sm.huixiangedu.cn

[E06] 替换子串
来源：http://as.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tr.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://jc.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ip.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://ow.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wh.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ym.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nq.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ps.hahajie.cn

[E07] 按分隔符拆分
来源：http://tz.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ig.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dm.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uv.huanxung.cn

TS:   s.split(",")
来源：http://dg.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yq.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pe.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://bk.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xw.szsharing.cn

[E08] 数组按分隔符合并
来源：http://re.shxzukj.cn

Py:   ",".join(items)
来源：http://lp.9csxet.cn

PHP:  implode(",", $items);
来源：http://pk.chemitech.net.cn

JS:   items.join(",")
来源：http://gp.jctech888.com.cn

TS:   items.join(",")
来源：http://vn.szsharing.cn

Java: String.join(",", items)
来源：http://bz.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://yl.521024.cn

Ruby: items.join(",")
来源：http://cd.nszjky.cn

C#:   string.Join(",", items)
来源：http://vf.521024.cn

[E09] 去除所有空白字符
来源：http://uq.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qo.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ok.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://sj.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://gx.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://uy.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mh.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yr.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://io.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://mh.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mw.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pn.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://wk.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://wu.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://re.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ch.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pt.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://al.yuntaijiaju.cn

[E11] 反转字符串
来源：http://le.colortex.cn

Py:   s[::-1]
来源：http://ea.huixiangedu.cn

PHP:  strrev($s);
来源：http://so.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://sr.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://yr.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pe.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mc.szxytkj.cn

Ruby: s.reverse
来源：http://bm.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nh.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://fb.jianghongdianzi.cn

Py:   s.count("a")
来源：http://ok.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://oj.huanxung.cn

JS:   s.split("a").length - 1
来源：http://or.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://vn.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kg.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://pm.huanxung.cn

Ruby: s.count("a")
来源：http://ad.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://mb.huanxung.cn

[E13] 逐字符遍历
来源：http://aa.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://np.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cd.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ua.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nk.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cn.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uz.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://si.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://we.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://ff.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xx.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ku.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cn.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hq.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pt.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xz.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rb.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mp.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://zo.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ea.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mw.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hm.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pl.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mj.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hq.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qo.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bg.yuntaijiaju.cn

[E16] 数字千分位
来源：http://sv.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://wn.521024.cn

PHP:  number_format(1234567);
来源：http://ky.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mh.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pc.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xl.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://um.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jd.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://oi.yuexingan06.cn

[E17] 首字母大写
来源：http://dg.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hr.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qd.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://am.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://da.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pk.colortex.cn

Ruby: s.capitalize
来源：http://cg.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gc.huixiangedu.cn

[E18] 模板占位符替换
来源：http://xx.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lb.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rc.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zb.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lo.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xa.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jx.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bz.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ci.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ke.muxihuayi.cn

Py:   s.splitlines()
来源：http://io.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vz.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://kc.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://ag.jctech888.com.cn

Java: s.lines().toList()
来源：http://zt.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://hz.szxytkj.cn

Ruby: s.lines
来源：http://ub.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://ng.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://zi.asd995.cn

Py:   if not s:
来源：http://zs.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bn.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dj.jctech888.com.cn

TS:   if (s === "") {}
来源：http://md.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://pi.yuexingan06.cn

Go:   if s == "" {}
来源：http://kq.huanxung.cn

Ruby: if s.empty?
来源：http://hm.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cj.shxzskj.cn

[E21] 超长截断加省略号
来源：http://au.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nv.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ku.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ss.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ty.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zy.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://wm.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sh.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rf.colortex.cn

[E22] 字节长度与字符长度
来源：http://ci.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ks.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jb.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lo.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qm.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bv.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gg.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://yu.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://di.lnxyls.cn

================================================================================
来源：http://yq.nszjky.cn

F. 文件与目录
来源：http://tu.yuntaijiaju.cn

================================================================================
来源：http://mn.nicolike.cn

[F01] 读取整个文件
来源：http://rp.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ro.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://sg.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ph.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mu.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ie.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gl.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://og.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://yk.asd995.cn

[F02] 逐行读取文件
来源：http://ie.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://he.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://np.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yw.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://db.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://re.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zk.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hb.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://mz.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uz.muxihuayi.cn


<!-- 参考信息 -->