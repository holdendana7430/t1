代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rq.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ff.panjiajie.cn

JS:   arr.push(4);
来源：http://sl.shxzukj.cn

TS:   arr.push(4);
来源：http://ze.shxzskj.cn

Java: list.add(4);
来源：http://tt.521024.cn

Go:   arr = append(arr, 4)
来源：http://fp.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://ov.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://qn.huanxung.cn

[D03] 在指定位置插入元素
来源：http://aq.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://sm.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oh.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fr.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://oc.9csxet.cn

Java: list.add(0, 0);
来源：http://uf.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://el.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://in.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://yg.lnxyls.cn

[D04] 删除元素
来源：http://xq.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ui.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eq.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pc.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ny.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ct.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rg.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sa.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xq.haigaiapp.cn

[D05] 访问与修改元素
来源：http://di.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kw.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ip.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ex.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://lk.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://uk.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://kj.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://za.shxzskj.cn

[D06] 数组长度
来源：http://ld.bjjhwx.cn

Py:   len(arr)
来源：http://lk.yuntaijiaju.cn

PHP:  count($arr);
来源：http://ji.chemitech.net.cn

JS:   arr.length
来源：http://oq.shtwfgs.cn

TS:   arr.length
来源：http://wp.yuntaijiaju.cn

Java: list.size();
来源：http://qv.muxihuayi.cn

Go:   len(arr)
来源：http://pm.nszjky.cn

Ruby: arr.length; arr.size
来源：http://ot.jianghongdianzi.cn

C#:   list.Count;
来源：http://mo.nszjky.cn

[D07] 切片 / 取子数组
来源：http://yn.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ur.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yv.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://oa.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://xu.panjiajie.cn

Java: list.subList(1, 4);
来源：http://bd.colortex.cn

Go:   arr[1:4]
来源：http://ld.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://vy.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://fu.nicolike.cn

[D08] 合并两个数组
来源：http://cl.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://ps.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://qb.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ie.asd995.cn

TS:   [...a, ...b];
来源：http://pa.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cj.huixiangedu.cn

Go:   append(a, b...)
来源：http://vw.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://oy.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://qh.chemitech.net.cn

[D09] 排序（升序）
来源：http://bt.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vn.nszjky.cn

PHP:  sort($arr);
来源：http://vd.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://az.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kw.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ut.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ap.asd995.cn

Ruby: arr.sort
来源：http://ry.huixinmuqiang.cn

C#:   list.Sort();
来源：http://rt.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lh.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pm.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://az.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xd.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://av.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bd.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mx.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bs.haigaiapp.cn

[D11] 反转数组
来源：http://ci.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zk.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://mc.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kn.hahajie.cn

TS:   [...arr].reverse();
来源：http://rb.asd995.cn

Java: Collections.reverse(list);
来源：http://ng.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://fq.yuexingan06.cn

Ruby: arr.reverse
来源：http://xa.yuexingan06.cn

C#:   list.Reverse();
来源：http://yb.shxzskj.cn

[D12] 查找元素下标
来源：http://ni.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://vw.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://av.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uu.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wh.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://op.asd995.cn

Go:   slices.Index(arr, x)
来源：http://gh.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://gu.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://lu.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://kk.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bc.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hk.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://cw.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://ik.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fz.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xk.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fo.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://yv.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://en.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://hw.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://no.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ps.huanxung.cn

Go:   // 手写循环
来源：http://hy.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sy.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hu.bookmarksfly.cn

[D15] 去重
来源：http://da.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sx.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://ft.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://rm.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://fz.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dl.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sb.bjjhwx.cn

Ruby: arr.uniq
来源：http://rd.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://nf.szsharing.cn

[D16] 求和与平均值
来源：http://db.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uk.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ru.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xv.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fl.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jq.hahajie.cn

Go:   // 手写循环累加
来源：http://py.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ed.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://dl.huanxung.cn

[D17] 最大值与最小值
来源：http://tx.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://du.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://xf.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tb.panjiajie.cn

TS:   Math.max(...arr);
来源：http://pz.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://da.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ug.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://zb.colortex.cn

C#:   list.Max();  list.Min()
来源：http://xv.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ss.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ny.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://sz.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zj.shxzskj.cn

