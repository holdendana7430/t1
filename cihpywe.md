代发 wailian999

Java: list.add(4);
来源：http://rf.colortex.cn

Go:   arr = append(arr, 4)
来源：http://eo.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://ym.huanxung.cn

C#:   list.Add(4);
来源：http://zh.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://su.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://ma.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nw.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ih.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://rr.nicolike.cn

Java: list.add(0, 0);
来源：http://ap.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wo.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kx.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://xc.colortex.cn

[D04] 删除元素
来源：http://sn.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sc.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ed.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jp.colortex.cn

TS:   arr.splice(0, 1);
来源：http://sz.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ey.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wu.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ya.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ck.muxihuayi.cn

[D05] 访问与修改元素
来源：http://sy.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wi.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yi.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ky.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://fj.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://na.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://hr.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wo.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nw.hnjuh.cn

[D06] 数组长度
来源：http://bj.wgjwhj.cn

Py:   len(arr)
来源：http://bl.521024.cn

PHP:  count($arr);
来源：http://xr.szsharing.cn

JS:   arr.length
来源：http://fs.huixinmuqiang.cn

TS:   arr.length
来源：http://pt.huixinmuqiang.cn

Java: list.size();
来源：http://od.yuexingan06.cn

Go:   len(arr)
来源：http://zr.colortex.cn

Ruby: arr.length; arr.size
来源：http://nh.colortex.cn

C#:   list.Count;
来源：http://na.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://fn.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rr.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wj.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://xg.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://mc.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://lz.bjjhwx.cn

Go:   arr[1:4]
来源：http://iu.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ux.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ig.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://pm.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://lj.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://qv.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sb.newstarts.cn

TS:   [...a, ...b];
来源：http://aq.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://au.hahajie.cn

Go:   append(a, b...)
来源：http://lj.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://bg.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ze.lnxyls.cn

[D09] 排序（升序）
来源：http://mx.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://ny.hahajie.cn

PHP:  sort($arr);
来源：http://ly.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kh.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bo.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://li.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ju.bjjhwx.cn

Ruby: arr.sort
来源：http://rg.wgjwhj.cn

C#:   list.Sort();
来源：http://wf.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ps.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kj.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ax.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wx.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://et.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://np.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ac.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ma.huixiangedu.cn

[D11] 反转数组
来源：http://kd.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ty.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://td.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wa.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://ym.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://wz.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://oi.chemitech.net.cn

Ruby: arr.reverse
来源：http://ji.nicolike.cn

C#:   list.Reverse();
来源：http://lo.lnxyls.cn

[D12] 查找元素下标
来源：http://wu.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://fm.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qo.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qy.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sl.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://br.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://iv.newstarts.cn

Ruby: arr.index(x)
来源：http://wt.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://cm.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://bo.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wc.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lo.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://xp.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://jq.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uo.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ae.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vx.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pd.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://lg.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ri.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xp.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ga.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://vn.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sa.shxzukj.cn

Go:   // 手写循环
来源：http://kq.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ms.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eu.hnjuh.cn

[D15] 去重
来源：http://fq.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cz.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://lq.521024.cn

JS:   [...new Set(arr)]
来源：http://qw.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://bz.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pf.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jh.lnxyls.cn

Ruby: arr.uniq
来源：http://ce.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ro.panjiajie.cn

[D16] 求和与平均值
来源：http://my.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qj.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ts.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lv.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://af.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tf.szsharing.cn

Go:   // 手写循环累加
来源：http://fy.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rd.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://do.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://sy.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://wz.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://fh.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jp.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://mp.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ep.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://os.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://sz.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://ji.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://mx.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mz.asd995.cn

PHP:  array_merge(...$nested);
来源：http://lv.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vy.9csxet.cn

TS:   nested.flat();
来源：http://gg.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xe.gzmigu.cn

Go:   // 手写双层循环
来源：http://dh.9csxet.cn

Ruby: nested.flatten
来源：http://ru.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bu.bjjhwx.cn

[D19] 按字段分组
来源：http://ld.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rt.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bh.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://af.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lv.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hq.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ii.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ij.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wf.asd995.cn

