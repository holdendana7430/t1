代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zz.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jx.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ve.gzmigu.cn

Ruby: # 无泛型
来源：http://ij.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cr.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://qh.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rb.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://zf.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oi.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mr.szxytkj.cn

Java: // 无解构
来源：http://yo.chemitech.net.cn

Go:   // 无解构
来源：http://dy.9csxet.cn

Ruby: a, b = pair
来源：http://jp.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://yi.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://vo.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bz.haigaiapp.cn

PHP:  // 无重载
来源：http://cv.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gx.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gl.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://id.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ya.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://mb.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://fs.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://ex.hahajie.cn

================================================================================
来源：http://fy.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://uo.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ry.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ni.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://is.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://di.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qm.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ut.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://va.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sh.521024.cn

[D02] 追加元素到末尾
来源：http://po.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ok.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xs.panjiajie.cn

JS:   arr.push(4);
来源：http://tu.wgjwhj.cn

TS:   arr.push(4);
来源：http://kr.bookmarksfly.cn

Java: list.add(4);
来源：http://ix.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://ee.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://eo.wgjwhj.cn

C#:   list.Add(4);
来源：http://js.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://eu.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://wo.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wn.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://py.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yg.lnxyls.cn

Java: list.add(0, 0);
来源：http://ce.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pr.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vk.colortex.cn

C#:   list.Insert(0, 0);
来源：http://kv.huixiangedu.cn

[D04] 删除元素
来源：http://il.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uv.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://el.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fx.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ic.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rc.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rf.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oa.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tr.asd995.cn

[D05] 访问与修改元素
来源：http://hr.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ej.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xk.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://in.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://sr.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://rn.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://hg.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ys.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sp.jianghongdianzi.cn

[D06] 数组长度
来源：http://qi.yuntaijiaju.cn

Py:   len(arr)
来源：http://ut.shxzukj.cn

PHP:  count($arr);
来源：http://zn.shtwfgs.cn

JS:   arr.length
来源：http://ky.asd995.cn

TS:   arr.length
来源：http://bx.huixinmuqiang.cn

Java: list.size();
来源：http://zc.szsharing.cn

Go:   len(arr)
来源：http://pm.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://ip.yuexingan06.cn

C#:   list.Count;
来源：http://vi.colortex.cn

[D07] 切片 / 取子数组
来源：http://oy.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xn.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lt.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://kf.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://ru.shxzukj.cn

Java: list.subList(1, 4);
来源：http://jn.muxihuayi.cn

Go:   arr[1:4]
来源：http://af.521024.cn

Ruby: arr[1, 3]
来源：http://bc.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://qx.newstarts.cn

[D08] 合并两个数组
来源：http://mk.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://mz.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://pn.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bc.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ta.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://by.chemitech.net.cn

Go:   append(a, b...)
来源：http://ri.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ji.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://hv.szxytkj.cn

[D09] 排序（升序）
来源：http://kl.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ly.huixiangedu.cn

PHP:  sort($arr);
来源：http://us.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bu.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vf.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yh.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jt.muxihuayi.cn

Ruby: arr.sort
来源：http://fy.gzmigu.cn

C#:   list.Sort();
来源：http://qq.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://az.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gy.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sg.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dy.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ov.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mv.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ky.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fy.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mh.huixinmuqiang.cn

[D11] 反转数组
来源：http://sz.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wj.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://fm.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zu.hahajie.cn

TS:   [...arr].reverse();
来源：http://uy.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://fj.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://bb.9csxet.cn

Ruby: arr.reverse
来源：http://yo.521024.cn

C#:   list.Reverse();
来源：http://df.haigaiapp.cn

[D12] 查找元素下标
来源：http://ab.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ll.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oo.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uy.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wt.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rm.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://rx.hnjuh.cn

Ruby: arr.index(x)
来源：http://pa.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://ef.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://du.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ec.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://of.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://oo.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://ff.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jv.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bt.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vp.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ju.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://qx.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ac.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bj.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://qv.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://wz.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oa.gzmigu.cn

Go:   // 手写循环
来源：http://yn.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xl.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ag.newstarts.cn

