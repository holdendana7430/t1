代发 wailian999

D. 数组 / 列表 / 集合
来源：http://im.yuexingan06.cn

================================================================================
来源：http://ae.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ja.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qr.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kv.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qq.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://me.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pr.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://qt.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://ud.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ku.shxzskj.cn

[D02] 追加元素到末尾
来源：http://om.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vp.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ij.shxzukj.cn

JS:   arr.push(4);
来源：http://hf.hahajie.cn

TS:   arr.push(4);
来源：http://vc.yuexingan06.cn

Java: list.add(4);
来源：http://rm.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://dq.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ph.huanxung.cn

C#:   list.Add(4);
来源：http://up.colortex.cn

[D03] 在指定位置插入元素
来源：http://vw.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ta.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fx.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wn.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://qk.asd995.cn

Java: list.add(0, 0);
来源：http://ry.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sg.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ug.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://zc.shtwfgs.cn

[D04] 删除元素
来源：http://cj.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sb.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cf.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fk.colortex.cn

TS:   arr.splice(0, 1);
来源：http://bk.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ni.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://da.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ms.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sk.asd995.cn

[D05] 访问与修改元素
来源：http://zz.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mt.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://os.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xq.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://xu.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://br.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://te.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qd.muxihuayi.cn

[D06] 数组长度
来源：http://kc.hnjuh.cn

Py:   len(arr)
来源：http://xc.shtwfgs.cn

PHP:  count($arr);
来源：http://qh.nicolike.cn

JS:   arr.length
来源：http://jt.bookmarksfly.cn

TS:   arr.length
来源：http://rv.hnjuh.cn

Java: list.size();
来源：http://qs.9csxet.cn

Go:   len(arr)
来源：http://of.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://xr.panjiajie.cn

C#:   list.Count;
来源：http://jp.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://qr.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fc.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ab.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://ow.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://pl.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://qf.bjjhwx.cn

Go:   arr[1:4]
来源：http://yn.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://hc.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://la.panjiajie.cn

[D08] 合并两个数组
来源：http://vl.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ox.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://pg.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ad.shtwfgs.cn

TS:   [...a, ...b];
来源：http://or.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vh.nicolike.cn

Go:   append(a, b...)
来源：http://by.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://eu.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ai.hahajie.cn

[D09] 排序（升序）
来源：http://xe.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://tl.chemitech.net.cn

PHP:  sort($arr);
来源：http://ho.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nh.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rj.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://op.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ps.haigaiapp.cn

Ruby: arr.sort
来源：http://sg.yuntaijiaju.cn

C#:   list.Sort();
来源：http://no.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dj.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cp.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bv.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cz.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vb.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qh.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yp.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hn.jianghongdianzi.cn

[D11] 反转数组
来源：http://qo.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://li.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://vw.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rv.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ye.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://xn.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://tw.huixiangedu.cn

Ruby: arr.reverse
来源：http://cv.hnjuh.cn

C#:   list.Reverse();
来源：http://eq.yuexingan06.cn

[D12] 查找元素下标
来源：http://mw.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://uk.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qk.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fw.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cz.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hu.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://ct.muxihuayi.cn

Ruby: arr.index(x)
来源：http://ah.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://hc.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://uk.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://su.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jo.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://qu.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://go.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://im.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ye.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fp.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zg.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://je.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rl.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wn.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://xm.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://qp.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ld.jianghongdianzi.cn

Go:   // 手写循环
来源：http://gl.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gl.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pr.newstarts.cn

[D15] 去重
来源：http://ir.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ly.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://lw.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://jx.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://oj.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ie.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://un.chemitech.net.cn

Ruby: arr.uniq
来源：http://oq.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://rl.yuexingan06.cn

[D16] 求和与平均值
来源：http://of.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aa.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ih.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jj.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uu.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yx.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://uj.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://if.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://iu.hnjuh.cn