[D20] 统计每个元素出现次数
来源：http://vm.huixiangedu.cn

Py:   Counter(arr)
来源：http://kz.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://nt.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vz.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nm.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hy.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ni.shxzukj.cn

Ruby: arr.tally
来源：http://wt.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dc.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://go.szsharing.cn

Py:   x in arr
来源：http://gd.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://va.nszjky.cn

JS:   arr.includes(x)
来源：http://cw.hnjuh.cn

TS:   arr.includes(x)
来源：http://fn.lnxyls.cn

Java: list.contains(x)
来源：http://yg.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://tw.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://lp.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://xu.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://dv.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ec.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wy.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dd.jianghongdianzi.cn

TS:   [...arr];
来源：http://ku.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://qm.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ip.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://tf.szxytkj.cn

C#:   new List<int>(list);
来源：http://rg.huixiangedu.cn

[D23] reduce 累积计算
来源：http://bb.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mx.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bh.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mo.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hk.jctech888.com.cn

Go:   // 手写循环
来源：http://za.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oi.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cn.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://jr.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bi.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fu.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sm.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mw.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kh.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ab.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sa.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nu.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://np.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ou.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ya.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rh.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ek.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ti.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bn.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eq.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lh.huixiangedu.cn

[D26] 数组转字符串
来源：http://nk.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://hp.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://pt.9csxet.cn

JS:   arr.join(", ")
来源：http://uk.shxzukj.cn

TS:   arr.join(", ")
来源：http://ml.asd995.cn

Java: String.join(", ", list)
来源：http://hz.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://by.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://jv.asd995.cn

C#:   string.Join(", ", list)
来源：http://le.521024.cn

================================================================================
来源：http://cb.jianghongdianzi.cn

E. 字符串处理
来源：http://dv.colortex.cn

================================================================================
来源：http://mj.nszjky.cn

[E01] 拼接字符串
来源：http://cj.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://me.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oy.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pz.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://am.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mw.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jd.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pt.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sj.9csxet.cn

[E02] 重复字符串
来源：http://ai.asd995.cn

Py:   "ab" * 3
来源：http://sx.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ie.asd995.cn

JS:   "ab".repeat(3)
来源：http://sr.szsharing.cn

TS:   "ab".repeat(3)
来源：http://if.lnxyls.cn

Java: "ab".repeat(3)
来源：http://zp.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://mt.szsharing.cn

Ruby: "ab" * 3
来源：http://kf.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://if.521024.cn

[E03] 截取子串
来源：http://vm.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hd.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rr.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zl.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://yx.lnxyls.cn

Java: s.substring(1, 4)
来源：http://se.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ir.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ps.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://yx.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://uc.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://cu.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://yl.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dc.szxytkj.cn

TS:   s.indexOf("x")
来源：http://gb.asd995.cn

Java: s.indexOf("x")
来源：http://xv.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://sa.bookmarksfly.cn

Ruby: s.index("x")
来源：http://in.9csxet.cn

C#:   s.IndexOf("x")
来源：http://sl.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fu.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vx.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dn.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bi.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yi.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bq.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mo.huixinmuqiang.cn

[E06] 替换子串
来源：http://sc.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pn.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://sc.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://zs.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://io.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://js.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lv.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://eo.hahajie.cn

[E07] 按分隔符拆分
来源：http://fl.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iq.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zf.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iy.9csxet.cn

TS:   s.split(",")
来源：http://go.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hj.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jl.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://lg.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://os.huanxung.cn

[E08] 数组按分隔符合并
来源：http://dt.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://yb.shxzskj.cn

PHP:  implode(",", $items);
来源：http://zc.9csxet.cn

JS:   items.join(",")
来源：http://lo.szxytkj.cn

TS:   items.join(",")
来源：http://qg.jctech888.com.cn

Java: String.join(",", items)
来源：http://wt.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://gu.hahajie.cn

Ruby: items.join(",")
来源：http://lq.9csxet.cn

C#:   string.Join(",", items)
来源：http://mb.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ve.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ex.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sf.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://ur.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://uu.colortex.cn


<!-- 参考信息 -->