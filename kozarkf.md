代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ks.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ha.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://nu.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://er.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://zx.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://zx.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gm.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://gv.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qd.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pb.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qo.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oy.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ta.gzmigu.cn

Go:   func add(a, b int) int
来源：http://dl.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tq.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nx.szxytkj.cn

[C14] 泛型函数
来源：http://zi.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kc.bjjhwx.cn

PHP:  // 无泛型
来源：http://lv.chemitech.net.cn

JS:   // 无泛型
来源：http://cc.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kx.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iv.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fa.hahajie.cn

Ruby: # 无泛型
来源：http://kn.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oc.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://av.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wz.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://mv.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hc.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ti.9csxet.cn

Java: // 无解构
来源：http://ay.shxzukj.cn

Go:   // 无解构
来源：http://nv.muxihuayi.cn

Ruby: a, b = pair
来源：http://im.hahajie.cn

C#:   var (a, b) = pair;
来源：http://dp.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ch.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lo.szxytkj.cn

PHP:  // 无重载
来源：http://jh.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://of.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://qd.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uh.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ie.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://xf.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sn.gzmigu.cn

================================================================================
来源：http://ae.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://ex.colortex.cn

================================================================================
来源：http://jl.nicolike.cn

[D01] 创建数组 / 列表
来源：http://js.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hw.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lc.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://em.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cj.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pb.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://sc.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qy.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://fv.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yc.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://av.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://pd.nszjky.cn

TS:   arr.push(4);
来源：http://nj.nszjky.cn

Java: list.add(4);
来源：http://pi.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://aw.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://sv.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://hq.nicolike.cn

[D03] 在指定位置插入元素
来源：http://rc.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://la.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vb.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zj.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://yl.hahajie.cn

Java: list.add(0, 0);
来源：http://lr.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hb.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ap.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://pi.shxzukj.cn

[D04] 删除元素
来源：http://pj.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fb.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vm.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ql.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://zl.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kc.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uu.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xk.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nr.gzmigu.cn

[D05] 访问与修改元素
来源：http://xx.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ro.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://do.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ie.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://zu.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://sj.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://dx.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://du.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aa.colortex.cn

[D06] 数组长度
来源：http://ar.hnjuh.cn

Py:   len(arr)
来源：http://dy.521024.cn

PHP:  count($arr);
来源：http://ng.shxzskj.cn

JS:   arr.length
来源：http://wn.wgjwhj.cn

TS:   arr.length
来源：http://ok.huixiangedu.cn

Java: list.size();
来源：http://pg.hnjuh.cn

Go:   len(arr)
来源：http://mh.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://yy.chemitech.net.cn

C#:   list.Count;
来源：http://vq.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://wc.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ne.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ml.asd995.cn

JS:   arr.slice(1, 4);
来源：http://wt.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ei.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://eq.wgjwhj.cn

Go:   arr[1:4]
来源：http://hh.nszjky.cn

Ruby: arr[1, 3]
来源：http://hp.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://pz.szxytkj.cn

[D08] 合并两个数组
来源：http://xu.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://qm.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://zf.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tg.9csxet.cn

TS:   [...a, ...b];
来源：http://ym.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vg.yuexingan06.cn

Go:   append(a, b...)
来源：http://dq.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://ga.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://dy.hahajie.cn

[D09] 排序（升序）
来源：http://eu.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://qt.shtwfgs.cn

PHP:  sort($arr);
来源：http://op.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ol.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://do.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wg.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zx.huanxung.cn

Ruby: arr.sort
来源：http://ty.shtwfgs.cn

C#:   list.Sort();
来源：http://cx.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zp.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://op.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kt.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vg.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ah.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://is.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jz.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wj.muxihuayi.cn

[D11] 反转数组
来源：http://az.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://js.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://ro.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bs.szxytkj.cn

TS:   [...arr].reverse();
来源：http://aa.hnjuh.cn

Java: Collections.reverse(list);
来源：http://cs.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://dr.haigaiapp.cn

Ruby: arr.reverse
来源：http://ll.muxihuayi.cn

