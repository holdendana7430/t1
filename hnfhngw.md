代发 wailian999

D. 数组 / 列表 / 集合
来源：http://yk.wgjwhj.cn

================================================================================
来源：http://oz.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://eh.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cw.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bf.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vb.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://md.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://li.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://dz.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://wn.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iz.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://rz.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hf.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yf.shxzskj.cn

JS:   arr.push(4);
来源：http://yq.hnjuh.cn

TS:   arr.push(4);
来源：http://fe.wgjwhj.cn

Java: list.add(4);
来源：http://xn.521024.cn

Go:   arr = append(arr, 4)
来源：http://ab.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://rj.wgjwhj.cn

C#:   list.Add(4);
来源：http://tg.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://bx.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://cz.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dw.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uz.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://el.9csxet.cn

Java: list.add(0, 0);
来源：http://sn.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uf.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hc.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://lf.hahajie.cn

[D04] 删除元素
来源：http://vg.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zy.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uk.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oz.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ka.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ri.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://of.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wt.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cx.hnjuh.cn

[D05] 访问与修改元素
来源：http://eg.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ii.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jv.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yx.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://dv.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://rx.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://fm.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tm.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dg.szxytkj.cn

[D06] 数组长度
来源：http://wf.huixinmuqiang.cn

Py:   len(arr)
来源：http://cy.wgjwhj.cn

PHP:  count($arr);
来源：http://cl.newstarts.cn

JS:   arr.length
来源：http://tk.jctech888.com.cn

TS:   arr.length
来源：http://pk.wgjwhj.cn

Java: list.size();
来源：http://zt.huixinmuqiang.cn

Go:   len(arr)
来源：http://mq.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://yi.lnxyls.cn

C#:   list.Count;
来源：http://cg.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://uz.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yy.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uv.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://wt.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://as.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://lk.nicolike.cn

Go:   arr[1:4]
来源：http://vf.asd995.cn

Ruby: arr[1, 3]
来源：http://yj.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://py.nszjky.cn

[D08] 合并两个数组
来源：http://vy.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://py.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://bx.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hn.nicolike.cn

TS:   [...a, ...b];
来源：http://mc.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ps.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ct.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://wc.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://bm.yuexingan06.cn

[D09] 排序（升序）
来源：http://hh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://gn.gzmigu.cn

PHP:  sort($arr);
来源：http://xj.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://es.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oz.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eq.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qj.shxzukj.cn

Ruby: arr.sort
来源：http://xm.szxytkj.cn

C#:   list.Sort();
来源：http://bx.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zq.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tu.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sd.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fu.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lo.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mh.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ol.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qt.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ub.panjiajie.cn

[D11] 反转数组
来源：http://at.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uv.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://ap.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ar.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://ce.panjiajie.cn

Java: Collections.reverse(list);
来源：http://lo.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://wf.bookmarksfly.cn

Ruby: arr.reverse
来源：http://tl.shxzukj.cn

C#:   list.Reverse();
来源：http://cj.jctech888.com.cn

[D12] 查找元素下标
来源：http://mk.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://jc.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pf.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hs.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kd.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gn.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://qy.shtwfgs.cn

Ruby: arr.index(x)
来源：http://kt.asd995.cn

C#:   list.IndexOf(x);
来源：http://bv.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://sd.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eg.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kw.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://qa.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mr.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kr.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rq.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jt.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hw.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://us.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zx.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://af.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://mq.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://bo.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cu.jctech888.com.cn

Go:   // 手写循环
来源：http://fs.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://co.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jl.szsharing.cn

[D15] 去重
来源：http://cm.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sm.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://bf.asd995.cn

JS:   [...new Set(arr)]
来源：http://ke.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://kn.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bk.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uz.9csxet.cn

Ruby: arr.uniq
来源：http://eb.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://zc.yuexingan06.cn

[D16] 求和与平均值
来源：http://xr.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ou.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oq.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ck.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xj.chemitech.net.cn

Go:   // 手写循环累加
来源：http://co.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bt.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://uo.shxzukj.cn

