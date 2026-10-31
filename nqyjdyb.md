代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ae.shxzukj.cn

Go:   // 手写双层循环
来源：http://ou.asd995.cn

Ruby: nested.flatten
来源：http://yv.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dv.yuexingan06.cn

[D19] 按字段分组
来源：http://ui.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fg.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zp.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ut.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lh.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rm.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://pw.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rl.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qi.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://bl.shtwfgs.cn

Py:   Counter(arr)
来源：http://yi.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://fl.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tj.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tv.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://jb.lnxyls.cn

Ruby: arr.tally
来源：http://ar.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cu.huanxung.cn

[D21] 判断是否包含某元素
来源：http://qn.nicolike.cn

Py:   x in arr
来源：http://yc.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://qz.hnjuh.cn

JS:   arr.includes(x)
来源：http://ft.bjjhwx.cn

TS:   arr.includes(x)
来源：http://hp.gzmigu.cn

Java: list.contains(x)
来源：http://bk.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://bx.9csxet.cn

Ruby: arr.include?(x)
来源：http://od.nicolike.cn

C#:   list.Contains(x)
来源：http://ig.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://cm.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sr.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vn.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bg.huanxung.cn

TS:   [...arr];
来源：http://se.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://rh.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gm.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://in.muxihuayi.cn

C#:   new List<int>(list);
来源：http://vy.huixiangedu.cn

[D23] reduce 累积计算
来源：http://ly.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gq.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gm.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vi.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zb.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ug.9csxet.cn

Go:   // 手写循环
来源：http://hy.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fk.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kz.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://tv.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yf.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qd.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pc.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://td.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://il.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ld.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vo.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rl.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://ns.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lt.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ws.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ey.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yt.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ch.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zp.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ro.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nt.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://nj.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://uh.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://ee.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ff.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://xg.521024.cn

Java: String.join(", ", list)
来源：http://mp.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://lr.lnxyls.cn

Ruby: arr.join(", ")
来源：http://sg.huanxung.cn

C#:   string.Join(", ", list)
来源：http://yo.panjiajie.cn

================================================================================
来源：http://qi.yuntaijiaju.cn

E. 字符串处理
来源：http://ay.wgjwhj.cn

================================================================================
来源：http://wx.shtwfgs.cn

[E01] 拼接字符串
来源：http://fw.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qm.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gv.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ps.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://es.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qz.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dc.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://em.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ws.9csxet.cn

[E02] 重复字符串
来源：http://dz.chemitech.net.cn

Py:   "ab" * 3
来源：http://eg.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://qp.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://av.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://qx.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://pe.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://ct.shtwfgs.cn

Ruby: "ab" * 3
来源：http://hg.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dr.lnxyls.cn

[E03] 截取子串
来源：http://ch.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://np.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dg.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gd.asd995.cn

TS:   s.slice(1, 4)
来源：http://cg.newstarts.cn

Java: s.substring(1, 4)
来源：http://cu.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yf.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ui.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://zi.wgjwhj.cn

[E04] 查找子串位置
来源：http://tp.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://fe.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://bm.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.huanxung.cn

TS:   s.indexOf("x")
来源：http://wt.nszjky.cn

Java: s.indexOf("x")
来源：http://eh.colortex.cn

Go:   strings.Index(s, "x")
来源：http://vv.shxzukj.cn

Ruby: s.index("x")
来源：http://eo.hahajie.cn

C#:   s.IndexOf("x")
来源：http://iu.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nh.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wu.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ru.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ny.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xk.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bc.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://od.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ug.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nm.colortex.cn

[E06] 替换子串
来源：http://ff.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mw.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://rv.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://os.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://zg.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gy.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jx.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gz.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://xg.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ne.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lw.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://na.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lv.szsharing.cn

TS:   s.split(",")
来源：http://wt.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dg.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cd.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://yh.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://me.newstarts.cn

[E08] 数组按分隔符合并
来源：http://wv.hahajie.cn

