代发 wailian999

TS:   [...new Set(arr)]
来源：http://ui.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zv.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qx.colortex.cn

Ruby: arr.uniq
来源：http://xn.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://kd.huanxung.cn

[D16] 求和与平均值
来源：http://va.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ok.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kb.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pp.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xi.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ce.chemitech.net.cn

Go:   // 手写循环累加
来源：http://kc.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jh.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ua.yuexingan06.cn

[D17] 最大值与最小值
来源：http://xm.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://tj.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://cm.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vo.newstarts.cn

TS:   Math.max(...arr);
来源：http://wb.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qc.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hx.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://ya.asd995.cn

C#:   list.Max();  list.Min()
来源：http://ym.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://vu.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jd.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://qm.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fq.shxzukj.cn

TS:   nested.flat();
来源：http://ey.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jg.szxytkj.cn

Go:   // 手写双层循环
来源：http://wt.huixiangedu.cn

Ruby: nested.flatten
来源：http://mw.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kv.hahajie.cn

[D19] 按字段分组
来源：http://ki.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qu.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mo.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kt.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fe.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://el.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://xg.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jm.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cj.521024.cn

[D20] 统计每个元素出现次数
来源：http://vm.wgjwhj.cn

Py:   Counter(arr)
来源：http://pn.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://rl.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ba.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xc.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iq.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://hi.shtwfgs.cn

Ruby: arr.tally
来源：http://ig.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kn.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://jw.nicolike.cn

Py:   x in arr
来源：http://cg.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://de.szxytkj.cn

JS:   arr.includes(x)
来源：http://lw.lnxyls.cn

TS:   arr.includes(x)
来源：http://rm.jctech888.com.cn

Java: list.contains(x)
来源：http://ne.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://lu.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://jm.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://in.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://hc.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://to.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rk.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qe.colortex.cn

TS:   [...arr];
来源：http://ol.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://nd.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://be.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ax.huixiangedu.cn

C#:   new List<int>(list);
来源：http://tk.bjjhwx.cn

[D23] reduce 累积计算
来源：http://nb.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mj.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ne.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nx.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jz.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://me.huanxung.cn

Go:   // 手写循环
来源：http://om.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zg.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aq.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://kt.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uj.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dj.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qf.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://js.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ii.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fc.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ol.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xp.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://kq.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sn.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ug.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ah.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wo.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fg.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iv.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dj.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xf.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://vb.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://mv.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://mf.asd995.cn

JS:   arr.join(", ")
来源：http://cy.asd995.cn

TS:   arr.join(", ")
来源：http://dn.panjiajie.cn

Java: String.join(", ", list)
来源：http://uc.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://pc.szsharing.cn

Ruby: arr.join(", ")
来源：http://do.colortex.cn

C#:   string.Join(", ", list)
来源：http://hd.521024.cn

================================================================================
来源：http://yf.yuntaijiaju.cn

E. 字符串处理
来源：http://yx.shxzukj.cn

================================================================================
来源：http://jw.lnxyls.cn

[E01] 拼接字符串
来源：http://ye.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qv.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zz.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lx.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nf.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pn.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kl.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qw.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ac.hahajie.cn

[E02] 重复字符串
来源：http://fs.huixiangedu.cn

Py:   "ab" * 3
来源：http://lb.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://aw.newstarts.cn

JS:   "ab".repeat(3)
来源：http://qz.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://xq.nicolike.cn

Java: "ab".repeat(3)
来源：http://cx.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://tl.jctech888.com.cn

Ruby: "ab" * 3
来源：http://nm.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nw.521024.cn

[E03] 截取子串
来源：http://ld.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cz.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nz.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cy.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://gw.hahajie.cn

Java: s.substring(1, 4)
来源：http://tc.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hv.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lb.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://yl.wgjwhj.cn

[E04] 查找子串位置
来源：http://oo.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://mc.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://av.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ku.hahajie.cn

TS:   s.indexOf("x")
来源：http://db.muxihuayi.cn

Java: s.indexOf("x")
来源：http://bs.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://mt.gzmigu.cn

