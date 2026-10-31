代发 wailian999

Ruby: arr.index(x)
来源：http://nl.colortex.cn

C#:   list.IndexOf(x);
来源：http://jl.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://cx.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://it.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ut.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://fv.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://ln.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://za.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vw.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ie.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bj.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://sp.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oh.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ki.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://yz.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://zs.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bl.jctech888.com.cn

Go:   // 手写循环
来源：http://ax.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://me.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xt.9csxet.cn

[D15] 去重
来源：http://ca.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ox.panjiajie.cn

PHP:  array_unique($arr);
来源：http://da.colortex.cn

JS:   [...new Set(arr)]
来源：http://jn.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://bi.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fl.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yl.haigaiapp.cn

Ruby: arr.uniq
来源：http://cq.521024.cn

C#:   list.Distinct().ToList()
来源：http://eo.shxzskj.cn

[D16] 求和与平均值
来源：http://kh.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pl.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zi.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oo.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gr.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iu.521024.cn

Go:   // 手写循环累加
来源：http://wk.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zr.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://ey.szsharing.cn

[D17] 最大值与最小值
来源：http://qn.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://br.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://cj.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://em.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ja.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ze.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ro.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://hd.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://sb.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://rq.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yx.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ut.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jd.wgjwhj.cn

TS:   nested.flat();
来源：http://dd.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ve.panjiajie.cn

Go:   // 手写双层循环
来源：http://lx.chemitech.net.cn

Ruby: nested.flatten
来源：http://pc.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gl.hnjuh.cn

[D19] 按字段分组
来源：http://ik.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ra.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://al.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xs.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cj.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://md.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://bb.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dz.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fc.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://wb.bjjhwx.cn

Py:   Counter(arr)
来源：http://zl.newstarts.cn

PHP:  array_count_values($arr);
来源：http://qy.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zq.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cd.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vi.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://xw.szxytkj.cn

Ruby: arr.tally
来源：http://rv.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fw.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://wh.asd995.cn

Py:   x in arr
来源：http://dk.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://sq.hnjuh.cn

JS:   arr.includes(x)
来源：http://no.shtwfgs.cn

TS:   arr.includes(x)
来源：http://wj.wgjwhj.cn

Java: list.contains(x)
来源：http://qn.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://sx.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://eq.yuexingan06.cn

C#:   list.Contains(x)
来源：http://zc.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://vy.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pq.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dp.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xg.jianghongdianzi.cn

TS:   [...arr];
来源：http://ba.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://ju.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ip.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://lz.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://oy.muxihuayi.cn

[D23] reduce 累积计算
来源：http://jk.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mb.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zx.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tb.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ek.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kw.chemitech.net.cn

Go:   // 手写循环
来源：http://zo.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ft.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gf.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://dr.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qt.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://us.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hv.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dk.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pe.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ct.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fq.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kr.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://hp.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bv.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gt.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://om.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nz.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cw.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://in.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qt.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nw.9csxet.cn

[D26] 数组转字符串
来源：http://iu.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://nj.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://an.shtwfgs.cn

JS:   arr.join(", ")
来源：http://bo.nszjky.cn

TS:   arr.join(", ")
来源：http://px.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://ao.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://ix.lnxyls.cn

Ruby: arr.join(", ")
来源：http://zb.nicolike.cn

C#:   string.Join(", ", list)
来源：http://zt.haigaiapp.cn

================================================================================
来源：http://yi.lnxyls.cn

E. 字符串处理
来源：http://mj.huanxung.cn

================================================================================
来源：http://ep.nszjky.cn

[E01] 拼接字符串
来源：http://om.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://av.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pz.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fp.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qh.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sa.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bc.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ch.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dp.huanxung.cn

[E02] 重复字符串
来源：http://uv.bookmarksfly.cn

Py:   "ab" * 3
来源：http://mm.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://xk.nszjky.cn

JS:   "ab".repeat(3)
来源：http://yu.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://gc.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://bn.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://vz.panjiajie.cn

Ruby: "ab" * 3
来源：http://if.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hs.huixiangedu.cn

[E03] 截取子串
来源：http://sz.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ks.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bk.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kd.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://ah.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://gk.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ov.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://aw.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://hj.colortex.cn

[E04] 查找子串位置
来源：http://wi.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://sb.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://fs.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ab.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://fu.muxihuayi.cn

Java: s.indexOf("x")
来源：http://xa.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://bt.szxytkj.cn

Ruby: s.index("x")
来源：http://qy.newstarts.cn

C#:   s.IndexOf("x")
来源：http://tl.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gx.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lf.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yj.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://se.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ce.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ju.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ij.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cb.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://il.huanxung.cn

[E06] 替换子串
来源：http://bd.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uu.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://kw.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vu.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://rx.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ro.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ev.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yk.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://jz.nszjky.cn

[E07] 按分隔符拆分
来源：http://jn.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ch.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yl.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lj.chemitech.net.cn

TS:   s.split(",")
来源：http://oz.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sn.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zb.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://xy.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wl.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://pp.panjiajie.cn

Py:   ",".join(items)
来源：http://ge.hnjuh.cn

PHP:  implode(",", $items);
来源：http://tk.colortex.cn

JS:   items.join(",")
来源：http://hw.shtwfgs.cn

TS:   items.join(",")
来源：http://mp.nszjky.cn

Java: String.join(",", items)
来源：http://pd.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ad.jctech888.com.cn

Ruby: items.join(",")
来源：http://um.shxzskj.cn

C#:   string.Join(",", items)
来源：http://gd.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ux.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pb.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ms.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://pp.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://zq.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://vi.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qv.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lx.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://jd.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ym.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hv.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://mq.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://od.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://cb.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yi.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ql.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nm.huanxung.cn

[E11] 反转字符串
来源：http://ob.yuexingan06.cn

Py:   s[::-1]
来源：http://mc.gzmigu.cn

PHP:  strrev($s);
来源：http://mf.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://nl.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://xh.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bs.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aq.shxzskj.cn

Ruby: s.reverse
来源：http://ra.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tr.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://wf.newstarts.cn

Py:   s.count("a")
来源：http://ft.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://bo.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://eh.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ag.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yh.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://yv.huixiangedu.cn

Ruby: s.count("a")
来源：http://pk.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://gn.nicolike.cn

[E13] 逐字符遍历
来源：http://ba.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://wj.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yy.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vn.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ud.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xj.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zv.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ym.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://up.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://un.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wo.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vs.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ul.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pb.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uq.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ov.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://on.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ll.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://ou.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bw.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ts.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vn.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pu.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tc.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ge.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pz.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://de.yuexingan06.cn

[E16] 数字千分位
来源：http://av.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://rr.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://jx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wp.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wi.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gx.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jx.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dx.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://kt.shxzskj.cn

[E17] 首字母大写
来源：http://ca.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ip.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fl.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xn.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gj.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ai.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lc.asd995.cn

Ruby: s.capitalize
来源：http://jl.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://af.huixiangedu.cn

[E18] 模板占位符替换
来源：http://og.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nl.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qj.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uy.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vl.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lk.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aw.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yh.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vj.hahajie.cn

[E19] 多行文本按行拆分
来源：http://tw.bookmarksfly.cn

Py:   s.splitlines()
来源：http://oq.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://el.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://eq.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://tu.shxzukj.cn

Java: s.lines().toList()
来源：http://xm.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://dm.wgjwhj.cn


<!-- 参考信息 -->