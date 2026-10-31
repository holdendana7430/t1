代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://wd.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kx.colortex.cn

TS:   Math.max(...arr);
来源：http://nh.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yg.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wj.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://mf.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://lx.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://kc.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xo.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://yt.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mc.wgjwhj.cn

TS:   nested.flat();
来源：http://ce.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://js.shtwfgs.cn

Go:   // 手写双层循环
来源：http://hi.521024.cn

Ruby: nested.flatten
来源：http://hu.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pj.haigaiapp.cn

[D19] 按字段分组
来源：http://rl.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jp.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ny.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ht.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bt.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dp.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://uu.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gc.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uz.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://xq.szxytkj.cn

Py:   Counter(arr)
来源：http://fq.newstarts.cn

PHP:  array_count_values($arr);
来源：http://dl.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://un.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nw.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cn.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://rf.shxzskj.cn

Ruby: arr.tally
来源：http://vg.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wo.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://np.asd995.cn

Py:   x in arr
来源：http://ei.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ie.nszjky.cn

JS:   arr.includes(x)
来源：http://uc.huixiangedu.cn

TS:   arr.includes(x)
来源：http://kg.shxzskj.cn

Java: list.contains(x)
来源：http://yg.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://jq.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://aa.shtwfgs.cn

C#:   list.Contains(x)
来源：http://hj.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://tp.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xp.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ld.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xg.chemitech.net.cn

TS:   [...arr];
来源：http://zy.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://lh.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ly.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://jr.bjjhwx.cn

C#:   new List<int>(list);
来源：http://xi.nszjky.cn

[D23] reduce 累积计算
来源：http://kd.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kb.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sy.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cv.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ax.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://me.yuexingan06.cn

Go:   // 手写循环
来源：http://yr.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nr.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ol.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ca.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gn.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aq.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ns.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vf.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yy.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aj.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vw.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qt.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://yo.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rh.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gl.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vb.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sm.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jh.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://we.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kr.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kq.szsharing.cn

[D26] 数组转字符串
来源：http://qe.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://my.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://es.bjjhwx.cn

JS:   arr.join(", ")
来源：http://bx.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://gw.hahajie.cn

Java: String.join(", ", list)
来源：http://xw.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://de.521024.cn

Ruby: arr.join(", ")
来源：http://un.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ad.wgjwhj.cn

================================================================================
来源：http://yr.gzmigu.cn

E. 字符串处理
来源：http://ci.haigaiapp.cn

================================================================================
来源：http://vw.muxihuayi.cn

[E01] 拼接字符串
来源：http://oq.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://on.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fi.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ls.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ko.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hp.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yw.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gz.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ts.wgjwhj.cn

[E02] 重复字符串
来源：http://as.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://rx.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://nk.newstarts.cn

JS:   "ab".repeat(3)
来源：http://io.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://xa.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://bd.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://dv.shxzukj.cn

Ruby: "ab" * 3
来源：http://ai.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://go.haigaiapp.cn

[E03] 截取子串
来源：http://hc.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kb.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://js.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cd.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://nd.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://oe.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mt.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xo.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://wm.shtwfgs.cn

[E04] 查找子串位置
来源：http://ws.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://zi.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://zj.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sx.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://fb.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://nv.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://ux.panjiajie.cn

Ruby: s.index("x")
来源：http://wh.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://dy.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jo.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ug.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nr.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fq.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jb.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yb.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://js.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pe.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ff.wgjwhj.cn

[E06] 替换子串
来源：http://mf.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jo.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://em.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fn.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://lv.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ot.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bj.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ej.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ml.huanxung.cn

[E07] 按分隔符拆分
来源：http://ey.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nb.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tl.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ux.nszjky.cn

TS:   s.split(",")
来源：http://un.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xp.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xh.asd995.cn

Ruby: s.split(",");  s.split
来源：http://tl.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rs.521024.cn

[E08] 数组按分隔符合并
来源：http://wt.shtwfgs.cn

Py:   ",".join(items)
来源：http://ec.shxzukj.cn

PHP:  implode(",", $items);
来源：http://xq.gzmigu.cn

JS:   items.join(",")
来源：http://st.nszjky.cn

TS:   items.join(",")
来源：http://bk.colortex.cn

Java: String.join(",", items)
来源：http://zn.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://cn.huixiangedu.cn

Ruby: items.join(",")
来源：http://tx.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://bd.9csxet.cn

[E09] 去除所有空白字符
来源：http://ia.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yr.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://br.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://bo.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://zd.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://gz.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bi.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dm.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://al.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://re.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yl.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sm.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://hk.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://hu.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://tn.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ky.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tj.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mk.szsharing.cn

[E11] 反转字符串
来源：http://jj.wgjwhj.cn

Py:   s[::-1]
来源：http://cj.huanxung.cn

PHP:  strrev($s);
来源：http://mt.colortex.cn

JS:   [...s].reverse().join("")
来源：http://bk.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://zp.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ru.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://if.shxzukj.cn

Ruby: s.reverse
来源：http://jg.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hw.szsharing.cn

[E12] 统计某字符出现次数
来源：http://vw.9csxet.cn

Py:   s.count("a")
来源：http://yq.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://pc.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://eu.asd995.cn

TS:   s.split("a").length - 1
来源：http://ti.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wq.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://dm.shxzukj.cn

Ruby: s.count("a")
来源：http://pc.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://dg.nicolike.cn

[E13] 逐字符遍历
来源：http://so.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://tz.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xf.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ti.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eu.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bh.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ib.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rf.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yx.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://kc.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fa.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gr.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ot.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ob.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ds.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ea.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oi.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ju.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://oa.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ow.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nj.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nb.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gk.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oa.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hp.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gi.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sk.asd995.cn

[E16] 数字千分位
来源：http://yc.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://zf.nszjky.cn

PHP:  number_format(1234567);
来源：http://ez.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ow.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bf.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ku.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dq.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ha.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://de.jctech888.com.cn

[E17] 首字母大写
来源：http://sv.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pf.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vg.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fr.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cc.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://en.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kj.hnjuh.cn

Ruby: s.capitalize
来源：http://ra.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sj.szsharing.cn

[E18] 模板占位符替换
来源：http://fa.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fe.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://az.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qu.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xs.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rl.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cu.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pj.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xs.asd995.cn

[E19] 多行文本按行拆分
来源：http://yv.szxytkj.cn

Py:   s.splitlines()
来源：http://zr.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ks.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://vl.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://ga.chemitech.net.cn

Java: s.lines().toList()
来源：http://zi.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://yc.hnjuh.cn

Ruby: s.lines
来源：http://zq.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://gl.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://dj.shtwfgs.cn

Py:   if not s:
来源：http://ym.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rx.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qn.nicolike.cn

TS:   if (s === "") {}
来源：http://kx.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://rs.bjjhwx.cn

Go:   if s == "" {}
来源：http://py.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://ry.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yw.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://et.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ny.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hm.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sy.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vw.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hd.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://oo.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fh.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://im.colortex.cn

[E22] 字节长度与字符长度
来源：http://ch.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iz.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://el.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ll.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jp.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hs.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://rz.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tu.hahajie.cn

================================================================================
来源：http://hg.panjiajie.cn

F. 文件与目录
来源：http://ny.shxzukj.cn

================================================================================
来源：http://sa.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://ia.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://in.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://qb.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://za.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://za.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nu.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fc.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ku.bookmarksfly.cn


<!-- 参考信息 -->