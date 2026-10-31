代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://gd.nicolike.cn

C#:   using System.Text;
来源：http://gg.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://rx.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://ay.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://se.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://zr.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://hu.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pt.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://wt.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://hg.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qg.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://yr.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bd.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vs.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qb.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aj.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vx.colortex.cn

Go:   func add(a, b int) int
来源：http://oh.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rx.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sg.panjiajie.cn

[C14] 泛型函数
来源：http://em.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ov.yuexingan06.cn

PHP:  // 无泛型
来源：http://so.muxihuayi.cn

JS:   // 无泛型
来源：http://lr.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xa.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tz.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zg.shtwfgs.cn

Ruby: # 无泛型
来源：http://mj.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iy.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://ja.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ic.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://jq.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://er.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ii.colortex.cn

Java: // 无解构
来源：http://rr.521024.cn

Go:   // 无解构
来源：http://by.yuexingan06.cn

Ruby: a, b = pair
来源：http://cl.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://me.newstarts.cn

[C16] 函数 / 方法重载
来源：http://bz.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aw.huixinmuqiang.cn

PHP:  // 无重载
来源：http://uq.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rw.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://go.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kx.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://yu.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://iq.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oq.huixiangedu.cn

================================================================================
来源：http://xl.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://sj.shxzukj.cn

================================================================================
来源：http://uf.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://uo.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kt.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://js.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rn.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wc.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ws.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://cc.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ix.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fk.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ik.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vu.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ew.szxytkj.cn

JS:   arr.push(4);
来源：http://dq.wgjwhj.cn

TS:   arr.push(4);
来源：http://ho.huixiangedu.cn

Java: list.add(4);
来源：http://vz.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://tl.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://my.wgjwhj.cn

C#:   list.Add(4);
来源：http://kw.szsharing.cn

[D03] 在指定位置插入元素
来源：http://bp.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://id.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://za.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uj.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://yj.bjjhwx.cn

Java: list.add(0, 0);
来源：http://mo.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sw.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ik.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://st.shxzskj.cn

[D04] 删除元素
来源：http://ks.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nw.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hv.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ke.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://fr.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zn.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rt.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xj.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ds.521024.cn

[D05] 访问与修改元素
来源：http://wu.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wg.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cn.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://il.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://tc.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://wa.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://wz.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lf.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ye.panjiajie.cn

[D06] 数组长度
来源：http://rx.bookmarksfly.cn

Py:   len(arr)
来源：http://dn.jianghongdianzi.cn

PHP:  count($arr);
来源：http://io.gzmigu.cn

JS:   arr.length
来源：http://ky.bjjhwx.cn

TS:   arr.length
来源：http://co.huanxung.cn

Java: list.size();
来源：http://mt.jctech888.com.cn

Go:   len(arr)
来源：http://vy.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://zh.muxihuayi.cn

C#:   list.Count;
来源：http://us.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://cb.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ed.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tl.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://mj.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://or.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://fs.bookmarksfly.cn

Go:   arr[1:4]
来源：http://pk.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://wl.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://ld.colortex.cn

[D08] 合并两个数组
来源：http://wp.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://oo.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://ci.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ju.shxzskj.cn

TS:   [...a, ...b];
来源：http://sf.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uw.muxihuayi.cn

Go:   append(a, b...)
来源：http://mj.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://yq.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://si.panjiajie.cn

[D09] 排序（升序）
来源：http://ea.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.chemitech.net.cn

PHP:  sort($arr);
来源：http://cq.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sn.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://os.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dz.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vm.huanxung.cn

Ruby: arr.sort
来源：http://py.huanxung.cn

C#:   list.Sort();
来源：http://jy.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rl.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gy.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sm.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ao.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tn.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fj.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://py.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xf.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gx.newstarts.cn

[D11] 反转数组
来源：http://ve.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cq.szsharing.cn

PHP:  array_reverse($arr);
来源：http://as.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bc.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://sg.asd995.cn

Java: Collections.reverse(list);
来源：http://ov.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://ms.gzmigu.cn

