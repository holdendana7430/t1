代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://nh.jianghongdianzi.cn

Go:   // 手写循环
来源：http://jf.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wn.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ao.huanxung.cn

[D15] 去重
来源：http://qs.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pu.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ei.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ru.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://wk.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yi.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ip.szxytkj.cn

Ruby: arr.uniq
来源：http://kc.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ob.521024.cn

[D16] 求和与平均值
来源：http://kw.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://np.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ue.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wj.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://db.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ff.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ux.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iz.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ua.521024.cn

[D17] 最大值与最小值
来源：http://aa.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ww.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ri.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zu.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://pp.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mr.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sz.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://oi.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://he.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://re.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gz.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://oo.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aq.colortex.cn

TS:   nested.flat();
来源：http://lr.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rb.bjjhwx.cn

Go:   // 手写双层循环
来源：http://wg.shtwfgs.cn

Ruby: nested.flatten
来源：http://by.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://to.yuexingan06.cn

[D19] 按字段分组
来源：http://nv.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fy.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vo.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cu.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yv.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ar.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yg.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oi.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://uz.huixiangedu.cn

Py:   Counter(arr)
来源：http://uf.huanxung.cn

PHP:  array_count_values($arr);
来源：http://dw.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ql.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sz.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.521024.cn

Go:   // 手写 map[T]int
来源：http://un.521024.cn

Ruby: arr.tally
来源：http://bz.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sp.nszjky.cn

[D21] 判断是否包含某元素
来源：http://vn.asd995.cn

Py:   x in arr
来源：http://lj.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://hd.newstarts.cn

JS:   arr.includes(x)
来源：http://lj.szsharing.cn

TS:   arr.includes(x)
来源：http://vm.yuntaijiaju.cn

Java: list.contains(x)
来源：http://jt.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://sl.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://fz.szsharing.cn

C#:   list.Contains(x)
来源：http://xs.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://jx.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cx.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pi.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aq.nicolike.cn

TS:   [...arr];
来源：http://it.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://fw.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://df.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://nu.colortex.cn

C#:   new List<int>(list);
来源：http://kg.hnjuh.cn

[D23] reduce 累积计算
来源：http://xv.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cy.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pz.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://he.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qg.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hh.asd995.cn

Go:   // 手写循环
来源：http://mw.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yv.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tr.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://va.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tp.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zv.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ut.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zj.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zx.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lk.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ky.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kf.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://yi.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://em.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dl.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gu.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gi.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://on.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ra.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ga.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qw.szxytkj.cn

[D26] 数组转字符串
来源：http://ub.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://sc.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ly.9csxet.cn

JS:   arr.join(", ")
来源：http://pf.colortex.cn

TS:   arr.join(", ")
来源：http://wb.9csxet.cn

Java: String.join(", ", list)
来源：http://nc.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://hj.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://fw.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://pl.szxytkj.cn

================================================================================
来源：http://dd.hnjuh.cn

E. 字符串处理
来源：http://ay.szsharing.cn

================================================================================
来源：http://xp.shtwfgs.cn

[E01] 拼接字符串
来源：http://rw.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sq.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://an.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wx.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cq.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://an.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ri.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bs.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ag.521024.cn

[E02] 重复字符串
来源：http://ai.shxzukj.cn

Py:   "ab" * 3
来源：http://sw.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://lg.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://nb.newstarts.cn

TS:   "ab".repeat(3)
来源：http://aq.shxzukj.cn

Java: "ab".repeat(3)
来源：http://sd.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://aa.shxzskj.cn

Ruby: "ab" * 3
来源：http://kf.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ed.nicolike.cn

[E03] 截取子串
来源：http://wv.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zw.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sl.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qo.colortex.cn

TS:   s.slice(1, 4)
来源：http://fc.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://aj.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ks.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nt.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://cc.yuexingan06.cn

[E04] 查找子串位置
来源：http://eq.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ag.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://je.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xj.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://qq.shxzukj.cn

Java: s.indexOf("x")
来源：http://ql.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://os.lnxyls.cn

Ruby: s.index("x")
来源：http://kf.newstarts.cn

C#:   s.IndexOf("x")
来源：http://mx.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ih.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gp.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sp.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://af.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qw.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ho.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kv.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iw.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vk.bookmarksfly.cn

[E06] 替换子串
来源：http://vj.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://de.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://gt.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mf.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://xk.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lr.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zg.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ei.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://pc.lnxyls.cn

[E07] 按分隔符拆分
来源：http://ty.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sn.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tp.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hs.shtwfgs.cn

TS:   s.split(",")
来源：http://ga.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tp.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pd.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ds.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mt.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://hj.panjiajie.cn

Py:   ",".join(items)
来源：http://lc.gzmigu.cn

PHP:  implode(",", $items);
来源：http://of.haigaiapp.cn

JS:   items.join(",")
来源：http://bo.huixiangedu.cn

TS:   items.join(",")
来源：http://sy.shtwfgs.cn

Java: String.join(",", items)
来源：http://bq.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://kb.szsharing.cn

Ruby: items.join(",")
来源：http://eo.hnjuh.cn

C#:   string.Join(",", items)
来源：http://nd.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://as.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ni.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ds.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://ki.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://mi.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://mt.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wg.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yl.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ep.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://he.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://at.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ws.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://qh.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://oe.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://rz.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rf.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fw.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jt.bookmarksfly.cn

[E11] 反转字符串
来源：http://yw.jctech888.com.cn

Py:   s[::-1]
来源：http://ho.huixiangedu.cn

PHP:  strrev($s);
来源：http://gz.521024.cn

JS:   [...s].reverse().join("")
来源：http://gq.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://mt.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kp.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fq.jctech888.com.cn

Ruby: s.reverse
来源：http://bl.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yx.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://rp.gzmigu.cn

Py:   s.count("a")
来源：http://ue.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://dl.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://jj.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://zc.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jm.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://kc.yuexingan06.cn

Ruby: s.count("a")
来源：http://ew.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://rj.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://rp.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://qo.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mg.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bw.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yo.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eo.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ux.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cm.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gy.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://ix.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uh.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jc.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fo.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pp.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jn.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fc.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bw.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yv.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://zf.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fs.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sq.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cl.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xr.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xv.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nn.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rt.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ro.wgjwhj.cn

[E16] 数字千分位
来源：http://bw.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://us.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://ya.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jg.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mo.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ew.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ph.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rp.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://jb.hnjuh.cn

[E17] 首字母大写
来源：http://ux.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://re.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gc.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aw.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nh.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hw.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eu.newstarts.cn

Ruby: s.capitalize
来源：http://dl.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tb.panjiajie.cn

[E18] 模板占位符替换
来源：http://tg.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ng.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zm.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dd.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ip.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cu.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ec.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wi.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yx.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://lv.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ra.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://df.521024.cn

JS:   s.split(/\r?\n/)
来源：http://ru.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://fp.9csxet.cn

Java: s.lines().toList()
来源：http://iu.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://gr.huixiangedu.cn

Ruby: s.lines
来源：http://pf.wgjwhj.cn

C#:   s.Split('\n')
来源：http://kw.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://um.521024.cn

Py:   if not s:
来源：http://ad.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gm.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cp.shxzskj.cn

TS:   if (s === "") {}
来源：http://gu.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://bu.nszjky.cn

Go:   if s == "" {}
来源：http://sj.bookmarksfly.cn

Ruby: if s.empty?
来源：http://gg.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://be.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://au.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nq.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ei.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wf.hahajie.cn


<!-- 参考信息 -->