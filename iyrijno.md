代发 wailian999

[D07] 切片 / 取子数组
来源：http://gt.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wd.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xw.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://yz.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://jd.hnjuh.cn

Java: list.subList(1, 4);
来源：http://zv.shtwfgs.cn

Go:   arr[1:4]
来源：http://cd.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://xq.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ys.haigaiapp.cn

[D08] 合并两个数组
来源：http://sq.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://lw.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://bu.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iy.jctech888.com.cn

TS:   [...a, ...b];
来源：http://fp.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xx.gzmigu.cn

Go:   append(a, b...)
来源：http://as.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://di.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://ze.huanxung.cn

[D09] 排序（升序）
来源：http://va.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://it.haigaiapp.cn

PHP:  sort($arr);
来源：http://ii.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mi.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://et.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dk.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cg.nszjky.cn

Ruby: arr.sort
来源：http://we.shxzukj.cn

C#:   list.Sort();
来源：http://xk.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ed.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xb.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vd.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ev.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jw.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mv.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ki.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rz.newstarts.cn

[D11] 反转数组
来源：http://iy.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jw.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://id.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://he.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://pl.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://fp.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://tk.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://fw.wgjwhj.cn

C#:   list.Reverse();
来源：http://sk.nszjky.cn

[D12] 查找元素下标
来源：http://kq.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://as.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fr.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sq.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pl.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zt.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://hv.haigaiapp.cn

Ruby: arr.index(x)
来源：http://bd.szsharing.cn

C#:   list.IndexOf(x);
来源：http://jr.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://up.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vw.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fw.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ti.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://vb.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mv.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oi.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ld.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ls.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://uj.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vf.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pz.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://qm.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://ml.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ry.yuntaijiaju.cn

Go:   // 手写循环
来源：http://dm.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pt.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kb.wgjwhj.cn

[D15] 去重
来源：http://fl.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nq.newstarts.cn

PHP:  array_unique($arr);
来源：http://ih.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://zu.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://ql.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zi.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cl.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://sm.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://uk.hnjuh.cn

[D16] 求和与平均值
来源：http://aw.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mx.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ab.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yd.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://in.wgjwhj.cn

Go:   // 手写循环累加
来源：http://zh.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uf.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://on.wgjwhj.cn

[D17] 最大值与最小值
来源：http://gf.asd995.cn

Py:   max(arr);  min(arr)
来源：http://lk.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://uv.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uo.szxytkj.cn

TS:   Math.max(...arr);
来源：http://zw.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ur.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yw.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://ju.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ec.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://oa.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nb.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ju.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jr.bookmarksfly.cn

TS:   nested.flat();
来源：http://ym.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gd.gzmigu.cn

Go:   // 手写双层循环
来源：http://ko.szsharing.cn

Ruby: nested.flatten
来源：http://yk.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vy.gzmigu.cn

[D19] 按字段分组
来源：http://hk.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qp.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hc.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fi.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://me.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fn.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://yn.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zc.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cw.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://kf.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://es.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://te.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vn.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cz.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://is.colortex.cn

Go:   // 手写 map[T]int
来源：http://ph.521024.cn

Ruby: arr.tally
来源：http://ht.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yb.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://rz.lnxyls.cn

Py:   x in arr
来源：http://mo.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://rz.jctech888.com.cn

JS:   arr.includes(x)
来源：http://zk.newstarts.cn

TS:   arr.includes(x)
来源：http://rg.yuexingan06.cn

Java: list.contains(x)
来源：http://ni.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://lw.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://af.yuexingan06.cn

C#:   list.Contains(x)
来源：http://gq.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://op.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qx.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gm.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aj.bjjhwx.cn

TS:   [...arr];
来源：http://xj.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://pj.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xn.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://jm.asd995.cn

C#:   new List<int>(list);
来源：http://jo.nicolike.cn

[D23] reduce 累积计算
来源：http://mo.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oo.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pj.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yc.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sx.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qe.huanxung.cn

