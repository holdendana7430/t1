代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://qv.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ec.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://bi.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cj.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://jy.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://ec.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ff.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://gh.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fq.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dc.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://db.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gt.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://am.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lf.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gx.9csxet.cn

[C14] 泛型函数
来源：http://ci.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fr.haigaiapp.cn

PHP:  // 无泛型
来源：http://qt.colortex.cn

JS:   // 无泛型
来源：http://xb.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wh.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zh.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://ry.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fp.9csxet.cn

[C15] 解构 / 展开参数
来源：http://kc.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sd.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://jl.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dj.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bk.nicolike.cn

Java: // 无解构
来源：http://rf.wgjwhj.cn

Go:   // 无解构
来源：http://zf.haigaiapp.cn

Ruby: a, b = pair
来源：http://fz.9csxet.cn

C#:   var (a, b) = pair;
来源：http://hq.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://rj.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wg.shxzskj.cn

PHP:  // 无重载
来源：http://cw.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yv.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ru.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://at.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://sz.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://td.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nv.bjjhwx.cn

================================================================================
来源：http://lt.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://eh.shxzukj.cn

================================================================================
来源：http://oa.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://yq.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ke.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gm.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ey.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cz.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://xf.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://sz.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vy.9csxet.cn

[D02] 追加元素到末尾
来源：http://hb.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pb.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bw.wgjwhj.cn

JS:   arr.push(4);
来源：http://gj.huanxung.cn

TS:   arr.push(4);
来源：http://jk.nszjky.cn

Java: list.add(4);
来源：http://gj.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://nl.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://gq.shtwfgs.cn

C#:   list.Add(4);
来源：http://jo.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://vt.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://pb.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mh.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wo.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ae.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://bp.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oo.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ie.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://ch.yuntaijiaju.cn

[D04] 删除元素
来源：http://ya.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tq.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rq.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nm.colortex.cn

TS:   arr.splice(0, 1);
来源：http://se.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zt.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ld.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uj.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rq.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://dp.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bf.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jh.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://og.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://ga.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://yz.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://kv.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oj.hnjuh.cn

[D06] 数组长度
来源：http://ku.nszjky.cn

Py:   len(arr)
来源：http://tv.huixinmuqiang.cn

PHP:  count($arr);
来源：http://xm.szxytkj.cn

JS:   arr.length
来源：http://hj.bjjhwx.cn

TS:   arr.length
来源：http://lx.nszjky.cn

Java: list.size();
来源：http://uh.yuntaijiaju.cn

Go:   len(arr)
来源：http://tr.asd995.cn

Ruby: arr.length; arr.size
来源：http://ei.panjiajie.cn

C#:   list.Count;
来源：http://ta.newstarts.cn

[D07] 切片 / 取子数组
来源：http://fa.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ae.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cz.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://rn.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://ws.huanxung.cn

Java: list.subList(1, 4);
来源：http://xs.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://rf.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://az.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://gp.yuexingan06.cn

[D08] 合并两个数组
来源：http://lk.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://la.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://oz.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gf.bjjhwx.cn

TS:   [...a, ...b];
来源：http://or.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hv.muxihuayi.cn

Go:   append(a, b...)
来源：http://nf.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://ox.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://ul.szsharing.cn

[D09] 排序（升序）
来源：http://fd.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://nm.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://tf.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://li.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sw.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kh.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mq.yuntaijiaju.cn

Ruby: arr.sort
来源：http://fm.muxihuayi.cn

C#:   list.Sort();
来源：http://lv.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ml.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pl.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xp.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zg.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dy.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uc.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sm.nicolike.cn

[D11] 反转数组
来源：http://le.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eu.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ao.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gh.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://uh.panjiajie.cn

Java: Collections.reverse(list);
来源：http://bt.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://il.colortex.cn

Ruby: arr.reverse
来源：http://aj.muxihuayi.cn

C#:   list.Reverse();
来源：http://mu.asd995.cn

