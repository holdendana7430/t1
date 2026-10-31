代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xz.9csxet.cn

Go:   // 手写双层循环
来源：http://nn.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://rc.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iu.shxzskj.cn

[D19] 按字段分组
来源：http://aj.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bz.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vx.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fy.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ys.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yw.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://se.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tz.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ed.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://aw.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://oj.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://wh.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ri.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dg.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://bk.9csxet.cn

Ruby: arr.tally
来源：http://fj.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://et.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://ih.jctech888.com.cn

Py:   x in arr
来源：http://bg.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://yi.nszjky.cn

JS:   arr.includes(x)
来源：http://nk.nszjky.cn

TS:   arr.includes(x)
来源：http://dy.chemitech.net.cn

Java: list.contains(x)
来源：http://xo.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://lj.asd995.cn

Ruby: arr.include?(x)
来源：http://om.hahajie.cn

C#:   list.Contains(x)
来源：http://zf.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://ix.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kz.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aw.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dk.lnxyls.cn

TS:   [...arr];
来源：http://ir.521024.cn

Java: new ArrayList<>(list);
来源：http://an.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cc.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://xp.panjiajie.cn

C#:   new List<int>(list);
来源：http://wy.nszjky.cn

[D23] reduce 累积计算
来源：http://tx.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yy.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://et.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rt.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nr.newstarts.cn

Go:   // 手写循环
来源：http://te.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ai.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nc.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://wq.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ov.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aw.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fp.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://is.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ze.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kv.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wc.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xl.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://an.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rx.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lv.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qk.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://td.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vu.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://le.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oj.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jb.hnjuh.cn

[D26] 数组转字符串
来源：http://ol.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ui.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://iy.nszjky.cn

JS:   arr.join(", ")
来源：http://yw.asd995.cn

TS:   arr.join(", ")
来源：http://gv.shxzskj.cn

Java: String.join(", ", list)
来源：http://ot.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://vt.hahajie.cn

Ruby: arr.join(", ")
来源：http://ba.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://ae.9csxet.cn

================================================================================
来源：http://ej.asd995.cn

E. 字符串处理
来源：http://zh.gzmigu.cn

================================================================================
来源：http://tx.nicolike.cn

[E01] 拼接字符串
来源：http://ih.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cb.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ne.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ml.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qf.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wf.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vg.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iw.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xp.shtwfgs.cn

[E02] 重复字符串
来源：http://ha.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://jv.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://ks.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://du.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://le.newstarts.cn

Java: "ab".repeat(3)
来源：http://oz.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://pl.shxzskj.cn

Ruby: "ab" * 3
来源：http://wk.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jd.newstarts.cn

[E03] 截取子串
来源：http://bc.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://up.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xp.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ya.newstarts.cn

TS:   s.slice(1, 4)
来源：http://qs.asd995.cn

Java: s.substring(1, 4)
来源：http://om.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ts.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tn.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://js.shxzskj.cn

[E04] 查找子串位置
来源：http://mo.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://ya.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://tb.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pe.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ui.jctech888.com.cn

Java: s.indexOf("x")
来源：http://pn.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://cd.bookmarksfly.cn

Ruby: s.index("x")
来源：http://xs.521024.cn

C#:   s.IndexOf("x")
来源：http://ga.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nx.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oc.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sn.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ff.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vq.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://be.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rd.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qu.shtwfgs.cn

[E06] 替换子串
来源：http://ll.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fv.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://yw.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rr.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://lt.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zb.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dm.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zy.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://uu.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://hp.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ur.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ke.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kg.shxzskj.cn

TS:   s.split(",")
来源：http://cm.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fd.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ww.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://ce.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://up.nicolike.cn

[E08] 数组按分隔符合并
来源：http://jt.asd995.cn

Py:   ",".join(items)
来源：http://un.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ko.nicolike.cn

JS:   items.join(",")
来源：http://jt.bookmarksfly.cn

TS:   items.join(",")
来源：http://cm.shxzskj.cn

Java: String.join(",", items)
来源：http://vf.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://kr.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://mg.shxzskj.cn

C#:   string.Join(",", items)
来源：http://qk.gzmigu.cn

[E09] 去除所有空白字符
来源：http://ti.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kl.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ki.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://yw.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://kp.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://yn.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://li.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iq.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wz.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://yl.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vr.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yq.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://hm.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://zn.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://yj.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cb.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lh.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uq.jianghongdianzi.cn

[E11] 反转字符串
来源：http://eh.szsharing.cn

Py:   s[::-1]
来源：http://wq.haigaiapp.cn

PHP:  strrev($s);
来源：http://oz.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://az.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://bm.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pr.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wz.shtwfgs.cn

Ruby: s.reverse
来源：http://sz.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rb.9csxet.cn

[E12] 统计某字符出现次数
来源：http://vl.bookmarksfly.cn

Py:   s.count("a")
来源：http://ch.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://wr.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://ig.nicolike.cn

TS:   s.split("a").length - 1
来源：http://oa.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vr.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://em.bookmarksfly.cn

Ruby: s.count("a")
来源：http://gj.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://cl.hnjuh.cn

[E13] 逐字符遍历
来源：http://bn.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://sd.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wj.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fn.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xo.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lk.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hv.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lz.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pz.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://cl.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fp.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ax.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xa.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qy.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ma.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oe.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tv.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hh.521024.cn

[E15] HTML 转义 / 反转义
来源：http://af.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ay.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://em.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ke.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ec.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fz.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dm.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://un.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mm.shxzukj.cn

[E16] 数字千分位
来源：http://uz.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://ds.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://bs.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gf.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dy.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pq.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xy.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kx.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://jb.yuexingan06.cn

[E17] 首字母大写
来源：http://gc.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fs.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ya.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lg.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oh.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://js.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wb.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://no.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jq.huanxung.cn

[E18] 模板占位符替换
来源：http://yf.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ga.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sz.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ec.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ba.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fi.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rk.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ih.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://se.huanxung.cn

[E19] 多行文本按行拆分
来源：http://zn.hahajie.cn

Py:   s.splitlines()
来源：http://yu.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hj.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://ob.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://il.shxzskj.cn

Java: s.lines().toList()
来源：http://qu.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://aa.hahajie.cn

Ruby: s.lines
来源：http://oe.shtwfgs.cn

C#:   s.Split('\n')
来源：http://qx.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://rj.nicolike.cn

Py:   if not s:
来源：http://vs.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://si.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cn.newstarts.cn

TS:   if (s === "") {}
来源：http://vl.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://bg.9csxet.cn

Go:   if s == "" {}
来源：http://uv.yuexingan06.cn

Ruby: if s.empty?
来源：http://xz.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kj.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://cw.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rx.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jf.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kd.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kv.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ea.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ha.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://el.521024.cn

[E22] 字节长度与字符长度
来源：http://ei.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gq.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wo.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://su.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hf.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jo.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://zk.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://yi.szsharing.cn

F. 文件与目录
来源：http://lu.hahajie.cn

================================================================================
来源：http://zv.nszjky.cn

[F01] 读取整个文件
来源：http://pa.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yh.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://uq.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dp.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wt.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xs.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gk.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://yr.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://df.gzmigu.cn

[F02] 逐行读取文件
来源：http://rz.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://py.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rm.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wi.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yk.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yr.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xm.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zr.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://io.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://tl.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xg.haigaiapp.cn


<!-- 参考信息 -->