[D17] 最大值与最小值
来源：http://gp.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://yw.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://uq.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hg.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://bj.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rj.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kz.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://zx.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://jq.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://iz.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pa.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://jj.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vp.yuexingan06.cn

TS:   nested.flat();
来源：http://ye.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://or.szxytkj.cn

Go:   // 手写双层循环
来源：http://eg.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://hm.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bx.yuntaijiaju.cn

[D19] 按字段分组
来源：http://qc.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://km.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zz.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bu.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ln.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ar.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://yv.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jz.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zk.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ou.521024.cn

Py:   Counter(arr)
来源：http://gw.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ra.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sc.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ie.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qf.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://kn.huixinmuqiang.cn

Ruby: arr.tally
来源：http://ux.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://na.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://nr.yuntaijiaju.cn

Py:   x in arr
来源：http://yv.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ka.shxzskj.cn

JS:   arr.includes(x)
来源：http://ov.muxihuayi.cn

TS:   arr.includes(x)
来源：http://ek.gzmigu.cn

Java: list.contains(x)
来源：http://sp.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://fb.hahajie.cn

Ruby: arr.include?(x)
来源：http://ns.521024.cn

C#:   list.Contains(x)
来源：http://ay.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://bh.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ld.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://id.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bh.wgjwhj.cn

TS:   [...arr];
来源：http://rd.newstarts.cn

Java: new ArrayList<>(list);
来源：http://wg.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xx.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://pk.newstarts.cn

C#:   new List<int>(list);
来源：http://xy.haigaiapp.cn

[D23] reduce 累积计算
来源：http://tn.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tu.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nb.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bt.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mu.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ai.gzmigu.cn

Go:   // 手写循环
来源：http://vr.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zp.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qp.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://tt.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oy.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sa.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hg.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xm.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ff.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://or.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kh.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://em.521024.cn

[D25] Set 集合去重与交并差
来源：http://iz.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yb.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jk.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://li.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://no.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aa.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mb.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uq.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ao.colortex.cn

[D26] 数组转字符串
来源：http://gz.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ly.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://dn.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://fj.asd995.cn

TS:   arr.join(", ")
来源：http://co.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://cf.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://ix.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://rw.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://vy.bookmarksfly.cn

================================================================================
来源：http://gq.shtwfgs.cn

E. 字符串处理
来源：http://sc.yuntaijiaju.cn

================================================================================
来源：http://fn.yuexingan06.cn

[E01] 拼接字符串
来源：http://ou.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lx.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dv.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ih.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hl.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zq.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hw.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ep.chemitech.net.cn

[E02] 重复字符串
来源：http://ht.hahajie.cn

Py:   "ab" * 3
来源：http://kt.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://hs.521024.cn

JS:   "ab".repeat(3)
来源：http://wd.szsharing.cn

TS:   "ab".repeat(3)
来源：http://rx.shxzskj.cn

Java: "ab".repeat(3)
来源：http://xk.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://yx.shxzukj.cn

Ruby: "ab" * 3
来源：http://sk.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lb.lnxyls.cn

[E03] 截取子串
来源：http://el.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ep.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ao.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cz.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://le.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://bv.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ng.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pb.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://ph.hahajie.cn

[E04] 查找子串位置
来源：http://gz.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://tp.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://ha.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nj.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://cp.szsharing.cn

Java: s.indexOf("x")
来源：http://qk.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://cj.szsharing.cn

Ruby: s.index("x")
来源：http://ks.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://zr.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rj.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rq.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rd.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eb.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gq.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://um.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mp.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gr.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pp.huixinmuqiang.cn

[E06] 替换子串
来源：http://ws.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tw.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://hq.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://nq.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ei.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bq.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bu.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://fj.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://bu.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pt.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ox.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gk.yuntaijiaju.cn

TS:   s.split(",")
来源：http://gb.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://up.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sl.hnjuh.cn


<!-- 参考信息 -->