[D12] 查找元素下标
来源：http://jh.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://vi.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pu.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ne.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fe.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dh.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://gf.szsharing.cn

Ruby: arr.index(x)
来源：http://eo.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://jz.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ce.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dp.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kx.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://md.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://hz.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lx.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nz.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dx.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ni.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://nz.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yh.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jq.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://vb.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://lb.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://do.hnjuh.cn

Go:   // 手写循环
来源：http://vo.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dq.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rg.szxytkj.cn

[D15] 去重
来源：http://aj.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vn.nicolike.cn

PHP:  array_unique($arr);
来源：http://wk.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://wb.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://sk.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jd.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zn.bjjhwx.cn

Ruby: arr.uniq
来源：http://du.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://sr.szsharing.cn

[D16] 求和与平均值
来源：http://jv.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lt.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nn.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dc.nszjky.cn

Go:   // 手写循环累加
来源：http://an.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://am.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://ju.nicolike.cn

[D17] 最大值与最小值
来源：http://zc.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://kz.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://vv.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jb.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://oy.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yw.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://os.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://un.asd995.cn

C#:   list.Max();  list.Min()
来源：http://ap.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://by.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sn.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://bp.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cq.colortex.cn

TS:   nested.flat();
来源：http://yi.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ym.lnxyls.cn

Go:   // 手写双层循环
来源：http://ix.lnxyls.cn

Ruby: nested.flatten
来源：http://yt.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zv.asd995.cn

[D19] 按字段分组
来源：http://yn.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qb.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qe.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fq.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ui.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kv.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://pg.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://db.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ss.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://to.gzmigu.cn

Py:   Counter(arr)
来源：http://rf.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://io.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wp.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fm.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ow.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://oi.bookmarksfly.cn

Ruby: arr.tally
来源：http://qf.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mh.newstarts.cn

[D21] 判断是否包含某元素
来源：http://jt.gzmigu.cn

Py:   x in arr
来源：http://hr.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ol.huanxung.cn

JS:   arr.includes(x)
来源：http://sk.shxzskj.cn

TS:   arr.includes(x)
来源：http://gy.jctech888.com.cn

Java: list.contains(x)
来源：http://np.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://xu.asd995.cn

Ruby: arr.include?(x)
来源：http://md.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://bm.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xt.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pk.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yw.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fb.panjiajie.cn

TS:   [...arr];
来源：http://xi.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://wo.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ks.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://vo.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://bb.huanxung.cn

[D23] reduce 累积计算
来源：http://mx.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gz.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://du.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lt.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ge.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qx.hahajie.cn

Go:   // 手写循环
来源：http://mg.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bv.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vo.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://cc.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://si.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ce.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xv.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gg.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sl.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fx.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ic.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ki.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://kz.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vf.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fr.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tp.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xf.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ce.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uk.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vy.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qm.szsharing.cn

[D26] 数组转字符串
来源：http://bv.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ot.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://in.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://lu.huanxung.cn

TS:   arr.join(", ")
来源：http://zu.shxzskj.cn

Java: String.join(", ", list)
来源：http://an.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://pb.huanxung.cn

Ruby: arr.join(", ")
来源：http://gh.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://jl.panjiajie.cn

================================================================================
来源：http://he.wgjwhj.cn

E. 字符串处理
来源：http://nl.shxzukj.cn

================================================================================
来源：http://sq.colortex.cn

[E01] 拼接字符串
来源：http://ia.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ya.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gj.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tx.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://te.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://no.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://of.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sb.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gr.9csxet.cn

[E02] 重复字符串
来源：http://bu.asd995.cn

Py:   "ab" * 3
来源：http://wf.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ew.hahajie.cn

JS:   "ab".repeat(3)
来源：http://mh.szsharing.cn

TS:   "ab".repeat(3)
来源：http://km.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://nz.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://wt.hnjuh.cn

Ruby: "ab" * 3
来源：http://jl.yuntaijiaju.cn


<!-- 参考信息 -->