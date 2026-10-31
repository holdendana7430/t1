代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://bp.9csxet.cn

C#:   using System.Text;
来源：http://sx.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://hl.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://lf.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://wh.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://bi.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://in.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pj.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://jj.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://sr.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qf.521024.cn

[C13] 类型声明 / 类型注解
来源：http://yx.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ug.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gf.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ya.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pn.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rv.huanxung.cn

Go:   func add(a, b int) int
来源：http://nq.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mb.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://la.hnjuh.cn

[C14] 泛型函数
来源：http://bk.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bw.szxytkj.cn

PHP:  // 无泛型
来源：http://am.newstarts.cn

JS:   // 无泛型
来源：http://ub.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wl.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ky.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kf.lnxyls.cn

Ruby: # 无泛型
来源：http://ns.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wc.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://rj.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kh.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://fb.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iq.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wi.colortex.cn

Java: // 无解构
来源：http://vh.huixinmuqiang.cn

Go:   // 无解构
来源：http://nz.huixiangedu.cn

Ruby: a, b = pair
来源：http://fu.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://wb.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://pw.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ra.hahajie.cn

PHP:  // 无重载
来源：http://gq.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ay.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://jv.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oe.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://tw.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://mv.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gi.szxytkj.cn

================================================================================
来源：http://yr.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://zw.jianghongdianzi.cn

================================================================================
来源：http://wy.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://we.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sm.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kq.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xf.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bc.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://br.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://ry.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://wl.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bj.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://pu.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wr.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fp.muxihuayi.cn

JS:   arr.push(4);
来源：http://bg.szsharing.cn

TS:   arr.push(4);
来源：http://qo.gzmigu.cn

Java: list.add(4);
来源：http://my.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://pg.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://au.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://kr.521024.cn

[D03] 在指定位置插入元素
来源：http://az.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://wx.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ry.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ms.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://xm.yuexingan06.cn

Java: list.add(0, 0);
来源：http://tm.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hr.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://md.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://lv.szsharing.cn

[D04] 删除元素
来源：http://wr.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pr.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bw.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wt.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://eh.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mz.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ro.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ms.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ii.hahajie.cn

[D05] 访问与修改元素
来源：http://qg.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rs.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fk.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ez.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://xy.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://ih.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://lm.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lw.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ud.bookmarksfly.cn

[D06] 数组长度
来源：http://ns.newstarts.cn

Py:   len(arr)
来源：http://fg.newstarts.cn

PHP:  count($arr);
来源：http://kn.hnjuh.cn

JS:   arr.length
来源：http://up.yuntaijiaju.cn

TS:   arr.length
来源：http://im.bjjhwx.cn

Java: list.size();
来源：http://um.chemitech.net.cn

Go:   len(arr)
来源：http://fi.newstarts.cn

Ruby: arr.length; arr.size
来源：http://gk.wgjwhj.cn

C#:   list.Count;
来源：http://hh.nszjky.cn

[D07] 切片 / 取子数组
来源：http://bt.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bs.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ub.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://zo.521024.cn

TS:   arr.slice(1, 4);
来源：http://ny.nicolike.cn

Java: list.subList(1, 4);
来源：http://qe.bjjhwx.cn

Go:   arr[1:4]
来源：http://iu.nicolike.cn

Ruby: arr[1, 3]
来源：http://fk.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://az.hnjuh.cn

[D08] 合并两个数组
来源：http://gc.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://zp.521024.cn

PHP:  array_merge($a, $b);
来源：http://ld.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lw.jctech888.com.cn

TS:   [...a, ...b];
来源：http://xu.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://va.shtwfgs.cn

Go:   append(a, b...)
来源：http://co.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://vw.521024.cn

C#:   a.Concat(b).ToList()
来源：http://gt.wgjwhj.cn

[D09] 排序（升序）
来源：http://zk.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mw.haigaiapp.cn

PHP:  sort($arr);
来源：http://ww.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vw.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ie.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lb.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gf.colortex.cn

Ruby: arr.sort
来源：http://ir.szxytkj.cn

