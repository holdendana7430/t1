代发 wailian999

[D19] 按字段分组
来源：http://rc.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ct.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oj.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tq.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cs.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vv.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://im.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vg.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://if.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://tx.shtwfgs.cn

Py:   Counter(arr)
来源：http://yv.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://dp.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ys.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hi.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cp.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://un.muxihuayi.cn

Ruby: arr.tally
来源：http://qw.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vw.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://dr.haigaiapp.cn

Py:   x in arr
来源：http://xo.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://fb.szsharing.cn

JS:   arr.includes(x)
来源：http://ew.shxzskj.cn

TS:   arr.includes(x)
来源：http://bs.shtwfgs.cn

Java: list.contains(x)
来源：http://ju.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://mf.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://ap.lnxyls.cn

C#:   list.Contains(x)
来源：http://qf.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://pm.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mk.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ff.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nd.9csxet.cn

TS:   [...arr];
来源：http://uk.521024.cn

Java: new ArrayList<>(list);
来源：http://zy.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fi.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://eu.colortex.cn

C#:   new List<int>(list);
来源：http://fk.gzmigu.cn

[D23] reduce 累积计算
来源：http://rr.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://um.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vx.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mb.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wd.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ac.shtwfgs.cn

Go:   // 手写循环
来源：http://qs.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wp.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cg.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://yu.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tm.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gp.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ig.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://co.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://si.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bn.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ts.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://tb.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hs.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xa.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bw.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wz.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pq.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xm.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://db.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ez.colortex.cn

[D26] 数组转字符串
来源：http://hu.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://ax.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://jj.chemitech.net.cn

JS:   arr.join(", ")
来源：http://xr.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ia.jctech888.com.cn

Java: String.join(", ", list)
来源：http://bd.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://kc.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://cw.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://fg.szxytkj.cn

================================================================================
来源：http://zy.jianghongdianzi.cn

E. 字符串处理
来源：http://nz.shxzskj.cn

================================================================================
来源：http://ve.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://lm.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gt.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sx.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://st.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zy.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://og.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kr.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nr.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iy.9csxet.cn

[E02] 重复字符串
来源：http://oc.haigaiapp.cn

Py:   "ab" * 3
来源：http://yl.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://hc.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://bl.521024.cn

TS:   "ab".repeat(3)
来源：http://ja.newstarts.cn

Java: "ab".repeat(3)
来源：http://lu.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ha.nszjky.cn

Ruby: "ab" * 3
来源：http://zw.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oa.asd995.cn

[E03] 截取子串
来源：http://sh.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vr.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nu.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ie.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://lr.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://aq.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rl.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tu.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://zh.huanxung.cn

[E04] 查找子串位置
来源：http://fa.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://er.nicolike.cn

PHP:  strpos($s, "x");
来源：http://qc.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ne.9csxet.cn

TS:   s.indexOf("x")
来源：http://lc.szsharing.cn

Java: s.indexOf("x")
来源：http://py.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://wy.jctech888.com.cn

Ruby: s.index("x")
来源：http://re.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://mw.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cw.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gv.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vm.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ah.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aw.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pk.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jc.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yu.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hr.bjjhwx.cn

[E06] 替换子串
来源：http://rt.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bu.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://sl.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jg.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://de.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eg.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zr.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qa.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://qx.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://mu.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dx.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ax.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vg.hnjuh.cn

TS:   s.split(",")
来源：http://xg.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sh.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wi.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://wl.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gd.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://xg.muxihuayi.cn

Py:   ",".join(items)
来源：http://ea.colortex.cn

PHP:  implode(",", $items);
来源：http://qk.szsharing.cn

JS:   items.join(",")
来源：http://vu.muxihuayi.cn

TS:   items.join(",")
来源：http://hk.yuexingan06.cn

Java: String.join(",", items)
来源：http://kv.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://kz.shxzskj.cn

Ruby: items.join(",")
来源：http://ku.colortex.cn

C#:   string.Join(",", items)
来源：http://mz.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://at.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nm.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ow.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://yr.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://vb.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://rs.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yc.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oi.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qj.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://rx.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rb.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xk.521024.cn

JS:   "7".padStart(3, "0")
来源：http://hn.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://cj.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://hc.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qa.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jk.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mk.colortex.cn

[E11] 反转字符串
来源：http://gk.huixiangedu.cn

Py:   s[::-1]
来源：http://qo.jctech888.com.cn

PHP:  strrev($s);
来源：http://tw.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://co.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://at.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fz.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hh.9csxet.cn

Ruby: s.reverse
来源：http://kt.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xy.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://zf.hahajie.cn

Py:   s.count("a")
来源：http://jp.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ww.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ts.huanxung.cn

TS:   s.split("a").length - 1
来源：http://ng.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wg.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://ub.bookmarksfly.cn

Ruby: s.count("a")
来源：http://rz.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://dw.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://lg.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://qo.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vj.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://up.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tb.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tt.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cn.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://op.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xf.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://fp.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://up.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ad.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ij.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uy.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zm.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xe.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yj.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ki.521024.cn

[E15] HTML 转义 / 反转义
来源：http://qb.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xh.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ns.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pg.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rb.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zr.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ea.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sr.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mv.bookmarksfly.cn

[E16] 数字千分位
来源：http://fo.nszjky.cn

Py:   f"{1234567:,}"
来源：http://wb.asd995.cn

PHP:  number_format(1234567);
来源：http://vt.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cy.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nk.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://de.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lt.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sv.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://wn.hahajie.cn

[E17] 首字母大写
来源：http://zy.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dt.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://br.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nj.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bm.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jb.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uk.hahajie.cn

Ruby: s.capitalize
来源：http://gh.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://br.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://up.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ra.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sh.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bz.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gc.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ga.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qz.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dl.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qw.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ho.521024.cn

Py:   s.splitlines()
来源：http://ni.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vt.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://wh.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://mr.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://hn.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://xk.lnxyls.cn

Ruby: s.lines
来源：http://tf.haigaiapp.cn

C#:   s.Split('\n')
来源：http://mq.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ue.nicolike.cn

Py:   if not s:
来源：http://mn.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ks.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jw.shxzukj.cn

TS:   if (s === "") {}
来源：http://ij.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://va.haigaiapp.cn

Go:   if s == "" {}
来源：http://qt.bookmarksfly.cn

Ruby: if s.empty?
来源：http://zf.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gl.szsharing.cn

[E21] 超长截断加省略号
来源：http://qr.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://el.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gy.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kr.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ee.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://us.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://nb.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fv.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rd.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://ll.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sc.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ga.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fa.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hb.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tl.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://wz.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ty.lnxyls.cn

================================================================================
来源：http://ke.huixiangedu.cn

F. 文件与目录
来源：http://jm.wgjwhj.cn

================================================================================
来源：http://ac.panjiajie.cn

[F01] 读取整个文件
来源：http://ne.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uj.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://br.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qk.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lx.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qg.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sj.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://vh.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://yb.shxzskj.cn

[F02] 逐行读取文件
来源：http://od.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hu.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kh.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vd.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tg.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ri.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jw.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rk.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://le.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://wj.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tu.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://il.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vp.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ei.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://id.hahajie.cn


<!-- 参考信息 -->