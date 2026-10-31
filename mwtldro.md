代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://si.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://de.colortex.cn

TS:   Math.max(...arr);
来源：http://mk.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ta.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ab.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://jr.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://ua.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://uc.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ee.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://pg.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mt.shxzskj.cn

TS:   nested.flat();
来源：http://xc.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bk.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://hi.huanxung.cn

Ruby: nested.flatten
来源：http://jd.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yq.bjjhwx.cn

[D19] 按字段分组
来源：http://se.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ds.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ug.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lx.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jn.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fs.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://wy.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fi.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ni.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://uw.hnjuh.cn

Py:   Counter(arr)
来源：http://lv.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://fv.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yq.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hu.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nn.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://hd.huixinmuqiang.cn

Ruby: arr.tally
来源：http://pb.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://le.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://nx.szxytkj.cn

Py:   x in arr
来源：http://bg.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://ig.shxzukj.cn

JS:   arr.includes(x)
来源：http://ei.521024.cn

TS:   arr.includes(x)
来源：http://az.asd995.cn

Java: list.contains(x)
来源：http://tq.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://xw.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://pq.nszjky.cn

C#:   list.Contains(x)
来源：http://sc.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://os.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wv.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pm.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sy.wgjwhj.cn

TS:   [...arr];
来源：http://hs.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://gu.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zr.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://uo.yuexingan06.cn

C#:   new List<int>(list);
来源：http://ey.521024.cn

[D23] reduce 累积计算
来源：http://qp.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vo.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hp.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cq.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wv.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gv.nicolike.cn

Go:   // 手写循环
来源：http://na.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yo.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hy.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://iz.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zj.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kr.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://md.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nx.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yw.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jj.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yn.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ix.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://kj.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dv.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kb.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ee.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jk.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ly.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://by.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ma.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xv.szsharing.cn

[D26] 数组转字符串
来源：http://yn.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://dm.colortex.cn

PHP:  implode(", ", $arr);
来源：http://fj.wgjwhj.cn

JS:   arr.join(", ")
来源：http://sc.huanxung.cn

TS:   arr.join(", ")
来源：http://sq.hnjuh.cn

Java: String.join(", ", list)
来源：http://cp.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://gm.hahajie.cn

Ruby: arr.join(", ")
来源：http://ns.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://oy.wgjwhj.cn

================================================================================
来源：http://nc.szsharing.cn

E. 字符串处理
来源：http://vf.colortex.cn

================================================================================
来源：http://xe.jctech888.com.cn

[E01] 拼接字符串
来源：http://pu.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mx.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xg.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gz.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pt.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aj.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vd.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tb.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hn.hahajie.cn

[E02] 重复字符串
来源：http://se.yuexingan06.cn

Py:   "ab" * 3
来源：http://wp.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://pi.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://pt.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://he.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://hg.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://gq.521024.cn

Ruby: "ab" * 3
来源：http://zg.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sp.colortex.cn

[E03] 截取子串
来源：http://wl.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ff.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kq.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ew.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://nl.9csxet.cn

Java: s.substring(1, 4)
来源：http://lk.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sz.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kf.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://mw.lnxyls.cn

[E04] 查找子串位置
来源：http://np.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://yd.521024.cn

PHP:  strpos($s, "x");
来源：http://aa.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ef.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://aa.9csxet.cn

Java: s.indexOf("x")
来源：http://fv.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://lj.shtwfgs.cn

Ruby: s.index("x")
来源：http://rz.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ws.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sn.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ys.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yc.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bi.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wh.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fi.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zn.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ad.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cw.shxzskj.cn

[E06] 替换子串
来源：http://gu.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pt.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://af.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iq.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://mk.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pm.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wy.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yo.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://js.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://wm.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eg.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bm.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ji.gzmigu.cn

TS:   s.split(",")
来源：http://ep.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eu.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yb.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://yv.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dw.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://ra.shxzskj.cn

Py:   ",".join(items)
来源：http://xq.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://fn.gzmigu.cn

JS:   items.join(",")
来源：http://aq.521024.cn

TS:   items.join(",")
来源：http://wx.9csxet.cn

Java: String.join(",", items)
来源：http://tk.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://sz.9csxet.cn

Ruby: items.join(",")
来源：http://rg.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://fk.nicolike.cn

[E09] 去除所有空白字符
来源：http://ov.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ac.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sc.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://ti.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://dv.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://uv.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vn.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rh.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zp.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://ch.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bj.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dt.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://pc.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://dj.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://wl.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://am.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ik.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dg.bjjhwx.cn

[E11] 反转字符串
来源：http://jz.lnxyls.cn

Py:   s[::-1]
来源：http://zg.lnxyls.cn

PHP:  strrev($s);
来源：http://ju.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://th.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://qv.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tc.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fo.lnxyls.cn

Ruby: s.reverse
来源：http://ap.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bl.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://mw.yuexingan06.cn

Py:   s.count("a")
来源：http://ld.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://bi.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://hn.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://lt.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ph.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://hg.bjjhwx.cn

Ruby: s.count("a")
来源：http://ls.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://vw.hahajie.cn

[E13] 逐字符遍历
来源：http://jr.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://hs.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wh.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://et.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wj.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bp.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ti.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lm.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lw.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://kl.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ex.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tf.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nk.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wk.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ww.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oy.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nh.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aj.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://gt.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zj.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ie.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cp.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xd.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ua.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ar.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nl.szsharing.cn

[E16] 数字千分位
来源：http://ug.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://jb.hahajie.cn

PHP:  number_format(1234567);
来源：http://gk.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hr.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gj.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gj.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ue.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nz.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://av.huixinmuqiang.cn

[E17] 首字母大写
来源：http://za.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zd.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ns.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jc.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xv.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ea.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bg.9csxet.cn

Ruby: s.capitalize
来源：http://zf.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eq.nicolike.cn

[E18] 模板占位符替换
来源：http://zn.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xf.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jw.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xw.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://so.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xp.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tv.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://th.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ug.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://jp.huixiangedu.cn

Py:   s.splitlines()
来源：http://pa.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dn.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://az.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://ro.bookmarksfly.cn

Java: s.lines().toList()
来源：http://xh.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://jd.yuntaijiaju.cn

Ruby: s.lines
来源：http://wx.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://hr.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://jp.nicolike.cn

Py:   if not s:
来源：http://mc.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ui.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fy.lnxyls.cn

TS:   if (s === "") {}
来源：http://wc.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://bu.lnxyls.cn

Go:   if s == "" {}
来源：http://ts.huixiangedu.cn

Ruby: if s.empty?
来源：http://le.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qi.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://nr.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fq.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ob.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://el.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ze.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zp.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ey.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://on.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vn.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://qa.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eu.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mn.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pn.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xn.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://om.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jb.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://qd.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gg.yuexingan06.cn

================================================================================
来源：http://qm.bookmarksfly.cn

F. 文件与目录
来源：http://xt.bookmarksfly.cn

================================================================================
来源：http://yr.szxytkj.cn

[F01] 读取整个文件
来源：http://kp.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://vv.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iy.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ns.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://js.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sz.9csxet.cn

Ruby: File.read("a.txt")
来源：http://ce.bjjhwx.cn


<!-- 参考信息 -->