Go:   // 手写循环
来源：http://bf.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nl.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://af.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://hc.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fj.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ei.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xc.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://va.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://df.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qk.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vu.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bp.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://hq.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gx.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xv.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yt.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cm.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tp.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gl.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://io.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hp.yuexingan06.cn

[D26] 数组转字符串
来源：http://za.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://zp.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://nv.shtwfgs.cn

JS:   arr.join(", ")
来源：http://kz.muxihuayi.cn

TS:   arr.join(", ")
来源：http://kq.shxzukj.cn

Java: String.join(", ", list)
来源：http://ju.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://ws.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://zc.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://me.9csxet.cn

================================================================================
来源：http://bp.asd995.cn

E. 字符串处理
来源：http://vz.huixiangedu.cn

================================================================================
来源：http://sq.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://pf.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dd.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xo.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xj.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dl.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vb.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nf.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cn.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fd.gzmigu.cn

[E02] 重复字符串
来源：http://xp.muxihuayi.cn

Py:   "ab" * 3
来源：http://tf.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://xn.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://tf.521024.cn

TS:   "ab".repeat(3)
来源：http://oy.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://fv.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://nx.gzmigu.cn

Ruby: "ab" * 3
来源：http://ak.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zv.huixinmuqiang.cn

[E03] 截取子串
来源：http://sk.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vt.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kl.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://te.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://gd.gzmigu.cn

Java: s.substring(1, 4)
来源：http://an.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pr.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cq.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://sw.szsharing.cn

[E04] 查找子串位置
来源：http://ia.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://hm.huanxung.cn

PHP:  strpos($s, "x");
来源：http://xl.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zf.huanxung.cn

TS:   s.indexOf("x")
来源：http://un.shxzskj.cn

Java: s.indexOf("x")
来源：http://ab.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://hz.colortex.cn

Ruby: s.index("x")
来源：http://ij.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://bj.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ns.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ha.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gw.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kx.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ti.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://km.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kb.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vx.shxzskj.cn

[E06] 替换子串
来源：http://hg.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hg.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ev.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wy.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://cj.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fc.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mz.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://be.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://cs.shxzukj.cn

[E07] 按分隔符拆分
来源：http://be.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://li.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ur.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://di.hnjuh.cn

TS:   s.split(",")
来源：http://yj.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jf.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://an.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://oq.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tb.newstarts.cn

[E08] 数组按分隔符合并
来源：http://xh.huanxung.cn

Py:   ",".join(items)
来源：http://uw.huanxung.cn

PHP:  implode(",", $items);
来源：http://cj.huanxung.cn

JS:   items.join(",")
来源：http://ie.gzmigu.cn

TS:   items.join(",")
来源：http://xy.521024.cn

Java: String.join(",", items)
来源：http://dg.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://dg.asd995.cn

Ruby: items.join(",")
来源：http://qg.gzmigu.cn

C#:   string.Join(",", items)
来源：http://xt.9csxet.cn

[E09] 去除所有空白字符
来源：http://fa.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ec.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mk.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://rs.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://tw.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://kx.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sz.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kv.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://og.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://yo.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ha.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tb.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://zl.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://rv.szsharing.cn

Java: String.format("%03d", 7)
来源：http://yj.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tc.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qe.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://en.huanxung.cn

[E11] 反转字符串
来源：http://vu.gzmigu.cn

Py:   s[::-1]
来源：http://nq.hahajie.cn

PHP:  strrev($s);
来源：http://gc.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://us.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://aa.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sa.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ja.521024.cn

Ruby: s.reverse
来源：http://na.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xx.newstarts.cn

[E12] 统计某字符出现次数
来源：http://hx.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ad.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ck.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://su.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://ep.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xx.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://kp.hnjuh.cn

Ruby: s.count("a")
来源：http://ah.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://wd.szsharing.cn

[E13] 逐字符遍历
来源：http://cl.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://jb.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kj.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nv.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dy.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://il.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zu.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gd.huixiangedu.cn


<!-- 参考信息 -->