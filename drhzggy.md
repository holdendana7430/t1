代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://df.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kc.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wk.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://kj.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wy.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ih.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ia.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://cg.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ae.bookmarksfly.cn

Go:   // 手写循环
来源：http://iw.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zy.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bf.nicolike.cn

[D15] 去重
来源：http://mq.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xi.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://iy.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://sj.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://kx.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qe.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vy.huanxung.cn

Ruby: arr.uniq
来源：http://qh.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://vl.muxihuayi.cn

[D16] 求和与平均值
来源：http://ap.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yu.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zw.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wr.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mr.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://da.9csxet.cn

Go:   // 手写循环累加
来源：http://hk.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vx.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://qb.huanxung.cn

[D17] 最大值与最小值
来源：http://qa.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://py.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://qe.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kq.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ym.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gp.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oj.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://iy.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://aq.colortex.cn

[D18] 扁平化嵌套数组
来源：http://bc.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wj.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://xo.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jt.nszjky.cn

TS:   nested.flat();
来源：http://ne.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dj.panjiajie.cn

Go:   // 手写双层循环
来源：http://hd.wgjwhj.cn

Ruby: nested.flatten
来源：http://rb.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yg.nicolike.cn

[D19] 按字段分组
来源：http://wg.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bw.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vo.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xp.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bf.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bf.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://qv.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ki.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cn.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://yk.szsharing.cn

Py:   Counter(arr)
来源：http://ej.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://td.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sm.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sm.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oc.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://he.nszjky.cn

Ruby: arr.tally
来源：http://jj.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uk.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://tk.colortex.cn

Py:   x in arr
来源：http://wn.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://bc.hnjuh.cn

JS:   arr.includes(x)
来源：http://yz.9csxet.cn

TS:   arr.includes(x)
来源：http://gl.asd995.cn

Java: list.contains(x)
来源：http://mf.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://ul.hnjuh.cn

Ruby: arr.include?(x)
来源：http://vw.9csxet.cn

C#:   list.Contains(x)
来源：http://nd.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://dv.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nu.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rb.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://go.yuntaijiaju.cn

TS:   [...arr];
来源：http://pz.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://zl.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bt.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://yh.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://hz.jctech888.com.cn

[D23] reduce 累积计算
来源：http://rc.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xm.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pq.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://me.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oq.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ls.lnxyls.cn

Go:   // 手写循环
来源：http://gj.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wn.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ma.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://rr.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mo.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oy.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xg.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qm.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ij.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mn.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xx.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rj.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://nj.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jx.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rd.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ug.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kg.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://os.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zv.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nb.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ic.muxihuayi.cn

[D26] 数组转字符串
来源：http://wo.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://cz.asd995.cn

PHP:  implode(", ", $arr);
来源：http://np.wgjwhj.cn

JS:   arr.join(", ")
来源：http://cy.hnjuh.cn

TS:   arr.join(", ")
来源：http://wo.colortex.cn

Java: String.join(", ", list)
来源：http://al.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://dw.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://ot.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ly.gzmigu.cn

================================================================================
来源：http://ma.9csxet.cn

E. 字符串处理
来源：http://yl.haigaiapp.cn

================================================================================
来源：http://uz.hnjuh.cn

[E01] 拼接字符串
来源：http://dc.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bj.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qk.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gi.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ke.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tk.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pw.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ve.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://of.hnjuh.cn

[E02] 重复字符串
来源：http://wc.chemitech.net.cn

Py:   "ab" * 3
来源：http://oh.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://pp.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://vf.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://zp.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://un.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://lc.szxytkj.cn

Ruby: "ab" * 3
来源：http://tw.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kx.shtwfgs.cn

[E03] 截取子串
来源：http://im.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jb.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ol.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gt.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://nf.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://bb.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jv.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jf.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://fl.9csxet.cn

[E04] 查找子串位置
来源：http://nb.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://fg.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://ba.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yx.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://pf.521024.cn

Java: s.indexOf("x")
来源：http://rx.asd995.cn

Go:   strings.Index(s, "x")
来源：http://dv.bookmarksfly.cn

Ruby: s.index("x")
来源：http://vw.asd995.cn

C#:   s.IndexOf("x")
来源：http://ei.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gh.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yb.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ea.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://th.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://su.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zw.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tv.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pc.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://en.huixinmuqiang.cn

[E06] 替换子串
来源：http://sr.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pe.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zu.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://dx.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xz.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zt.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lw.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://zr.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://vc.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bb.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mz.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aj.bjjhwx.cn

TS:   s.split(",")
来源：http://fe.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fg.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lp.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://yc.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sb.colortex.cn

[E08] 数组按分隔符合并
来源：http://rb.shtwfgs.cn

Py:   ",".join(items)
来源：http://is.9csxet.cn

PHP:  implode(",", $items);
来源：http://bi.9csxet.cn

JS:   items.join(",")
来源：http://eo.haigaiapp.cn

TS:   items.join(",")
来源：http://pz.jctech888.com.cn

Java: String.join(",", items)
来源：http://zd.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://yg.newstarts.cn

Ruby: items.join(",")
来源：http://ya.panjiajie.cn

C#:   string.Join(",", items)
来源：http://gh.hahajie.cn

[E09] 去除所有空白字符
来源：http://to.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nu.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ph.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://sb.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://tl.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://hb.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ji.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yi.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lk.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://mw.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qq.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uc.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://zn.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://xz.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://wc.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jc.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gs.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cs.muxihuayi.cn

[E11] 反转字符串
来源：http://mq.9csxet.cn

Py:   s[::-1]
来源：http://fp.huanxung.cn

PHP:  strrev($s);
来源：http://sn.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://bv.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://qu.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ws.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uw.nszjky.cn

Ruby: s.reverse
来源：http://vf.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://es.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://qe.huixinmuqiang.cn

Py:   s.count("a")
来源：http://ju.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://ip.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ir.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://cb.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ar.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://wn.asd995.cn

Ruby: s.count("a")
来源：http://gf.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://wi.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ig.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://rl.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nt.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uu.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pt.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bw.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ow.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wi.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kr.huanxung.cn

[E14] URL 编码与 Base64
来源：http://vj.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ew.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zq.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mq.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pn.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xs.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wx.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ca.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mr.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://sy.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cg.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nm.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rx.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jj.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nz.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qt.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ve.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tz.chemitech.net.cn

[E16] 数字千分位
来源：http://te.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://qx.lnxyls.cn

PHP:  number_format(1234567);
来源：http://dd.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zd.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ui.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oh.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dx.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://th.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://ca.shtwfgs.cn

[E17] 首字母大写
来源：http://lb.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mq.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fn.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gh.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kj.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mw.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wa.newstarts.cn

Ruby: s.capitalize
来源：http://ff.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cx.jctech888.com.cn

[E18] 模板占位符替换
来源：http://xc.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pn.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jg.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dk.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://de.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bz.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jd.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://um.szsharing.cn

[E19] 多行文本按行拆分
来源：http://qc.colortex.cn

Py:   s.splitlines()
来源：http://xg.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ua.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://db.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://uk.9csxet.cn

Java: s.lines().toList()
来源：http://dm.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://xm.bjjhwx.cn

Ruby: s.lines
来源：http://gz.hnjuh.cn

C#:   s.Split('\n')
来源：http://ae.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://pe.panjiajie.cn

Py:   if not s:
来源：http://aj.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bb.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lw.9csxet.cn

TS:   if (s === "") {}
来源：http://ap.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://eh.bjjhwx.cn


<!-- 参考信息 -->