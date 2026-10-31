代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rs.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qt.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zo.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qs.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://hz.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pr.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xq.hnjuh.cn

[C14] 泛型函数
来源：http://jz.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jg.panjiajie.cn

PHP:  // 无泛型
来源：http://gz.huanxung.cn

JS:   // 无泛型
来源：http://ky.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yz.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lh.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vx.panjiajie.cn

Ruby: # 无泛型
来源：http://yu.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yv.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://jz.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sd.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://kc.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ma.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tp.jianghongdianzi.cn

Java: // 无解构
来源：http://ay.nszjky.cn

Go:   // 无解构
来源：http://lu.bjjhwx.cn

Ruby: a, b = pair
来源：http://vs.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://th.asd995.cn

[C16] 函数 / 方法重载
来源：http://zj.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wp.shtwfgs.cn

PHP:  // 无重载
来源：http://so.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://il.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://hs.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xl.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ks.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://zn.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rr.shtwfgs.cn

================================================================================
来源：http://nj.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://hb.shxzskj.cn

================================================================================
来源：http://yo.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://lz.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pn.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zi.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ub.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uj.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sf.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://be.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://rg.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://so.9csxet.cn

[D02] 追加元素到末尾
来源：http://rw.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wg.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iw.nszjky.cn

JS:   arr.push(4);
来源：http://dz.shxzukj.cn

TS:   arr.push(4);
来源：http://qt.jianghongdianzi.cn

Java: list.add(4);
来源：http://rq.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://wv.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://xm.9csxet.cn

C#:   list.Add(4);
来源：http://jg.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://af.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://ft.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sm.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wr.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://yb.hahajie.cn

Java: list.add(0, 0);
来源：http://ws.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bq.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dg.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ie.jctech888.com.cn

[D04] 删除元素
来源：http://ft.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jb.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ih.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vl.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://iy.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dt.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fv.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://up.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://de.shxzskj.cn

[D05] 访问与修改元素
来源：http://gk.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zs.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ok.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xk.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://qr.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ip.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://wp.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gn.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ck.hnjuh.cn

[D06] 数组长度
来源：http://do.colortex.cn

Py:   len(arr)
来源：http://fa.shtwfgs.cn

PHP:  count($arr);
来源：http://nb.shxzskj.cn

JS:   arr.length
来源：http://tq.nicolike.cn

TS:   arr.length
来源：http://us.jctech888.com.cn

Java: list.size();
来源：http://db.hnjuh.cn

Go:   len(arr)
来源：http://ca.huanxung.cn

Ruby: arr.length; arr.size
来源：http://oc.newstarts.cn

C#:   list.Count;
来源：http://mv.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://pr.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ii.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://km.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://hh.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://mu.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://pb.haigaiapp.cn

Go:   arr[1:4]
来源：http://xa.hnjuh.cn

Ruby: arr[1, 3]
来源：http://kt.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://tg.newstarts.cn

[D08] 合并两个数组
来源：http://qd.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://rk.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://un.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gm.jctech888.com.cn

TS:   [...a, ...b];
来源：http://et.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ek.yuexingan06.cn

Go:   append(a, b...)
来源：http://tv.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://jo.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://zp.bjjhwx.cn

[D09] 排序（升序）
来源：http://dv.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://fr.9csxet.cn

PHP:  sort($arr);
来源：http://xg.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://du.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jl.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://za.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gw.521024.cn

Ruby: arr.sort
来源：http://ry.huixinmuqiang.cn

C#:   list.Sort();
来源：http://nq.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cv.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rm.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sp.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://na.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://or.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oz.wgjwhj.cn

[D11] 反转数组
来源：http://xr.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hf.521024.cn

PHP:  array_reverse($arr);
来源：http://ni.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cu.szsharing.cn

TS:   [...arr].reverse();
来源：http://xp.lnxyls.cn

Java: Collections.reverse(list);
来源：http://ey.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://nd.hnjuh.cn

Ruby: arr.reverse
来源：http://kh.nicolike.cn

C#:   list.Reverse();
来源：http://ne.lnxyls.cn

[D12] 查找元素下标
来源：http://pz.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://li.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yd.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xg.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jo.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bs.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://du.colortex.cn

