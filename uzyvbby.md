代发 wailian999

Java: list.add(4);
来源：http://jl.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://ls.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://fh.yuexingan06.cn

C#:   list.Add(4);
来源：http://gc.asd995.cn

[D03] 在指定位置插入元素
来源：http://uo.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://hi.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ea.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dc.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://pq.9csxet.cn

Java: list.add(0, 0);
来源：http://rx.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yd.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xj.colortex.cn

C#:   list.Insert(0, 0);
来源：http://zz.hahajie.cn

[D04] 删除元素
来源：http://vm.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kf.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hc.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ji.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ra.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mn.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dj.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wu.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ea.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://ev.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jc.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uw.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://db.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://lw.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://cw.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://nv.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zk.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sa.chemitech.net.cn

[D06] 数组长度
来源：http://ag.haigaiapp.cn

Py:   len(arr)
来源：http://yd.bookmarksfly.cn

PHP:  count($arr);
来源：http://he.huixinmuqiang.cn

JS:   arr.length
来源：http://us.newstarts.cn

TS:   arr.length
来源：http://xr.huanxung.cn

Java: list.size();
来源：http://my.muxihuayi.cn

Go:   len(arr)
来源：http://ds.newstarts.cn

Ruby: arr.length; arr.size
来源：http://sp.yuntaijiaju.cn

C#:   list.Count;
来源：http://vu.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://vk.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oz.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dh.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://sd.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://sv.newstarts.cn

Java: list.subList(1, 4);
来源：http://xq.asd995.cn

Go:   arr[1:4]
来源：http://gf.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ee.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://my.haigaiapp.cn

[D08] 合并两个数组
来源：http://yj.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ld.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://jg.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gl.haigaiapp.cn

TS:   [...a, ...b];
来源：http://mj.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vz.szxytkj.cn

Go:   append(a, b...)
来源：http://cm.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://hh.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://xk.asd995.cn

[D09] 排序（升序）
来源：http://ei.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://zu.bookmarksfly.cn

PHP:  sort($arr);
来源：http://qt.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jr.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cr.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lw.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uk.wgjwhj.cn

Ruby: arr.sort
来源：http://rm.huixinmuqiang.cn

C#:   list.Sort();
来源：http://tq.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uk.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ug.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uy.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dv.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qf.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lc.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zb.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kb.shxzskj.cn

[D11] 反转数组
来源：http://ed.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ok.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://lu.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jh.nszjky.cn

TS:   [...arr].reverse();
来源：http://gv.nicolike.cn

Java: Collections.reverse(list);
来源：http://by.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://fn.huanxung.cn

Ruby: arr.reverse
来源：http://rh.asd995.cn

C#:   list.Reverse();
来源：http://gw.bookmarksfly.cn

[D12] 查找元素下标
来源：http://tx.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://hd.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fz.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rh.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xk.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://su.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://oy.gzmigu.cn

Ruby: arr.index(x)
来源：http://fl.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://bz.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://jm.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sa.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ox.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://hu.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://if.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wk.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bt.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pw.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qb.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://af.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wl.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://je.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://op.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://bw.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pq.colortex.cn

Go:   // 手写循环
来源：http://wc.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mo.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cz.asd995.cn

[D15] 去重
来源：http://dq.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wf.shxzskj.cn

PHP:  array_unique($arr);
来源：http://gs.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xw.huanxung.cn

TS:   [...new Set(arr)]
来源：http://pn.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ry.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ry.muxihuayi.cn

Ruby: arr.uniq
来源：http://jr.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://bq.huixiangedu.cn

[D16] 求和与平均值
来源：http://zd.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pi.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pk.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yz.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fe.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qp.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://qg.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kv.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ey.shxzukj.cn

[D17] 最大值与最小值
来源：http://lw.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://bd.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://mz.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yf.panjiajie.cn

TS:   Math.max(...arr);
来源：http://hh.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xn.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cd.colortex.cn

Ruby: arr.max;  arr.min
来源：http://dw.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://dx.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://cf.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ku.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://tj.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ev.jctech888.com.cn

TS:   nested.flat();
来源：http://uf.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qg.newstarts.cn

Go:   // 手写双层循环
来源：http://hl.yuexingan06.cn

Ruby: nested.flatten
来源：http://ju.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yx.lnxyls.cn

[D19] 按字段分组
来源：http://tu.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ee.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kz.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rl.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hx.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ml.colortex.cn

