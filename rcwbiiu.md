代发 wailian999

D. 数组 / 列表 / 集合
来源：http://tc.nicolike.cn

================================================================================
来源：http://pa.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://os.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dt.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hn.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tp.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iw.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oc.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://bh.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ck.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ht.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://uq.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jm.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://in.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://uj.nicolike.cn

TS:   arr.push(4);
来源：http://kf.newstarts.cn

Java: list.add(4);
来源：http://ob.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://rt.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://vm.chemitech.net.cn

C#:   list.Add(4);
来源：http://vx.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://me.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://so.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xa.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://qz.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://wr.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ju.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ez.asd995.cn

C#:   list.Insert(0, 0);
来源：http://yv.shtwfgs.cn

[D04] 删除元素
来源：http://zk.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gp.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ul.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://in.colortex.cn

TS:   arr.splice(0, 1);
来源：http://qe.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hw.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kz.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pm.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xn.szsharing.cn

[D05] 访问与修改元素
来源：http://kv.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eq.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yt.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fn.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://vr.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wh.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://dc.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rq.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mh.hahajie.cn

[D06] 数组长度
来源：http://fk.9csxet.cn

Py:   len(arr)
来源：http://tn.shtwfgs.cn

PHP:  count($arr);
来源：http://ov.chemitech.net.cn

JS:   arr.length
来源：http://gl.szsharing.cn

TS:   arr.length
来源：http://bk.521024.cn

Java: list.size();
来源：http://bt.yuexingan06.cn

Go:   len(arr)
来源：http://rh.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://pl.chemitech.net.cn

C#:   list.Count;
来源：http://jj.521024.cn

[D07] 切片 / 取子数组
来源：http://zh.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wg.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xf.521024.cn

JS:   arr.slice(1, 4);
来源：http://jh.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://nt.colortex.cn

Java: list.subList(1, 4);
来源：http://yj.colortex.cn

Go:   arr[1:4]
来源：http://wc.nszjky.cn

Ruby: arr[1, 3]
来源：http://wn.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://ns.huixiangedu.cn

[D08] 合并两个数组
来源：http://sv.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://ru.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://ln.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ed.521024.cn

TS:   [...a, ...b];
来源：http://lm.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rr.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ty.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://bw.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://me.shxzskj.cn

[D09] 排序（升序）
来源：http://nq.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://dy.jctech888.com.cn

PHP:  sort($arr);
来源：http://kn.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bl.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sg.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yf.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cx.szxytkj.cn

Ruby: arr.sort
来源：http://qk.lnxyls.cn

C#:   list.Sort();
来源：http://kt.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oo.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ns.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ht.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lw.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://on.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fj.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ki.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://am.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vv.szsharing.cn

[D11] 反转数组
来源：http://og.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ct.nszjky.cn

PHP:  array_reverse($arr);
来源：http://cf.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ad.nszjky.cn

TS:   [...arr].reverse();
来源：http://qj.9csxet.cn

Java: Collections.reverse(list);
来源：http://ac.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://lo.newstarts.cn

Ruby: arr.reverse
来源：http://tc.szxytkj.cn

C#:   list.Reverse();
来源：http://pg.hnjuh.cn

[D12] 查找元素下标
来源：http://nj.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ui.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dm.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hi.asd995.cn

Go:   slices.Index(arr, x)
来源：http://ll.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://rg.nszjky.cn

C#:   list.IndexOf(x);
来源：http://to.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://vg.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oi.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ov.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://av.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://nc.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://or.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qz.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ab.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rk.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://md.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://un.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://em.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://wg.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://qr.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qd.szxytkj.cn

Go:   // 手写循环
来源：http://lk.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ac.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yo.nicolike.cn

[D15] 去重
来源：http://tw.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ob.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://bc.hahajie.cn

JS:   [...new Set(arr)]
来源：http://bi.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://go.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wt.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mj.huixiangedu.cn

Ruby: arr.uniq
来源：http://ko.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://jy.hnjuh.cn

[D16] 求和与平均值
来源：http://fk.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mh.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ri.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ef.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ln.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gw.colortex.cn

