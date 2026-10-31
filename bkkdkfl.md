代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ll.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://sz.wgjwhj.cn

[D17] 最大值与最小值
来源：http://lh.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://rn.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://py.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qg.gzmigu.cn

TS:   Math.max(...arr);
来源：http://tc.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ci.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nj.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://fg.asd995.cn

C#:   list.Max();  list.Min()
来源：http://tk.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://mi.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ey.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ai.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pw.newstarts.cn

TS:   nested.flat();
来源：http://pu.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sc.huixiangedu.cn

Go:   // 手写双层循环
来源：http://fv.shxzukj.cn

Ruby: nested.flatten
来源：http://qv.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uy.9csxet.cn

[D19] 按字段分组
来源：http://eu.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pr.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jp.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sj.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yk.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ur.asd995.cn

Go:   // 手写 map[string][]T
来源：http://fe.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jd.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iz.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://gj.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://zh.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://mi.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rk.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ux.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uw.newstarts.cn

Go:   // 手写 map[T]int
来源：http://rp.yuexingan06.cn

Ruby: arr.tally
来源：http://wz.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sz.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://nh.shtwfgs.cn

Py:   x in arr
来源：http://is.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://uv.shtwfgs.cn

JS:   arr.includes(x)
来源：http://hr.shxzukj.cn

TS:   arr.includes(x)
来源：http://ss.yuntaijiaju.cn

Java: list.contains(x)
来源：http://er.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://dn.nicolike.cn

Ruby: arr.include?(x)
来源：http://hs.shxzukj.cn

C#:   list.Contains(x)
来源：http://xo.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://tx.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iu.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bp.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yc.yuntaijiaju.cn

TS:   [...arr];
来源：http://la.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ea.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vf.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://ei.wgjwhj.cn

C#:   new List<int>(list);
来源：http://bv.shxzukj.cn

[D23] reduce 累积计算
来源：http://fu.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lc.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ud.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kn.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kr.bjjhwx.cn

Go:   // 手写循环
来源：http://lk.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aw.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hv.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://pk.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cz.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ix.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://og.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sn.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rc.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iu.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xx.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gs.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://vx.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://da.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://so.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pi.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lv.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tg.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ki.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ed.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xh.nicolike.cn

[D26] 数组转字符串
来源：http://cn.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://zi.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://ip.bjjhwx.cn

JS:   arr.join(", ")
来源：http://hy.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://lw.nicolike.cn

Java: String.join(", ", list)
来源：http://bf.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://bu.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://sz.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://qc.wgjwhj.cn

================================================================================
来源：http://jw.lnxyls.cn

E. 字符串处理
来源：http://et.haigaiapp.cn

================================================================================
来源：http://db.gzmigu.cn

[E01] 拼接字符串
来源：http://ta.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eh.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fk.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ay.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yd.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eg.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://em.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xv.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kg.panjiajie.cn

[E02] 重复字符串
来源：http://rf.hnjuh.cn

Py:   "ab" * 3
来源：http://bo.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://mn.newstarts.cn

JS:   "ab".repeat(3)
来源：http://kz.asd995.cn

TS:   "ab".repeat(3)
来源：http://gt.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://hy.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://bw.bjjhwx.cn

Ruby: "ab" * 3
来源：http://kq.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lu.nicolike.cn

[E03] 截取子串
来源：http://cg.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://md.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vs.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xv.asd995.cn

TS:   s.slice(1, 4)
来源：http://lz.shxzskj.cn

Java: s.substring(1, 4)
来源：http://we.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gz.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ah.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://rs.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://vq.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://yl.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://yz.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jv.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://pe.hahajie.cn

Java: s.indexOf("x")
来源：http://lv.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://ei.muxihuayi.cn

Ruby: s.index("x")
来源：http://ul.colortex.cn

C#:   s.IndexOf("x")
来源：http://ss.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mj.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hg.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ju.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ab.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://do.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qu.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oq.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ug.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://il.huixinmuqiang.cn

[E06] 替换子串
来源：http://sk.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vl.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://zo.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tf.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://of.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zw.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ld.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mv.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://bw.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://ve.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qx.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cm.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ly.shxzskj.cn

TS:   s.split(",")
来源：http://tw.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zk.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nq.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://pk.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yv.521024.cn

[E08] 数组按分隔符合并
来源：http://sm.jctech888.com.cn

Py:   ",".join(items)
来源：http://mv.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://em.muxihuayi.cn

JS:   items.join(",")
来源：http://wk.huanxung.cn

TS:   items.join(",")
来源：http://kr.asd995.cn

Java: String.join(",", items)
来源：http://uv.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://bx.muxihuayi.cn

Ruby: items.join(",")
来源：http://kj.hnjuh.cn

C#:   string.Join(",", items)
来源：http://hy.lnxyls.cn

[E09] 去除所有空白字符
来源：http://hf.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ix.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fb.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://kb.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://pi.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://hw.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dj.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fb.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://tb.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qh.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://gy.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://yq.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://wy.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kw.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dr.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cc.huixiangedu.cn

[E11] 反转字符串
来源：http://hh.wgjwhj.cn

Py:   s[::-1]
来源：http://uh.colortex.cn

PHP:  strrev($s);
来源：http://hy.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://fl.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://ug.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vl.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ye.asd995.cn

Ruby: s.reverse
来源：http://yy.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://np.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://fs.huixinmuqiang.cn

Py:   s.count("a")
来源：http://yj.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://ls.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://sp.521024.cn

TS:   s.split("a").length - 1
来源：http://gg.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yg.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://mk.wgjwhj.cn

Ruby: s.count("a")
来源：http://li.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://xb.shxzukj.cn

[E13] 逐字符遍历
来源：http://xx.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://wn.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bw.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xg.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yz.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://az.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ev.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cf.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mm.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ab.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ic.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pr.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qb.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vd.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gb.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ha.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sh.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mf.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://ft.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://km.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bn.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xa.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lx.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kc.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ui.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sb.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ei.shxzukj.cn

[E16] 数字千分位
来源：http://bs.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://kc.hahajie.cn

PHP:  number_format(1234567);
来源：http://sa.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://db.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tn.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hn.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ad.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://do.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://ap.bjjhwx.cn

[E17] 首字母大写
来源：http://rm.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jn.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qv.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qa.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cs.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pj.hahajie.cn

Ruby: s.capitalize
来源：http://yq.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pi.521024.cn

[E18] 模板占位符替换
来源：http://pe.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://et.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ov.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bx.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lv.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hd.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qn.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vn.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fu.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://ho.shxzskj.cn

Py:   s.splitlines()
来源：http://aq.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xx.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://cz.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ry.nszjky.cn

Java: s.lines().toList()
来源：http://oa.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://jy.huixinmuqiang.cn

Ruby: s.lines
来源：http://jl.newstarts.cn

C#:   s.Split('\n')
来源：http://te.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://xu.szsharing.cn

Py:   if not s:
来源：http://mg.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hq.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wj.yuexingan06.cn

TS:   if (s === "") {}
来源：http://qo.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://tp.shxzukj.cn

Go:   if s == "" {}
来源：http://mg.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://pn.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xd.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://jv.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ll.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dx.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://us.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ag.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zb.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ks.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yg.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zw.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://gw.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rm.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zz.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cn.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://id.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ly.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bg.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://dq.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qr.nicolike.cn

================================================================================
来源：http://es.hnjuh.cn

F. 文件与目录
来源：http://il.yuexingan06.cn

================================================================================
来源：http://ra.colortex.cn

[F01] 读取整个文件
来源：http://hl.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wi.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://lo.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nd.hahajie.cn


<!-- 参考信息 -->