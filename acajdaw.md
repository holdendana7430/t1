代发 wailian999

Py:   len(arr)
来源：http://ws.chemitech.net.cn

PHP:  count($arr);
来源：http://cq.colortex.cn

JS:   arr.length
来源：http://mr.haigaiapp.cn

TS:   arr.length
来源：http://mk.shtwfgs.cn

Java: list.size();
来源：http://jp.hnjuh.cn

Go:   len(arr)
来源：http://sr.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://en.szsharing.cn

C#:   list.Count;
来源：http://ck.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://qy.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hn.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lx.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://rx.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://sy.hnjuh.cn

Java: list.subList(1, 4);
来源：http://jl.yuexingan06.cn

Go:   arr[1:4]
来源：http://qw.huanxung.cn

Ruby: arr[1, 3]
来源：http://jy.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ep.newstarts.cn

[D08] 合并两个数组
来源：http://vw.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://dp.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://by.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ll.asd995.cn

TS:   [...a, ...b];
来源：http://ry.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ff.521024.cn

Go:   append(a, b...)
来源：http://rc.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://dl.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://kk.shtwfgs.cn

[D09] 排序（升序）
来源：http://fv.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://zx.wgjwhj.cn

PHP:  sort($arr);
来源：http://xo.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ah.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://le.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nc.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wi.hnjuh.cn

Ruby: arr.sort
来源：http://um.wgjwhj.cn

C#:   list.Sort();
来源：http://yy.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ba.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sw.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://by.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qe.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://we.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uu.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ee.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fa.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ji.asd995.cn

[D11] 反转数组
来源：http://qj.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://al.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://tl.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vb.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://dx.newstarts.cn

Java: Collections.reverse(list);
来源：http://wf.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ml.shxzskj.cn

Ruby: arr.reverse
来源：http://iu.bookmarksfly.cn

C#:   list.Reverse();
来源：http://oz.521024.cn

[D12] 查找元素下标
来源：http://qq.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ps.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qo.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://am.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ex.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jh.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://vm.muxihuayi.cn

Ruby: arr.index(x)
来源：http://ha.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://kt.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://tp.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ln.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://sd.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://xc.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wt.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cc.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xi.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ig.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://nr.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ve.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wg.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://qk.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://hh.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ah.chemitech.net.cn

Go:   // 手写循环
来源：http://fo.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nf.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wk.asd995.cn

[D15] 去重
来源：http://ns.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ki.shxzskj.cn

PHP:  array_unique($arr);
来源：http://jg.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://qc.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://ss.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cf.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ov.szsharing.cn

Ruby: arr.uniq
来源：http://ar.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://eq.jctech888.com.cn

[D16] 求和与平均值
来源：http://xk.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://as.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qh.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ui.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ub.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rl.newstarts.cn

Go:   // 手写循环累加
来源：http://zq.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bo.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://ys.shtwfgs.cn

[D17] 最大值与最小值
来源：http://pt.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://wt.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://xr.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zj.panjiajie.cn

TS:   Math.max(...arr);
来源：http://bx.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cc.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oy.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://se.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://tp.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://yi.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xy.521024.cn

PHP:  array_merge(...$nested);
来源：http://ji.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hu.chemitech.net.cn

TS:   nested.flat();
来源：http://mt.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gx.lnxyls.cn

Go:   // 手写双层循环
来源：http://oh.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://qy.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ej.huixinmuqiang.cn

[D19] 按字段分组
来源：http://fi.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bz.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lv.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gn.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ym.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yn.colortex.cn

Go:   // 手写 map[string][]T
来源：http://lv.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wb.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uy.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ru.panjiajie.cn

Py:   Counter(arr)
来源：http://ra.9csxet.cn

PHP:  array_count_values($arr);
来源：http://gg.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bt.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wa.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tz.asd995.cn

Go:   // 手写 map[T]int
来源：http://sh.huanxung.cn

Ruby: arr.tally
来源：http://wl.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fh.colortex.cn

[D21] 判断是否包含某元素
来源：http://lb.gzmigu.cn

Py:   x in arr
来源：http://wh.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://tn.newstarts.cn

JS:   arr.includes(x)
来源：http://ir.shxzukj.cn

TS:   arr.includes(x)
来源：http://xt.nszjky.cn

