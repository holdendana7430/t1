代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://tq.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ku.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pk.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://by.shxzukj.cn

[C14] 泛型函数
来源：http://jt.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://id.hahajie.cn

PHP:  // 无泛型
来源：http://zw.jctech888.com.cn

JS:   // 无泛型
来源：http://uc.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://la.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cz.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xj.shtwfgs.cn

Ruby: # 无泛型
来源：http://iu.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ym.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ke.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dq.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://mg.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gb.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bj.muxihuayi.cn

Java: // 无解构
来源：http://yf.haigaiapp.cn

Go:   // 无解构
来源：http://bt.shtwfgs.cn

Ruby: a, b = pair
来源：http://kv.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ck.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://hm.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mc.bjjhwx.cn

PHP:  // 无重载
来源：http://cj.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nd.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://ra.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ve.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://tw.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://ew.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ae.lnxyls.cn

================================================================================
来源：http://kp.521024.cn

D. 数组 / 列表 / 集合
来源：http://ze.szxytkj.cn

================================================================================
来源：http://nl.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://hj.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ax.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dc.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tf.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hh.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rq.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://du.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://mi.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kx.hahajie.cn

[D02] 追加元素到末尾
来源：http://jf.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zs.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ft.szsharing.cn

JS:   arr.push(4);
来源：http://br.panjiajie.cn

TS:   arr.push(4);
来源：http://zu.huanxung.cn

Java: list.add(4);
来源：http://qq.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://be.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://ks.hahajie.cn

C#:   list.Add(4);
来源：http://rm.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://uy.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://hj.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hv.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tj.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://hu.hahajie.cn

Java: list.add(0, 0);
来源：http://ib.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bx.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zx.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://kv.hnjuh.cn

[D04] 删除元素
来源：http://oj.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sz.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wi.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oz.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ah.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dn.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://na.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://my.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tw.colortex.cn

[D05] 访问与修改元素
来源：http://yr.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sy.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://es.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lk.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://hq.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://sy.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://gh.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wa.yuntaijiaju.cn

[D06] 数组长度
来源：http://qq.huixiangedu.cn

Py:   len(arr)
来源：http://kl.yuexingan06.cn

PHP:  count($arr);
来源：http://pc.bookmarksfly.cn

JS:   arr.length
来源：http://rf.shtwfgs.cn

TS:   arr.length
来源：http://nm.colortex.cn

Java: list.size();
来源：http://ef.huanxung.cn

Go:   len(arr)
来源：http://dy.nszjky.cn

Ruby: arr.length; arr.size
来源：http://ij.gzmigu.cn

C#:   list.Count;
来源：http://jr.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://jb.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ci.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xb.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://dv.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://xg.szxytkj.cn

Java: list.subList(1, 4);
来源：http://ct.colortex.cn

Go:   arr[1:4]
来源：http://tw.nszjky.cn

Ruby: arr[1, 3]
来源：http://xk.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://kq.huixiangedu.cn

[D08] 合并两个数组
来源：http://wp.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://kl.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://gv.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vr.hnjuh.cn

TS:   [...a, ...b];
来源：http://im.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yi.9csxet.cn

Go:   append(a, b...)
来源：http://ro.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://fv.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://hu.asd995.cn

[D09] 排序（升序）
来源：http://dv.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://my.shxzukj.cn

PHP:  sort($arr);
来源：http://be.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zf.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qg.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eb.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pj.lnxyls.cn

Ruby: arr.sort
来源：http://xe.hahajie.cn

C#:   list.Sort();
来源：http://id.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hh.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mh.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ms.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ix.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vr.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zp.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wv.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fu.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://px.chemitech.net.cn

[D11] 反转数组
来源：http://nj.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ws.nicolike.cn

PHP:  array_reverse($arr);
来源：http://gd.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xo.huanxung.cn

TS:   [...arr].reverse();
来源：http://fh.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://fl.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://yd.szxytkj.cn

Ruby: arr.reverse
来源：http://fc.bookmarksfly.cn

