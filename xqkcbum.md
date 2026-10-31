代发 wailian999

Py:   len(arr)
来源：http://rp.chemitech.net.cn

PHP:  count($arr);
来源：http://na.jianghongdianzi.cn

JS:   arr.length
来源：http://tf.jianghongdianzi.cn

TS:   arr.length
来源：http://cd.lnxyls.cn

Java: list.size();
来源：http://ty.bjjhwx.cn

Go:   len(arr)
来源：http://gw.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://he.hahajie.cn

C#:   list.Count;
来源：http://ag.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://gp.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gq.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yt.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://va.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://pw.colortex.cn

Java: list.subList(1, 4);
来源：http://uv.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://hs.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://tm.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://ow.chemitech.net.cn

[D08] 合并两个数组
来源：http://su.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://lf.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://of.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uy.asd995.cn

TS:   [...a, ...b];
来源：http://es.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://go.521024.cn

Go:   append(a, b...)
来源：http://en.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://wd.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://ud.szsharing.cn

[D09] 排序（升序）
来源：http://rp.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://qx.panjiajie.cn

PHP:  sort($arr);
来源：http://ax.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hj.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wj.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nf.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yh.gzmigu.cn

Ruby: arr.sort
来源：http://ub.521024.cn

C#:   list.Sort();
来源：http://vq.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gb.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jj.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xi.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gp.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dk.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qj.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ee.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jg.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lc.colortex.cn

[D11] 反转数组
来源：http://nj.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rq.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://tb.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lz.hahajie.cn

TS:   [...arr].reverse();
来源：http://wl.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://xw.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://gt.shtwfgs.cn

Ruby: arr.reverse
来源：http://dc.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://fi.szsharing.cn

[D12] 查找元素下标
来源：http://va.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://xv.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lh.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ls.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ap.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vb.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://dg.bjjhwx.cn

Ruby: arr.index(x)
来源：http://ht.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://od.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://la.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bg.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dy.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://jq.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://dn.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://il.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qq.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zs.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bj.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ea.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cy.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://og.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://nd.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://vd.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wj.chemitech.net.cn

Go:   // 手写循环
来源：http://le.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://us.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mj.haigaiapp.cn

[D15] 去重
来源：http://dq.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ud.hnjuh.cn

PHP:  array_unique($arr);
来源：http://kx.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://ue.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://tt.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uv.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xv.lnxyls.cn

Ruby: arr.uniq
来源：http://cy.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://cf.wgjwhj.cn

[D16] 求和与平均值
来源：http://pf.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gk.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rt.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nm.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cr.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wm.chemitech.net.cn

Go:   // 手写循环累加
来源：http://qm.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lf.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://vb.newstarts.cn

[D17] 最大值与最小值
来源：http://ca.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://lh.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://qr.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yn.lnxyls.cn

TS:   Math.max(...arr);
来源：http://gb.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ag.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ga.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://pj.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://by.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://lk.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sg.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://lt.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zk.wgjwhj.cn

TS:   nested.flat();
来源：http://go.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ir.haigaiapp.cn

Go:   // 手写双层循环
来源：http://vq.panjiajie.cn

Ruby: nested.flatten
来源：http://ck.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wc.szxytkj.cn

[D19] 按字段分组
来源：http://hs.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://up.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ma.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://be.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xf.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mu.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://zd.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ud.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wh.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://eu.yuexingan06.cn

Py:   Counter(arr)
来源：http://ut.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://sw.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hr.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lf.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qi.nicolike.cn

Go:   // 手写 map[T]int
来源：http://lg.hnjuh.cn

Ruby: arr.tally
来源：http://ik.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ol.szsharing.cn

[D21] 判断是否包含某元素
来源：http://by.muxihuayi.cn

Py:   x in arr
来源：http://cl.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://ye.9csxet.cn

JS:   arr.includes(x)
来源：http://mf.gzmigu.cn

TS:   arr.includes(x)
来源：http://hh.shxzskj.cn

Java: list.contains(x)
来源：http://wz.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://pa.asd995.cn

Ruby: arr.include?(x)
来源：http://hb.nszjky.cn