Ruby: arr.index(x)
来源：http://aw.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://wi.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://ot.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ab.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wo.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://lx.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://be.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sa.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mu.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ag.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ob.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://dk.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tj.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jn.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://oc.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://qz.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dc.lnxyls.cn

Go:   // 手写循环
来源：http://hv.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vf.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://va.jianghongdianzi.cn

[D15] 去重
来源：http://je.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xm.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://hn.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ao.colortex.cn

TS:   [...new Set(arr)]
来源：http://kc.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tc.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ex.wgjwhj.cn

Ruby: arr.uniq
来源：http://dl.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://uo.asd995.cn

[D16] 求和与平均值
来源：http://ca.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gf.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lp.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ac.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ns.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oj.hnjuh.cn

Go:   // 手写循环累加
来源：http://qw.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ka.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://zo.gzmigu.cn

[D17] 最大值与最小值
来源：http://kn.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://mk.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://ua.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pz.nicolike.cn

TS:   Math.max(...arr);
来源：http://tl.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://de.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jg.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ms.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://nb.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://vs.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ob.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://sd.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bz.nicolike.cn

TS:   nested.flat();
来源：http://fr.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ep.hahajie.cn

Go:   // 手写双层循环
来源：http://fi.chemitech.net.cn

Ruby: nested.flatten
来源：http://wx.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rd.hnjuh.cn

[D19] 按字段分组
来源：http://gp.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wz.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ex.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vo.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sk.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tt.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://bl.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qf.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ew.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://cx.newstarts.cn

Py:   Counter(arr)
来源：http://vw.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://fb.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fy.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qh.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://uv.szsharing.cn

Ruby: arr.tally
来源：http://oe.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ue.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://rj.wgjwhj.cn

Py:   x in arr
来源：http://wc.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://to.shtwfgs.cn

JS:   arr.includes(x)
来源：http://hx.yuexingan06.cn

TS:   arr.includes(x)
来源：http://jj.shxzskj.cn

Java: list.contains(x)
来源：http://ig.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ml.521024.cn

Ruby: arr.include?(x)
来源：http://fi.panjiajie.cn

C#:   list.Contains(x)
来源：http://vm.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://fz.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://im.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qc.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yt.lnxyls.cn

TS:   [...arr];
来源：http://ga.nszjky.cn

Java: new ArrayList<>(list);
来源：http://lv.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gw.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://nt.nicolike.cn

C#:   new List<int>(list);
来源：http://pz.nicolike.cn

[D23] reduce 累积计算
来源：http://vq.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nx.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fp.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://an.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xf.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fz.yuexingan06.cn

Go:   // 手写循环
来源：http://ux.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://va.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ax.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://zi.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bs.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ji.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jq.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ab.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gx.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jv.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ar.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ze.colortex.cn

[D25] Set 集合去重与交并差
来源：http://nd.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yz.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wf.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://et.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sk.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vk.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sl.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vv.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yo.bookmarksfly.cn

[D26] 数组转字符串
来源：http://pq.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ws.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://ay.bjjhwx.cn

JS:   arr.join(", ")
来源：http://gd.yuexingan06.cn

TS:   arr.join(", ")
来源：http://jh.gzmigu.cn

Java: String.join(", ", list)
来源：http://py.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://ok.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://zp.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://fn.panjiajie.cn

E. 字符串处理
来源：http://ro.shxzukj.cn

================================================================================
来源：http://gs.bookmarksfly.cn

[E01] 拼接字符串
来源：http://nn.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://va.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nv.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://no.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wp.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xy.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rc.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wu.huixiangedu.cn

[E02] 重复字符串
来源：http://lo.huanxung.cn

Py:   "ab" * 3
来源：http://ts.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://rq.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://yo.newstarts.cn

TS:   "ab".repeat(3)
来源：http://br.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://az.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://za.shxzskj.cn

Ruby: "ab" * 3
来源：http://cz.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yv.jctech888.com.cn

[E03] 截取子串
来源：http://ci.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cr.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bd.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bp.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://lu.gzmigu.cn

Java: s.substring(1, 4)
来源：http://ha.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sp.9csxet.cn


<!-- 参考信息 -->