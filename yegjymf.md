代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ds.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://iu.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pg.szsharing.cn

TS:   nested.flat();
来源：http://tj.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tk.521024.cn

Go:   // 手写双层循环
来源：http://te.gzmigu.cn

Ruby: nested.flatten
来源：http://mq.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ip.nszjky.cn

[D19] 按字段分组
来源：http://qu.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://on.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fc.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kb.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gx.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pi.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://cu.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wi.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ke.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://lf.asd995.cn

Py:   Counter(arr)
来源：http://ma.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://zg.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ml.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xn.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gb.nicolike.cn

Go:   // 手写 map[T]int
来源：http://gt.asd995.cn

Ruby: arr.tally
来源：http://fm.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://be.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://cw.wgjwhj.cn

Py:   x in arr
来源：http://kx.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://jk.haigaiapp.cn

JS:   arr.includes(x)
来源：http://ng.muxihuayi.cn

TS:   arr.includes(x)
来源：http://sc.jianghongdianzi.cn

Java: list.contains(x)
来源：http://ge.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://yg.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://sc.nicolike.cn

C#:   list.Contains(x)
来源：http://nd.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://no.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ep.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sc.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jk.colortex.cn

TS:   [...arr];
来源：http://jl.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://op.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tc.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://ll.hnjuh.cn

C#:   new List<int>(list);
来源：http://df.nicolike.cn

[D23] reduce 累积计算
来源：http://wl.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ze.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kl.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zf.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://df.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dt.huixiangedu.cn

Go:   // 手写循环
来源：http://jr.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iy.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dv.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://sr.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gy.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ka.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nj.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eu.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uz.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ei.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nu.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wx.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://zb.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zs.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jz.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fq.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xy.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fz.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cn.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cm.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://md.panjiajie.cn

[D26] 数组转字符串
来源：http://ix.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://bk.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://at.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://hj.muxihuayi.cn

TS:   arr.join(", ")
来源：http://to.521024.cn

Java: String.join(", ", list)
来源：http://tk.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://go.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://xg.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://ph.jianghongdianzi.cn

================================================================================
来源：http://vu.hahajie.cn

E. 字符串处理
来源：http://lw.hnjuh.cn

================================================================================
来源：http://wn.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://qu.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cx.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iq.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://le.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pa.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://to.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cg.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jo.yuexingan06.cn

[E02] 重复字符串
来源：http://qe.bookmarksfly.cn

Py:   "ab" * 3
来源：http://zw.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://mf.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://lj.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://hc.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://cu.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://kq.chemitech.net.cn

Ruby: "ab" * 3
来源：http://qz.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nl.jianghongdianzi.cn

[E03] 截取子串
来源：http://od.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://et.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fm.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fo.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ff.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://xe.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gf.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fv.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://vp.nicolike.cn

[E04] 查找子串位置
来源：http://sn.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://bx.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://oe.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fq.huanxung.cn

TS:   s.indexOf("x")
来源：http://ei.9csxet.cn

Java: s.indexOf("x")
来源：http://rv.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://no.huanxung.cn

Ruby: s.index("x")
来源：http://it.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://su.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yb.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pj.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://en.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ld.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rv.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://es.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nu.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mn.gzmigu.cn

[E06] 替换子串
来源：http://lp.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lc.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://oj.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ss.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ac.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vr.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ms.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://ua.shxzskj.cn

[E07] 按分隔符拆分
来源：http://pw.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xc.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bf.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tu.hahajie.cn

TS:   s.split(",")
来源：http://hl.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gj.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wd.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://op.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ep.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://zm.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://lt.szsharing.cn

PHP:  implode(",", $items);
来源：http://cn.shxzskj.cn

JS:   items.join(",")
来源：http://hy.szsharing.cn

TS:   items.join(",")
来源：http://ya.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://ty.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://ah.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://rl.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://pe.nicolike.cn

[E09] 去除所有空白字符
来源：http://qr.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fr.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bp.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://lp.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://zu.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://va.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xx.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dc.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wg.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://mg.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kd.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xi.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://mk.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://pd.hahajie.cn

Java: String.format("%03d", 7)
来源：http://fa.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qg.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ge.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rp.asd995.cn

[E11] 反转字符串
来源：http://kg.huixinmuqiang.cn

Py:   s[::-1]
来源：http://rw.wgjwhj.cn

PHP:  strrev($s);
来源：http://lu.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://ax.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://yr.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bx.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ps.szsharing.cn

Ruby: s.reverse
来源：http://pp.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ca.asd995.cn

[E12] 统计某字符出现次数
来源：http://ab.yuntaijiaju.cn

Py:   s.count("a")
来源：http://hz.521024.cn

PHP:  substr_count($s, "a");
来源：http://on.hahajie.cn

JS:   s.split("a").length - 1
来源：http://jl.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ci.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jx.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://ob.newstarts.cn

Ruby: s.count("a")
来源：http://wf.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://lw.lnxyls.cn

[E13] 逐字符遍历
来源：http://od.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://es.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ea.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jz.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://av.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jz.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nn.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jl.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://el.asd995.cn

[E14] URL 编码与 Base64
来源：http://sh.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ze.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oz.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xe.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pv.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://br.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rp.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eu.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kz.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://dq.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sc.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zq.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jj.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://au.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xl.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nu.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sq.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zv.asd995.cn

[E16] 数字千分位
来源：http://cn.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://in.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://ii.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hc.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ub.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rn.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dd.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qw.521024.cn

C#:   1234567.ToString("N0")
来源：http://jm.huixinmuqiang.cn

[E17] 首字母大写
来源：http://jy.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lk.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zy.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kn.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lm.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qx.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gb.newstarts.cn

Ruby: s.capitalize
来源：http://fh.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bl.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://oj.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://et.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cg.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hk.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fp.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sn.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://md.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eh.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://do.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://xp.muxihuayi.cn

Py:   s.splitlines()
来源：http://zi.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sd.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://bh.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ic.huanxung.cn

Java: s.lines().toList()
来源：http://pq.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://xq.yuexingan06.cn

Ruby: s.lines
来源：http://zx.asd995.cn

C#:   s.Split('\n')
来源：http://qj.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ty.9csxet.cn

Py:   if not s:
来源：http://tm.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zd.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://li.9csxet.cn

TS:   if (s === "") {}
来源：http://xe.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://xf.haigaiapp.cn

Go:   if s == "" {}
来源：http://ti.newstarts.cn

Ruby: if s.empty?
来源：http://mc.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dz.nszjky.cn

[E21] 超长截断加省略号
来源：http://ui.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ui.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ju.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jh.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uy.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zn.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://yi.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jm.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fn.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://cl.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ao.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yb.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hl.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kq.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ln.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://au.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vu.hnjuh.cn

================================================================================
来源：http://vj.jianghongdianzi.cn

F. 文件与目录
来源：http://ph.muxihuayi.cn

================================================================================
来源：http://xx.shtwfgs.cn

[F01] 读取整个文件
来源：http://va.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bf.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://of.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ck.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cq.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ob.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ft.nicolike.cn

Ruby: File.read("a.txt")
来源：http://hc.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://pw.szsharing.cn

[F02] 逐行读取文件
来源：http://mn.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lc.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yk.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vg.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kj.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://un.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hh.shtwfgs.cn


<!-- 参考信息 -->