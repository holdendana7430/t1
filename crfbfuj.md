代发 wailian999

[C14] 泛型函数
来源：http://ss.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cb.shxzukj.cn

PHP:  // 无泛型
来源：http://hr.asd995.cn

JS:   // 无泛型
来源：http://sa.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ep.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zf.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mc.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://gw.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gs.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://li.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aa.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://kj.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://so.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hw.9csxet.cn

Java: // 无解构
来源：http://ia.hnjuh.cn

Go:   // 无解构
来源：http://nt.asd995.cn

Ruby: a, b = pair
来源：http://ig.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://er.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://at.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cc.521024.cn

PHP:  // 无重载
来源：http://ie.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xa.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ds.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uh.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://gv.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://ou.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ky.hahajie.cn

================================================================================
来源：http://ti.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://pr.wgjwhj.cn

================================================================================
来源：http://ik.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://fz.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ok.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hf.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fr.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://np.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fl.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://ux.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://yl.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fx.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ct.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ci.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dw.szsharing.cn

JS:   arr.push(4);
来源：http://me.jctech888.com.cn

TS:   arr.push(4);
来源：http://fb.jianghongdianzi.cn

Java: list.add(4);
来源：http://em.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://pr.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://it.huixiangedu.cn

C#:   list.Add(4);
来源：http://ca.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://wg.colortex.cn

Py:   arr.insert(0, 0)
来源：http://tj.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vm.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dt.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://cn.521024.cn

Java: list.add(0, 0);
来源：http://nf.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dp.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hi.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://jv.shxzukj.cn

[D04] 删除元素
来源：http://ud.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hy.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ro.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gg.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://wb.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xn.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dg.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cm.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sj.hahajie.cn

[D05] 访问与修改元素
来源：http://xs.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jf.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wj.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://hb.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://ey.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://tx.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dk.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ep.huixinmuqiang.cn

[D06] 数组长度
来源：http://hz.szsharing.cn

Py:   len(arr)
来源：http://bd.haigaiapp.cn

PHP:  count($arr);
来源：http://jp.szsharing.cn

JS:   arr.length
来源：http://zh.nicolike.cn

TS:   arr.length
来源：http://iu.nicolike.cn

Java: list.size();
来源：http://yv.bjjhwx.cn

Go:   len(arr)
来源：http://gh.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://uf.9csxet.cn

C#:   list.Count;
来源：http://pq.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://fj.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tm.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ld.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://xj.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://tl.panjiajie.cn

Java: list.subList(1, 4);
来源：http://wg.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://dv.nszjky.cn

Ruby: arr[1, 3]
来源：http://ia.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://tl.shxzskj.cn

[D08] 合并两个数组
来源：http://ec.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://bo.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ly.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ft.shxzskj.cn

TS:   [...a, ...b];
来源：http://mx.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nv.gzmigu.cn

Go:   append(a, b...)
来源：http://mu.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://dk.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://cb.haigaiapp.cn

[D09] 排序（升序）
来源：http://fu.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://zt.haigaiapp.cn

PHP:  sort($arr);
来源：http://gq.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cv.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xe.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dw.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dn.nicolike.cn

Ruby: arr.sort
来源：http://uf.shxzskj.cn

C#:   list.Sort();
来源：http://gc.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bt.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hx.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kz.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hx.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eh.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://st.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://um.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://st.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ai.hahajie.cn

[D11] 反转数组
来源：http://jc.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ej.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://sg.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://je.9csxet.cn

TS:   [...arr].reverse();
来源：http://td.shxzukj.cn

Java: Collections.reverse(list);
来源：http://yj.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://hi.hnjuh.cn

Ruby: arr.reverse
来源：http://fj.nicolike.cn

C#:   list.Reverse();
来源：http://rj.lnxyls.cn

[D12] 查找元素下标
来源：http://nb.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://wm.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dr.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fg.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dp.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nf.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://bq.asd995.cn

Ruby: arr.index(x)
来源：http://zg.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://xk.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://yv.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nt.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fe.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://jw.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://il.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nl.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ye.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pu.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aj.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://uy.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://er.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://af.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://lw.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://cr.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wi.chemitech.net.cn