Ruby: arr.reverse
来源：http://im.panjiajie.cn

C#:   list.Reverse();
来源：http://xh.chemitech.net.cn

[D12] 查找元素下标
来源：http://zx.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://pa.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yu.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ve.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sl.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oj.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://ud.shxzskj.cn

Ruby: arr.index(x)
来源：http://kl.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://jr.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://au.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dw.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dr.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://cl.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://bu.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ut.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rd.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sd.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ry.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://ir.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kh.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ro.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://tg.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://li.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wc.shtwfgs.cn

Go:   // 手写循环
来源：http://kj.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://po.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://to.huixiangedu.cn

[D15] 去重
来源：http://lx.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://as.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://kf.nicolike.cn

JS:   [...new Set(arr)]
来源：http://us.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ol.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qs.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mg.haigaiapp.cn

Ruby: arr.uniq
来源：http://xl.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ol.huixiangedu.cn

[D16] 求和与平均值
来源：http://ma.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://if.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hc.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vk.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fl.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gy.yuexingan06.cn

Go:   // 手写循环累加
来源：http://eu.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iz.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://nm.lnxyls.cn

[D17] 最大值与最小值
来源：http://iu.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://ad.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://lh.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yi.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://wt.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://do.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://us.colortex.cn

Ruby: arr.max;  arr.min
来源：http://vw.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://qh.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://kh.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gs.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://jq.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ln.huanxung.cn

TS:   nested.flat();
来源：http://fk.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ih.shxzskj.cn

Go:   // 手写双层循环
来源：http://hh.bookmarksfly.cn

Ruby: nested.flatten
来源：http://br.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oc.huixiangedu.cn

[D19] 按字段分组
来源：http://ji.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zw.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sz.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ix.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jx.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fv.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ek.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fv.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kx.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://mq.hahajie.cn

Py:   Counter(arr)
来源：http://ix.nicolike.cn

PHP:  array_count_values($arr);
来源：http://nd.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hw.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pb.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kt.521024.cn

Go:   // 手写 map[T]int
来源：http://cg.shxzskj.cn

Ruby: arr.tally
来源：http://xi.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tl.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://kv.newstarts.cn

Py:   x in arr
来源：http://dh.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://mc.hnjuh.cn

JS:   arr.includes(x)
来源：http://jm.haigaiapp.cn

TS:   arr.includes(x)
来源：http://as.bookmarksfly.cn

Java: list.contains(x)
来源：http://oc.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://wr.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://bi.nszjky.cn

C#:   list.Contains(x)
来源：http://zf.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://nx.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nw.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cl.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yt.hnjuh.cn

TS:   [...arr];
来源：http://ht.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ow.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wp.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://jc.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://av.bjjhwx.cn

[D23] reduce 累积计算
来源：http://gv.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://en.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vi.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://za.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yc.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sj.shtwfgs.cn

Go:   // 手写循环
来源：http://tc.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jk.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zy.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://bz.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hr.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ua.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zd.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vz.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jc.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ut.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ww.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xc.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://sf.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mm.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ap.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gv.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wh.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pw.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tg.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rt.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yu.szxytkj.cn

[D26] 数组转字符串
来源：http://st.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://uo.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://rl.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://pb.lnxyls.cn

TS:   arr.join(", ")
来源：http://cf.huixiangedu.cn

Java: String.join(", ", list)
来源：http://wj.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://nl.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://fa.521024.cn

C#:   string.Join(", ", list)
来源：http://ue.huixiangedu.cn

================================================================================
来源：http://sn.huixinmuqiang.cn

E. 字符串处理
来源：http://tl.panjiajie.cn

================================================================================
来源：http://nr.shxzukj.cn

[E01] 拼接字符串
来源：http://bq.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ob.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sw.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yh.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ws.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ys.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qn.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ny.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wp.bjjhwx.cn

[E02] 重复字符串
来源：http://rk.szxytkj.cn

Py:   "ab" * 3
来源：http://wj.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://js.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://nh.asd995.cn


<!-- 参考信息 -->