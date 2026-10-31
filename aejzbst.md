代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://nr.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://yo.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aa.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://vz.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mn.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oz.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gb.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lt.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://il.hnjuh.cn

Go:   func add(a, b int) int
来源：http://zl.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://km.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yd.wgjwhj.cn

[C14] 泛型函数
来源：http://en.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cy.wgjwhj.cn

PHP:  // 无泛型
来源：http://xx.huixiangedu.cn

JS:   // 无泛型
来源：http://kt.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rc.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ct.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wn.szsharing.cn

Ruby: # 无泛型
来源：http://da.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yv.asd995.cn

[C15] 解构 / 展开参数
来源：http://rn.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xy.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://fu.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qa.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yi.yuexingan06.cn

Java: // 无解构
来源：http://yn.gzmigu.cn

Go:   // 无解构
来源：http://cg.hahajie.cn

Ruby: a, b = pair
来源：http://lh.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://np.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://hv.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qq.huixinmuqiang.cn

PHP:  // 无重载
来源：http://mx.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://id.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://ha.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ga.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://iu.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://dh.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kh.lnxyls.cn

================================================================================
来源：http://gd.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ya.gzmigu.cn

================================================================================
来源：http://ci.asd995.cn

[D01] 创建数组 / 列表
来源：http://sj.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jm.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fd.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ek.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dq.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jb.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ac.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://oj.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rv.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://rj.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gm.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ic.muxihuayi.cn

JS:   arr.push(4);
来源：http://ct.nicolike.cn

TS:   arr.push(4);
来源：http://pf.asd995.cn

Java: list.add(4);
来源：http://tm.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://vn.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://uk.gzmigu.cn

C#:   list.Add(4);
来源：http://rk.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://oe.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://lh.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pu.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gz.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://of.jctech888.com.cn

Java: list.add(0, 0);
来源：http://vv.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kk.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bn.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://wy.bjjhwx.cn

[D04] 删除元素
来源：http://ld.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yj.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vk.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ig.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://rk.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nc.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sc.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vw.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mc.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://nz.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sj.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nk.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qp.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://dw.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://cw.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://xg.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ic.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tr.shtwfgs.cn

[D06] 数组长度
来源：http://rw.521024.cn

Py:   len(arr)
来源：http://nl.shxzskj.cn

PHP:  count($arr);
来源：http://sy.nszjky.cn

JS:   arr.length
来源：http://kq.bjjhwx.cn

TS:   arr.length
来源：http://ug.bookmarksfly.cn

Java: list.size();
来源：http://uw.asd995.cn

Go:   len(arr)
来源：http://uy.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://on.panjiajie.cn

C#:   list.Count;
来源：http://od.asd995.cn

[D07] 切片 / 取子数组
来源：http://lh.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xt.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nv.asd995.cn

JS:   arr.slice(1, 4);
来源：http://rc.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://au.gzmigu.cn

Java: list.subList(1, 4);
来源：http://dr.huixiangedu.cn

Go:   arr[1:4]
来源：http://ui.huanxung.cn

Ruby: arr[1, 3]
来源：http://wz.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://zc.szxytkj.cn

[D08] 合并两个数组
来源：http://pf.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://vu.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://vw.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ok.asd995.cn

TS:   [...a, ...b];
来源：http://vf.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hy.shxzukj.cn

Go:   append(a, b...)
来源：http://gv.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://pi.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://qf.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://vi.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ju.haigaiapp.cn

PHP:  sort($arr);
来源：http://pn.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zj.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ep.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ic.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ko.newstarts.cn

Ruby: arr.sort
来源：http://zb.chemitech.net.cn

C#:   list.Sort();
来源：http://kz.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rr.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fl.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ch.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cs.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jn.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cy.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kp.shtwfgs.cn

[D11] 反转数组
来源：http://mz.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ly.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://mm.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hj.huanxung.cn

TS:   [...arr].reverse();
来源：http://yc.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://mj.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ze.haigaiapp.cn

Ruby: arr.reverse
来源：http://iy.colortex.cn

C#:   list.Reverse();
来源：http://pe.haigaiapp.cn

[D12] 查找元素下标
来源：http://at.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://jt.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ws.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eh.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aw.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://il.asd995.cn

