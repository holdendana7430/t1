代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ii.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://gq.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://oh.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://em.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://df.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://ng.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://id.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://yn.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ky.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nf.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://up.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lm.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://by.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fw.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fq.hahajie.cn

[C14] 泛型函数
来源：http://te.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ja.szxytkj.cn

PHP:  // 无泛型
来源：http://aa.bookmarksfly.cn

JS:   // 无泛型
来源：http://cu.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dh.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://je.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ob.muxihuayi.cn

Ruby: # 无泛型
来源：http://mr.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ne.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://xb.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vn.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://nd.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fs.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ni.bjjhwx.cn

Java: // 无解构
来源：http://xu.szxytkj.cn

Go:   // 无解构
来源：http://gc.shxzskj.cn

Ruby: a, b = pair
来源：http://qo.nicolike.cn

C#:   var (a, b) = pair;
来源：http://mj.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://fw.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lc.muxihuayi.cn

PHP:  // 无重载
来源：http://ie.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ju.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://fl.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zw.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://mi.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://lg.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vb.521024.cn

================================================================================
来源：http://zx.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ps.huixiangedu.cn

================================================================================
来源：http://rx.colortex.cn

[D01] 创建数组 / 列表
来源：http://jw.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xa.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hs.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tz.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yr.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pm.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://zt.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ya.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zv.panjiajie.cn

[D02] 追加元素到末尾
来源：http://zp.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cj.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cx.haigaiapp.cn

JS:   arr.push(4);
来源：http://ol.szsharing.cn

TS:   arr.push(4);
来源：http://bl.jctech888.com.cn

Java: list.add(4);
来源：http://nv.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://gx.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://pr.huixiangedu.cn

C#:   list.Add(4);
来源：http://pu.521024.cn

[D03] 在指定位置插入元素
来源：http://ew.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://cb.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vd.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ik.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://vx.huanxung.cn

Java: list.add(0, 0);
来源：http://bk.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kw.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sn.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://ar.muxihuayi.cn

[D04] 删除元素
来源：http://yn.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yw.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ko.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://gh.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kh.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wn.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jn.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tn.haigaiapp.cn

[D05] 访问与修改元素
来源：http://re.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bu.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://do.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zc.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://zh.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://by.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://fk.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://la.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gh.shtwfgs.cn

[D06] 数组长度
来源：http://dv.nszjky.cn

Py:   len(arr)
来源：http://ri.bjjhwx.cn

PHP:  count($arr);
来源：http://xh.bookmarksfly.cn

JS:   arr.length
来源：http://qa.muxihuayi.cn

TS:   arr.length
来源：http://no.yuexingan06.cn

Java: list.size();
来源：http://ja.chemitech.net.cn

Go:   len(arr)
来源：http://cb.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://ji.jianghongdianzi.cn

C#:   list.Count;
来源：http://cv.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://np.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iw.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yd.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://rg.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://em.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://hr.bjjhwx.cn

Go:   arr[1:4]
来源：http://iy.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://jn.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://ni.jctech888.com.cn

[D08] 合并两个数组
来源：http://fo.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ux.asd995.cn

PHP:  array_merge($a, $b);
来源：http://uj.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://em.haigaiapp.cn

TS:   [...a, ...b];
来源：http://zi.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ny.bjjhwx.cn

Go:   append(a, b...)
来源：http://ll.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://mo.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://zi.szxytkj.cn

[D09] 排序（升序）
来源：http://yc.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sw.wgjwhj.cn

PHP:  sort($arr);
来源：http://mr.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vc.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tm.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ml.newstarts.cn

Ruby: arr.sort
来源：http://fx.hnjuh.cn

C#:   list.Sort();
来源：http://te.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oe.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fh.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nr.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qa.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jb.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qi.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ie.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wv.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://af.chemitech.net.cn

[D11] 反转数组
来源：http://bk.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eq.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://kn.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qf.newstarts.cn

TS:   [...arr].reverse();
来源：http://mt.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://az.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://mu.shxzskj.cn

