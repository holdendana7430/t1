代发 wailian999

[D19] 按字段分组
来源：http://rc.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qr.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sv.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sl.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tb.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jx.asd995.cn

Go:   // 手写 map[string][]T
来源：http://hf.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wi.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cq.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://qf.szsharing.cn

Py:   Counter(arr)
来源：http://xa.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ik.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vp.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://la.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ur.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://qj.panjiajie.cn

Ruby: arr.tally
来源：http://rh.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qf.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://vz.colortex.cn

Py:   x in arr
来源：http://xw.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://cb.521024.cn

JS:   arr.includes(x)
来源：http://bh.muxihuayi.cn

TS:   arr.includes(x)
来源：http://cd.shtwfgs.cn

Java: list.contains(x)
来源：http://rg.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://tr.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://wj.haigaiapp.cn

C#:   list.Contains(x)
来源：http://az.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://px.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vq.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jp.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.haigaiapp.cn

TS:   [...arr];
来源：http://cn.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://hc.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sf.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://vf.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://lp.lnxyls.cn

[D23] reduce 累积计算
来源：http://sp.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sw.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wq.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rn.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gq.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wm.shxzskj.cn

Go:   // 手写循环
来源：http://xk.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fw.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dz.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://bf.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fr.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cj.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://em.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ha.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rs.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pc.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gx.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xv.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://wy.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ig.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hk.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pv.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bj.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wg.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://en.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nh.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fp.asd995.cn

[D26] 数组转字符串
来源：http://la.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://xt.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ty.shxzukj.cn

JS:   arr.join(", ")
来源：http://ne.shtwfgs.cn

TS:   arr.join(", ")
来源：http://wh.nicolike.cn

Java: String.join(", ", list)
来源：http://at.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://aq.nicolike.cn

Ruby: arr.join(", ")
来源：http://ma.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ek.bookmarksfly.cn

================================================================================
来源：http://ko.nicolike.cn

E. 字符串处理
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://dm.9csxet.cn

[E01] 拼接字符串
来源：http://ex.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oq.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sj.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sn.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://li.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://us.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gu.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://le.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://um.colortex.cn

[E02] 重复字符串
来源：http://pv.521024.cn

Py:   "ab" * 3
来源：http://pu.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://zd.521024.cn

JS:   "ab".repeat(3)
来源：http://em.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://bb.szsharing.cn

Java: "ab".repeat(3)
来源：http://ll.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xv.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ua.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jc.nszjky.cn

[E03] 截取子串
来源：http://jz.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zn.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://za.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fy.huanxung.cn

TS:   s.slice(1, 4)
来源：http://yj.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ov.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zf.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bh.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://bq.shxzukj.cn

[E04] 查找子串位置
来源：http://cq.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://sm.huanxung.cn

PHP:  strpos($s, "x");
来源：http://kc.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mr.shxzukj.cn

TS:   s.indexOf("x")
来源：http://gu.szxytkj.cn

Java: s.indexOf("x")
来源：http://uc.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://ii.asd995.cn

Ruby: s.index("x")
来源：http://qg.asd995.cn

C#:   s.IndexOf("x")
来源：http://nn.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://if.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tu.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ak.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wy.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lv.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rx.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://st.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vr.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ho.9csxet.cn

[E06] 替换子串
来源：http://oj.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qh.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://hi.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://wc.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ff.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yc.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://le.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://zk.521024.cn

[E07] 按分隔符拆分
来源：http://fr.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kd.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ai.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zp.szsharing.cn

TS:   s.split(",")
来源：http://ql.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cp.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ps.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://vd.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sj.hahajie.cn

[E08] 数组按分隔符合并
来源：http://gs.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://pk.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://cm.colortex.cn

JS:   items.join(",")
来源：http://pn.newstarts.cn

TS:   items.join(",")
来源：http://gy.521024.cn

Java: String.join(",", items)
来源：http://qu.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://rb.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://ek.newstarts.cn

C#:   string.Join(",", items)
来源：http://ux.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://vc.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ho.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ni.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://np.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://pd.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://yb.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ud.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fd.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://et.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://qj.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mx.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://td.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ax.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://jx.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://kc.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jo.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hi.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://za.muxihuayi.cn

[E11] 反转字符串
来源：http://jn.nszjky.cn

Py:   s[::-1]
来源：http://dz.asd995.cn

PHP:  strrev($s);
来源：http://hh.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ez.asd995.cn

TS:   [...s].reverse().join("")
来源：http://ca.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gc.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nu.nicolike.cn

Ruby: s.reverse
来源：http://hp.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qv.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://mz.asd995.cn

Py:   s.count("a")
来源：http://ln.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://yt.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://vt.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://qq.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fh.521024.cn

Go:   strings.Count(s, "a")
来源：http://dr.wgjwhj.cn

Ruby: s.count("a")
来源：http://cs.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://ch.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://am.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://sb.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fb.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bf.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ip.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://si.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qd.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fi.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ld.colortex.cn

[E14] URL 编码与 Base64
来源：http://lx.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nz.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gp.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ns.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jw.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pj.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fj.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ru.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lf.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://pr.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aj.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jq.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tc.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ac.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pd.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ih.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mc.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zo.muxihuayi.cn

[E16] 数字千分位
来源：http://ct.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://wj.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://gy.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bs.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ss.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lt.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sy.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aa.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://bc.huixiangedu.cn

[E17] 首字母大写
来源：http://ns.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rt.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ac.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://co.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jn.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hx.haigaiapp.cn

Ruby: s.capitalize
来源：http://rf.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zi.szxytkj.cn

[E18] 模板占位符替换
来源：http://fr.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gp.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zg.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mf.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tb.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qi.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yp.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wa.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zp.hahajie.cn

[E19] 多行文本按行拆分
来源：http://bl.asd995.cn

Py:   s.splitlines()
来源：http://xd.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ai.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://qa.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://uj.szxytkj.cn

Java: s.lines().toList()
来源：http://rn.521024.cn

Go:   strings.Split(s, "\n")
来源：http://vx.jianghongdianzi.cn

Ruby: s.lines
来源：http://xq.shxzskj.cn

C#:   s.Split('\n')
来源：http://oa.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://dz.hahajie.cn

Py:   if not s:
来源：http://tv.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://da.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jm.asd995.cn

TS:   if (s === "") {}
来源：http://dl.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://hl.huixiangedu.cn

Go:   if s == "" {}
来源：http://as.bjjhwx.cn

Ruby: if s.empty?
来源：http://hz.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://so.hnjuh.cn

[E21] 超长截断加省略号
来源：http://oy.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hk.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kr.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ea.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sb.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://iz.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bz.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vj.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://mc.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mt.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zz.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hv.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qc.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jb.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uw.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://dh.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sf.szsharing.cn

================================================================================
来源：http://ti.bookmarksfly.cn

F. 文件与目录
来源：http://dg.bookmarksfly.cn

================================================================================
来源：http://tu.jctech888.com.cn

[F01] 读取整个文件
来源：http://us.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yp.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://kx.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jh.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ua.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://op.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://id.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://jv.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://qg.bjjhwx.cn

[F02] 逐行读取文件
来源：http://rr.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zp.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ld.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gi.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aw.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vl.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ps.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zb.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://so.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hj.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jl.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yw.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zu.hnjuh.cn


<!-- 参考信息 -->