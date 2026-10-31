代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ld.lnxyls.cn

Go:   func add(a, b int) int
来源：http://gp.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mc.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wb.chemitech.net.cn

[C14] 泛型函数
来源：http://kq.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fn.hnjuh.cn

PHP:  // 无泛型
来源：http://cn.colortex.cn

JS:   // 无泛型
来源：http://uc.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ad.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pf.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ay.521024.cn

Ruby: # 无泛型
来源：http://oy.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wi.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://do.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lx.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://qq.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ss.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nl.szsharing.cn

Java: // 无解构
来源：http://iy.szxytkj.cn

Go:   // 无解构
来源：http://zp.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://nx.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://kb.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ys.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://al.haigaiapp.cn

PHP:  // 无重载
来源：http://hh.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xl.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://lh.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://as.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://hc.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ih.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tj.jctech888.com.cn

================================================================================
来源：http://ru.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://ec.bjjhwx.cn

================================================================================
来源：http://pg.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://dc.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://up.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nj.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rd.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ov.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jo.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://rt.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://gr.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gu.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://qt.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lk.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cc.haigaiapp.cn

JS:   arr.push(4);
来源：http://ex.haigaiapp.cn

TS:   arr.push(4);
来源：http://zc.hahajie.cn

Java: list.add(4);
来源：http://bf.asd995.cn

Go:   arr = append(arr, 4)
来源：http://rf.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://jc.szxytkj.cn

C#:   list.Add(4);
来源：http://ik.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://bb.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://by.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gc.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kx.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://lv.panjiajie.cn

Java: list.add(0, 0);
来源：http://dl.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iz.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qh.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://bv.nszjky.cn

[D04] 删除元素
来源：http://xy.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vx.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uv.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mo.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://oe.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wz.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ce.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ti.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ht.shxzskj.cn

[D05] 访问与修改元素
来源：http://mc.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iz.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nw.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kz.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://wt.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://xk.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://zk.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://of.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zy.colortex.cn

[D06] 数组长度
来源：http://ac.shxzukj.cn

Py:   len(arr)
来源：http://ud.newstarts.cn

PHP:  count($arr);
来源：http://ns.huanxung.cn

JS:   arr.length
来源：http://dx.521024.cn

TS:   arr.length
来源：http://ja.huixiangedu.cn

Java: list.size();
来源：http://xy.haigaiapp.cn

Go:   len(arr)
来源：http://rf.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://mf.chemitech.net.cn

C#:   list.Count;
来源：http://cs.newstarts.cn

[D07] 切片 / 取子数组
来源：http://yo.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hd.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sz.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://yp.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://ys.521024.cn

Java: list.subList(1, 4);
来源：http://rt.huixiangedu.cn

Go:   arr[1:4]
来源：http://iv.colortex.cn

Ruby: arr[1, 3]
来源：http://wz.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://fl.yuexingan06.cn

[D08] 合并两个数组
来源：http://hs.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://wf.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://le.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mm.asd995.cn

TS:   [...a, ...b];
来源：http://xy.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://em.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://xl.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://pm.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ow.hahajie.cn

[D09] 排序（升序）
来源：http://jp.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yx.hnjuh.cn

PHP:  sort($arr);
来源：http://rd.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mg.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gr.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sw.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rr.huixiangedu.cn

Ruby: arr.sort
来源：http://kp.chemitech.net.cn

C#:   list.Sort();
来源：http://bn.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ny.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bt.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ay.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zr.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oo.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tk.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wp.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lu.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ct.nicolike.cn

[D11] 反转数组
来源：http://sa.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zo.521024.cn

PHP:  array_reverse($arr);
来源：http://kz.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ha.panjiajie.cn

TS:   [...arr].reverse();
来源：http://pm.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://mu.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://jn.haigaiapp.cn

Ruby: arr.reverse
来源：http://bd.asd995.cn

C#:   list.Reverse();
来源：http://ct.lnxyls.cn

[D12] 查找元素下标
来源：http://wk.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://kc.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rg.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zg.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fw.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ep.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://rh.hnjuh.cn

Ruby: arr.index(x)
来源：http://qs.huanxung.cn

