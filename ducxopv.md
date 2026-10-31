代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://nv.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://bs.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://iq.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mr.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://qe.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://bh.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tg.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://ea.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pw.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yz.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qa.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zn.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ir.asd995.cn

Go:   func add(a, b int) int
来源：http://rd.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tv.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hi.shxzskj.cn

[C14] 泛型函数
来源：http://nl.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jb.shxzukj.cn

PHP:  // 无泛型
来源：http://kc.shxzskj.cn

JS:   // 无泛型
来源：http://yz.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uv.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ao.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iv.chemitech.net.cn

Ruby: # 无泛型
来源：http://li.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bt.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ym.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sr.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://yd.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sb.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ip.yuntaijiaju.cn

Java: // 无解构
来源：http://qd.yuexingan06.cn

Go:   // 无解构
来源：http://td.haigaiapp.cn

Ruby: a, b = pair
来源：http://gf.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://ll.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ap.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qk.asd995.cn

PHP:  // 无重载
来源：http://vt.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ve.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://fa.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://to.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://qj.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://jo.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aj.nszjky.cn

================================================================================
来源：http://xh.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ug.521024.cn

================================================================================
来源：http://kv.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://is.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jr.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fe.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kk.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pw.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kb.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ao.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://id.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ih.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://da.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kc.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xc.szxytkj.cn

JS:   arr.push(4);
来源：http://zt.muxihuayi.cn

TS:   arr.push(4);
来源：http://nr.jianghongdianzi.cn

Java: list.add(4);
来源：http://od.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://qy.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://cr.hnjuh.cn

C#:   list.Add(4);
来源：http://fq.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://fr.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://cu.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yb.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pk.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://wo.newstarts.cn

Java: list.add(0, 0);
来源：http://rs.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uz.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mt.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://tx.hahajie.cn

[D04] 删除元素
来源：http://jt.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ho.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qx.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ul.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://na.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uq.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xb.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ly.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wx.bjjhwx.cn

[D05] 访问与修改元素
来源：http://qa.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uf.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wh.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zl.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://dc.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://xo.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://us.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sd.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ir.nszjky.cn

[D06] 数组长度
来源：http://sh.chemitech.net.cn

Py:   len(arr)
来源：http://wy.gzmigu.cn

PHP:  count($arr);
来源：http://ij.yuexingan06.cn

JS:   arr.length
来源：http://ys.shxzukj.cn

TS:   arr.length
来源：http://xz.muxihuayi.cn

Java: list.size();
来源：http://vs.panjiajie.cn

Go:   len(arr)
来源：http://lk.newstarts.cn

Ruby: arr.length; arr.size
来源：http://uo.hnjuh.cn

C#:   list.Count;
来源：http://qo.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://zi.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vf.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zv.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://br.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ea.nicolike.cn

Java: list.subList(1, 4);
来源：http://aw.chemitech.net.cn

Go:   arr[1:4]
来源：http://rb.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://vs.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://pz.szxytkj.cn

[D08] 合并两个数组
来源：http://pm.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://oy.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://iw.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://so.nszjky.cn

TS:   [...a, ...b];
来源：http://xx.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://my.9csxet.cn

Go:   append(a, b...)
来源：http://oa.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://li.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://is.lnxyls.cn

[D09] 排序（升序）
来源：http://jn.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://pi.shtwfgs.cn

PHP:  sort($arr);
来源：http://pm.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gg.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://as.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xd.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://na.panjiajie.cn

Ruby: arr.sort
来源：http://lo.colortex.cn

C#:   list.Sort();
来源：http://zm.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ol.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dl.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ra.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qk.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pb.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yl.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wt.nicolike.cn

[D11] 反转数组
来源：http://mt.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ig.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ax.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cz.hahajie.cn

TS:   [...arr].reverse();
来源：http://kd.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://zs.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://sh.hnjuh.cn

Ruby: arr.reverse
来源：http://ok.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://bw.newstarts.cn