Go:   // 手写 map[string][]T
来源：http://vx.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ya.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mf.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://gc.wgjwhj.cn

Py:   Counter(arr)
来源：http://jt.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ik.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mp.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ib.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bl.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://tr.521024.cn

Ruby: arr.tally
来源：http://pp.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xb.nicolike.cn

[D21] 判断是否包含某元素
来源：http://yp.bjjhwx.cn

Py:   x in arr
来源：http://wz.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://xb.muxihuayi.cn

JS:   arr.includes(x)
来源：http://vq.szsharing.cn

TS:   arr.includes(x)
来源：http://wm.shxzukj.cn

Java: list.contains(x)
来源：http://ju.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://bk.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://lp.bjjhwx.cn

C#:   list.Contains(x)
来源：http://cq.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://es.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ge.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mn.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iu.hnjuh.cn

TS:   [...arr];
来源：http://rp.asd995.cn

Java: new ArrayList<>(list);
来源：http://rd.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zb.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://am.hahajie.cn

C#:   new List<int>(list);
来源：http://lh.gzmigu.cn

[D23] reduce 累积计算
来源：http://eb.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ab.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://js.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://id.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jj.lnxyls.cn

Go:   // 手写循环
来源：http://lm.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bc.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qx.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://vh.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vw.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aq.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fa.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://es.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eg.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gi.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://re.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rh.colortex.cn

[D25] Set 集合去重与交并差
来源：http://qf.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ew.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zv.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ws.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fc.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xt.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ii.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yl.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://re.huanxung.cn

[D26] 数组转字符串
来源：http://eg.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://bx.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://vi.shxzukj.cn

JS:   arr.join(", ")
来源：http://yz.chemitech.net.cn

TS:   arr.join(", ")
来源：http://gm.hahajie.cn

Java: String.join(", ", list)
来源：http://je.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://yh.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://hn.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://cz.newstarts.cn

================================================================================
来源：http://dy.newstarts.cn

E. 字符串处理
来源：http://pn.nszjky.cn

================================================================================
来源：http://ji.colortex.cn

[E01] 拼接字符串
来源：http://vy.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bl.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cz.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eh.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xv.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ef.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xj.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ku.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://su.yuexingan06.cn

[E02] 重复字符串
来源：http://lw.jctech888.com.cn

Py:   "ab" * 3
来源：http://xn.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ja.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://dc.newstarts.cn

TS:   "ab".repeat(3)
来源：http://gy.nszjky.cn

Java: "ab".repeat(3)
来源：http://ui.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ai.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://wp.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xv.521024.cn

[E03] 截取子串
来源：http://ci.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tv.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ls.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kp.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://vk.nicolike.cn

Java: s.substring(1, 4)
来源：http://fb.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oc.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://us.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://xt.chemitech.net.cn

[E04] 查找子串位置
来源：http://nx.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://nv.9csxet.cn

PHP:  strpos($s, "x");
来源：http://yj.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tr.gzmigu.cn

TS:   s.indexOf("x")
来源：http://pp.szsharing.cn

Java: s.indexOf("x")
来源：http://vn.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://rn.haigaiapp.cn

Ruby: s.index("x")
来源：http://qt.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://oj.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rv.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ed.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bh.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aw.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qq.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fy.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jz.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hf.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xb.colortex.cn

[E06] 替换子串
来源：http://fh.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://la.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://yp.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tg.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://rh.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wv.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kg.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tr.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ew.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://kc.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://na.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://au.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fi.yuexingan06.cn

TS:   s.split(",")
来源：http://hm.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fj.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dw.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://ik.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yr.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ig.gzmigu.cn

Py:   ",".join(items)
来源：http://uy.newstarts.cn

PHP:  implode(",", $items);
来源：http://pq.yuexingan06.cn

JS:   items.join(",")
来源：http://wi.jianghongdianzi.cn

TS:   items.join(",")
来源：http://dc.asd995.cn

Java: String.join(",", items)
来源：http://op.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://jr.szsharing.cn

Ruby: items.join(",")
来源：http://qm.szxytkj.cn

C#:   string.Join(",", items)
来源：http://iv.9csxet.cn

[E09] 去除所有空白字符
来源：http://sf.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uo.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ot.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://wj.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://rs.haigaiapp.cn


<!-- 参考信息 -->