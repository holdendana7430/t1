代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hx.shtwfgs.cn

C#:   using System.Text;
来源：http://ku.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://ps.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://jo.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://gp.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://fn.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://dl.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rd.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://xl.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://sz.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xi.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://et.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ae.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nr.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lh.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qw.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wa.szxytkj.cn

Go:   func add(a, b int) int
来源：http://vz.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xa.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://re.szsharing.cn

[C14] 泛型函数
来源：http://bc.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://og.wgjwhj.cn

PHP:  // 无泛型
来源：http://vs.shxzukj.cn

JS:   // 无泛型
来源：http://qu.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xf.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ft.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jn.nicolike.cn

Ruby: # 无泛型
来源：http://gb.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yi.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://tv.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://er.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://li.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qp.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zr.wgjwhj.cn

Java: // 无解构
来源：http://lm.yuntaijiaju.cn

Go:   // 无解构
来源：http://au.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://wl.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://md.nszjky.cn

[C16] 函数 / 方法重载
来源：http://uh.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ah.szxytkj.cn

PHP:  // 无重载
来源：http://nf.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yu.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://lv.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ay.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://jw.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ap.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zl.shxzskj.cn

================================================================================
来源：http://dk.521024.cn

D. 数组 / 列表 / 集合
来源：http://vc.nszjky.cn

================================================================================
来源：http://ep.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://qw.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://im.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://so.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pj.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ea.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qe.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://hz.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://gb.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mx.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://yy.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jb.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oo.bjjhwx.cn

JS:   arr.push(4);
来源：http://yz.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://yo.panjiajie.cn

Java: list.add(4);
来源：http://pi.colortex.cn

Go:   arr = append(arr, 4)
来源：http://te.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://kz.shxzukj.cn

C#:   list.Add(4);
来源：http://uf.521024.cn

[D03] 在指定位置插入元素
来源：http://wk.521024.cn

Py:   arr.insert(0, 0)
来源：http://de.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wo.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bg.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ja.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ik.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gc.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://al.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://np.muxihuayi.cn

[D04] 删除元素
来源：http://is.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ft.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pn.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fq.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://ex.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wi.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iy.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ra.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xx.huanxung.cn

[D05] 访问与修改元素
来源：http://kx.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vm.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tm.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ka.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://hs.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://wn.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://dy.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ee.yuexingan06.cn

[D06] 数组长度
来源：http://en.bookmarksfly.cn

Py:   len(arr)
来源：http://jd.haigaiapp.cn

PHP:  count($arr);
来源：http://qz.asd995.cn

JS:   arr.length
来源：http://qx.lnxyls.cn

TS:   arr.length
来源：http://gy.9csxet.cn

Java: list.size();
来源：http://mi.bookmarksfly.cn

Go:   len(arr)
来源：http://wh.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://og.nicolike.cn

C#:   list.Count;
来源：http://dm.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://na.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://et.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aw.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ed.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://cz.nszjky.cn

Java: list.subList(1, 4);
来源：http://iu.asd995.cn

Go:   arr[1:4]
来源：http://wd.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://bg.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://gz.shtwfgs.cn

[D08] 合并两个数组
来源：http://wt.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://oy.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://yj.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ky.9csxet.cn

TS:   [...a, ...b];
来源：http://ms.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dp.szxytkj.cn

Go:   append(a, b...)
来源：http://dk.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://fd.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://gm.jctech888.com.cn

[D09] 排序（升序）
来源：http://kq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://kn.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://oi.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vp.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ru.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iy.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rz.chemitech.net.cn

Ruby: arr.sort
来源：http://us.colortex.cn

C#:   list.Sort();
来源：http://ir.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://us.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jh.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://th.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ij.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://km.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cp.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ex.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://as.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nk.9csxet.cn

[D11] 反转数组
来源：http://ap.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ku.szsharing.cn

PHP:  array_reverse($arr);
来源：http://dn.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nx.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://yu.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://ll.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://hn.asd995.cn

