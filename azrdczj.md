代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yc.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fn.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://co.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://hf.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qe.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://gd.muxihuayi.cn

[D17] 最大值与最小值
来源：http://ae.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://pi.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://bv.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pf.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ls.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yf.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fp.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://sz.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://bg.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://yi.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lm.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://qa.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ce.hahajie.cn

TS:   nested.flat();
来源：http://li.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jy.9csxet.cn

Go:   // 手写双层循环
来源：http://vb.colortex.cn

Ruby: nested.flatten
来源：http://wc.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pp.hahajie.cn

[D19] 按字段分组
来源：http://ap.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://na.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xq.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kd.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zg.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vl.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://qg.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://as.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bs.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://pm.shtwfgs.cn

Py:   Counter(arr)
来源：http://vm.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://lg.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ic.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ee.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oi.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ne.newstarts.cn

Ruby: arr.tally
来源：http://ny.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dz.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://zh.wgjwhj.cn

Py:   x in arr
来源：http://vj.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://aw.szxytkj.cn

JS:   arr.includes(x)
来源：http://oq.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://ml.521024.cn

Java: list.contains(x)
来源：http://un.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://jl.nszjky.cn

Ruby: arr.include?(x)
来源：http://jr.521024.cn

C#:   list.Contains(x)
来源：http://rz.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://mz.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fx.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://if.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hf.nszjky.cn

TS:   [...arr];
来源：http://ar.huanxung.cn

Java: new ArrayList<>(list);
来源：http://nh.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ph.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://de.bjjhwx.cn

C#:   new List<int>(list);
来源：http://nb.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://zd.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jf.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yu.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qy.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kl.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jc.szsharing.cn

Go:   // 手写循环
来源：http://ax.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qr.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fx.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://pu.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wb.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eq.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ix.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ec.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://at.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ts.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://md.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ff.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ij.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ff.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ve.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://az.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gh.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gq.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fu.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bf.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vz.szxytkj.cn

[D26] 数组转字符串
来源：http://vx.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://yz.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://tb.bjjhwx.cn

JS:   arr.join(", ")
来源：http://tx.huixiangedu.cn

TS:   arr.join(", ")
来源：http://hi.colortex.cn

Java: String.join(", ", list)
来源：http://tx.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://fu.521024.cn

Ruby: arr.join(", ")
来源：http://oc.9csxet.cn

C#:   string.Join(", ", list)
来源：http://sr.bjjhwx.cn

================================================================================
来源：http://zx.yuntaijiaju.cn

E. 字符串处理
来源：http://xb.shxzskj.cn

================================================================================
来源：http://uk.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://zs.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ww.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zg.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sn.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yh.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yd.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pn.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hg.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ig.9csxet.cn

[E02] 重复字符串
来源：http://ve.chemitech.net.cn

Py:   "ab" * 3
来源：http://fm.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ou.szsharing.cn

JS:   "ab".repeat(3)
来源：http://rm.colortex.cn

TS:   "ab".repeat(3)
来源：http://eh.asd995.cn

Java: "ab".repeat(3)
来源：http://nt.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://jy.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ig.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://co.chemitech.net.cn

[E03] 截取子串
来源：http://nn.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wd.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cj.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://we.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://dq.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://yl.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dd.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qh.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://fv.9csxet.cn

[E04] 查找子串位置
来源：http://ht.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ry.nszjky.cn

PHP:  strpos($s, "x");
来源：http://aa.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://np.521024.cn

TS:   s.indexOf("x")
来源：http://wk.panjiajie.cn

Java: s.indexOf("x")
来源：http://mo.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://nk.yuexingan06.cn

Ruby: s.index("x")
来源：http://td.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://nx.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qc.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pk.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://do.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yr.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iv.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xf.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rh.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ff.lnxyls.cn

[E06] 替换子串
来源：http://ue.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vs.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://ci.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ra.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://on.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hd.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ym.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fi.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://wp.hahajie.cn

[E07] 按分隔符拆分
来源：http://cq.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hf.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sw.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://it.shxzukj.cn

TS:   s.split(",")
来源：http://oj.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fg.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wb.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://gl.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yj.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://lo.asd995.cn

Py:   ",".join(items)
来源：http://pj.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://js.muxihuayi.cn

JS:   items.join(",")
来源：http://ke.chemitech.net.cn

TS:   items.join(",")
来源：http://mg.gzmigu.cn

Java: String.join(",", items)
来源：http://xp.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://sp.shxzskj.cn

Ruby: items.join(",")
来源：http://rb.colortex.cn

C#:   string.Join(",", items)
来源：http://sv.huanxung.cn

[E09] 去除所有空白字符
来源：http://jo.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://su.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ez.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://zr.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wf.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://pz.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xd.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ti.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bn.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://pz.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oi.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jj.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://vq.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://af.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ye.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xx.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://df.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mi.shxzskj.cn

[E11] 反转字符串
来源：http://hc.hahajie.cn

Py:   s[::-1]
来源：http://rc.shtwfgs.cn

PHP:  strrev($s);
来源：http://ri.asd995.cn

JS:   [...s].reverse().join("")
来源：http://lw.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://uw.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yy.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fs.colortex.cn

Ruby: s.reverse
来源：http://fi.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://to.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://xg.wgjwhj.cn

Py:   s.count("a")
来源：http://ch.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://xm.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://nd.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://tx.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rq.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://mz.hahajie.cn

Ruby: s.count("a")
来源：http://ks.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://wr.9csxet.cn

[E13] 逐字符遍历
来源：http://nz.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://fb.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xt.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://po.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uh.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oe.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nf.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bb.huanxung.cn

[E14] URL 编码与 Base64
来源：http://id.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oz.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tk.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mw.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gw.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lk.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qe.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gu.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lm.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://xo.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tm.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eh.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zo.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ts.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ho.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ig.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gx.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ug.colortex.cn

[E16] 数字千分位
来源：http://kp.nszjky.cn

Py:   f"{1234567:,}"
来源：http://di.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://qf.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pk.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ss.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ru.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ld.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nu.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://cz.hnjuh.cn

[E17] 首字母大写
来源：http://dy.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sq.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ke.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uo.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ae.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zj.colortex.cn

Ruby: s.capitalize
来源：http://qf.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ui.jctech888.com.cn

[E18] 模板占位符替换
来源：http://gv.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dd.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oa.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ay.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rk.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wb.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pr.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hr.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bq.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://mg.bjjhwx.cn

Py:   s.splitlines()
来源：http://nm.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rj.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://kw.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://qz.521024.cn

Java: s.lines().toList()
来源：http://or.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://in.colortex.cn

Ruby: s.lines
来源：http://tc.lnxyls.cn

C#:   s.Split('\n')
来源：http://yc.asd995.cn

[E20] 判断字符串是否为空
来源：http://ei.colortex.cn

Py:   if not s:
来源：http://ly.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bh.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hg.521024.cn

TS:   if (s === "") {}
来源：http://vm.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://wu.521024.cn

Go:   if s == "" {}
来源：http://sf.bookmarksfly.cn

Ruby: if s.empty?
来源：http://nf.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ev.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ok.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ck.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xz.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cf.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gv.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jh.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yz.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wv.newstarts.cn

[E22] 字节长度与字符长度
来源：http://zd.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cw.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tn.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tk.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qu.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yh.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uc.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://qx.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dn.huixinmuqiang.cn

================================================================================
来源：http://ej.szsharing.cn

F. 文件与目录
来源：http://ao.nszjky.cn

================================================================================
来源：http://zq.yuexingan06.cn


<!-- 参考信息 -->