C#:   list.Reverse();
来源：http://zc.haigaiapp.cn

[D12] 查找元素下标
来源：http://xv.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://hl.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://id.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aw.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nb.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sh.521024.cn

Go:   slices.Index(arr, x)
来源：http://at.colortex.cn

Ruby: arr.index(x)
来源：http://sq.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ty.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://ip.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nz.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pi.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://pn.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://xy.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wp.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kf.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ra.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hd.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://li.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ud.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yr.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://il.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://ms.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://is.wgjwhj.cn

Go:   // 手写循环
来源：http://ce.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vq.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://au.huixiangedu.cn

[D15] 去重
来源：http://gs.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pj.shxzskj.cn

PHP:  array_unique($arr);
来源：http://rj.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://vq.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://il.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fd.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wv.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://hm.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://aj.nszjky.cn

[D16] 求和与平均值
来源：http://be.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://it.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sw.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kl.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gm.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mc.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://rj.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nq.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://nc.yuexingan06.cn

[D17] 最大值与最小值
来源：http://qg.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://xc.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://eu.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ep.521024.cn

TS:   Math.max(...arr);
来源：http://kl.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ju.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lx.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://lh.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://bv.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://jz.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dq.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://xs.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://af.shxzukj.cn

TS:   nested.flat();
来源：http://bm.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ez.panjiajie.cn

Go:   // 手写双层循环
来源：http://ew.bookmarksfly.cn

Ruby: nested.flatten
来源：http://nn.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hv.nszjky.cn

[D19] 按字段分组
来源：http://mx.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ah.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zy.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cn.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://os.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zo.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://vo.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://js.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hb.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://nt.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://rp.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://jx.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vu.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xb.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wu.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://uf.gzmigu.cn

Ruby: arr.tally
来源：http://rx.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lp.9csxet.cn

[D21] 判断是否包含某元素
来源：http://kp.lnxyls.cn

Py:   x in arr
来源：http://ou.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://cc.wgjwhj.cn

JS:   arr.includes(x)
来源：http://ea.jctech888.com.cn

TS:   arr.includes(x)
来源：http://kl.521024.cn

Java: list.contains(x)
来源：http://rv.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://cn.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://gs.lnxyls.cn

C#:   list.Contains(x)
来源：http://dz.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://zb.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ly.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bm.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xo.huixiangedu.cn

TS:   [...arr];
来源：http://tg.hahajie.cn

Java: new ArrayList<>(list);
来源：http://sd.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qv.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://oz.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://lg.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://bw.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bz.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hm.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vi.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tq.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cg.chemitech.net.cn

Go:   // 手写循环
来源：http://jv.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hw.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bt.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://cw.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kw.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vn.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mz.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nn.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ez.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yy.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://se.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ro.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://rb.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eq.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ye.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mh.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qg.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zp.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qq.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mk.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yf.jctech888.com.cn

[D26] 数组转字符串
来源：http://el.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://qe.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://da.nicolike.cn

JS:   arr.join(", ")
来源：http://sh.chemitech.net.cn

TS:   arr.join(", ")
来源：http://tm.panjiajie.cn

Java: String.join(", ", list)
来源：http://gf.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://sl.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://db.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ge.jianghongdianzi.cn

================================================================================
来源：http://gq.jctech888.com.cn

E. 字符串处理
来源：http://nk.nszjky.cn

================================================================================
来源：http://tw.szxytkj.cn

[E01] 拼接字符串
来源：http://sh.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ys.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lr.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xq.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ex.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bf.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nd.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ty.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vw.shtwfgs.cn

[E02] 重复字符串
来源：http://yt.bookmarksfly.cn

Py:   "ab" * 3
来源：http://rb.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://sh.huanxung.cn

JS:   "ab".repeat(3)
来源：http://op.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://pj.newstarts.cn

Java: "ab".repeat(3)
来源：http://um.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://om.yuexingan06.cn

Ruby: "ab" * 3
来源：http://vm.huixinmuqiang.cn


<!-- 参考信息 -->