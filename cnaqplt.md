代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mk.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://af.nicolike.cn

JS:   arr.push(4);
来源：http://ws.shxzskj.cn

TS:   arr.push(4);
来源：http://ky.hnjuh.cn

Java: list.add(4);
来源：http://vi.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://af.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://rr.panjiajie.cn

C#:   list.Add(4);
来源：http://ef.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://og.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://lh.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pn.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bu.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zt.huanxung.cn

Java: list.add(0, 0);
来源：http://as.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wu.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ft.colortex.cn

C#:   list.Insert(0, 0);
来源：http://nv.huixinmuqiang.cn

[D04] 删除元素
来源：http://st.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xe.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lx.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ac.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://gt.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zp.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xp.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sz.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ac.shxzskj.cn

[D05] 访问与修改元素
来源：http://hp.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pl.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ci.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xp.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://xv.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://mi.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://da.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yp.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lz.jianghongdianzi.cn

[D06] 数组长度
来源：http://qp.newstarts.cn

Py:   len(arr)
来源：http://yp.shxzukj.cn

PHP:  count($arr);
来源：http://ic.shtwfgs.cn

JS:   arr.length
来源：http://om.newstarts.cn

TS:   arr.length
来源：http://dq.shxzskj.cn

Java: list.size();
来源：http://eh.wgjwhj.cn

Go:   len(arr)
来源：http://sz.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://jr.colortex.cn

C#:   list.Count;
来源：http://qk.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://tn.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hr.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bv.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://tb.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://hu.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://uc.yuexingan06.cn

Go:   arr[1:4]
来源：http://aq.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://hm.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ih.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ik.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://vd.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ob.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kd.shxzukj.cn

TS:   [...a, ...b];
来源：http://jq.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hs.colortex.cn

Go:   append(a, b...)
来源：http://oq.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://nh.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://es.panjiajie.cn

[D09] 排序（升序）
来源：http://ef.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://by.521024.cn

PHP:  sort($arr);
来源：http://jg.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gg.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ve.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aa.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jw.nicolike.cn

Ruby: arr.sort
来源：http://no.szxytkj.cn

C#:   list.Sort();
来源：http://at.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ed.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ym.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ng.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ez.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ix.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hn.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://va.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ct.haigaiapp.cn

[D11] 反转数组
来源：http://ch.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://az.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://lh.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ea.huanxung.cn

TS:   [...arr].reverse();
来源：http://ul.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://fv.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://pu.panjiajie.cn

Ruby: arr.reverse
来源：http://eg.gzmigu.cn

C#:   list.Reverse();
来源：http://wk.asd995.cn

[D12] 查找元素下标
来源：http://bp.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://dv.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mo.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hs.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fe.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ag.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://rr.wgjwhj.cn

Ruby: arr.index(x)
来源：http://re.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://zl.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://xy.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hy.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dq.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://yd.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://dl.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gd.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fv.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zv.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pp.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://uo.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yv.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kn.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://ag.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ou.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tk.asd995.cn

Go:   // 手写循环
来源：http://vu.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jg.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lc.huanxung.cn

[D15] 去重
来源：http://et.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bx.colortex.cn

PHP:  array_unique($arr);
来源：http://fs.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://jr.nszjky.cn

TS:   [...new Set(arr)]
来源：http://ip.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ps.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dj.jctech888.com.cn

Ruby: arr.uniq
来源：http://bc.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://mf.colortex.cn

[D16] 求和与平均值
来源：http://qw.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jg.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rz.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xz.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oc.hahajie.cn

Go:   // 手写循环累加
来源：http://dk.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://po.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://od.muxihuayi.cn

[D17] 最大值与最小值
来源：http://dq.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://xw.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://qb.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://we.gzmigu.cn

TS:   Math.max(...arr);
来源：http://vc.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bv.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lm.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://jv.colortex.cn

C#:   list.Max();  list.Min()
来源：http://ei.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://sn.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vl.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://mn.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zm.szxytkj.cn

TS:   nested.flat();
来源：http://ne.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cv.nicolike.cn

Go:   // 手写双层循环
来源：http://yn.panjiajie.cn

Ruby: nested.flatten
来源：http://xz.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eq.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ci.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hl.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nb.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hk.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xw.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nw.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://xw.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cz.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cg.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://mk.lnxyls.cn

