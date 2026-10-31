代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xz.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ut.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lb.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zk.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mj.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lr.chemitech.net.cn

[D05] 访问与修改元素
来源：http://mw.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dz.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kb.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hv.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://lo.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://jv.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://sm.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uk.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yy.yuexingan06.cn

[D06] 数组长度
来源：http://uq.bjjhwx.cn

Py:   len(arr)
来源：http://gu.shxzukj.cn

PHP:  count($arr);
来源：http://po.shxzukj.cn

JS:   arr.length
来源：http://qg.chemitech.net.cn

TS:   arr.length
来源：http://lz.jianghongdianzi.cn

Java: list.size();
来源：http://me.huanxung.cn

Go:   len(arr)
来源：http://ex.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://sg.wgjwhj.cn

C#:   list.Count;
来源：http://qq.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://he.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zp.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tu.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ty.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://xl.shxzskj.cn

Java: list.subList(1, 4);
来源：http://fa.hahajie.cn

Go:   arr[1:4]
来源：http://zr.9csxet.cn

Ruby: arr[1, 3]
来源：http://te.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://vh.hnjuh.cn

[D08] 合并两个数组
来源：http://tb.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://vt.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://su.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ne.9csxet.cn

TS:   [...a, ...b];
来源：http://hq.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ge.9csxet.cn

Go:   append(a, b...)
来源：http://zv.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ca.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ti.chemitech.net.cn

[D09] 排序（升序）
来源：http://ap.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://od.wgjwhj.cn

PHP:  sort($arr);
来源：http://zy.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ry.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zg.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xq.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://an.jctech888.com.cn

Ruby: arr.sort
来源：http://wj.huixinmuqiang.cn

C#:   list.Sort();
来源：http://re.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ed.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ta.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://to.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jt.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lj.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cr.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gj.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aq.szsharing.cn

[D11] 反转数组
来源：http://um.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zj.nicolike.cn

PHP:  array_reverse($arr);
来源：http://sm.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gb.huanxung.cn

TS:   [...arr].reverse();
来源：http://bp.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://ow.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://nk.gzmigu.cn

Ruby: arr.reverse
来源：http://ge.nszjky.cn

C#:   list.Reverse();
来源：http://ro.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://if.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://rn.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bj.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cn.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qw.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zo.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://ic.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://td.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://jf.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://wu.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zu.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xp.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://oi.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://vv.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hw.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rz.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pn.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fc.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://yi.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yu.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zw.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://us.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://sf.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sw.muxihuayi.cn

Go:   // 手写循环
来源：http://lt.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yb.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ku.szsharing.cn

[D15] 去重
来源：http://cz.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kb.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ak.asd995.cn

JS:   [...new Set(arr)]
来源：http://en.colortex.cn

TS:   [...new Set(arr)]
来源：http://zf.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zs.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hq.9csxet.cn

Ruby: arr.uniq
来源：http://sj.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://fw.huanxung.cn

[D16] 求和与平均值
来源：http://qg.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ar.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pk.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wx.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://up.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gz.newstarts.cn

Go:   // 手写循环累加
来源：http://ex.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ls.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://qr.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://gn.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://pa.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://zg.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gd.hahajie.cn

TS:   Math.max(...arr);
来源：http://it.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ow.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vw.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://bx.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://yr.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://fs.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xv.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://fn.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ss.huanxung.cn

TS:   nested.flat();
来源：http://fs.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ze.yuexingan06.cn

Go:   // 手写双层循环
来源：http://ue.hnjuh.cn

Ruby: nested.flatten
来源：http://xr.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ba.9csxet.cn

[D19] 按字段分组
来源：http://tg.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tf.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vg.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xx.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://un.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://th.asd995.cn

Go:   // 手写 map[string][]T
来源：http://mq.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xu.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bt.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://dz.szsharing.cn

Py:   Counter(arr)
来源：http://gu.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ov.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sn.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jl.huanxung.cn

Go:   // 手写 map[T]int
来源：http://xj.nszjky.cn

Ruby: arr.tally
来源：http://rw.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aw.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://er.9csxet.cn

Py:   x in arr
来源：http://yy.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://vz.newstarts.cn

