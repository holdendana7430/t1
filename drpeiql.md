代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://rr.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://fq.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://gk.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ew.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://uy.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://id.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qz.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://zw.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pv.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mo.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xl.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://as.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sy.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ok.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mj.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sk.bjjhwx.cn

[C14] 泛型函数
来源：http://og.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zi.gzmigu.cn

PHP:  // 无泛型
来源：http://pa.hahajie.cn

JS:   // 无泛型
来源：http://ys.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ha.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wu.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ir.huanxung.cn

Ruby: # 无泛型
来源：http://hy.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fy.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://pr.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vj.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://cz.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zk.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mx.huixinmuqiang.cn

Java: // 无解构
来源：http://uc.9csxet.cn

Go:   // 无解构
来源：http://xv.wgjwhj.cn

Ruby: a, b = pair
来源：http://rg.521024.cn

C#:   var (a, b) = pair;
来源：http://jx.nszjky.cn

[C16] 函数 / 方法重载
来源：http://oh.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nh.wgjwhj.cn

PHP:  // 无重载
来源：http://fu.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wd.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://be.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xp.521024.cn

Go:   // 无重载：用不同函数名
来源：http://vo.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://md.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yh.lnxyls.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://te.nszjky.cn

================================================================================
来源：http://dm.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://lh.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cf.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ri.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oo.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dr.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tz.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://it.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://rz.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hk.nicolike.cn

[D02] 追加元素到末尾
来源：http://xw.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fs.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gc.9csxet.cn

JS:   arr.push(4);
来源：http://tl.bookmarksfly.cn

TS:   arr.push(4);
来源：http://bx.hahajie.cn

Java: list.add(4);
来源：http://qw.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://xf.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ix.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://kk.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://ue.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://qi.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fz.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qg.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ge.nicolike.cn

Java: list.add(0, 0);
来源：http://dq.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vm.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tm.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://bt.yuexingan06.cn

[D04] 删除元素
来源：http://gk.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://om.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gz.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gp.521024.cn

TS:   arr.splice(0, 1);
来源：http://ho.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jz.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iu.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xu.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fq.bjjhwx.cn

[D05] 访问与修改元素
来源：http://mg.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wx.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fa.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ub.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://nj.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://hs.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ie.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fb.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ef.huixiangedu.cn

[D06] 数组长度
来源：http://md.hahajie.cn

Py:   len(arr)
来源：http://kh.asd995.cn

PHP:  count($arr);
来源：http://mn.szxytkj.cn

JS:   arr.length
来源：http://zi.jianghongdianzi.cn

TS:   arr.length
来源：http://fr.szxytkj.cn

Java: list.size();
来源：http://pj.muxihuayi.cn

Go:   len(arr)
来源：http://zy.9csxet.cn

Ruby: arr.length; arr.size
来源：http://sq.huanxung.cn

C#:   list.Count;
来源：http://uy.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://uq.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qq.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kg.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://jk.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://jl.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://lo.shxzskj.cn

Go:   arr[1:4]
来源：http://ds.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zl.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ik.shxzukj.cn

[D08] 合并两个数组
来源：http://dg.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://ym.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://au.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fc.hahajie.cn

TS:   [...a, ...b];
来源：http://cf.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lr.hahajie.cn

Go:   append(a, b...)
来源：http://vn.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://nz.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://dj.bjjhwx.cn

[D09] 排序（升序）
来源：http://ik.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://um.shtwfgs.cn

PHP:  sort($arr);
来源：http://yr.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ke.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://se.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wi.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xz.szxytkj.cn

Ruby: arr.sort
来源：http://qb.wgjwhj.cn

C#:   list.Sort();
来源：http://ge.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yj.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cu.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wx.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dj.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://er.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fg.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dy.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lq.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://co.yuntaijiaju.cn

[D11] 反转数组
来源：http://ga.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lv.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://yx.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://do.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://bz.shxzukj.cn

Java: Collections.reverse(list);
来源：http://jd.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://fk.lnxyls.cn

Ruby: arr.reverse
来源：http://vp.hnjuh.cn

C#:   list.Reverse();
来源：http://tn.shxzskj.cn