C#:   list.IndexOf(x);
来源：http://un.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://ly.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oi.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pc.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://mt.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ka.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ki.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kb.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tv.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ox.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://ky.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vg.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hn.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://hw.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://cj.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bm.nicolike.cn

Go:   // 手写循环
来源：http://lt.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ac.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://to.panjiajie.cn

[D15] 去重
来源：http://ob.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qk.shxzukj.cn

PHP:  array_unique($arr);
来源：http://yt.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://dv.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://ik.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ng.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bx.newstarts.cn

Ruby: arr.uniq
来源：http://yb.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ms.hahajie.cn

[D16] 求和与平均值
来源：http://ip.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vw.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cu.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tr.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dd.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dm.huanxung.cn

Go:   // 手写循环累加
来源：http://hr.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dr.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://je.lnxyls.cn

[D17] 最大值与最小值
来源：http://so.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://bf.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://my.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://es.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ev.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vr.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xf.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://hc.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://ne.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://rx.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vg.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ai.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ud.huixiangedu.cn

TS:   nested.flat();
来源：http://lk.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://li.huixiangedu.cn

Go:   // 手写双层循环
来源：http://nm.bookmarksfly.cn

Ruby: nested.flatten
来源：http://zt.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ub.shxzskj.cn

[D19] 按字段分组
来源：http://ly.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ew.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wp.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ll.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://al.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tp.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://ei.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sw.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://av.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://yr.wgjwhj.cn

Py:   Counter(arr)
来源：http://io.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://jy.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ss.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qy.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ly.9csxet.cn

Go:   // 手写 map[T]int
来源：http://bc.haigaiapp.cn

Ruby: arr.tally
来源：http://mv.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fk.nszjky.cn

[D21] 判断是否包含某元素
来源：http://hf.shxzskj.cn

Py:   x in arr
来源：http://km.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://ep.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://jj.huanxung.cn

TS:   arr.includes(x)
来源：http://wj.huixinmuqiang.cn

Java: list.contains(x)
来源：http://nk.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://pb.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://xs.hnjuh.cn

C#:   list.Contains(x)
来源：http://fm.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://az.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cf.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ny.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ld.muxihuayi.cn

TS:   [...arr];
来源：http://xy.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://ou.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yz.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://he.chemitech.net.cn

C#:   new List<int>(list);
来源：http://xf.muxihuayi.cn

[D23] reduce 累积计算
来源：http://on.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mp.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eo.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oc.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bg.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yi.9csxet.cn

Go:   // 手写循环
来源：http://rm.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ll.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pd.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://gk.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ez.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rc.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wc.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ky.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yt.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tu.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rs.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zz.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://mh.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://op.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vw.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ew.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://id.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rn.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pe.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://de.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sb.huixiangedu.cn

[D26] 数组转字符串
来源：http://rp.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://ch.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://wi.nicolike.cn

JS:   arr.join(", ")
来源：http://rp.chemitech.net.cn

TS:   arr.join(", ")
来源：http://sl.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://az.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://lk.nicolike.cn

Ruby: arr.join(", ")
来源：http://tm.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://jk.jctech888.com.cn

================================================================================
来源：http://xw.newstarts.cn

E. 字符串处理
来源：http://pp.chemitech.net.cn

================================================================================
来源：http://si.nszjky.cn

[E01] 拼接字符串
来源：http://qv.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ub.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jo.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ud.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eo.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://se.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ni.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yu.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mz.bjjhwx.cn

[E02] 重复字符串
来源：http://gp.lnxyls.cn

Py:   "ab" * 3
来源：http://sr.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://xm.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://yv.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://xj.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://qm.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://tl.huanxung.cn

Ruby: "ab" * 3
来源：http://ua.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cg.haigaiapp.cn

[E03] 截取子串
来源：http://jl.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://we.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fc.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tx.huanxung.cn

TS:   s.slice(1, 4)
来源：http://uz.nszjky.cn

Java: s.substring(1, 4)
来源：http://to.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ac.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qr.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ao.nicolike.cn

[E04] 查找子串位置
来源：http://rs.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ia.muxihuayi.cn


<!-- 参考信息 -->