JS:   arr.includes(x)
来源：http://po.chemitech.net.cn

TS:   arr.includes(x)
来源：http://dx.yuexingan06.cn

Java: list.contains(x)
来源：http://si.521024.cn

Go:   slices.Contains(arr, x)
来源：http://wi.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://xn.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://ji.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://qy.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ad.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wc.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sy.9csxet.cn

TS:   [...arr];
来源：http://er.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://wn.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pd.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://vg.colortex.cn

C#:   new List<int>(list);
来源：http://av.newstarts.cn

[D23] reduce 累积计算
来源：http://un.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vi.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fs.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kt.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tw.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lt.yuexingan06.cn

Go:   // 手写循环
来源：http://qj.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xb.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kw.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://mk.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uc.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zc.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lj.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gi.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ll.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hy.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://et.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://db.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://pk.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ih.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jz.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ys.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gt.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eu.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tn.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gx.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fy.szxytkj.cn

[D26] 数组转字符串
来源：http://po.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://zh.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://rn.nszjky.cn

JS:   arr.join(", ")
来源：http://vd.szxytkj.cn

TS:   arr.join(", ")
来源：http://mo.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://zq.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://eb.nszjky.cn

Ruby: arr.join(", ")
来源：http://sn.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://uq.nszjky.cn

================================================================================
来源：http://ap.gzmigu.cn

E. 字符串处理
来源：http://yy.yuntaijiaju.cn

================================================================================
来源：http://sy.huixiangedu.cn

[E01] 拼接字符串
来源：http://lh.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pz.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://di.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://er.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oh.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yo.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fu.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uj.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xy.yuntaijiaju.cn

[E02] 重复字符串
来源：http://yk.nicolike.cn

Py:   "ab" * 3
来源：http://mk.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://be.szsharing.cn

JS:   "ab".repeat(3)
来源：http://dy.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://fo.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ha.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://ur.haigaiapp.cn

Ruby: "ab" * 3
来源：http://so.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ez.haigaiapp.cn

[E03] 截取子串
来源：http://sy.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ih.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qa.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ks.9csxet.cn

TS:   s.slice(1, 4)
来源：http://qk.panjiajie.cn

Java: s.substring(1, 4)
来源：http://xb.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ye.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qq.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ph.shxzskj.cn

[E04] 查找子串位置
来源：http://bn.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://tz.nicolike.cn

PHP:  strpos($s, "x");
来源：http://jg.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nk.shxzukj.cn

TS:   s.indexOf("x")
来源：http://fs.jctech888.com.cn

Java: s.indexOf("x")
来源：http://dj.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://eh.nicolike.cn

Ruby: s.index("x")
来源：http://jn.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://kc.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vs.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://un.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fw.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fn.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rt.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ij.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vx.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lq.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fh.shxzukj.cn

[E06] 替换子串
来源：http://kf.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://if.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://iy.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eb.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ow.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ob.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cp.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fb.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://yq.nszjky.cn

[E07] 按分隔符拆分
来源：http://vk.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jx.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bu.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://da.huixiangedu.cn

TS:   s.split(",")
来源：http://lg.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://es.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hm.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://xo.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cc.newstarts.cn

[E08] 数组按分隔符合并
来源：http://bp.muxihuayi.cn

Py:   ",".join(items)
来源：http://rz.huanxung.cn

PHP:  implode(",", $items);
来源：http://ms.haigaiapp.cn

JS:   items.join(",")
来源：http://sr.hahajie.cn

TS:   items.join(",")
来源：http://yx.huanxung.cn

Java: String.join(",", items)
来源：http://kw.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://cb.szsharing.cn

Ruby: items.join(",")
来源：http://ig.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://ff.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://jh.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qx.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://de.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://og.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://cb.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://bj.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uw.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lh.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bp.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://bt.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fz.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ik.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://in.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ch.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://dm.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qt.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ss.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ix.shtwfgs.cn

[E11] 反转字符串
来源：http://hu.shxzukj.cn

Py:   s[::-1]
来源：http://ue.haigaiapp.cn

PHP:  strrev($s);
来源：http://nr.asd995.cn


<!-- 参考信息 -->