[D12] 查找元素下标
来源：http://qf.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://qg.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iw.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://di.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kp.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ea.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://fr.wgjwhj.cn

Ruby: arr.index(x)
来源：http://ea.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://dp.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://qe.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bb.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xj.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://gn.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://hn.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xr.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ah.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rq.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qt.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://dq.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qx.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yr.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ec.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://ek.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xw.szxytkj.cn

Go:   // 手写循环
来源：http://wr.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xl.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uc.521024.cn

[D15] 去重
来源：http://vs.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zm.szsharing.cn

PHP:  array_unique($arr);
来源：http://en.newstarts.cn

JS:   [...new Set(arr)]
来源：http://mc.huanxung.cn

TS:   [...new Set(arr)]
来源：http://qs.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gv.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xd.521024.cn

Ruby: arr.uniq
来源：http://bi.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ql.521024.cn

[D16] 求和与平均值
来源：http://zo.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ij.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pt.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lg.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kh.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ba.hahajie.cn

Go:   // 手写循环累加
来源：http://pi.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xu.521024.cn

C#:   list.Sum();  list.Average()
来源：http://li.shxzskj.cn

[D17] 最大值与最小值
来源：http://an.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://no.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ha.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ch.panjiajie.cn

TS:   Math.max(...arr);
来源：http://gn.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jf.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nf.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://yo.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://jj.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://dc.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pq.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://yu.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qd.huanxung.cn

TS:   nested.flat();
来源：http://zd.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fy.asd995.cn

Go:   // 手写双层循环
来源：http://pf.9csxet.cn

Ruby: nested.flatten
来源：http://ns.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cd.szsharing.cn

[D19] 按字段分组
来源：http://wa.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://av.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xs.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ae.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fr.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.asd995.cn

Go:   // 手写 map[string][]T
来源：http://pr.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://py.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cw.asd995.cn

[D20] 统计每个元素出现次数
来源：http://bo.jctech888.com.cn

Py:   Counter(arr)
来源：http://du.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ef.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zz.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ga.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ta.newstarts.cn

Go:   // 手写 map[T]int
来源：http://km.huixiangedu.cn

Ruby: arr.tally
来源：http://xm.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wk.colortex.cn

[D21] 判断是否包含某元素
来源：http://df.newstarts.cn

Py:   x in arr
来源：http://tw.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ym.gzmigu.cn

JS:   arr.includes(x)
来源：http://th.nszjky.cn

TS:   arr.includes(x)
来源：http://tx.jianghongdianzi.cn

Java: list.contains(x)
来源：http://bt.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://id.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://br.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://an.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://fj.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xa.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dj.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lr.521024.cn

TS:   [...arr];
来源：http://mz.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://jp.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dn.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://hi.shtwfgs.cn

C#:   new List<int>(list);
来源：http://wm.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://gz.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ix.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gd.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xw.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tx.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://on.asd995.cn

Go:   // 手写循环
来源：http://iy.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bi.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uh.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://ce.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ac.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rg.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qn.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wk.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pa.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jw.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ax.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xm.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://mx.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gi.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hs.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sl.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qh.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ej.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jc.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tu.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ws.wgjwhj.cn

[D26] 数组转字符串
来源：http://sb.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://zi.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://tz.shxzskj.cn

JS:   arr.join(", ")
来源：http://qs.huixiangedu.cn

TS:   arr.join(", ")
来源：http://iy.huanxung.cn

Java: String.join(", ", list)
来源：http://ev.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://ic.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://ws.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://ze.newstarts.cn

================================================================================
来源：http://ar.wgjwhj.cn

E. 字符串处理
来源：http://ex.huixinmuqiang.cn

================================================================================
来源：http://ld.muxihuayi.cn

[E01] 拼接字符串
来源：http://cn.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fp.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ws.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://my.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cb.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vk.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://be.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hi.hnjuh.cn

[E02] 重复字符串
来源：http://km.lnxyls.cn

Py:   "ab" * 3
来源：http://kj.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://vb.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://xd.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://wp.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://dk.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://gj.jctech888.com.cn

Ruby: "ab" * 3
来源：http://fx.521024.cn


<!-- 参考信息 -->