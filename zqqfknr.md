代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ju.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://wr.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://if.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nm.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://kv.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://uj.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ez.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://ta.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zu.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vd.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ej.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ca.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://qn.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wj.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rn.panjiajie.cn

[C14] 泛型函数
来源：http://pt.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oz.nszjky.cn

PHP:  // 无泛型
来源：http://dn.hahajie.cn

JS:   // 无泛型
来源：http://by.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ie.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oe.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qr.nszjky.cn

Ruby: # 无泛型
来源：http://lw.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cq.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://ks.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fz.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://sk.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iq.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wp.huixinmuqiang.cn

Java: // 无解构
来源：http://am.lnxyls.cn

Go:   // 无解构
来源：http://yb.hahajie.cn

Ruby: a, b = pair
来源：http://hp.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://af.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://aw.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rk.panjiajie.cn

PHP:  // 无重载
来源：http://kv.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jl.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://rc.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ys.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://op.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://bk.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ai.9csxet.cn

================================================================================
来源：http://zy.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://oc.asd995.cn

================================================================================
来源：http://tj.nicolike.cn

[D01] 创建数组 / 列表
来源：http://bt.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ui.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kc.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wf.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mg.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uz.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ew.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ce.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ds.gzmigu.cn

[D02] 追加元素到末尾
来源：http://fk.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://he.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://um.huanxung.cn

JS:   arr.push(4);
来源：http://jv.nicolike.cn

TS:   arr.push(4);
来源：http://fa.szsharing.cn

Java: list.add(4);
来源：http://lx.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://if.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://wq.nicolike.cn

C#:   list.Add(4);
来源：http://nc.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://gs.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://pg.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yk.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mr.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://yu.gzmigu.cn

Java: list.add(0, 0);
来源：http://lg.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tr.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jh.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://lh.bookmarksfly.cn

[D04] 删除元素
来源：http://ln.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jo.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://db.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uf.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://as.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dy.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yy.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ce.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://js.szxytkj.cn

[D05] 访问与修改元素
来源：http://rk.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dy.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ny.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ay.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://wx.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://mv.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://vs.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://et.hnjuh.cn

[D06] 数组长度
来源：http://gs.yuntaijiaju.cn

Py:   len(arr)
来源：http://qe.9csxet.cn

PHP:  count($arr);
来源：http://rr.yuexingan06.cn

JS:   arr.length
来源：http://cm.nicolike.cn

TS:   arr.length
来源：http://pb.shxzukj.cn

Java: list.size();
来源：http://os.jianghongdianzi.cn

Go:   len(arr)
来源：http://rd.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://dz.colortex.cn

C#:   list.Count;
来源：http://xz.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://sd.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oh.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://xl.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://oa.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://qa.panjiajie.cn

Go:   arr[1:4]
来源：http://ru.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://wc.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://vy.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://jw.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://hv.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://mq.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://be.szxytkj.cn

TS:   [...a, ...b];
来源：http://fd.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bs.yuexingan06.cn

Go:   append(a, b...)
来源：http://dm.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ts.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://cw.nicolike.cn

[D09] 排序（升序）
来源：http://qi.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://sy.hnjuh.cn

PHP:  sort($arr);
来源：http://wp.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xy.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sw.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sz.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rp.haigaiapp.cn

Ruby: arr.sort
来源：http://qn.yuexingan06.cn

C#:   list.Sort();
来源：http://bj.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qu.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ih.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zz.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ur.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://me.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://la.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yb.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qx.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yj.huixinmuqiang.cn

[D11] 反转数组
来源：http://hm.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ca.nszjky.cn

PHP:  array_reverse($arr);
来源：http://kd.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hd.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://wk.shxzskj.cn

Java: Collections.reverse(list);
来源：http://vk.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://so.chemitech.net.cn

Ruby: arr.reverse
来源：http://zr.hahajie.cn

C#:   list.Reverse();
来源：http://oc.9csxet.cn