Java: list.contains(x)
来源：http://pk.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://vp.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://cs.521024.cn

C#:   list.Contains(x)
来源：http://kp.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://ji.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jv.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ff.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ej.haigaiapp.cn

TS:   [...arr];
来源：http://ki.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ih.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pj.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://zn.wgjwhj.cn

C#:   new List<int>(list);
来源：http://kz.521024.cn

[D23] reduce 累积计算
来源：http://oh.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bh.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://le.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kt.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://at.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ia.huixiangedu.cn

Go:   // 手写循环
来源：http://nx.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kg.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lc.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://mw.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gt.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fa.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cz.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qo.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nk.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://he.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fk.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sa.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://tr.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bl.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ja.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sz.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fp.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aw.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nb.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cr.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sf.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ey.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://iu.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://bk.colortex.cn

JS:   arr.join(", ")
来源：http://li.huanxung.cn

TS:   arr.join(", ")
来源：http://ej.szsharing.cn

Java: String.join(", ", list)
来源：http://zp.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://rn.huanxung.cn

Ruby: arr.join(", ")
来源：http://wt.nicolike.cn

C#:   string.Join(", ", list)
来源：http://rf.jctech888.com.cn

================================================================================
来源：http://ns.muxihuayi.cn

E. 字符串处理
来源：http://sf.lnxyls.cn

================================================================================
来源：http://ka.521024.cn

[E01] 拼接字符串
来源：http://ve.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ve.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://es.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eo.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ik.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://al.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zp.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://od.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vy.colortex.cn

[E02] 重复字符串
来源：http://me.9csxet.cn

Py:   "ab" * 3
来源：http://cz.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://lh.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://cm.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://yi.nszjky.cn

Java: "ab".repeat(3)
来源：http://qq.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://zs.szsharing.cn

Ruby: "ab" * 3
来源：http://li.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://af.asd995.cn

[E03] 截取子串
来源：http://wn.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qc.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://me.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ki.asd995.cn

TS:   s.slice(1, 4)
来源：http://mc.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://md.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bm.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mr.521024.cn

C#:   s.Substring(1, 3)
来源：http://xf.shxzukj.cn

[E04] 查找子串位置
来源：http://ox.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://rj.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ee.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dk.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ej.jctech888.com.cn

Java: s.indexOf("x")
来源：http://sp.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://bc.panjiajie.cn

Ruby: s.index("x")
来源：http://uv.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://hx.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dh.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kt.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://am.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hb.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ov.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wo.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gf.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pl.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zx.asd995.cn

[E06] 替换子串
来源：http://qq.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tn.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://hu.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://up.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vl.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://on.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://vq.hahajie.cn

[E07] 按分隔符拆分
来源：http://or.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rb.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dd.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mq.lnxyls.cn

TS:   s.split(",")
来源：http://ap.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sw.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zu.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://vs.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aw.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://cz.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://xs.asd995.cn

PHP:  implode(",", $items);
来源：http://sq.shxzskj.cn

JS:   items.join(",")
来源：http://wp.panjiajie.cn

TS:   items.join(",")
来源：http://ew.szsharing.cn

Java: String.join(",", items)
来源：http://xn.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://jz.jctech888.com.cn

Ruby: items.join(",")
来源：http://rx.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://go.newstarts.cn

[E09] 去除所有空白字符
来源：http://xg.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qu.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oe.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://kr.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://lk.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://bs.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kt.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://er.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ri.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://oj.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rt.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jg.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://dx.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://bd.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://rx.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jf.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uh.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xv.hnjuh.cn

[E11] 反转字符串
来源：http://rv.chemitech.net.cn

Py:   s[::-1]
来源：http://og.muxihuayi.cn

PHP:  strrev($s);
来源：http://yy.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://vo.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://lr.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mm.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://de.shxzskj.cn

Ruby: s.reverse
来源：http://ln.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sq.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://dy.szxytkj.cn

Py:   s.count("a")
来源：http://wf.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://as.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://pf.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://ck.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ov.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://wo.chemitech.net.cn

Ruby: s.count("a")
来源：http://an.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://ew.lnxyls.cn

[E13] 逐字符遍历
来源：http://qs.gzmigu.cn


<!-- 参考信息 -->