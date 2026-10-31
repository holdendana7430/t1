代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yi.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://la.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ez.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sj.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://px.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://df.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://px.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gt.yuexingan06.cn

[C14] 泛型函数
来源：http://tc.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rp.nszjky.cn

PHP:  // 无泛型
来源：http://do.shtwfgs.cn

JS:   // 无泛型
来源：http://yg.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mx.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jt.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gy.haigaiapp.cn

Ruby: # 无泛型
来源：http://ed.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kb.hahajie.cn

[C15] 解构 / 展开参数
来源：http://qd.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uz.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://da.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://al.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sx.lnxyls.cn

Java: // 无解构
来源：http://vq.nszjky.cn

Go:   // 无解构
来源：http://gg.asd995.cn

Ruby: a, b = pair
来源：http://vh.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ld.521024.cn

[C16] 函数 / 方法重载
来源：http://um.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fz.shtwfgs.cn

PHP:  // 无重载
来源：http://mk.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dv.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ih.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pf.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://gc.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ou.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ps.bjjhwx.cn

================================================================================
来源：http://ll.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://hy.lnxyls.cn

================================================================================
来源：http://ua.nszjky.cn

[D01] 创建数组 / 列表
来源：http://rx.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jz.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ss.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oy.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vr.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ak.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://eh.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://hn.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ia.gzmigu.cn

[D02] 追加元素到末尾
来源：http://bd.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zi.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mu.panjiajie.cn

JS:   arr.push(4);
来源：http://ve.newstarts.cn

TS:   arr.push(4);
来源：http://tn.asd995.cn

Java: list.add(4);
来源：http://vs.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://kr.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://pc.colortex.cn

C#:   list.Add(4);
来源：http://ze.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://rr.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://ne.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ko.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rj.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://kq.shxzskj.cn

Java: list.add(0, 0);
来源：http://gk.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jm.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ij.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://uo.jctech888.com.cn

[D04] 删除元素
来源：http://yv.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://py.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rx.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hb.asd995.cn

TS:   arr.splice(0, 1);
来源：http://jh.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ao.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ht.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://er.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gf.haigaiapp.cn

[D05] 访问与修改元素
来源：http://oe.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bs.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dn.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iy.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://kb.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://zn.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://op.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cx.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ud.newstarts.cn

[D06] 数组长度
来源：http://hz.yuexingan06.cn

Py:   len(arr)
来源：http://kv.szsharing.cn

PHP:  count($arr);
来源：http://ex.huixiangedu.cn

JS:   arr.length
来源：http://fa.521024.cn

TS:   arr.length
来源：http://ct.jianghongdianzi.cn

Java: list.size();
来源：http://bi.szxytkj.cn

Go:   len(arr)
来源：http://nw.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://sk.szsharing.cn

C#:   list.Count;
来源：http://zq.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://hp.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pb.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yb.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ut.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://st.shxzskj.cn

Java: list.subList(1, 4);
来源：http://zh.szsharing.cn

Go:   arr[1:4]
来源：http://nk.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ao.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://km.bjjhwx.cn

[D08] 合并两个数组
来源：http://pm.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://wb.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://pt.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gg.shxzskj.cn

TS:   [...a, ...b];
来源：http://hs.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ok.colortex.cn

Go:   append(a, b...)
来源：http://uy.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://sy.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://dx.gzmigu.cn

[D09] 排序（升序）
来源：http://jc.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ga.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://no.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ud.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ps.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rd.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gw.shxzskj.cn

Ruby: arr.sort
来源：http://qm.haigaiapp.cn

C#:   list.Sort();
来源：http://nq.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qp.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nl.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zo.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yw.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dz.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cf.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zl.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tq.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ya.jianghongdianzi.cn

[D11] 反转数组
来源：http://qn.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://en.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://rk.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ky.asd995.cn

TS:   [...arr].reverse();
来源：http://rq.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://kf.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://oz.nicolike.cn