Py:   Counter(arr)
来源：http://kb.nszjky.cn

PHP:  array_count_values($arr);
来源：http://eb.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fy.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pq.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://pt.newstarts.cn

Ruby: arr.tally
来源：http://lo.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vx.colortex.cn

[D21] 判断是否包含某元素
来源：http://jp.wgjwhj.cn

Py:   x in arr
来源：http://np.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://hq.szsharing.cn

JS:   arr.includes(x)
来源：http://tp.jctech888.com.cn

TS:   arr.includes(x)
来源：http://pn.bookmarksfly.cn

Java: list.contains(x)
来源：http://ic.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ow.huanxung.cn

Ruby: arr.include?(x)
来源：http://lc.nicolike.cn

C#:   list.Contains(x)
来源：http://kr.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://wj.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aa.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qj.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://al.9csxet.cn

TS:   [...arr];
来源：http://tj.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ep.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fk.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://bq.jctech888.com.cn

C#:   new List<int>(list);
来源：http://kb.9csxet.cn

[D23] reduce 累积计算
来源：http://ur.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rj.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ul.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://up.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mg.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jb.nicolike.cn

Go:   // 手写循环
来源：http://pp.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nv.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dd.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ul.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rs.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tw.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xc.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jy.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://km.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dd.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oq.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wc.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://rk.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dx.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dw.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://px.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qt.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://st.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sq.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://me.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gg.yuexingan06.cn

[D26] 数组转字符串
来源：http://pf.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://kr.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://rj.hnjuh.cn

JS:   arr.join(", ")
来源：http://il.szxytkj.cn

TS:   arr.join(", ")
来源：http://rv.shxzukj.cn

Java: String.join(", ", list)
来源：http://ij.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://yk.szsharing.cn

Ruby: arr.join(", ")
来源：http://mp.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://pl.nicolike.cn

================================================================================
来源：http://tx.newstarts.cn

E. 字符串处理
来源：http://eb.shxzukj.cn

================================================================================
来源：http://vv.jctech888.com.cn

[E01] 拼接字符串
来源：http://ye.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wa.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vf.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hj.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://go.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bq.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lp.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://if.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dw.9csxet.cn

[E02] 重复字符串
来源：http://zm.muxihuayi.cn

Py:   "ab" * 3
来源：http://xu.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://zm.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://pk.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://fc.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://aq.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://gv.panjiajie.cn

Ruby: "ab" * 3
来源：http://jp.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://so.jctech888.com.cn

[E03] 截取子串
来源：http://kp.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ck.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mt.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vv.colortex.cn

TS:   s.slice(1, 4)
来源：http://ou.hnjuh.cn

Java: s.substring(1, 4)
来源：http://ea.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mt.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sd.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://dr.wgjwhj.cn

[E04] 查找子串位置
来源：http://ny.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://jh.newstarts.cn

PHP:  strpos($s, "x");
来源：http://os.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kd.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://jt.huixiangedu.cn

Java: s.indexOf("x")
来源：http://su.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://ts.521024.cn

Ruby: s.index("x")
来源：http://qb.newstarts.cn

C#:   s.IndexOf("x")
来源：http://hf.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hd.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uf.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://be.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://we.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pt.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cp.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yo.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mc.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aw.asd995.cn

[E06] 替换子串
来源：http://fl.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wu.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ep.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://iy.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fj.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pv.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ze.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://db.panjiajie.cn

[E07] 按分隔符拆分
来源：http://ak.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sr.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nw.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sq.colortex.cn

TS:   s.split(",")
来源：http://bg.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rw.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fa.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://iv.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lx.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://nh.shxzukj.cn

Py:   ",".join(items)
来源：http://ms.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://nr.shxzskj.cn

JS:   items.join(",")
来源：http://oz.9csxet.cn

TS:   items.join(",")
来源：http://tw.huanxung.cn

Java: String.join(",", items)
来源：http://hf.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://ds.shtwfgs.cn

Ruby: items.join(",")
来源：http://bx.panjiajie.cn

C#:   string.Join(",", items)
来源：http://vt.szsharing.cn

[E09] 去除所有空白字符
来源：http://fn.newstarts.cn


<!-- 参考信息 -->