TS:   nested.flat();
来源：http://hk.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ay.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ta.asd995.cn

Ruby: nested.flatten
来源：http://rb.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oh.gzmigu.cn

[D19] 按字段分组
来源：http://ha.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://em.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uy.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ac.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rd.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zw.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://kh.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mw.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yd.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://tk.colortex.cn

Py:   Counter(arr)
来源：http://sj.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://hs.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pz.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mr.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wq.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://ba.panjiajie.cn

Ruby: arr.tally
来源：http://mi.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tc.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://hr.gzmigu.cn

Py:   x in arr
来源：http://pa.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://wm.yuexingan06.cn

JS:   arr.includes(x)
来源：http://mm.gzmigu.cn

TS:   arr.includes(x)
来源：http://cu.bookmarksfly.cn

Java: list.contains(x)
来源：http://at.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://xm.szsharing.cn

Ruby: arr.include?(x)
来源：http://fm.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ky.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://vl.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lh.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://te.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gp.521024.cn

TS:   [...arr];
来源：http://wg.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://vj.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dl.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://fp.nicolike.cn

[D23] reduce 累积计算
来源：http://bt.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yp.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fl.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yb.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dc.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tf.jctech888.com.cn

Go:   // 手写循环
来源：http://pb.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xu.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://se.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://md.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aw.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ui.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ll.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sk.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://af.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fy.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://by.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dp.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://nb.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ub.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://my.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eb.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mn.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cn.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xf.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bx.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mn.hnjuh.cn

[D26] 数组转字符串
来源：http://aq.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://mr.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://lw.panjiajie.cn

JS:   arr.join(", ")
来源：http://xq.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://vc.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://hc.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://gc.huanxung.cn

Ruby: arr.join(", ")
来源：http://kc.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://kp.9csxet.cn

================================================================================
来源：http://jk.jianghongdianzi.cn

E. 字符串处理
来源：http://hr.jctech888.com.cn

================================================================================
来源：http://yk.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://eg.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jh.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yc.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tr.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lr.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rp.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yk.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zl.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://da.bjjhwx.cn

[E02] 重复字符串
来源：http://wg.asd995.cn

Py:   "ab" * 3
来源：http://ju.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://wj.szsharing.cn

JS:   "ab".repeat(3)
来源：http://gr.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://fd.nicolike.cn

Java: "ab".repeat(3)
来源：http://us.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://iz.yuexingan06.cn

Ruby: "ab" * 3
来源：http://wm.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eb.panjiajie.cn

[E03] 截取子串
来源：http://zt.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pp.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wc.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zr.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://zv.521024.cn

Java: s.substring(1, 4)
来源：http://ry.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lp.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ec.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://zo.hnjuh.cn

[E04] 查找子串位置
来源：http://mz.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://pq.colortex.cn

PHP:  strpos($s, "x");
来源：http://hc.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vg.521024.cn

TS:   s.indexOf("x")
来源：http://jf.yuexingan06.cn

Java: s.indexOf("x")
来源：http://vs.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://fz.lnxyls.cn

Ruby: s.index("x")
来源：http://rx.521024.cn

C#:   s.IndexOf("x")
来源：http://th.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qe.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ti.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xd.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ws.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wb.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wh.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bt.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yy.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ur.huanxung.cn

[E06] 替换子串
来源：http://di.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xv.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://eg.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vl.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://pg.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fu.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vv.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fe.521024.cn

C#:   s.Replace("a", "b")
来源：http://ix.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://ko.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bw.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://it.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yh.huixiangedu.cn

TS:   s.split(",")
来源：http://pm.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cj.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qy.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://xr.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xs.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://kx.gzmigu.cn

Py:   ",".join(items)
来源：http://nm.nicolike.cn

PHP:  implode(",", $items);
来源：http://xu.panjiajie.cn

JS:   items.join(",")
来源：http://ru.jctech888.com.cn

TS:   items.join(",")
来源：http://fz.shxzskj.cn

Java: String.join(",", items)
来源：http://ny.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://oa.muxihuayi.cn

Ruby: items.join(",")
来源：http://ec.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://ws.gzmigu.cn

[E09] 去除所有空白字符
来源：http://ew.colortex.cn


<!-- 参考信息 -->