Go:   // 手写循环
来源：http://qn.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lc.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xq.gzmigu.cn

[D15] 去重
来源：http://ex.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ib.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ga.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://xr.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://gd.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qi.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ze.huixiangedu.cn

Ruby: arr.uniq
来源：http://du.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://te.shxzukj.cn

[D16] 求和与平均值
来源：http://sa.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://py.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vi.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ag.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pq.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ib.hahajie.cn

Go:   // 手写循环累加
来源：http://lp.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iv.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://cr.lnxyls.cn

[D17] 最大值与最小值
来源：http://nf.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://od.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://rp.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dk.521024.cn

TS:   Math.max(...arr);
来源：http://re.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xy.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hn.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://tz.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://tu.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://pw.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vs.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://bc.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rr.bjjhwx.cn

TS:   nested.flat();
来源：http://wv.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kz.9csxet.cn

Go:   // 手写双层循环
来源：http://mn.haigaiapp.cn

Ruby: nested.flatten
来源：http://qf.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gx.panjiajie.cn

[D19] 按字段分组
来源：http://ql.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hl.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ae.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ru.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fb.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://th.asd995.cn

Go:   // 手写 map[string][]T
来源：http://fr.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gq.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ly.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://gk.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://hm.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://lb.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ar.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eg.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mu.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://os.nszjky.cn

Ruby: arr.tally
来源：http://mg.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bc.521024.cn

[D21] 判断是否包含某元素
来源：http://be.szsharing.cn

Py:   x in arr
来源：http://yh.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://cr.hahajie.cn

JS:   arr.includes(x)
来源：http://ii.9csxet.cn

TS:   arr.includes(x)
来源：http://zh.asd995.cn

Java: list.contains(x)
来源：http://uo.521024.cn

Go:   slices.Contains(arr, x)
来源：http://ze.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://hg.9csxet.cn

C#:   list.Contains(x)
来源：http://dz.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://xo.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zl.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://on.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://op.shxzukj.cn

TS:   [...arr];
来源：http://vt.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://po.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cm.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://pc.muxihuayi.cn

C#:   new List<int>(list);
来源：http://ys.haigaiapp.cn

[D23] reduce 累积计算
来源：http://ia.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ss.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pe.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yo.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ru.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yc.nszjky.cn

Go:   // 手写循环
来源：http://xu.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gs.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yw.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://xm.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uj.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kd.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dw.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wk.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ka.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fs.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zm.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fo.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://mg.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ob.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ut.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ft.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ii.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ka.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cc.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ma.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gg.chemitech.net.cn

[D26] 数组转字符串
来源：http://mc.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://tu.asd995.cn

PHP:  implode(", ", $arr);
来源：http://pq.szsharing.cn

JS:   arr.join(", ")
来源：http://hy.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://qz.hahajie.cn

Java: String.join(", ", list)
来源：http://pj.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://br.newstarts.cn

Ruby: arr.join(", ")
来源：http://lk.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://zz.szxytkj.cn

================================================================================
来源：http://ly.chemitech.net.cn

E. 字符串处理
来源：http://hs.shxzskj.cn

================================================================================
来源：http://yq.9csxet.cn

[E01] 拼接字符串
来源：http://me.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sg.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dw.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tl.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wx.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lw.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nn.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gg.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pr.hnjuh.cn

[E02] 重复字符串
来源：http://cm.bookmarksfly.cn

Py:   "ab" * 3
来源：http://zf.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://mw.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://hc.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://ua.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ll.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://yo.lnxyls.cn

Ruby: "ab" * 3
来源：http://qi.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sx.gzmigu.cn

[E03] 截取子串
来源：http://ch.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://en.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lh.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lq.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://pu.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://jm.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ew.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ny.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://zu.gzmigu.cn

[E04] 查找子串位置
来源：http://ae.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://pa.newstarts.cn

PHP:  strpos($s, "x");
来源：http://nd.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cb.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://sw.haigaiapp.cn

Java: s.indexOf("x")
来源：http://zv.muxihuayi.cn


<!-- 参考信息 -->