代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ei.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://zk.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://vs.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xj.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://ky.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://wq.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://je.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://pg.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vu.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xl.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gl.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://og.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mw.szxytkj.cn

Go:   func add(a, b int) int
来源：http://xu.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fa.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tq.hnjuh.cn

[C14] 泛型函数
来源：http://kj.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tf.bjjhwx.cn

PHP:  // 无泛型
来源：http://ph.newstarts.cn

JS:   // 无泛型
来源：http://ye.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vx.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ho.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ao.colortex.cn

Ruby: # 无泛型
来源：http://wu.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cu.nicolike.cn

[C15] 解构 / 展开参数
来源：http://qu.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rv.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://sh.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nt.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qt.nicolike.cn

Java: // 无解构
来源：http://kk.shtwfgs.cn

Go:   // 无解构
来源：http://jq.haigaiapp.cn

Ruby: a, b = pair
来源：http://td.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://ul.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://zi.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ax.jctech888.com.cn

PHP:  // 无重载
来源：http://rv.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ij.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://mh.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nr.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://wq.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://le.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://er.szxytkj.cn

================================================================================
来源：http://jq.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://qi.haigaiapp.cn

================================================================================
来源：http://wd.huanxung.cn

[D01] 创建数组 / 列表
来源：http://gm.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://us.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ym.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cm.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://me.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ft.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://kb.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://wr.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sp.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://ag.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iv.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ku.shxzukj.cn

JS:   arr.push(4);
来源：http://nu.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://mh.szsharing.cn

Java: list.add(4);
来源：http://il.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://zk.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://xr.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://tb.colortex.cn

[D03] 在指定位置插入元素
来源：http://er.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://xn.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lx.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sl.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://ur.nszjky.cn

Java: list.add(0, 0);
来源：http://jv.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ku.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://az.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://mt.shxzskj.cn

[D04] 删除元素
来源：http://hx.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wh.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://os.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jp.colortex.cn

TS:   arr.splice(0, 1);
来源：http://wi.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wk.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eo.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tf.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cx.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ab.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ot.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wk.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oa.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ee.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://pi.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://nf.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ul.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qr.bjjhwx.cn

[D06] 数组长度
来源：http://tq.bjjhwx.cn

Py:   len(arr)
来源：http://oj.nszjky.cn

PHP:  count($arr);
来源：http://jh.haigaiapp.cn

JS:   arr.length
来源：http://mh.szxytkj.cn

TS:   arr.length
来源：http://wl.bookmarksfly.cn

Java: list.size();
来源：http://om.szsharing.cn

Go:   len(arr)
来源：http://ut.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://sk.szxytkj.cn

C#:   list.Count;
来源：http://sc.huanxung.cn

[D07] 切片 / 取子数组
来源：http://vg.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cv.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ik.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://np.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://av.asd995.cn

Java: list.subList(1, 4);
来源：http://rl.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://gh.521024.cn

Ruby: arr[1, 3]
来源：http://vp.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ml.szsharing.cn

[D08] 合并两个数组
来源：http://ev.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://yh.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://cy.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ii.hnjuh.cn

TS:   [...a, ...b];
来源：http://cm.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ca.huixiangedu.cn

Go:   append(a, b...)
来源：http://mh.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://sa.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://kf.gzmigu.cn

[D09] 排序（升序）
来源：http://uh.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://to.9csxet.cn

PHP:  sort($arr);
来源：http://pu.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mi.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yi.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://it.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jj.shtwfgs.cn

Ruby: arr.sort
来源：http://rb.gzmigu.cn

C#:   list.Sort();
来源：http://mq.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ii.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hv.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://le.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lb.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ew.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cn.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xs.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pe.hahajie.cn

[D11] 反转数组
来源：http://rq.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qy.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://aw.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jc.shxzskj.cn

TS:   [...arr].reverse();
来源：http://hx.gzmigu.cn

Java: Collections.reverse(list);
来源：http://px.asd995.cn

Go:   slices.Reverse(arr)
来源：http://ny.521024.cn

Ruby: arr.reverse
来源：http://ml.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://yh.bjjhwx.cn