[D15] 去重
来源：http://og.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sm.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://no.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://hn.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://to.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sc.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://no.521024.cn

Ruby: arr.uniq
来源：http://bn.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://of.bjjhwx.cn

[D16] 求和与平均值
来源：http://qt.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jl.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bk.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gn.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fk.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://no.chemitech.net.cn

Go:   // 手写循环累加
来源：http://vd.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sm.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://qd.yuexingan06.cn

[D17] 最大值与最小值
来源：http://mj.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://se.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://uf.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tw.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://iw.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jj.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bi.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ob.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://wy.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://vt.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://na.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://nv.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zy.jianghongdianzi.cn

TS:   nested.flat();
来源：http://gm.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xz.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://fy.hnjuh.cn

Ruby: nested.flatten
来源：http://db.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qy.jianghongdianzi.cn

[D19] 按字段分组
来源：http://lv.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mm.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jk.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://en.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dc.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vd.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://qt.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ic.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oe.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://kb.shtwfgs.cn

Py:   Counter(arr)
来源：http://qe.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://th.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ej.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vm.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ku.hahajie.cn

Go:   // 手写 map[T]int
来源：http://nm.panjiajie.cn

Ruby: arr.tally
来源：http://yd.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vm.colortex.cn

[D21] 判断是否包含某元素
来源：http://bp.yuntaijiaju.cn

Py:   x in arr
来源：http://rf.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://jt.panjiajie.cn

JS:   arr.includes(x)
来源：http://rj.haigaiapp.cn

TS:   arr.includes(x)
来源：http://yo.muxihuayi.cn

Java: list.contains(x)
来源：http://gi.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://sw.shxzukj.cn

Ruby: arr.include?(x)
来源：http://kp.panjiajie.cn

C#:   list.Contains(x)
来源：http://xw.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://pn.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wq.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gj.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pf.shtwfgs.cn

TS:   [...arr];
来源：http://wk.9csxet.cn

Java: new ArrayList<>(list);
来源：http://nn.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vo.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://dw.hnjuh.cn

C#:   new List<int>(list);
来源：http://sl.newstarts.cn

[D23] reduce 累积计算
来源：http://mz.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yu.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zc.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kf.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ug.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mo.huanxung.cn

Go:   // 手写循环
来源：http://jg.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uf.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uv.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://ui.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gu.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ai.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gk.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fi.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hw.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ev.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://so.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ai.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://ap.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ik.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://da.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jv.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uy.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bj.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lz.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://po.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yi.lnxyls.cn

[D26] 数组转字符串
来源：http://qn.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://ia.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://bi.huixiangedu.cn

JS:   arr.join(", ")
来源：http://sz.jctech888.com.cn

TS:   arr.join(", ")
来源：http://qb.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ik.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://iy.9csxet.cn

Ruby: arr.join(", ")
来源：http://we.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://du.521024.cn

================================================================================
来源：http://vx.hnjuh.cn

E. 字符串处理
来源：http://cj.shxzukj.cn

================================================================================
来源：http://ni.szxytkj.cn

[E01] 拼接字符串
来源：http://bg.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oq.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tj.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gc.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ll.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qk.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sx.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ny.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yi.newstarts.cn

[E02] 重复字符串
来源：http://sh.szsharing.cn

Py:   "ab" * 3
来源：http://ti.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://wo.szsharing.cn

JS:   "ab".repeat(3)
来源：http://bd.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://ur.szxytkj.cn

Java: "ab".repeat(3)
来源：http://bk.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://bs.panjiajie.cn

Ruby: "ab" * 3
来源：http://it.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kh.yuexingan06.cn

[E03] 截取子串
来源：http://gn.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kf.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ag.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ry.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://gy.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://um.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rq.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vn.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://sa.hnjuh.cn

[E04] 查找子串位置
来源：http://it.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://jc.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://hc.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bn.nicolike.cn

TS:   s.indexOf("x")
来源：http://fa.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://zp.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ml.wgjwhj.cn

Ruby: s.index("x")
来源：http://sn.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://ab.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mm.gzmigu.cn


<!-- 参考信息 -->