C#:   list.Sort();
来源：http://el.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rw.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mn.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ok.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://in.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ql.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kk.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://je.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gi.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ci.9csxet.cn

[D11] 反转数组
来源：http://yj.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ob.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://im.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nm.szsharing.cn

TS:   [...arr].reverse();
来源：http://vp.asd995.cn

Java: Collections.reverse(list);
来源：http://ll.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://ar.shxzukj.cn

Ruby: arr.reverse
来源：http://nt.521024.cn

C#:   list.Reverse();
来源：http://ci.521024.cn

[D12] 查找元素下标
来源：http://wl.521024.cn

Py:   arr.index(x);  x in arr
来源：http://sa.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qk.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vv.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qd.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dl.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://ao.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://kx.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://wb.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://xl.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ao.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hl.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://al.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://pn.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ih.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nn.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fu.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qc.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://it.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qo.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cc.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://gy.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://ng.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iw.bjjhwx.cn

Go:   // 手写循环
来源：http://lw.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://is.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ec.haigaiapp.cn

[D15] 去重
来源：http://bs.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kz.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ru.newstarts.cn

JS:   [...new Set(arr)]
来源：http://lh.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://jh.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ar.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cc.colortex.cn

Ruby: arr.uniq
来源：http://my.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://xa.szsharing.cn

[D16] 求和与平均值
来源：http://oh.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fu.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jh.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vn.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gt.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yv.hnjuh.cn

Go:   // 手写循环累加
来源：http://hb.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lu.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://ss.szsharing.cn

[D17] 最大值与最小值
来源：http://vm.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://yx.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://qf.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qu.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://fx.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hs.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://an.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://xf.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://bm.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ct.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pg.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://se.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ty.shxzukj.cn

TS:   nested.flat();
来源：http://al.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zo.huixiangedu.cn

Go:   // 手写双层循环
来源：http://ke.newstarts.cn

Ruby: nested.flatten
来源：http://en.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://au.shxzskj.cn

[D19] 按字段分组
来源：http://st.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yu.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rb.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nw.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dn.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://qj.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gw.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mj.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://tf.shxzukj.cn

Py:   Counter(arr)
来源：http://rc.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://uj.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rm.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eo.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tr.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://yl.colortex.cn

Ruby: arr.tally
来源：http://ig.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ll.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ur.panjiajie.cn

Py:   x in arr
来源：http://wr.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://lo.haigaiapp.cn

JS:   arr.includes(x)
来源：http://fs.lnxyls.cn

TS:   arr.includes(x)
来源：http://oz.bjjhwx.cn

Java: list.contains(x)
来源：http://ai.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ez.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://yx.wgjwhj.cn

C#:   list.Contains(x)
来源：http://el.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://vp.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uq.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ss.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sb.shxzukj.cn

TS:   [...arr];
来源：http://tx.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://bu.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://px.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://xf.newstarts.cn

C#:   new List<int>(list);
来源：http://wg.panjiajie.cn

[D23] reduce 累积计算
来源：http://tw.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hs.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tk.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sv.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lq.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ao.asd995.cn

Go:   // 手写循环
来源：http://io.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vu.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yg.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://cc.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hr.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bs.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xe.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vw.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ln.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lv.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hl.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://re.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://tk.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ie.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uj.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ko.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zp.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ur.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vq.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oh.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ll.shtwfgs.cn

[D26] 数组转字符串
来源：http://ph.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://mz.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://ac.colortex.cn

JS:   arr.join(", ")
来源：http://sm.muxihuayi.cn

TS:   arr.join(", ")
来源：http://ut.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ua.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://wp.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://tm.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://bk.huanxung.cn

================================================================================
来源：http://fy.panjiajie.cn

E. 字符串处理
来源：http://pr.newstarts.cn

================================================================================
来源：http://fd.jctech888.com.cn

[E01] 拼接字符串
来源：http://ne.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gq.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gl.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ke.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gc.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uj.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dx.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ds.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://we.wgjwhj.cn

[E02] 重复字符串
来源：http://fe.panjiajie.cn

Py:   "ab" * 3
来源：http://lj.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://hu.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://hf.jianghongdianzi.cn


<!-- 参考信息 -->