Ruby: arr.reverse
来源：http://gg.szxytkj.cn

C#:   list.Reverse();
来源：http://uy.yuexingan06.cn

[D12] 查找元素下标
来源：http://cz.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ot.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iz.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hf.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tl.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yc.colortex.cn

Go:   slices.Index(arr, x)
来源：http://zp.muxihuayi.cn

Ruby: arr.index(x)
来源：http://df.nicolike.cn

C#:   list.IndexOf(x);
来源：http://vr.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://vp.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fd.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dh.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://yz.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://zh.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dh.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://we.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kk.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mt.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://xd.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vk.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ps.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://tt.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://xn.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://st.nszjky.cn

Go:   // 手写循环
来源：http://ze.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mi.haigaiapp.cn

[D15] 去重
来源：http://ie.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ib.hnjuh.cn

PHP:  array_unique($arr);
来源：http://mt.colortex.cn

JS:   [...new Set(arr)]
来源：http://vv.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://st.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jd.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ez.bookmarksfly.cn

Ruby: arr.uniq
来源：http://mh.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://jg.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ly.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ns.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hs.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://io.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ie.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nu.nszjky.cn

Go:   // 手写循环累加
来源：http://jq.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ak.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://vx.nicolike.cn

[D17] 最大值与最小值
来源：http://cl.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://oh.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://gg.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ol.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://hs.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uc.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ca.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ev.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://xp.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://qn.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://om.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://kv.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lq.lnxyls.cn

TS:   nested.flat();
来源：http://pm.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sh.yuexingan06.cn

Go:   // 手写双层循环
来源：http://ui.lnxyls.cn

Ruby: nested.flatten
来源：http://uj.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yc.newstarts.cn

[D19] 按字段分组
来源：http://gh.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zb.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gs.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ie.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://al.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ai.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://dn.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xx.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pn.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://dc.colortex.cn

Py:   Counter(arr)
来源：http://se.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://tn.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pt.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ql.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ib.521024.cn

Go:   // 手写 map[T]int
来源：http://nw.lnxyls.cn

Ruby: arr.tally
来源：http://ll.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mm.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://rz.colortex.cn

Py:   x in arr
来源：http://hx.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://dn.yuexingan06.cn

JS:   arr.includes(x)
来源：http://xd.chemitech.net.cn

TS:   arr.includes(x)
来源：http://kt.bookmarksfly.cn

Java: list.contains(x)
来源：http://ue.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://le.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://fh.huixiangedu.cn

C#:   list.Contains(x)
来源：http://uw.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://hf.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ay.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://le.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://am.huixinmuqiang.cn

TS:   [...arr];
来源：http://pg.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://qx.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hm.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://bj.shxzukj.cn

C#:   new List<int>(list);
来源：http://su.huixiangedu.cn

[D23] reduce 累积计算
来源：http://he.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ia.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jy.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gj.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ea.yuexingan06.cn

Go:   // 手写循环
来源：http://lj.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gg.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ov.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://kv.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yb.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cc.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ls.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dm.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qb.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ee.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eg.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xx.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://vl.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sb.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jw.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://po.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wb.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ge.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yc.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ah.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ad.yuexingan06.cn

[D26] 数组转字符串
来源：http://vk.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://di.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://zb.panjiajie.cn

JS:   arr.join(", ")
来源：http://nh.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ou.haigaiapp.cn

Java: String.join(", ", list)
来源：http://yu.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://hm.9csxet.cn

Ruby: arr.join(", ")
来源：http://bz.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ta.shxzukj.cn

================================================================================
来源：http://ae.yuexingan06.cn

E. 字符串处理
来源：http://gg.wgjwhj.cn

================================================================================
来源：http://wp.yuexingan06.cn

[E01] 拼接字符串
来源：http://ll.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hu.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xv.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yq.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cc.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://of.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ut.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oj.yuntaijiaju.cn

[E02] 重复字符串
来源：http://nh.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://dp.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://hk.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://wn.szsharing.cn


<!-- 参考信息 -->