Go:   // 手写循环累加
来源：http://zx.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jb.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://cr.yuexingan06.cn

[D17] 最大值与最小值
来源：http://ub.521024.cn

Py:   max(arr);  min(arr)
来源：http://ds.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://os.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hl.shxzskj.cn

TS:   Math.max(...arr);
来源：http://jk.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://if.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xz.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://nt.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://qz.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://tq.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ez.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://jc.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ox.jctech888.com.cn

TS:   nested.flat();
来源：http://ng.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wm.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://cf.521024.cn

Ruby: nested.flatten
来源：http://bs.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bh.szsharing.cn

[D19] 按字段分组
来源：http://tg.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lx.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rs.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mj.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://se.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://do.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://uy.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qg.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lb.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://dd.haigaiapp.cn

Py:   Counter(arr)
来源：http://bk.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://de.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ck.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yr.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sv.nszjky.cn

Go:   // 手写 map[T]int
来源：http://gv.jianghongdianzi.cn

Ruby: arr.tally
来源：http://si.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xa.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://xl.bookmarksfly.cn

Py:   x in arr
来源：http://zm.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://nk.huanxung.cn

JS:   arr.includes(x)
来源：http://pn.hahajie.cn

TS:   arr.includes(x)
来源：http://dk.shxzskj.cn

Java: list.contains(x)
来源：http://sy.521024.cn

Go:   slices.Contains(arr, x)
来源：http://dz.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://xy.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://cy.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xt.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wm.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qo.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ke.lnxyls.cn

TS:   [...arr];
来源：http://ey.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://ru.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kj.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://zu.szsharing.cn

C#:   new List<int>(list);
来源：http://cs.haigaiapp.cn

[D23] reduce 累积计算
来源：http://uh.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://es.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jj.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://by.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://is.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uo.9csxet.cn

Go:   // 手写循环
来源：http://eq.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gk.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gi.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://bg.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ow.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://el.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pb.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://or.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tt.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pn.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rc.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ii.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://pk.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eu.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zh.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://po.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qt.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://es.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ph.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wx.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jr.lnxyls.cn

[D26] 数组转字符串
来源：http://ko.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://vz.521024.cn

PHP:  implode(", ", $arr);
来源：http://cm.gzmigu.cn

JS:   arr.join(", ")
来源：http://ju.szsharing.cn

TS:   arr.join(", ")
来源：http://yd.nicolike.cn

Java: String.join(", ", list)
来源：http://pk.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://dd.gzmigu.cn

Ruby: arr.join(", ")
来源：http://xl.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://if.szsharing.cn

================================================================================
来源：http://kw.lnxyls.cn

E. 字符串处理
来源：http://qr.bjjhwx.cn

================================================================================
来源：http://gz.bookmarksfly.cn

[E01] 拼接字符串
来源：http://he.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ws.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yq.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ie.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gj.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ky.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uj.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jp.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xe.521024.cn

[E02] 重复字符串
来源：http://xk.gzmigu.cn

Py:   "ab" * 3
来源：http://cf.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://zw.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://hr.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://ir.shxzskj.cn

Java: "ab".repeat(3)
来源：http://gp.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://ah.chemitech.net.cn

Ruby: "ab" * 3
来源：http://no.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vx.wgjwhj.cn

[E03] 截取子串
来源：http://hb.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nt.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gb.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://en.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://wd.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://og.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lk.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ra.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://sr.lnxyls.cn

[E04] 查找子串位置
来源：http://gj.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://pn.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://hr.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bh.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://op.colortex.cn

Java: s.indexOf("x")
来源：http://zy.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://wy.bjjhwx.cn

Ruby: s.index("x")
来源：http://nh.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://bk.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ai.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vh.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tt.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dm.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ty.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jj.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gt.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gy.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iy.colortex.cn

[E06] 替换子串
来源：http://qv.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gk.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://we.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ch.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://xz.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yf.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wh.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ro.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://us.gzmigu.cn

[E07] 按分隔符拆分
来源：http://yp.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vh.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ba.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ze.bookmarksfly.cn

TS:   s.split(",")
来源：http://bh.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vd.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ld.bjjhwx.cn


<!-- 参考信息 -->