Go:   slices.Index(arr, x)
来源：http://eb.haigaiapp.cn

Ruby: arr.index(x)
来源：http://bu.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://vu.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://dt.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ie.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://de.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://dp.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ep.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oy.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wi.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lt.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ge.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://wg.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ii.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rb.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://mm.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://qa.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://um.bjjhwx.cn

Go:   // 手写循环
来源：http://xz.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ia.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://np.asd995.cn

[D15] 去重
来源：http://xs.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ub.hnjuh.cn

PHP:  array_unique($arr);
来源：http://nz.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://us.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://uh.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zr.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ai.yuexingan06.cn

Ruby: arr.uniq
来源：http://xi.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://wj.newstarts.cn

[D16] 求和与平均值
来源：http://am.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://av.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pt.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xb.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mh.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dl.panjiajie.cn

Go:   // 手写循环累加
来源：http://yn.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xf.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://tk.521024.cn

[D17] 最大值与最小值
来源：http://tm.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://wb.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ek.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gv.shxzukj.cn

TS:   Math.max(...arr);
来源：http://vq.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wh.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vj.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ac.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://sd.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://rf.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uf.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://dn.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ke.521024.cn

TS:   nested.flat();
来源：http://tn.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jg.szsharing.cn

Go:   // 手写双层循环
来源：http://kk.gzmigu.cn

Ruby: nested.flatten
来源：http://oi.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qp.newstarts.cn

[D19] 按字段分组
来源：http://pm.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lz.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ef.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ho.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ou.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nk.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://ji.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oq.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zo.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://tg.colortex.cn

Py:   Counter(arr)
来源：http://kz.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://jf.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rd.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vh.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gc.huanxung.cn

Go:   // 手写 map[T]int
来源：http://vm.yuntaijiaju.cn

Ruby: arr.tally
来源：http://vx.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ot.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://ht.colortex.cn

Py:   x in arr
来源：http://tb.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://zs.nicolike.cn

JS:   arr.includes(x)
来源：http://ag.shxzukj.cn

TS:   arr.includes(x)
来源：http://ce.jianghongdianzi.cn

Java: list.contains(x)
来源：http://oy.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://il.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://yl.nicolike.cn

C#:   list.Contains(x)
来源：http://uz.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://eq.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nj.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hn.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dy.nszjky.cn

TS:   [...arr];
来源：http://jc.asd995.cn

Java: new ArrayList<>(list);
来源：http://it.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ek.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://qz.panjiajie.cn

C#:   new List<int>(list);
来源：http://dm.hnjuh.cn

[D23] reduce 累积计算
来源：http://zr.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sv.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cu.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fs.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://me.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://co.huixiangedu.cn

Go:   // 手写循环
来源：http://ol.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dv.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yc.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://jm.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dm.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xx.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wm.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://av.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://li.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cp.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bz.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://by.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ef.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rw.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pj.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bz.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oh.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://su.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://de.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xp.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nr.chemitech.net.cn

[D26] 数组转字符串
来源：http://yv.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://um.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://lr.hnjuh.cn

JS:   arr.join(", ")
来源：http://or.gzmigu.cn

TS:   arr.join(", ")
来源：http://cc.nicolike.cn

Java: String.join(", ", list)
来源：http://lk.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://ud.colortex.cn

Ruby: arr.join(", ")
来源：http://am.nicolike.cn

C#:   string.Join(", ", list)
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://mi.hnjuh.cn

E. 字符串处理
来源：http://sa.jianghongdianzi.cn

================================================================================
来源：http://ei.gzmigu.cn

[E01] 拼接字符串
来源：http://eg.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ov.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kn.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dk.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jf.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ol.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cm.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gn.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hc.jctech888.com.cn

[E02] 重复字符串
来源：http://jh.nicolike.cn

Py:   "ab" * 3
来源：http://vr.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ux.colortex.cn

JS:   "ab".repeat(3)
来源：http://ef.hahajie.cn

TS:   "ab".repeat(3)
来源：http://kl.nszjky.cn

Java: "ab".repeat(3)
来源：http://bb.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://jp.colortex.cn

Ruby: "ab" * 3
来源：http://pr.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bz.gzmigu.cn

[E03] 截取子串
来源：http://db.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fv.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lt.yuexingan06.cn


<!-- 参考信息 -->