[D12] 查找元素下标
来源：http://wg.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://gg.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gg.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fu.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://or.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tq.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://jb.yuexingan06.cn

Ruby: arr.index(x)
来源：http://qk.hahajie.cn

C#:   list.IndexOf(x);
来源：http://uw.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://ua.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wj.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mq.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://jm.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://wg.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cj.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tm.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zy.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vf.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://db.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ks.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bh.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://zt.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ue.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xk.jianghongdianzi.cn

Go:   // 手写循环
来源：http://bi.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ei.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bn.jctech888.com.cn

[D15] 去重
来源：http://nx.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zq.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://op.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ta.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://lh.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lo.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hl.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://te.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://rs.9csxet.cn

[D16] 求和与平均值
来源：http://vl.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mj.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://en.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ll.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xg.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://te.szsharing.cn

Go:   // 手写循环累加
来源：http://fw.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://in.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://dd.hahajie.cn

[D17] 最大值与最小值
来源：http://pt.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://ee.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://az.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ap.nszjky.cn

TS:   Math.max(...arr);
来源：http://xt.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wf.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fm.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ty.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://lv.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://zy.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ej.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://lf.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sz.asd995.cn

TS:   nested.flat();
来源：http://hf.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fu.newstarts.cn

Go:   // 手写双层循环
来源：http://fq.szxytkj.cn

Ruby: nested.flatten
来源：http://ck.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dm.muxihuayi.cn

[D19] 按字段分组
来源：http://bu.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vn.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ak.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nf.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://th.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ix.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://ap.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://np.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ew.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ea.huanxung.cn

Py:   Counter(arr)
来源：http://fl.colortex.cn

PHP:  array_count_values($arr);
来源：http://dl.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bp.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zv.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kr.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://wn.colortex.cn

Ruby: arr.tally
来源：http://uk.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://im.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://vd.jianghongdianzi.cn

Py:   x in arr
来源：http://vu.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://sq.huixiangedu.cn

JS:   arr.includes(x)
来源：http://he.huanxung.cn

TS:   arr.includes(x)
来源：http://ph.lnxyls.cn

Java: list.contains(x)
来源：http://xp.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://mh.newstarts.cn

Ruby: arr.include?(x)
来源：http://ri.shtwfgs.cn

C#:   list.Contains(x)
来源：http://ov.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://yb.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fc.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lx.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xd.chemitech.net.cn

TS:   [...arr];
来源：http://te.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://hl.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://co.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://ik.lnxyls.cn

C#:   new List<int>(list);
来源：http://fh.asd995.cn

[D23] reduce 累积计算
来源：http://fi.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xf.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xk.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zl.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qx.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ze.hnjuh.cn

Go:   // 手写循环
来源：http://xm.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://il.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iy.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://hc.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gc.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ne.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eo.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ln.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rz.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://up.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zp.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vp.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://dz.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ra.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tq.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gq.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nn.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tc.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fd.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://to.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ox.jctech888.com.cn

[D26] 数组转字符串
来源：http://pc.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://tu.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://jv.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ec.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://gc.chemitech.net.cn

Java: String.join(", ", list)
来源：http://vu.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://zv.colortex.cn

Ruby: arr.join(", ")
来源：http://jq.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://xj.colortex.cn

================================================================================
来源：http://gd.yuntaijiaju.cn

E. 字符串处理
来源：http://rr.jctech888.com.cn

================================================================================
来源：http://kk.newstarts.cn

[E01] 拼接字符串
来源：http://au.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zb.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xm.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tg.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aw.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bm.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xz.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qs.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iz.lnxyls.cn

[E02] 重复字符串
来源：http://ft.bjjhwx.cn

Py:   "ab" * 3
来源：http://ge.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ig.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://sm.colortex.cn

TS:   "ab".repeat(3)
来源：http://mm.gzmigu.cn

Java: "ab".repeat(3)
来源：http://nk.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://nv.gzmigu.cn

Ruby: "ab" * 3
来源：http://uz.hnjuh.cn


<!-- 参考信息 -->