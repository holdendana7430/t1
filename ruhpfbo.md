代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hu.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gk.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://te.nicolike.cn

Go:   // 手写循环累加
来源：http://jp.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ub.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://uz.szxytkj.cn

[D17] 最大值与最小值
来源：http://gb.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://xd.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://ze.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tb.colortex.cn

TS:   Math.max(...arr);
来源：http://hw.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ns.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rd.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ls.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://gz.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://xl.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ku.colortex.cn

PHP:  array_merge(...$nested);
来源：http://tx.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rk.nszjky.cn

TS:   nested.flat();
来源：http://ft.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bl.shtwfgs.cn

Go:   // 手写双层循环
来源：http://go.huixiangedu.cn

Ruby: nested.flatten
来源：http://kh.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jb.huanxung.cn

[D19] 按字段分组
来源：http://bz.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dx.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qo.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eg.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cl.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vz.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://su.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pz.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vc.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://eq.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://fa.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://hg.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ke.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qz.521024.cn

Go:   // 手写 map[T]int
来源：http://vc.colortex.cn

Ruby: arr.tally
来源：http://fo.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zx.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://bc.shtwfgs.cn

Py:   x in arr
来源：http://qp.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://xu.shtwfgs.cn

JS:   arr.includes(x)
来源：http://yc.yuexingan06.cn

TS:   arr.includes(x)
来源：http://va.chemitech.net.cn

Java: list.contains(x)
来源：http://ct.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://fu.panjiajie.cn

Ruby: arr.include?(x)
来源：http://bk.chemitech.net.cn

C#:   list.Contains(x)
来源：http://ed.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://vm.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://se.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xb.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://so.shtwfgs.cn

TS:   [...arr];
来源：http://tf.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://gj.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mj.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://fc.hahajie.cn

C#:   new List<int>(list);
来源：http://pp.szxytkj.cn

[D23] reduce 累积计算
来源：http://kq.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ln.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gb.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jj.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ct.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kh.szxytkj.cn

Go:   // 手写循环
来源：http://hg.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://de.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xw.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://wf.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://br.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ut.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pu.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wc.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ym.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gb.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vm.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://te.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://lk.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eo.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://si.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ho.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lc.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vd.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sl.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hl.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rl.hahajie.cn

[D26] 数组转字符串
来源：http://gv.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://tm.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://ua.hnjuh.cn

JS:   arr.join(", ")
来源：http://ob.chemitech.net.cn

TS:   arr.join(", ")
来源：http://js.yuexingan06.cn

Java: String.join(", ", list)
来源：http://ov.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://hm.nicolike.cn

Ruby: arr.join(", ")
来源：http://al.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://tx.hnjuh.cn

================================================================================
来源：http://df.jianghongdianzi.cn

E. 字符串处理
来源：http://kk.shxzskj.cn

================================================================================
来源：http://gm.haigaiapp.cn

[E01] 拼接字符串
来源：http://lh.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dz.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mu.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lb.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jd.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jq.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eb.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://or.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wl.nicolike.cn

[E02] 重复字符串
来源：http://mc.haigaiapp.cn

Py:   "ab" * 3
来源：http://nm.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://ui.9csxet.cn

JS:   "ab".repeat(3)
来源：http://dm.hahajie.cn

TS:   "ab".repeat(3)
来源：http://he.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://dn.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://et.shxzskj.cn

Ruby: "ab" * 3
来源：http://dk.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zd.shxzskj.cn

[E03] 截取子串
来源：http://hw.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ff.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fx.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ik.huanxung.cn

Java: s.substring(1, 4)
来源：http://nv.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vo.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pn.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://jp.szsharing.cn

[E04] 查找子串位置
来源：http://eu.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://mk.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://jp.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ex.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ri.bjjhwx.cn

Java: s.indexOf("x")
来源：http://vd.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://uz.huixiangedu.cn

Ruby: s.index("x")
来源：http://fl.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://yo.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://su.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://it.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sp.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qu.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hp.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pw.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zt.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dq.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nk.yuexingan06.cn

[E06] 替换子串
来源：http://xh.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fy.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://pp.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ao.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://wt.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gr.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://es.asd995.cn

C#:   s.Replace("a", "b")
来源：http://lg.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://nb.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dj.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jd.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fi.szxytkj.cn

TS:   s.split(",")
来源：http://us.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pa.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vu.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://yh.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dr.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://au.huanxung.cn

Py:   ",".join(items)
来源：http://ep.9csxet.cn

PHP:  implode(",", $items);
来源：http://ur.hnjuh.cn

JS:   items.join(",")
来源：http://bz.nicolike.cn

TS:   items.join(",")
来源：http://af.newstarts.cn

Java: String.join(",", items)
来源：http://tl.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://xh.9csxet.cn

Ruby: items.join(",")
来源：http://qe.szxytkj.cn

C#:   string.Join(",", items)
来源：http://oh.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://rp.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://so.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kk.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://vz.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://fj.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://hg.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://is.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://li.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ci.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://gp.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sq.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://te.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ci.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://fn.hahajie.cn

Java: String.format("%03d", 7)
来源：http://ja.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hx.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sq.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lm.hahajie.cn

[E11] 反转字符串
来源：http://fv.shxzskj.cn

Py:   s[::-1]
来源：http://fi.lnxyls.cn

PHP:  strrev($s);
来源：http://rq.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://pa.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://vp.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kk.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ay.yuexingan06.cn

Ruby: s.reverse
来源：http://pa.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xa.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://ji.huixinmuqiang.cn

Py:   s.count("a")
来源：http://kd.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://eh.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://es.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://da.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xz.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://uw.asd995.cn

Ruby: s.count("a")
来源：http://hw.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://qo.newstarts.cn

[E13] 逐字符遍历
来源：http://sp.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://jn.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://da.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ed.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ah.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ac.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xa.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xc.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zh.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://dd.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wj.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ac.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mv.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fr.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dx.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rn.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tj.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hs.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://tg.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oq.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fr.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://af.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wl.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vt.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xr.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iw.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ad.shtwfgs.cn

[E16] 数字千分位
来源：http://ah.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://zo.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://ay.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cf.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kj.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fz.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kp.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ht.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://qy.haigaiapp.cn

[E17] 首字母大写
来源：http://ya.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jn.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sf.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wt.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yq.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qq.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fn.shtwfgs.cn

Ruby: s.capitalize
来源：http://du.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ay.521024.cn

[E18] 模板占位符替换
来源：http://cu.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rx.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mz.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ns.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dw.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vu.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ro.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xi.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fi.521024.cn

[E19] 多行文本按行拆分
来源：http://up.gzmigu.cn

Py:   s.splitlines()
来源：http://jn.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rd.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://rr.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ze.gzmigu.cn

Java: s.lines().toList()
来源：http://mq.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://mc.hnjuh.cn

Ruby: s.lines
来源：http://ep.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ji.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://kt.panjiajie.cn

Py:   if not s:
来源：http://pd.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://al.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sj.newstarts.cn

TS:   if (s === "") {}
来源：http://sn.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://zr.lnxyls.cn

Go:   if s == "" {}
来源：http://hx.shtwfgs.cn

Ruby: if s.empty?
来源：http://sc.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://qg.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://os.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aa.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ch.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bp.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ad.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://bw.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rj.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://so.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://ji.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rj.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ru.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jr.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lj.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://un.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xm.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://bp.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jd.gzmigu.cn

================================================================================
来源：http://xn.haigaiapp.cn

F. 文件与目录
来源：http://uk.wgjwhj.cn

================================================================================
来源：http://nh.szsharing.cn


<!-- 参考信息 -->