C#:   list.Contains(x)
来源：http://dx.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://vv.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cc.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wh.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mf.bookmarksfly.cn

TS:   [...arr];
来源：http://cx.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://fa.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://po.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://jt.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://se.asd995.cn

[D23] reduce 累积计算
来源：http://oo.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vi.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wb.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lq.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jj.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oe.yuntaijiaju.cn

Go:   // 手写循环
来源：http://zz.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://in.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pl.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://az.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kx.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hq.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lf.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nk.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cy.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zm.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cm.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://om.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://zg.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://um.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lu.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nb.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pr.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qh.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://go.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bq.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ks.shxzukj.cn

[D26] 数组转字符串
来源：http://sb.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://ew.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://pt.muxihuayi.cn

JS:   arr.join(", ")
来源：http://mz.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ci.lnxyls.cn

Java: String.join(", ", list)
来源：http://yv.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://vb.colortex.cn

Ruby: arr.join(", ")
来源：http://md.hahajie.cn

C#:   string.Join(", ", list)
来源：http://tp.nicolike.cn

================================================================================
来源：http://yh.shxzukj.cn

E. 字符串处理
来源：http://cn.hnjuh.cn

================================================================================
来源：http://iy.colortex.cn

[E01] 拼接字符串
来源：http://ob.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gd.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lu.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jc.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kd.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://if.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gm.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nh.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pp.muxihuayi.cn

[E02] 重复字符串
来源：http://le.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://cs.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://ln.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://pj.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://xe.521024.cn

Java: "ab".repeat(3)
来源：http://hu.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://aa.shxzukj.cn

Ruby: "ab" * 3
来源：http://mt.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oh.hahajie.cn

[E03] 截取子串
来源：http://xw.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mf.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ze.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sy.asd995.cn

TS:   s.slice(1, 4)
来源：http://ea.hnjuh.cn

Java: s.substring(1, 4)
来源：http://rm.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zj.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yc.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://hy.nszjky.cn

[E04] 查找子串位置
来源：http://ao.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://zq.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://gv.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kb.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://cu.nicolike.cn

Java: s.indexOf("x")
来源：http://ai.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://mp.bjjhwx.cn

Ruby: s.index("x")
来源：http://kf.nicolike.cn

C#:   s.IndexOf("x")
来源：http://xe.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gs.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bu.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nh.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://un.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qv.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nt.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dp.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ub.newstarts.cn

[E06] 替换子串
来源：http://sg.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qd.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://bp.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://va.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://uz.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iz.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mr.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ay.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://zo.szsharing.cn

[E07] 按分隔符拆分
来源：http://kr.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ge.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qt.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://go.bjjhwx.cn

TS:   s.split(",")
来源：http://it.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yx.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://th.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://vd.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vr.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://hy.yuexingan06.cn

Py:   ",".join(items)
来源：http://bj.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://zl.haigaiapp.cn

JS:   items.join(",")
来源：http://az.chemitech.net.cn

TS:   items.join(",")
来源：http://vk.asd995.cn

Java: String.join(",", items)
来源：http://cg.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://xo.shxzukj.cn

Ruby: items.join(",")
来源：http://ag.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ti.lnxyls.cn

[E09] 去除所有空白字符
来源：http://gj.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xl.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xv.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://sf.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://bn.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://vk.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wo.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qp.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cl.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://uz.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yl.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ef.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://hl.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://xp.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://lu.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xs.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hb.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xm.shtwfgs.cn

[E11] 反转字符串
来源：http://jx.shxzukj.cn

Py:   s[::-1]
来源：http://nl.haigaiapp.cn

PHP:  strrev($s);
来源：http://mv.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://ht.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://ef.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dl.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vn.muxihuayi.cn

Ruby: s.reverse
来源：http://ya.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sy.hahajie.cn

[E12] 统计某字符出现次数
来源：http://kg.hnjuh.cn

Py:   s.count("a")
来源：http://tp.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://ws.521024.cn

JS:   s.split("a").length - 1
来源：http://ie.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://cb.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ws.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://ld.newstarts.cn

Ruby: s.count("a")
来源：http://oe.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://nu.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://mg.jianghongdianzi.cn


<!-- 参考信息 -->