Ruby: arr.reverse
来源：http://co.gzmigu.cn

C#:   list.Reverse();
来源：http://jh.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://oo.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://by.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zh.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pv.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ge.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://io.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://mb.shxzukj.cn

Ruby: arr.index(x)
来源：http://uj.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://yu.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://qk.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tx.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ub.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://bx.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://ku.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gp.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jf.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ay.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dx.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://kp.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dk.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://or.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://yg.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://as.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bf.yuexingan06.cn

Go:   // 手写循环
来源：http://dg.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ji.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuntaijiaju.cn

[D15] 去重
来源：http://jm.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vm.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://ec.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://py.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://go.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zh.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nu.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://kn.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://cw.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://sm.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ch.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oq.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jo.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jz.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bs.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://bl.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gs.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://kz.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://tt.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://rp.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://jy.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uq.szsharing.cn

TS:   Math.max(...arr);
来源：http://nx.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bh.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xk.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://ff.colortex.cn

C#:   list.Max();  list.Min()
来源：http://li.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://yw.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ng.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://hl.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gt.muxihuayi.cn

TS:   nested.flat();
来源：http://ii.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ek.gzmigu.cn

Go:   // 手写双层循环
来源：http://xy.panjiajie.cn

Ruby: nested.flatten
来源：http://dn.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ro.bookmarksfly.cn

[D19] 按字段分组
来源：http://ro.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ds.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vg.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nl.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mx.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pf.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://tb.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bp.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ym.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ik.hnjuh.cn

Py:   Counter(arr)
来源：http://qc.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://oa.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vr.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zc.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eh.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://xi.szsharing.cn

Ruby: arr.tally
来源：http://oz.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zt.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://tp.521024.cn

Py:   x in arr
来源：http://qq.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://hk.szsharing.cn

JS:   arr.includes(x)
来源：http://yr.shxzukj.cn

TS:   arr.includes(x)
来源：http://aw.9csxet.cn

Java: list.contains(x)
来源：http://be.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://ey.colortex.cn

Ruby: arr.include?(x)
来源：http://rb.haigaiapp.cn

C#:   list.Contains(x)
来源：http://bj.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://be.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lr.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mi.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aw.shxzukj.cn

TS:   [...arr];
来源：http://ov.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://qx.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kk.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://oo.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ze.muxihuayi.cn

[D23] reduce 累积计算
来源：http://iy.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://az.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xr.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bq.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jo.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fm.panjiajie.cn

Go:   // 手写循环
来源：http://sl.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://od.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xx.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://es.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oh.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tj.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kc.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jn.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vd.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rh.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bi.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://kw.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iy.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ha.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ul.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rx.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dn.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mb.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://do.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ht.bookmarksfly.cn

[D26] 数组转字符串
来源：http://gi.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://qq.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://qd.colortex.cn

JS:   arr.join(", ")
来源：http://ox.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://sw.9csxet.cn

Java: String.join(", ", list)
来源：http://dt.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://km.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://zi.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://be.szxytkj.cn

================================================================================
来源：http://nk.huanxung.cn

E. 字符串处理
来源：http://af.shxzukj.cn

================================================================================
来源：http://mi.szsharing.cn

[E01] 拼接字符串
来源：http://sf.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oi.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pn.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uy.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ny.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cs.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tp.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cf.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qh.huixinmuqiang.cn

[E02] 重复字符串
来源：http://tg.haigaiapp.cn

Py:   "ab" * 3
来源：http://mp.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://dk.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://yc.nszjky.cn

TS:   "ab".repeat(3)
来源：http://df.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://vu.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://sk.hnjuh.cn

Ruby: "ab" * 3
来源：http://pu.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://we.yuntaijiaju.cn

[E03] 截取子串
来源：http://dx.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jd.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://az.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wg.colortex.cn

TS:   s.slice(1, 4)
来源：http://lc.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://en.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rs.wgjwhj.cn


<!-- 参考信息 -->