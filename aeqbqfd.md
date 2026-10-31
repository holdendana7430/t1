代发 wailian999

[D15] 去重
来源：http://it.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mi.colortex.cn

PHP:  array_unique($arr);
来源：http://ly.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://lj.nszjky.cn

TS:   [...new Set(arr)]
来源：http://gi.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xf.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qn.huanxung.cn

Ruby: arr.uniq
来源：http://nd.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://xa.hnjuh.cn

[D16] 求和与平均值
来源：http://lh.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dx.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yk.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ms.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fr.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kk.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://yv.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cv.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://qw.huixiangedu.cn

[D17] 最大值与最小值
来源：http://hn.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://zv.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://gp.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rn.hnjuh.cn

TS:   Math.max(...arr);
来源：http://no.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yh.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://an.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://zw.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://ox.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://lp.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zg.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://pp.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kd.nicolike.cn

TS:   nested.flat();
来源：http://aa.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qv.shtwfgs.cn

Go:   // 手写双层循环
来源：http://ym.shxzukj.cn

Ruby: nested.flatten
来源：http://ih.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yi.hnjuh.cn

[D19] 按字段分组
来源：http://fz.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iu.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pf.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ll.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tp.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wo.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://mp.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://di.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oq.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ey.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://oe.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://xu.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pe.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hw.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sy.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://zi.yuexingan06.cn

Ruby: arr.tally
来源：http://fw.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mw.9csxet.cn

[D21] 判断是否包含某元素
来源：http://rb.bookmarksfly.cn

Py:   x in arr
来源：http://at.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://xk.shxzukj.cn

JS:   arr.includes(x)
来源：http://zw.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://uf.asd995.cn

Java: list.contains(x)
来源：http://sb.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://rp.panjiajie.cn

Ruby: arr.include?(x)
来源：http://cf.haigaiapp.cn

C#:   list.Contains(x)
来源：http://re.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://hv.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tj.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wf.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://id.yuexingan06.cn

TS:   [...arr];
来源：http://af.nicolike.cn

Java: new ArrayList<>(list);
来源：http://aj.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tl.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://re.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ft.gzmigu.cn

[D23] reduce 累积计算
来源：http://wi.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vl.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ch.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yq.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://io.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rs.chemitech.net.cn

Go:   // 手写循环
来源：http://ql.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vh.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mr.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://hi.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://td.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lg.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://as.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lh.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://go.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wj.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vy.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oa.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://be.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xf.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sh.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pr.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qv.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qj.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jz.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ak.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hn.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://df.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://ls.colortex.cn

PHP:  implode(", ", $arr);
来源：http://vb.hnjuh.cn

JS:   arr.join(", ")
来源：http://yu.muxihuayi.cn

TS:   arr.join(", ")
来源：http://aq.panjiajie.cn

Java: String.join(", ", list)
来源：http://lz.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://um.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://zj.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://sh.huixiangedu.cn

================================================================================
来源：http://ru.shtwfgs.cn

E. 字符串处理
来源：http://px.asd995.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://ig.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zz.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://li.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://px.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://he.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ak.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xl.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://en.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nc.lnxyls.cn

[E02] 重复字符串
来源：http://sn.nicolike.cn

Py:   "ab" * 3
来源：http://pi.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ft.huanxung.cn

JS:   "ab".repeat(3)
来源：http://kj.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://wd.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ud.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://zb.jctech888.com.cn

Ruby: "ab" * 3
来源：http://tx.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bh.szsharing.cn

[E03] 截取子串
来源：http://gs.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gw.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zy.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wa.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://mq.szsharing.cn

Java: s.substring(1, 4)
来源：http://tg.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://us.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uu.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ty.hahajie.cn

[E04] 查找子串位置
来源：http://ip.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://jt.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://ba.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wx.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://oq.hahajie.cn

Java: s.indexOf("x")
来源：http://zh.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://vj.shtwfgs.cn

Ruby: s.index("x")
来源：http://sq.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://ue.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zg.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aa.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://or.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wm.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vt.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qv.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ie.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ju.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tq.chemitech.net.cn

[E06] 替换子串
来源：http://xt.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hk.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://sk.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kj.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://it.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dt.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yc.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://ys.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://oj.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eq.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jj.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bj.lnxyls.cn

TS:   s.split(",")
来源：http://pi.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ny.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xx.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://yx.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pi.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://pc.newstarts.cn

Py:   ",".join(items)
来源：http://fs.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://xj.jctech888.com.cn

JS:   items.join(",")
来源：http://xj.wgjwhj.cn

TS:   items.join(",")
来源：http://ee.hahajie.cn

Java: String.join(",", items)
来源：http://zo.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://lo.szxytkj.cn

Ruby: items.join(",")
来源：http://pl.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://nk.gzmigu.cn

[E09] 去除所有空白字符
来源：http://oo.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hr.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ws.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ht.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://zw.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://sn.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gc.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eq.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://er.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://jt.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pr.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bc.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://qw.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://fz.521024.cn

Java: String.format("%03d", 7)
来源：http://mz.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hh.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ct.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qw.hahajie.cn

[E11] 反转字符串
来源：http://pl.colortex.cn

Py:   s[::-1]
来源：http://pv.lnxyls.cn

PHP:  strrev($s);
来源：http://fv.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://gl.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://nj.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lc.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yh.jctech888.com.cn

Ruby: s.reverse
来源：http://ar.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pe.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://is.521024.cn

Py:   s.count("a")
来源：http://xw.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://mi.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://oy.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://gv.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tw.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://cf.shtwfgs.cn

Ruby: s.count("a")
来源：http://bq.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://tm.yuexingan06.cn

[E13] 逐字符遍历
来源：http://al.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://cd.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ui.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jw.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zs.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ou.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fz.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nq.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fq.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://vv.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hp.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wu.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ve.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ri.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zz.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uw.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://un.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wi.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://oi.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kf.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qq.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rk.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://df.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qy.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ss.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bf.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bk.huixinmuqiang.cn

[E16] 数字千分位
来源：http://xq.huanxung.cn

Py:   f"{1234567:,}"
来源：http://zh.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://ow.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lw.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tc.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vm.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jy.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://az.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://er.yuntaijiaju.cn

[E17] 首字母大写
来源：http://kf.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aj.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yp.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mt.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wp.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://go.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yo.szxytkj.cn

Ruby: s.capitalize
来源：http://bd.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pv.lnxyls.cn

[E18] 模板占位符替换
来源：http://kw.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fh.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zj.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pp.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fp.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gk.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ww.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mv.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://za.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://mh.newstarts.cn

Py:   s.splitlines()
来源：http://gi.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pf.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://eh.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://le.nicolike.cn

Java: s.lines().toList()
来源：http://eg.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://fz.hnjuh.cn

Ruby: s.lines
来源：http://cy.bjjhwx.cn

C#:   s.Split('\n')
来源：http://gx.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://ro.hnjuh.cn

Py:   if not s:
来源：http://qq.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aw.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bh.szxytkj.cn

TS:   if (s === "") {}
来源：http://ty.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://rt.jctech888.com.cn

Go:   if s == "" {}
来源：http://uj.bjjhwx.cn

Ruby: if s.empty?
来源：http://rv.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://us.lnxyls.cn

[E21] 超长截断加省略号
来源：http://hp.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vc.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mj.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ou.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uk.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lk.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://gn.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tt.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://op.newstarts.cn


<!-- 参考信息 -->