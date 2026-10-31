代发 wailian999

[D03] 在指定位置插入元素
来源：http://be.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://km.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ty.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fx.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://gg.nszjky.cn

Java: list.add(0, 0);
来源：http://zc.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eo.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xm.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://kj.chemitech.net.cn

[D04] 删除元素
来源：http://uw.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jf.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eo.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gl.521024.cn

TS:   arr.splice(0, 1);
来源：http://hn.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yc.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qa.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oh.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aj.shxzskj.cn

[D05] 访问与修改元素
来源：http://kf.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hi.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hc.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ul.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://gd.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://fm.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ps.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gr.haigaiapp.cn

[D06] 数组长度
来源：http://fn.colortex.cn

Py:   len(arr)
来源：http://li.hahajie.cn

PHP:  count($arr);
来源：http://fr.chemitech.net.cn

JS:   arr.length
来源：http://la.huanxung.cn

TS:   arr.length
来源：http://jb.shxzukj.cn

Java: list.size();
来源：http://dg.szsharing.cn

Go:   len(arr)
来源：http://xi.newstarts.cn

Ruby: arr.length; arr.size
来源：http://fx.colortex.cn

C#:   list.Count;
来源：http://md.521024.cn

[D07] 切片 / 取子数组
来源：http://vb.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yp.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://li.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://yw.colortex.cn

TS:   arr.slice(1, 4);
来源：http://mb.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ua.newstarts.cn

Go:   arr[1:4]
来源：http://hj.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://mi.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://wa.hahajie.cn

[D08] 合并两个数组
来源：http://ji.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://ps.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://kt.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hw.521024.cn

TS:   [...a, ...b];
来源：http://ab.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ze.521024.cn

Go:   append(a, b...)
来源：http://xj.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://rw.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://jk.521024.cn

[D09] 排序（升序）
来源：http://cw.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://lh.asd995.cn

PHP:  sort($arr);
来源：http://ay.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fg.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ln.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://es.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tq.yuntaijiaju.cn

Ruby: arr.sort
来源：http://mh.muxihuayi.cn

C#:   list.Sort();
来源：http://vm.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uy.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lt.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cd.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vl.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wt.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oj.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ab.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xn.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gu.nicolike.cn

[D11] 反转数组
来源：http://il.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iw.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://bn.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mh.hnjuh.cn

TS:   [...arr].reverse();
来源：http://dw.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://tk.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://fn.bookmarksfly.cn

Ruby: arr.reverse
来源：http://da.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://ey.panjiajie.cn

[D12] 查找元素下标
来源：http://mt.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://qu.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yk.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lq.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qb.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cz.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://yj.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://px.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://aw.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ct.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uk.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fz.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://yz.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://rg.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cq.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jc.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yv.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kf.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://ac.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://en.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wh.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://kz.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://kk.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rc.shtwfgs.cn

Go:   // 手写循环
来源：http://fo.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zj.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.nszjky.cn

[D15] 去重
来源：http://xm.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qw.nszjky.cn

PHP:  array_unique($arr);
来源：http://xv.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://gp.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://ln.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ty.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fj.hnjuh.cn

Ruby: arr.uniq
来源：http://sd.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://hs.colortex.cn

[D16] 求和与平均值
来源：http://tz.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://an.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qh.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xz.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gq.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vk.panjiajie.cn

Go:   // 手写循环累加
来源：http://po.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://er.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://qp.hahajie.cn

[D17] 最大值与最小值
来源：http://um.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://dj.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ql.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dh.huanxung.cn

TS:   Math.max(...arr);
来源：http://qf.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://it.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://or.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://xv.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://sl.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ch.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rb.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://qq.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bv.hahajie.cn

TS:   nested.flat();
来源：http://bs.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wp.jctech888.com.cn

Go:   // 手写双层循环
来源：http://dk.panjiajie.cn

Ruby: nested.flatten
来源：http://ss.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://la.wgjwhj.cn