Ruby: s.index("x")
来源：http://dr.9csxet.cn

C#:   s.IndexOf("x")
来源：http://mh.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tb.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ll.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xy.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kw.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yp.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fv.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xq.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fx.panjiajie.cn

[E06] 替换子串
来源：http://ki.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ve.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ng.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ik.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://ls.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bn.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ix.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ad.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://ya.szxytkj.cn

[E07] 按分隔符拆分
来源：http://iu.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dg.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zq.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ri.huixinmuqiang.cn

TS:   s.split(",")
来源：http://tc.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kp.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://su.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://na.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ly.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://fb.chemitech.net.cn

Py:   ",".join(items)
来源：http://xw.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://to.bjjhwx.cn

JS:   items.join(",")
来源：http://sk.jctech888.com.cn

TS:   items.join(",")
来源：http://rd.jctech888.com.cn

Java: String.join(",", items)
来源：http://sf.colortex.cn

Go:   strings.Join(items, ",")
来源：http://kx.yuexingan06.cn

Ruby: items.join(",")
来源：http://ve.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://gm.huanxung.cn

[E09] 去除所有空白字符
来源：http://sy.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aw.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ic.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://pf.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://br.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://la.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lk.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ex.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gw.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ix.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ko.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oq.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://xb.521024.cn

TS:   "7".padStart(3, "0")
来源：http://oa.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://xq.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tf.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://et.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lo.szsharing.cn

[E11] 反转字符串
来源：http://zr.9csxet.cn

Py:   s[::-1]
来源：http://rj.chemitech.net.cn

PHP:  strrev($s);
来源：http://xg.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://zn.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://xe.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eg.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ov.hnjuh.cn

Ruby: s.reverse
来源：http://hd.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uu.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://fz.muxihuayi.cn

Py:   s.count("a")
来源：http://tq.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://wv.szsharing.cn

JS:   s.split("a").length - 1
来源：http://va.nszjky.cn

TS:   s.split("a").length - 1
来源：http://cn.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lb.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://in.hnjuh.cn

Ruby: s.count("a")
来源：http://sx.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://wu.colortex.cn

[E13] 逐字符遍历
来源：http://gw.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://mq.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://or.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xx.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xo.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tc.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://li.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xu.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ew.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://us.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ah.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yr.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qn.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gz.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://js.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fx.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ee.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qx.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://mj.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cq.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fv.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cn.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wd.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jc.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tg.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cg.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nk.panjiajie.cn

[E16] 数字千分位
来源：http://ib.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ua.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://sx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uz.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sv.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yt.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rv.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tl.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://fm.nicolike.cn

[E17] 首字母大写
来源：http://ny.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nc.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gc.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vr.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qi.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oj.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vx.nszjky.cn

Ruby: s.capitalize
来源：http://mc.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wi.colortex.cn

[E18] 模板占位符替换
来源：http://pf.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ac.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vk.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kf.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ja.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ll.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gk.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ae.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zm.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://vg.szxytkj.cn

Py:   s.splitlines()
来源：http://do.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rp.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://fc.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://lj.bookmarksfly.cn

Java: s.lines().toList()
来源：http://bm.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://mr.lnxyls.cn

Ruby: s.lines
来源：http://uf.yuexingan06.cn

C#:   s.Split('\n')
来源：http://qv.newstarts.cn

[E20] 判断字符串是否为空
来源：http://us.panjiajie.cn

Py:   if not s:
来源：http://gm.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kq.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ed.lnxyls.cn

TS:   if (s === "") {}
来源：http://lu.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://vg.shxzskj.cn

Go:   if s == "" {}
来源：http://pj.lnxyls.cn

Ruby: if s.empty?
来源：http://hb.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://id.asd995.cn

[E21] 超长截断加省略号
来源：http://mj.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pv.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fl.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lj.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mv.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zr.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://te.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eb.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rb.nszjky.cn

[E22] 字节长度与字符长度
来源：http://qo.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nj.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ya.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://do.chemitech.net.cn


<!-- 参考信息 -->