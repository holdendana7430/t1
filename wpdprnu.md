代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://eq.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hd.colortex.cn

Go:   // 手写 map[string][]T
来源：http://ha.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rk.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kb.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://zn.szxytkj.cn

Py:   Counter(arr)
来源：http://gi.nszjky.cn

PHP:  array_count_values($arr);
来源：http://sm.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ex.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bs.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cg.colortex.cn

Go:   // 手写 map[T]int
来源：http://os.szxytkj.cn

Ruby: arr.tally
来源：http://kt.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iq.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://zu.haigaiapp.cn

Py:   x in arr
来源：http://ht.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://iw.nszjky.cn

JS:   arr.includes(x)
来源：http://en.asd995.cn

TS:   arr.includes(x)
来源：http://vd.huixinmuqiang.cn

Java: list.contains(x)
来源：http://tg.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://ir.521024.cn

Ruby: arr.include?(x)
来源：http://qe.colortex.cn

C#:   list.Contains(x)
来源：http://sq.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://hn.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bl.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vy.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sq.huixinmuqiang.cn

TS:   [...arr];
来源：http://jx.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://cy.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ko.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://yx.huanxung.cn

C#:   new List<int>(list);
来源：http://kw.shxzukj.cn

[D23] reduce 累积计算
来源：http://qb.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qv.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wc.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ey.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://go.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fq.colortex.cn

Go:   // 手写循环
来源：http://kx.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sf.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ci.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://fp.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wg.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mo.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://li.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vy.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dy.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jc.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bh.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uw.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://wt.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mg.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qf.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bc.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zp.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://db.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nk.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qc.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yk.huanxung.cn

[D26] 数组转字符串
来源：http://zj.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://xv.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://zz.chemitech.net.cn

JS:   arr.join(", ")
来源：http://ip.asd995.cn

TS:   arr.join(", ")
来源：http://vd.panjiajie.cn

Java: String.join(", ", list)
来源：http://mw.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://cg.newstarts.cn

Ruby: arr.join(", ")
来源：http://ni.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ry.gzmigu.cn

================================================================================
来源：http://zd.hahajie.cn

E. 字符串处理
来源：http://li.hnjuh.cn

================================================================================
来源：http://aj.wgjwhj.cn

[E01] 拼接字符串
来源：http://qg.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pg.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zi.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nk.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://al.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mv.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rn.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wl.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kn.lnxyls.cn

[E02] 重复字符串
来源：http://lu.huixiangedu.cn

Py:   "ab" * 3
来源：http://tr.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://rb.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ec.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://nl.szsharing.cn

Java: "ab".repeat(3)
来源：http://ma.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://la.9csxet.cn

Ruby: "ab" * 3
来源：http://me.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fd.panjiajie.cn

[E03] 截取子串
来源：http://ux.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pv.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jg.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bb.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://sw.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://iu.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oh.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uj.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://zu.gzmigu.cn

[E04] 查找子串位置
来源：http://uv.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://zb.nszjky.cn

PHP:  strpos($s, "x");
来源：http://aq.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aj.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://er.shtwfgs.cn

Java: s.indexOf("x")
来源：http://md.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://ne.bookmarksfly.cn

Ruby: s.index("x")
来源：http://rz.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://vm.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ps.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://by.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xk.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://or.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aa.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ay.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zg.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dr.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ur.newstarts.cn

[E06] 替换子串
来源：http://gj.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vb.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://wk.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vq.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://bl.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pz.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zz.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ci.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://su.shxzskj.cn

[E07] 按分隔符拆分
来源：http://jv.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sp.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fr.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kt.asd995.cn

TS:   s.split(",")
来源：http://jc.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zq.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://in.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://qf.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vh.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://gu.yuexingan06.cn

Py:   ",".join(items)
来源：http://fz.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://zy.gzmigu.cn

JS:   items.join(",")
来源：http://ns.yuexingan06.cn

TS:   items.join(",")
来源：http://sr.bookmarksfly.cn

Java: String.join(",", items)
来源：http://mf.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://zz.shxzukj.cn

Ruby: items.join(",")
来源：http://xb.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://ay.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://qv.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cs.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gz.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://tq.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://dp.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://qk.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fz.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bb.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pv.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://fe.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wi.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fq.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://tb.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://zm.asd995.cn

Java: String.format("%03d", 7)
来源：http://pp.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oh.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://if.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nl.jctech888.com.cn

[E11] 反转字符串
来源：http://rr.asd995.cn

Py:   s[::-1]
来源：http://vf.hnjuh.cn

PHP:  strrev($s);
来源：http://go.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://kk.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://fb.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qh.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cw.muxihuayi.cn

Ruby: s.reverse
来源：http://qz.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dw.colortex.cn

[E12] 统计某字符出现次数
来源：http://bj.521024.cn

Py:   s.count("a")
来源：http://by.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://up.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://eo.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://fz.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gi.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://lq.asd995.cn

Ruby: s.count("a")
来源：http://nw.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://jx.shxzskj.cn

[E13] 逐字符遍历
来源：http://ow.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://hj.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pr.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tp.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kg.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://it.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rr.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ii.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qy.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://ts.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xs.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://px.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xp.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rc.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ow.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uf.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ro.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tm.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://mm.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ek.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ui.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ya.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://te.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mu.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ml.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xo.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gd.gzmigu.cn

[E16] 数字千分位
来源：http://wj.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://tj.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://rs.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pq.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ia.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qf.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://su.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cb.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://jp.9csxet.cn

[E17] 首字母大写
来源：http://gw.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ja.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ee.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mn.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pt.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sd.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ud.nicolike.cn

Ruby: s.capitalize
来源：http://cy.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rp.haigaiapp.cn

[E18] 模板占位符替换
来源：http://ta.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ra.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hq.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uu.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mw.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rp.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yl.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://na.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ik.9csxet.cn

[E19] 多行文本按行拆分
来源：http://tf.colortex.cn

Py:   s.splitlines()
来源：http://fe.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wi.521024.cn

JS:   s.split(/\r?\n/)
来源：http://rt.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ki.jctech888.com.cn

Java: s.lines().toList()
来源：http://eu.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://qs.huixiangedu.cn

Ruby: s.lines
来源：http://hh.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://fk.nszjky.cn

[E20] 判断字符串是否为空
来源：http://oe.lnxyls.cn

Py:   if not s:
来源：http://gq.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ie.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rm.chemitech.net.cn

TS:   if (s === "") {}
来源：http://vm.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://hj.yuexingan06.cn

Go:   if s == "" {}
来源：http://ps.nicolike.cn

Ruby: if s.empty?
来源：http://kq.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oo.szxytkj.cn

[E21] 超长截断加省略号
来源：http://nv.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vm.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lz.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dy.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ee.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fg.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://zj.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yq.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bt.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://ci.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dr.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vp.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xh.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ao.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ps.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gc.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://tq.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rb.nszjky.cn

================================================================================
来源：http://lz.szsharing.cn

F. 文件与目录
来源：http://dv.lnxyls.cn

================================================================================
来源：http://gk.gzmigu.cn

[F01] 读取整个文件
来源：http://bq.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xb.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://dl.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ig.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rz.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zi.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://va.asd995.cn

Ruby: File.read("a.txt")
来源：http://ht.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wc.yuexingan06.cn

[F02] 逐行读取文件
来源：http://va.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rc.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cq.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zq.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fz.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bw.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qu.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pa.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://af.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ha.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mv.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://em.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vd.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dt.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vi.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hw.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://aj.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mv.gzmigu.cn

[F04] 追加写入文件
来源：http://ig.huanxung.cn


<!-- 参考信息 -->