Py:   ",".join(items)
来源：http://ba.huanxung.cn

PHP:  implode(",", $items);
来源：http://rb.szxytkj.cn

JS:   items.join(",")
来源：http://pr.shxzskj.cn

TS:   items.join(",")
来源：http://je.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ko.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://jm.shtwfgs.cn

Ruby: items.join(",")
来源：http://qk.shxzukj.cn

C#:   string.Join(",", items)
来源：http://of.huanxung.cn

[E09] 去除所有空白字符
来源：http://fd.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qt.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mu.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://tx.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://rf.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://gm.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cc.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://js.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jh.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ug.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uz.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ip.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://rz.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://gc.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://mg.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ro.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ut.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ma.jctech888.com.cn

[E11] 反转字符串
来源：http://dk.yuntaijiaju.cn

Py:   s[::-1]
来源：http://rf.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://ws.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://ve.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://gl.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fm.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mm.colortex.cn

Ruby: s.reverse
来源：http://kx.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fs.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://le.bjjhwx.cn

Py:   s.count("a")
来源：http://dl.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://pt.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://qa.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://iz.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yt.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://gy.shxzukj.cn

Ruby: s.count("a")
来源：http://yj.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://bk.yuexingan06.cn

[E13] 逐字符遍历
来源：http://nf.521024.cn

Py:   for ch in s: print(ch)
来源：http://es.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://he.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sv.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qu.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ec.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jm.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wf.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zz.nszjky.cn

[E14] URL 编码与 Base64
来源：http://lf.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ed.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gf.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qj.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sx.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dz.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fi.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wl.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nq.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://bm.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ta.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vv.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fv.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cz.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zs.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sd.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tf.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ji.szsharing.cn

[E16] 数字千分位
来源：http://mx.nszjky.cn

Py:   f"{1234567:,}"
来源：http://kp.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ph.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pn.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zc.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tk.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qq.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kh.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://mv.muxihuayi.cn

[E17] 首字母大写
来源：http://wv.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jn.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pe.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mr.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qd.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://td.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xz.bookmarksfly.cn

Ruby: s.capitalize
来源：http://kc.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ho.colortex.cn

[E18] 模板占位符替换
来源：http://yq.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wf.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://it.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ou.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zf.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mm.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tw.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gw.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vt.newstarts.cn

[E19] 多行文本按行拆分
来源：http://iq.muxihuayi.cn

Py:   s.splitlines()
来源：http://zg.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bz.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://yc.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://la.yuexingan06.cn

Java: s.lines().toList()
来源：http://wg.521024.cn

Go:   strings.Split(s, "\n")
来源：http://oq.hahajie.cn

Ruby: s.lines
来源：http://ia.colortex.cn

C#:   s.Split('\n')
来源：http://re.hahajie.cn

[E20] 判断字符串是否为空
来源：http://on.szxytkj.cn

Py:   if not s:
来源：http://pq.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mn.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gl.nicolike.cn

TS:   if (s === "") {}
来源：http://ny.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://lz.nicolike.cn

Go:   if s == "" {}
来源：http://va.szxytkj.cn

Ruby: if s.empty?
来源：http://iv.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ge.hnjuh.cn

[E21] 超长截断加省略号
来源：http://gz.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zv.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dh.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ob.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gu.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mp.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://pn.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ui.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yq.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://di.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iv.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://km.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://co.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dk.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cg.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://td.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ai.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xf.szsharing.cn

================================================================================
来源：http://sr.panjiajie.cn

F. 文件与目录
来源：http://eu.jianghongdianzi.cn

================================================================================
来源：http://pa.lnxyls.cn

[F01] 读取整个文件
来源：http://xe.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ne.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://ac.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aw.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yr.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qj.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hf.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://zq.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://yp.lnxyls.cn

[F02] 逐行读取文件
来源：http://jh.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dz.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jb.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://li.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jq.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xs.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://da.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gb.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jk.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://gy.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xv.yuexingan06.cn


<!-- 参考信息 -->