C#:   list.Reverse();
来源：http://vk.chemitech.net.cn

[D12] 查找元素下标
来源：http://fz.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://xq.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uc.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qn.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://om.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cm.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://as.colortex.cn

Ruby: arr.index(x)
来源：http://ez.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ut.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://wy.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nv.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ll.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://xc.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://nf.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pf.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ed.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zj.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sx.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://hl.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gz.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xc.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://ob.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://ds.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xr.jctech888.com.cn

Go:   // 手写循环
来源：http://ry.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vz.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://og.colortex.cn

[D15] 去重
来源：http://ui.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pr.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ey.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://rj.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://fe.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wj.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kq.colortex.cn

Ruby: arr.uniq
来源：http://dc.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://mt.huanxung.cn

[D16] 求和与平均值
来源：http://jb.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ts.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qj.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://er.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yh.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gu.shxzukj.cn

Go:   // 手写循环累加
来源：http://gx.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rj.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://lg.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ap.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ty.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ep.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hb.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://mo.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://px.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nj.521024.cn

Ruby: arr.max;  arr.min
来源：http://ht.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://tq.521024.cn

[D18] 扁平化嵌套数组
来源：http://gh.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bx.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://fa.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ws.gzmigu.cn

TS:   nested.flat();
来源：http://kx.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bq.521024.cn

Go:   // 手写双层循环
来源：http://xa.asd995.cn

Ruby: nested.flatten
来源：http://qg.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yf.yuexingan06.cn

[D19] 按字段分组
来源：http://jz.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jp.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wu.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ho.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xc.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eg.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://ga.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tk.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cl.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://uo.lnxyls.cn

Py:   Counter(arr)
来源：http://db.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://nt.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rh.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wc.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ob.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://je.nicolike.cn

Ruby: arr.tally
来源：http://ra.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zp.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://jj.9csxet.cn

Py:   x in arr
来源：http://yw.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://rp.shxzskj.cn

JS:   arr.includes(x)
来源：http://jl.panjiajie.cn

TS:   arr.includes(x)
来源：http://ok.shxzskj.cn

Java: list.contains(x)
来源：http://aq.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://fw.asd995.cn

Ruby: arr.include?(x)
来源：http://sh.bjjhwx.cn

C#:   list.Contains(x)
来源：http://bs.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://tg.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vw.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oh.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fs.hahajie.cn

TS:   [...arr];
来源：http://qq.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://hs.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ek.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://yp.nicolike.cn

C#:   new List<int>(list);
来源：http://oz.panjiajie.cn

[D23] reduce 累积计算
来源：http://uc.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nq.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tv.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oq.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://au.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ye.hnjuh.cn

Go:   // 手写循环
来源：http://fh.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://la.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://om.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://cw.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lt.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mq.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ka.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lc.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://is.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://px.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cv.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sg.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://mc.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vj.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xg.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gn.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zm.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yr.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ue.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gy.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aa.jctech888.com.cn

[D26] 数组转字符串
来源：http://yy.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://uj.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://dm.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://jr.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ma.huanxung.cn

Java: String.join(", ", list)
来源：http://gc.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://rq.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://my.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://bz.panjiajie.cn

================================================================================
来源：http://ko.shxzukj.cn

E. 字符串处理
来源：http://io.newstarts.cn

================================================================================
来源：http://qf.bjjhwx.cn

[E01] 拼接字符串
来源：http://gu.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dm.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vy.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fz.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nx.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nq.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yo.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gg.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pv.haigaiapp.cn

[E02] 重复字符串
来源：http://pf.521024.cn

Py:   "ab" * 3
来源：http://ts.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://ze.hahajie.cn

JS:   "ab".repeat(3)
来源：http://ov.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://ij.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://nv.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://ow.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ic.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://af.newstarts.cn

[E03] 截取子串
来源：http://so.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tc.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dq.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://om.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ar.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://cb.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ec.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bs.colortex.cn

C#:   s.Substring(1, 3)
来源：http://il.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://jg.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://fz.lnxyls.cn


<!-- 参考信息 -->