[D17] 最大值与最小值
来源：http://oh.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ps.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://up.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fg.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://wc.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dt.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://to.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://kx.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://jf.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://kr.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ep.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://qn.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ib.chemitech.net.cn

TS:   nested.flat();
来源：http://ea.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://my.bjjhwx.cn

Go:   // 手写双层循环
来源：http://sr.huanxung.cn

Ruby: nested.flatten
来源：http://ee.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ol.jianghongdianzi.cn

[D19] 按字段分组
来源：http://as.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cr.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ll.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bm.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tl.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rv.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://qb.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vn.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hk.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://ia.newstarts.cn

Py:   Counter(arr)
来源：http://od.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://su.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://si.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bz.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vd.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ma.yuexingan06.cn

Ruby: arr.tally
来源：http://qw.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lg.huanxung.cn

[D21] 判断是否包含某元素
来源：http://gw.szxytkj.cn

Py:   x in arr
来源：http://ln.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://fz.szsharing.cn

JS:   arr.includes(x)
来源：http://tf.shxzukj.cn

TS:   arr.includes(x)
来源：http://zy.lnxyls.cn

Java: list.contains(x)
来源：http://nz.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://ro.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://vy.panjiajie.cn

C#:   list.Contains(x)
来源：http://dl.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ut.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dd.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cp.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://av.gzmigu.cn

TS:   [...arr];
来源：http://us.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://kv.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bg.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://lr.9csxet.cn

C#:   new List<int>(list);
来源：http://ee.chemitech.net.cn

[D23] reduce 累积计算
来源：http://ym.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vm.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rw.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://az.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ps.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wn.asd995.cn

Go:   // 手写循环
来源：http://ge.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mt.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://py.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://eh.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://um.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rn.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vh.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xo.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yd.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fk.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hq.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kg.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ay.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yb.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://az.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xb.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kq.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rv.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pm.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lm.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gy.wgjwhj.cn

[D26] 数组转字符串
来源：http://lv.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://qr.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://aa.yuexingan06.cn

JS:   arr.join(", ")
来源：http://th.szxytkj.cn

TS:   arr.join(", ")
来源：http://ob.szxytkj.cn

Java: String.join(", ", list)
来源：http://gt.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://hn.asd995.cn

Ruby: arr.join(", ")
来源：http://sn.nicolike.cn

C#:   string.Join(", ", list)
来源：http://yj.haigaiapp.cn

================================================================================
来源：http://it.521024.cn

E. 字符串处理
来源：http://ve.huixinmuqiang.cn

================================================================================
来源：http://dh.panjiajie.cn

[E01] 拼接字符串
来源：http://kv.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bx.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rh.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://up.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sr.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xl.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oq.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kf.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jp.jctech888.com.cn

[E02] 重复字符串
来源：http://po.yuexingan06.cn

Py:   "ab" * 3
来源：http://ct.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://tb.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://yr.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://qy.szsharing.cn

Java: "ab".repeat(3)
来源：http://lf.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://jj.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://wd.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dh.huixiangedu.cn

[E03] 截取子串
来源：http://zk.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dv.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bg.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jm.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ri.asd995.cn

Java: s.substring(1, 4)
来源：http://zn.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://po.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yp.asd995.cn

C#:   s.Substring(1, 3)
来源：http://lm.panjiajie.cn

[E04] 查找子串位置
来源：http://pw.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://cl.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://se.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nv.hnjuh.cn

TS:   s.indexOf("x")
来源：http://mg.9csxet.cn

Java: s.indexOf("x")
来源：http://qb.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://xo.haigaiapp.cn

Ruby: s.index("x")
来源：http://be.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://fm.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nw.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://of.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ao.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ry.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iz.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bl.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xp.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nd.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zx.nszjky.cn

[E06] 替换子串
来源：http://or.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zj.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://fd.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ou.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ax.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ef.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ml.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ty.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://nw.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ja.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eg.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hy.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nk.chemitech.net.cn

TS:   s.split(",")
来源：http://hw.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://du.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://br.521024.cn


<!-- 参考信息 -->