代发 wailian999

[D19] 按字段分组
来源：http://ow.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kc.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xm.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fh.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lz.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cs.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://lj.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xx.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gw.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://cf.yuexingan06.cn

Py:   Counter(arr)
来源：http://hw.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ic.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://by.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hk.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pb.szsharing.cn

Go:   // 手写 map[T]int
来源：http://lo.9csxet.cn

Ruby: arr.tally
来源：http://vc.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ii.asd995.cn

[D21] 判断是否包含某元素
来源：http://qj.asd995.cn

Py:   x in arr
来源：http://hc.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://kj.huixiangedu.cn

JS:   arr.includes(x)
来源：http://jc.chemitech.net.cn

TS:   arr.includes(x)
来源：http://pv.nicolike.cn

Java: list.contains(x)
来源：http://ne.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://gl.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://rk.szxytkj.cn

C#:   list.Contains(x)
来源：http://wn.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://yl.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sx.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hh.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yb.chemitech.net.cn

TS:   [...arr];
来源：http://yg.colortex.cn

Java: new ArrayList<>(list);
来源：http://aq.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jk.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://ls.hnjuh.cn

C#:   new List<int>(list);
来源：http://tm.haigaiapp.cn

[D23] reduce 累积计算
来源：http://az.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://du.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ot.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hp.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vs.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oz.huixinmuqiang.cn

Go:   // 手写循环
来源：http://xg.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yn.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://va.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://tv.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sm.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fx.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qg.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lr.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ia.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oj.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xn.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xv.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://zy.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lp.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bf.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rh.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ii.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fk.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mm.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kk.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jj.lnxyls.cn

[D26] 数组转字符串
来源：http://ph.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://he.521024.cn

PHP:  implode(", ", $arr);
来源：http://zr.muxihuayi.cn

JS:   arr.join(", ")
来源：http://hh.chemitech.net.cn

TS:   arr.join(", ")
来源：http://cb.jctech888.com.cn

Java: String.join(", ", list)
来源：http://am.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://jz.shxzukj.cn

Ruby: arr.join(", ")
来源：http://xx.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://lc.shtwfgs.cn

================================================================================
来源：http://iw.shxzukj.cn

E. 字符串处理
来源：http://oc.jianghongdianzi.cn

================================================================================
来源：http://lg.panjiajie.cn

[E01] 拼接字符串
来源：http://eq.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ii.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pn.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ya.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nk.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wn.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ly.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dp.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.colortex.cn

[E02] 重复字符串
来源：http://zb.huixiangedu.cn

Py:   "ab" * 3
来源：http://ja.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://nh.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://ey.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://hj.nszjky.cn

Java: "ab".repeat(3)
来源：http://vm.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://vv.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ka.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rb.bjjhwx.cn

[E03] 截取子串
来源：http://su.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bo.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://la.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ok.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://lm.newstarts.cn

Java: s.substring(1, 4)
来源：http://xr.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wp.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gg.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://hd.szxytkj.cn

[E04] 查找子串位置
来源：http://uv.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://sc.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://gj.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qv.szsharing.cn

TS:   s.indexOf("x")
来源：http://zp.muxihuayi.cn

Java: s.indexOf("x")
来源：http://he.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://cx.huanxung.cn

Ruby: s.index("x")
来源：http://aj.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://dc.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://la.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qc.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nc.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bs.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://df.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kx.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://au.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lx.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vl.bookmarksfly.cn

[E06] 替换子串
来源：http://ei.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mk.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://jf.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ty.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://qk.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eb.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ee.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://nh.colortex.cn

[E07] 按分隔符拆分
来源：http://bo.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hg.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ac.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bn.muxihuayi.cn

TS:   s.split(",")
来源：http://au.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vr.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lu.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://md.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qg.huanxung.cn

[E08] 数组按分隔符合并
来源：http://rj.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://tv.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://bi.yuexingan06.cn

JS:   items.join(",")
来源：http://wp.panjiajie.cn

TS:   items.join(",")
来源：http://oe.jctech888.com.cn

Java: String.join(",", items)
来源：http://dz.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://kx.521024.cn

Ruby: items.join(",")
来源：http://ht.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://fg.hnjuh.cn

[E09] 去除所有空白字符
来源：http://ke.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ht.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cz.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://wy.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://lx.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://qt.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://em.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jk.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ou.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://bg.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hv.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ny.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://md.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://jy.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://rv.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qg.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://po.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bv.colortex.cn

[E11] 反转字符串
来源：http://bi.chemitech.net.cn

Py:   s[::-1]
来源：http://yk.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://dy.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://ps.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://yk.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ge.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://en.jctech888.com.cn

Ruby: s.reverse
来源：http://hy.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nr.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://pl.nszjky.cn

Py:   s.count("a")
来源：http://ge.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://rq.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://gw.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://tq.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ry.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://mv.muxihuayi.cn

Ruby: s.count("a")
来源：http://li.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://jt.521024.cn

[E13] 逐字符遍历
来源：http://cf.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://mv.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qw.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://io.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://un.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lu.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ce.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://th.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uo.hahajie.cn

[E14] URL 编码与 Base64
来源：http://cb.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dw.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vu.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ln.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ad.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ia.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lz.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pc.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oj.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://kw.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yi.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zv.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wg.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oj.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fr.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wv.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pm.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gs.9csxet.cn

[E16] 数字千分位
来源：http://jh.colortex.cn

Py:   f"{1234567:,}"
来源：http://fz.asd995.cn

PHP:  number_format(1234567);
来源：http://ef.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yd.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://km.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tr.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xm.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rh.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://bv.shtwfgs.cn

[E17] 首字母大写
来源：http://pv.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sm.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pa.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bp.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ci.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fs.wgjwhj.cn

Ruby: s.capitalize
来源：http://de.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mz.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://fl.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ba.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ne.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aj.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pl.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zv.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qo.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://du.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hk.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://me.newstarts.cn

Py:   s.splitlines()
来源：http://mn.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://io.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://vb.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://aq.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://sz.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://at.huixiangedu.cn

Ruby: s.lines
来源：http://vi.yuexingan06.cn

C#:   s.Split('\n')
来源：http://vv.9csxet.cn

[E20] 判断字符串是否为空
来源：http://la.9csxet.cn

Py:   if not s:
来源：http://gx.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ya.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://px.huixiangedu.cn

TS:   if (s === "") {}
来源：http://nk.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://nq.panjiajie.cn

Go:   if s == "" {}
来源：http://cd.chemitech.net.cn

Ruby: if s.empty?
来源：http://fd.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fj.hnjuh.cn

[E21] 超长截断加省略号
来源：http://cr.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qz.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qy.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bp.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fp.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://pr.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ns.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jk.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://vl.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qf.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ic.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ey.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ex.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cg.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iw.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://qm.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://el.muxihuayi.cn

================================================================================
来源：http://bw.hahajie.cn

F. 文件与目录
来源：http://ya.9csxet.cn

================================================================================
来源：http://qo.haigaiapp.cn

[F01] 读取整个文件
来源：http://be.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ek.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://ij.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kp.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eh.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xe.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ix.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ve.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://de.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ju.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wi.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ga.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jw.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jm.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dv.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hy.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xy.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fb.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://qn.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fn.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ce.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lu.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://th.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jc.haigaiapp.cn


<!-- 参考信息 -->