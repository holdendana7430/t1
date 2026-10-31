代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://xz.chemitech.net.cn

Go:   // 手写循环
来源：http://jt.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zi.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gg.szsharing.cn

[D15] 去重
来源：http://iz.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tt.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://wj.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://fc.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://me.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xb.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xw.huanxung.cn

Ruby: arr.uniq
来源：http://mk.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://xi.colortex.cn

[D16] 求和与平均值
来源：http://gp.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jm.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ck.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fl.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qh.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qb.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://gn.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jg.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://cj.gzmigu.cn

[D17] 最大值与最小值
来源：http://hy.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://bd.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://wr.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nq.colortex.cn

TS:   Math.max(...arr);
来源：http://vb.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yx.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zq.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://jn.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://qd.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://is.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ra.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://vt.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fd.shxzukj.cn

TS:   nested.flat();
来源：http://nc.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cl.muxihuayi.cn

Go:   // 手写双层循环
来源：http://in.shxzukj.cn

Ruby: nested.flatten
来源：http://ea.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fv.9csxet.cn

[D19] 按字段分组
来源：http://ci.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yo.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jp.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ky.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bp.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lo.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://tj.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lk.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qz.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://jb.bookmarksfly.cn

Py:   Counter(arr)
来源：http://ug.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://oe.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ap.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dp.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jg.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ie.jctech888.com.cn

Ruby: arr.tally
来源：http://ms.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sc.hahajie.cn

[D21] 判断是否包含某元素
来源：http://wv.wgjwhj.cn

Py:   x in arr
来源：http://nt.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://yj.bjjhwx.cn

JS:   arr.includes(x)
来源：http://iw.asd995.cn

TS:   arr.includes(x)
来源：http://px.hahajie.cn

Java: list.contains(x)
来源：http://sx.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://wp.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://ov.gzmigu.cn

C#:   list.Contains(x)
来源：http://dv.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://ov.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fn.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://me.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ug.bookmarksfly.cn

TS:   [...arr];
来源：http://tk.nszjky.cn

Java: new ArrayList<>(list);
来源：http://fd.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://io.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://ne.muxihuayi.cn

C#:   new List<int>(list);
来源：http://vs.panjiajie.cn

[D23] reduce 累积计算
来源：http://ee.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://as.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dn.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yq.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dr.nszjky.cn

Go:   // 手写循环
来源：http://dx.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rg.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cp.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://xy.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pd.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rn.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oh.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rk.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://on.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ru.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hs.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sf.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://qv.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://km.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rx.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://us.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wy.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cx.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fb.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gk.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://um.panjiajie.cn

[D26] 数组转字符串
来源：http://jk.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://oq.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://yu.9csxet.cn

JS:   arr.join(", ")
来源：http://pz.521024.cn

TS:   arr.join(", ")
来源：http://gy.shtwfgs.cn

Java: String.join(", ", list)
来源：http://iw.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://bu.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://nj.colortex.cn

C#:   string.Join(", ", list)
来源：http://ca.asd995.cn

================================================================================
来源：http://lw.chemitech.net.cn

E. 字符串处理
来源：http://qg.szxytkj.cn

================================================================================
来源：http://iz.yuexingan06.cn

[E01] 拼接字符串
来源：http://yg.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vx.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dq.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hx.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qi.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cu.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ke.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wu.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pa.521024.cn

[E02] 重复字符串
来源：http://bm.szxytkj.cn

Py:   "ab" * 3
来源：http://xq.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://uy.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://ko.colortex.cn

TS:   "ab".repeat(3)
来源：http://ox.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://wl.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://pr.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ec.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pk.lnxyls.cn

[E03] 截取子串
来源：http://xw.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ma.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fg.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xl.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://vw.asd995.cn

Java: s.substring(1, 4)
来源：http://um.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fw.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rz.asd995.cn

C#:   s.Substring(1, 3)
来源：http://os.huixiangedu.cn