[D19] 按字段分组
来源：http://eo.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fj.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kw.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ob.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jr.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kc.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://bf.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ad.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nn.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ak.hahajie.cn

Py:   Counter(arr)
来源：http://xa.nszjky.cn

PHP:  array_count_values($arr);
来源：http://kw.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://px.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kn.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://wc.shxzukj.cn

Ruby: arr.tally
来源：http://iu.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iw.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://nh.jctech888.com.cn

Py:   x in arr
来源：http://av.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://nb.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://ua.colortex.cn

TS:   arr.includes(x)
来源：http://vx.nicolike.cn

Java: list.contains(x)
来源：http://vk.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://ds.szxytkj.cn

Ruby: arr.include?(x)
来源：http://fh.hahajie.cn

C#:   list.Contains(x)
来源：http://rz.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://dz.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uz.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iq.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pm.gzmigu.cn

TS:   [...arr];
来源：http://hn.asd995.cn

Java: new ArrayList<>(list);
来源：http://uu.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dt.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://fq.szsharing.cn

C#:   new List<int>(list);
来源：http://fm.shxzskj.cn

[D23] reduce 累积计算
来源：http://la.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sl.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ux.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ye.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ae.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ir.jctech888.com.cn

Go:   // 手写循环
来源：http://sl.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cq.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://js.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ia.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xr.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hn.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://am.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gp.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ny.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pq.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ey.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dk.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://oj.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jd.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lq.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cd.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ca.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zy.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jo.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ge.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yl.haigaiapp.cn

[D26] 数组转字符串
来源：http://hv.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ka.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://zz.panjiajie.cn

JS:   arr.join(", ")
来源：http://kn.bjjhwx.cn

TS:   arr.join(", ")
来源：http://mf.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://xw.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://su.9csxet.cn

Ruby: arr.join(", ")
来源：http://is.521024.cn

C#:   string.Join(", ", list)
来源：http://um.9csxet.cn

================================================================================
来源：http://xo.hahajie.cn

E. 字符串处理
来源：http://dt.huixinmuqiang.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://gk.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sj.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vg.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ir.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dj.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uo.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wl.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mx.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fs.panjiajie.cn

[E02] 重复字符串
来源：http://hx.bookmarksfly.cn

Py:   "ab" * 3
来源：http://gv.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://or.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ve.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://hx.szsharing.cn

Java: "ab".repeat(3)
来源：http://un.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://aa.hahajie.cn

Ruby: "ab" * 3
来源：http://ed.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bb.jctech888.com.cn

[E03] 截取子串
来源：http://up.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mf.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rh.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://th.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://xu.nszjky.cn

Java: s.substring(1, 4)
来源：http://jo.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mt.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ty.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ra.szsharing.cn

[E04] 查找子串位置
来源：http://qf.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://lw.asd995.cn

PHP:  strpos($s, "x");
来源：http://ug.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ri.nicolike.cn

TS:   s.indexOf("x")
来源：http://em.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://vp.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://xz.huanxung.cn

Ruby: s.index("x")
来源：http://wz.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://ey.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qy.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wf.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xz.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gu.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tr.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sm.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xu.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vu.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://md.szxytkj.cn

[E06] 替换子串
来源：http://gv.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ck.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://bv.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://tj.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aw.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lp.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ti.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://zg.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ns.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cd.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qh.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ma.huixiangedu.cn

TS:   s.split(",")
来源：http://ea.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sh.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jx.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://jx.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sb.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://fz.521024.cn

Py:   ",".join(items)
来源：http://hr.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://pd.gzmigu.cn

JS:   items.join(",")
来源：http://ra.newstarts.cn

TS:   items.join(",")
来源：http://ol.panjiajie.cn

Java: String.join(",", items)
来源：http://pb.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ug.nicolike.cn

Ruby: items.join(",")
来源：http://ig.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://zw.szxytkj.cn

[E09] 去除所有空白字符
来源：http://mw.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kp.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mc.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://wj.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://qc.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ct.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gl.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qz.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://in.nicolike.cn


<!-- 参考信息 -->