Ruby: arr.reverse
来源：http://bj.shxzukj.cn

C#:   list.Reverse();
来源：http://uv.shxzskj.cn

[D12] 查找元素下标
来源：http://af.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://tv.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iq.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jq.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sg.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cn.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://xq.hnjuh.cn

Ruby: arr.index(x)
来源：http://mj.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ys.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://sn.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vx.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yq.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://qq.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ss.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ks.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mu.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://un.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jz.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://zh.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mj.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iv.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://wv.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://yq.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fo.lnxyls.cn

Go:   // 手写循环
来源：http://wu.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zd.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sd.yuexingan06.cn

[D15] 去重
来源：http://ju.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pl.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://qn.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://ys.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ny.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://he.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ab.nicolike.cn

Ruby: arr.uniq
来源：http://lq.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://se.bjjhwx.cn

[D16] 求和与平均值
来源：http://cg.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yh.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fd.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ui.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vv.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tx.haigaiapp.cn

Go:   // 手写循环累加
来源：http://er.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ks.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://jx.huanxung.cn

[D17] 最大值与最小值
来源：http://ui.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://df.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://gd.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ep.asd995.cn

TS:   Math.max(...arr);
来源：http://aw.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vo.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yy.521024.cn

Ruby: arr.max;  arr.min
来源：http://ue.asd995.cn

C#:   list.Max();  list.Min()
来源：http://rr.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ot.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oa.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ht.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cw.szsharing.cn

TS:   nested.flat();
来源：http://lw.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lj.szxytkj.cn

Go:   // 手写双层循环
来源：http://bi.colortex.cn

Ruby: nested.flatten
来源：http://nz.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uz.chemitech.net.cn

[D19] 按字段分组
来源：http://xa.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://va.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wt.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oi.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qy.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://we.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://us.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vq.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zb.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://lx.nszjky.cn

Py:   Counter(arr)
来源：http://iq.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://dk.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bc.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://fe.newstarts.cn

Ruby: arr.tally
来源：http://zj.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gz.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://iw.gzmigu.cn

Py:   x in arr
来源：http://jm.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://bi.9csxet.cn

JS:   arr.includes(x)
来源：http://uy.szsharing.cn

TS:   arr.includes(x)
来源：http://ut.shtwfgs.cn

Java: list.contains(x)
来源：http://ug.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://bz.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://of.shtwfgs.cn

C#:   list.Contains(x)
来源：http://ot.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://ce.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mp.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fn.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zn.szxytkj.cn

TS:   [...arr];
来源：http://iy.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://wt.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bx.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://ym.hahajie.cn

C#:   new List<int>(list);
来源：http://iz.hahajie.cn

[D23] reduce 累积计算
来源：http://fm.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ub.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fs.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://en.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rx.9csxet.cn

Go:   // 手写循环
来源：http://vk.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fy.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://go.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://zi.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gg.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kd.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lf.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pc.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xe.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lx.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zg.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zf.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://eq.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fn.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qs.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rk.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ni.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cr.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oh.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gp.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://py.shxzukj.cn

[D26] 数组转字符串
来源：http://jb.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://jh.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://nl.hnjuh.cn

JS:   arr.join(", ")
来源：http://xu.colortex.cn

TS:   arr.join(", ")
来源：http://ps.shxzukj.cn

Java: String.join(", ", list)
来源：http://uu.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://fs.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://wu.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://fg.muxihuayi.cn

================================================================================
来源：http://on.9csxet.cn

E. 字符串处理
来源：http://vf.chemitech.net.cn

================================================================================
来源：http://eb.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://us.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yr.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gs.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bw.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://az.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oi.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ig.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wl.lnxyls.cn

[E02] 重复字符串
来源：http://uo.jctech888.com.cn

Py:   "ab" * 3
来源：http://nv.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://kf.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ho.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ff.9csxet.cn

Java: "ab".repeat(3)
来源：http://kr.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://dl.shxzukj.cn

Ruby: "ab" * 3
来源：http://sp.yuntaijiaju.cn


<!-- 参考信息 -->