[D12] 查找元素下标
来源：http://gb.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://oh.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kw.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://no.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uq.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://so.colortex.cn

Go:   slices.Index(arr, x)
来源：http://kr.lnxyls.cn

Ruby: arr.index(x)
来源：http://zh.nszjky.cn

C#:   list.IndexOf(x);
来源：http://do.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://xg.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vd.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://us.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://oq.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://vb.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iy.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aj.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yw.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vt.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://ct.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rp.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sq.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://vf.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://fb.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://de.9csxet.cn

Go:   // 手写循环
来源：http://dw.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ig.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ya.lnxyls.cn

[D15] 去重
来源：http://rp.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yh.hnjuh.cn

PHP:  array_unique($arr);
来源：http://si.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://cx.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://yj.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ig.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://in.gzmigu.cn

Ruby: arr.uniq
来源：http://fz.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://ed.panjiajie.cn

[D16] 求和与平均值
来源：http://fh.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bo.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zz.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dj.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ie.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gb.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://mv.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yw.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://ca.yuexingan06.cn

[D17] 最大值与最小值
来源：http://su.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://zb.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ro.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dp.szxytkj.cn

TS:   Math.max(...arr);
来源：http://bl.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cx.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fi.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://li.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://rk.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://rz.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xi.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://lu.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://va.9csxet.cn

TS:   nested.flat();
来源：http://fo.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jw.huixiangedu.cn

Go:   // 手写双层循环
来源：http://it.yuexingan06.cn

Ruby: nested.flatten
来源：http://cd.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wx.panjiajie.cn

[D19] 按字段分组
来源：http://ps.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yx.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yq.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wd.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lg.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jf.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://hr.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yo.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://up.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ga.gzmigu.cn

Py:   Counter(arr)
来源：http://iy.9csxet.cn

PHP:  array_count_values($arr);
来源：http://jg.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mc.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wp.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qg.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://oj.jctech888.com.cn

Ruby: arr.tally
来源：http://oq.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://px.asd995.cn

[D21] 判断是否包含某元素
来源：http://sw.lnxyls.cn

Py:   x in arr
来源：http://jt.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://xg.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ls.lnxyls.cn

TS:   arr.includes(x)
来源：http://hi.lnxyls.cn

Java: list.contains(x)
来源：http://ww.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ns.szxytkj.cn

Ruby: arr.include?(x)
来源：http://vc.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://sc.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://xk.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ak.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tj.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vi.szsharing.cn

TS:   [...arr];
来源：http://om.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://gw.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ce.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://is.shxzskj.cn

C#:   new List<int>(list);
来源：http://ip.chemitech.net.cn

[D23] reduce 累积计算
来源：http://tq.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kb.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hf.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yw.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://un.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bv.huixiangedu.cn

Go:   // 手写循环
来源：http://ve.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lz.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fn.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://kf.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ow.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zr.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lh.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lt.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sf.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ez.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nb.asd995.cn

[D25] Set 集合去重与交并差
来源：http://uw.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bw.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yu.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://al.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aw.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pe.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://im.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rj.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://op.huanxung.cn

[D26] 数组转字符串
来源：http://ju.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://ku.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ps.nicolike.cn

JS:   arr.join(", ")
来源：http://gx.shtwfgs.cn

TS:   arr.join(", ")
来源：http://fe.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://xh.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ik.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ug.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ko.asd995.cn

================================================================================
来源：http://cp.huixiangedu.cn

E. 字符串处理
来源：http://yo.hnjuh.cn

================================================================================
来源：http://bi.gzmigu.cn

[E01] 拼接字符串
来源：http://lk.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yb.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tf.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gb.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ym.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ib.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bo.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cx.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cs.nszjky.cn

[E02] 重复字符串
来源：http://so.panjiajie.cn

Py:   "ab" * 3
来源：http://pb.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://iv.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://jl.521024.cn

TS:   "ab".repeat(3)
来源：http://yf.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://is.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://cn.muxihuayi.cn

Ruby: "ab" * 3
来源：http://gr.gzmigu.cn


<!-- 参考信息 -->