[E04] 查找子串位置
来源：http://fd.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://eq.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ox.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hl.lnxyls.cn

TS:   s.indexOf("x")
来源：http://br.szsharing.cn

Java: s.indexOf("x")
来源：http://cg.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://ol.bjjhwx.cn

Ruby: s.index("x")
来源：http://id.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ff.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tx.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jm.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yv.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ln.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nl.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mb.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bp.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ow.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mw.chemitech.net.cn

[E06] 替换子串
来源：http://hu.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xi.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://eu.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://da.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://ab.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ah.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qx.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ec.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://yp.nszjky.cn

[E07] 按分隔符拆分
来源：http://mc.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dt.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vf.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qw.shxzukj.cn

TS:   s.split(",")
来源：http://la.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iq.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dj.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://ag.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xb.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://uh.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://hc.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://zb.jctech888.com.cn

JS:   items.join(",")
来源：http://zt.yuexingan06.cn

TS:   items.join(",")
来源：http://ig.muxihuayi.cn

Java: String.join(",", items)
来源：http://cd.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://gv.nszjky.cn

Ruby: items.join(",")
来源：http://bk.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://kj.521024.cn

[E09] 去除所有空白字符
来源：http://aw.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oi.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vz.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://mr.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://xo.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://er.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qu.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tg.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://of.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://av.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qt.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yc.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://kq.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://yo.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://uo.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://je.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fc.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ut.haigaiapp.cn

[E11] 反转字符串
来源：http://yz.shtwfgs.cn

Py:   s[::-1]
来源：http://kc.bookmarksfly.cn

PHP:  strrev($s);
来源：http://aw.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://ut.521024.cn

TS:   [...s].reverse().join("")
来源：http://vl.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kb.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sp.shxzukj.cn

Ruby: s.reverse
来源：http://gc.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gx.nszjky.cn

[E12] 统计某字符出现次数
来源：http://nx.muxihuayi.cn

Py:   s.count("a")
来源：http://fg.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://fc.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://lf.newstarts.cn

TS:   s.split("a").length - 1
来源：http://jr.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jr.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://dn.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://jh.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://yx.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://ol.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://tx.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rx.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ka.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://er.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hu.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wk.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rd.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cj.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://az.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tu.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ff.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yb.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ta.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fl.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ip.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ml.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://or.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://qr.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dx.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jk.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cu.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://er.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rg.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yn.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bw.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uv.nicolike.cn

[E16] 数字千分位
来源：http://pt.nszjky.cn

Py:   f"{1234567:,}"
来源：http://be.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://bp.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://js.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ai.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mz.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cv.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vp.colortex.cn

C#:   1234567.ToString("N0")
来源：http://hr.9csxet.cn

[E17] 首字母大写
来源：http://hq.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jy.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ai.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://na.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eb.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ny.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zy.shxzukj.cn

Ruby: s.capitalize
来源：http://om.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ur.shxzukj.cn

[E18] 模板占位符替换
来源：http://af.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tq.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ie.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qd.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mx.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ov.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kl.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fu.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://au.newstarts.cn

[E19] 多行文本按行拆分
来源：http://fp.jctech888.com.cn

Py:   s.splitlines()
来源：http://hk.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://we.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://ex.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ou.nszjky.cn

Java: s.lines().toList()
来源：http://ea.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://fn.lnxyls.cn

Ruby: s.lines
来源：http://yk.shxzskj.cn

C#:   s.Split('\n')
来源：http://gr.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://wu.bjjhwx.cn

Py:   if not s:
来源：http://xk.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://im.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sl.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://dy.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://ot.wgjwhj.cn

Go:   if s == "" {}
来源：http://py.newstarts.cn

Ruby: if s.empty?
来源：http://uk.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ia.shxzskj.cn

[E21] 超长截断加省略号
来源：http://em.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zl.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wj.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bs.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qz.huanxung.cn


<!-- 参考信息 -->