[D12] 查找元素下标
来源：http://ni.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://xf.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xj.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pt.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vs.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pi.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://kr.hnjuh.cn

Ruby: arr.index(x)
来源：http://iv.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ex.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://mr.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fo.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aq.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://zc.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://gj.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ef.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zk.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uz.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gn.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://rc.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yb.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ub.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://yv.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://ba.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ru.gzmigu.cn

Go:   // 手写循环
来源：http://hu.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wq.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ba.yuexingan06.cn

[D15] 去重
来源：http://hm.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rp.nszjky.cn

PHP:  array_unique($arr);
来源：http://vc.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://xe.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://mt.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ab.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wb.wgjwhj.cn

Ruby: arr.uniq
来源：http://ad.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://lr.asd995.cn

[D16] 求和与平均值
来源：http://hd.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rb.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ln.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://an.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hg.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://it.nszjky.cn

Go:   // 手写循环累加
来源：http://wa.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gz.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://iw.bjjhwx.cn

[D17] 最大值与最小值
来源：http://qn.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://bh.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://jc.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://le.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://qi.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gt.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rm.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://qq.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://nb.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://gn.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lq.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://zp.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ot.hahajie.cn

TS:   nested.flat();
来源：http://bd.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ff.szxytkj.cn

Go:   // 手写双层循环
来源：http://lq.hnjuh.cn

Ruby: nested.flatten
来源：http://ot.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ak.bjjhwx.cn

[D19] 按字段分组
来源：http://ky.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uw.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tm.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uk.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pf.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vu.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://hu.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lz.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pf.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://rs.colortex.cn

Py:   Counter(arr)
来源：http://hx.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://hd.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mj.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lp.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://bo.huanxung.cn

Ruby: arr.tally
来源：http://jv.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mh.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://oo.newstarts.cn

Py:   x in arr
来源：http://me.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://uv.nicolike.cn

JS:   arr.includes(x)
来源：http://tk.huixiangedu.cn

TS:   arr.includes(x)
来源：http://vp.521024.cn

Java: list.contains(x)
来源：http://qq.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://gc.nszjky.cn

Ruby: arr.include?(x)
来源：http://hf.shxzukj.cn

C#:   list.Contains(x)
来源：http://cl.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://ft.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ds.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tq.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xe.haigaiapp.cn

TS:   [...arr];
来源：http://fj.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://ed.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cz.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ei.gzmigu.cn

C#:   new List<int>(list);
来源：http://bb.bjjhwx.cn

[D23] reduce 累积计算
来源：http://wz.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jg.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vp.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://du.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ma.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xj.lnxyls.cn

Go:   // 手写循环
来源：http://as.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://th.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sn.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://zz.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tp.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rt.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xq.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sg.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zp.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wp.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ae.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yx.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://yc.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cf.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jc.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://je.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ul.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ry.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nk.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fz.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vu.shtwfgs.cn

[D26] 数组转字符串
来源：http://gz.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://dr.asd995.cn

PHP:  implode(", ", $arr);
来源：http://ni.hahajie.cn

JS:   arr.join(", ")
来源：http://my.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://pw.muxihuayi.cn

Java: String.join(", ", list)
来源：http://rf.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://oy.newstarts.cn

Ruby: arr.join(", ")
来源：http://bv.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ik.szxytkj.cn

================================================================================
来源：http://cb.gzmigu.cn

E. 字符串处理
来源：http://tv.shxzukj.cn

================================================================================
来源：http://gl.521024.cn

[E01] 拼接字符串
来源：http://gk.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lf.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mi.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ty.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bq.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://di.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jw.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ta.chemitech.net.cn

[E02] 重复字符串
来源：http://dt.szsharing.cn

Py:   "ab" * 3
来源：http://wm.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://pw.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ay.9csxet.cn

TS:   "ab".repeat(3)
来源：http://zm.panjiajie.cn

Java: "ab".repeat(3)
来源：http://pb.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://fo.newstarts.cn

Ruby: "ab" * 3
来源：http://lr.jctech888.com.cn


<!-- 参考信息 -->