代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tb.521024.cn

Go:   // 手写双层循环
来源：http://mn.muxihuayi.cn

Ruby: nested.flatten
来源：http://pm.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bk.bjjhwx.cn

[D19] 按字段分组
来源：http://pf.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dl.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hu.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://va.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://by.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wm.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://tz.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ra.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pi.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://hu.hnjuh.cn

Py:   Counter(arr)
来源：http://ww.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://ad.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xg.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jv.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ds.huanxung.cn

Go:   // 手写 map[T]int
来源：http://jn.9csxet.cn

Ruby: arr.tally
来源：http://gs.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tk.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://kw.9csxet.cn

Py:   x in arr
来源：http://eg.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://wg.colortex.cn

JS:   arr.includes(x)
来源：http://wt.521024.cn

TS:   arr.includes(x)
来源：http://fa.newstarts.cn

Java: list.contains(x)
来源：http://xf.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://am.9csxet.cn

Ruby: arr.include?(x)
来源：http://es.shtwfgs.cn

C#:   list.Contains(x)
来源：http://pr.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://uy.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tt.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xh.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://my.shxzskj.cn

TS:   [...arr];
来源：http://og.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://qk.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://na.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://mx.huanxung.cn

C#:   new List<int>(list);
来源：http://yr.hnjuh.cn

[D23] reduce 累积计算
来源：http://ed.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nk.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iy.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iq.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tl.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uz.colortex.cn

Go:   // 手写循环
来源：http://bz.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yy.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tl.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://ie.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ly.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kd.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fz.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ia.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://em.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bj.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vd.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qn.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://bj.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oe.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qy.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://as.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xe.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rw.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ww.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sw.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://en.colortex.cn

[D26] 数组转字符串
来源：http://on.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://me.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://mq.9csxet.cn

JS:   arr.join(", ")
来源：http://hv.shxzukj.cn

TS:   arr.join(", ")
来源：http://jh.wgjwhj.cn

Java: String.join(", ", list)
来源：http://do.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://kz.521024.cn

Ruby: arr.join(", ")
来源：http://sf.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://if.jianghongdianzi.cn

================================================================================
来源：http://xf.wgjwhj.cn

E. 字符串处理
来源：http://nv.haigaiapp.cn

================================================================================
来源：http://se.shxzskj.cn

[E01] 拼接字符串
来源：http://jt.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dz.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rq.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yg.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hi.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vs.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gd.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sv.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tm.hahajie.cn

[E02] 重复字符串
来源：http://fw.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://re.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://cb.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://jv.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://bq.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ei.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://nt.lnxyls.cn

Ruby: "ab" * 3
来源：http://nv.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ie.muxihuayi.cn

[E03] 截取子串
来源：http://de.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://je.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://px.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://to.521024.cn

TS:   s.slice(1, 4)
来源：http://cl.huanxung.cn

Java: s.substring(1, 4)
来源：http://ce.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://no.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yz.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://wp.chemitech.net.cn

[E04] 查找子串位置
来源：http://uk.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://xk.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://kd.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ka.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://dn.nszjky.cn

Java: s.indexOf("x")
来源：http://ik.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://uo.chemitech.net.cn

Ruby: s.index("x")
来源：http://jv.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://mh.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dr.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zc.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://id.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mu.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yg.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ie.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ie.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jx.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gq.panjiajie.cn

[E06] 替换子串
来源：http://xo.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://li.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://qx.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qz.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://mq.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nw.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://km.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zt.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://uv.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://uj.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fw.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yp.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fw.hahajie.cn

TS:   s.split(",")
来源：http://pz.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ay.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qf.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://zr.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://re.nicolike.cn

[E08] 数组按分隔符合并
来源：http://kc.bjjhwx.cn

Py:   ",".join(items)
来源：http://zh.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://ux.9csxet.cn

JS:   items.join(",")
来源：http://gw.panjiajie.cn

TS:   items.join(",")
来源：http://sm.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://tn.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://tz.wgjwhj.cn

Ruby: items.join(",")
来源：http://qr.huanxung.cn

C#:   string.Join(",", items)
来源：http://eh.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://sv.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cb.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gc.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://fp.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://pm.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://gl.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wr.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uu.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://my.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://kz.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gb.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wc.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://bu.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://kl.nicolike.cn

Java: String.format("%03d", 7)
来源：http://az.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ac.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nb.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dv.yuexingan06.cn

[E11] 反转字符串
来源：http://pk.muxihuayi.cn

Py:   s[::-1]
来源：http://uf.9csxet.cn

PHP:  strrev($s);
来源：http://dy.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://cj.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://nw.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tj.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zc.shxzukj.cn

Ruby: s.reverse
来源：http://gg.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ud.huanxung.cn

[E12] 统计某字符出现次数
来源：http://yh.newstarts.cn

Py:   s.count("a")
来源：http://ks.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://wr.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://zm.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://if.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ly.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://if.hahajie.cn

Ruby: s.count("a")
来源：http://nc.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://nw.muxihuayi.cn

[E13] 逐字符遍历
来源：http://yf.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://bt.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ng.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://an.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ky.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ya.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wv.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://at.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ya.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://oy.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wx.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nj.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mg.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yx.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zi.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://md.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vn.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://au.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://pu.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jc.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sw.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zr.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://le.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://je.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dk.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yt.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ra.bjjhwx.cn

[E16] 数字千分位
来源：http://qd.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://qm.colortex.cn

PHP:  number_format(1234567);
来源：http://sh.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nz.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hf.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ep.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pr.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://te.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://tp.colortex.cn

[E17] 首字母大写
来源：http://va.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fq.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kr.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nm.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rl.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ta.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uc.shxzskj.cn

Ruby: s.capitalize
来源：http://lf.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mr.huixiangedu.cn

[E18] 模板占位符替换
来源：http://yx.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://la.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sr.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hh.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hd.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dy.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dc.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lv.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://co.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://my.panjiajie.cn

Py:   s.splitlines()
来源：http://wt.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ji.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://zw.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://fs.hahajie.cn

Java: s.lines().toList()
来源：http://iq.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://xm.szxytkj.cn

Ruby: s.lines
来源：http://gm.chemitech.net.cn

C#:   s.Split('\n')
来源：http://jo.hahajie.cn

[E20] 判断字符串是否为空
来源：http://kb.colortex.cn

Py:   if not s:
来源：http://wu.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xs.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://js.chemitech.net.cn

TS:   if (s === "") {}
来源：http://vj.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://vc.bookmarksfly.cn

Go:   if s == "" {}
来源：http://fx.9csxet.cn

Ruby: if s.empty?
来源：http://sa.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://is.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://pa.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hw.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fi.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hm.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gj.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://if.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://fm.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cl.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oa.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://qx.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ij.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hk.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://js.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://en.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ve.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://dy.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rp.lnxyls.cn

================================================================================
来源：http://bl.hnjuh.cn

F. 文件与目录
来源：http://qp.nicolike.cn

================================================================================
来源：http://mr.newstarts.cn

[F01] 读取整个文件
来源：http://on.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vv.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://dz.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hb.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jm.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bu.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jw.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ua.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://ib.hahajie.cn

[F02] 逐行读取文件
来源：http://pi.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://la.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jy.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dw.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ek.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pf.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sc.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yr.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tt.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://dv.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bc.asd995.cn


<!-- 参考信息 -->