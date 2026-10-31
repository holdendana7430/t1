代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ht.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://gv.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://tu.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://db.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://kr.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://qj.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mr.521024.cn

[C13] 类型声明 / 类型注解
来源：http://xx.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ir.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vs.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gj.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yv.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ah.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://kd.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ev.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rh.gzmigu.cn

[C14] 泛型函数
来源：http://kq.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://op.shxzskj.cn

PHP:  // 无泛型
来源：http://ro.wgjwhj.cn

JS:   // 无泛型
来源：http://lz.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tt.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://km.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vh.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://co.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ce.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://zg.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sj.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ob.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ec.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kc.shtwfgs.cn

Java: // 无解构
来源：http://vc.newstarts.cn

Go:   // 无解构
来源：http://hw.bjjhwx.cn

Ruby: a, b = pair
来源：http://hv.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://ll.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://nx.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ob.hnjuh.cn

PHP:  // 无重载
来源：http://bq.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cn.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://xp.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gl.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://ok.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://nv.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zh.hnjuh.cn

================================================================================
来源：http://lo.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://cd.gzmigu.cn

================================================================================
来源：http://gn.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://zz.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uj.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://of.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lq.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ab.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gu.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://lt.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://mx.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sj.hnjuh.cn

[D02] 追加元素到末尾
来源：http://nr.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hh.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cr.9csxet.cn

JS:   arr.push(4);
来源：http://jx.chemitech.net.cn

TS:   arr.push(4);
来源：http://mu.chemitech.net.cn

Java: list.add(4);
来源：http://ib.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://uk.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://ly.bjjhwx.cn

C#:   list.Add(4);
来源：http://oi.9csxet.cn

[D03] 在指定位置插入元素
来源：http://dr.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://bz.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vy.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ii.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://do.szsharing.cn

Java: list.add(0, 0);
来源：http://ia.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cc.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iz.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://oj.asd995.cn

[D04] 删除元素
来源：http://ow.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xa.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eg.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qr.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://iy.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://op.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qc.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iv.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oz.bjjhwx.cn

[D05] 访问与修改元素
来源：http://sw.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qa.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rr.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fn.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ws.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://mw.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://hb.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mp.shtwfgs.cn

[D06] 数组长度
来源：http://hc.muxihuayi.cn

Py:   len(arr)
来源：http://ns.hahajie.cn

PHP:  count($arr);
来源：http://yl.chemitech.net.cn

JS:   arr.length
来源：http://vj.chemitech.net.cn

TS:   arr.length
来源：http://vh.huixinmuqiang.cn

Java: list.size();
来源：http://mw.newstarts.cn

Go:   len(arr)
来源：http://cj.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://sv.hahajie.cn

C#:   list.Count;
来源：http://dl.nszjky.cn

[D07] 切片 / 取子数组
来源：http://tf.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bz.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mm.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://om.521024.cn

TS:   arr.slice(1, 4);
来源：http://mi.lnxyls.cn

Java: list.subList(1, 4);
来源：http://vo.521024.cn

Go:   arr[1:4]
来源：http://pd.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://fl.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://hk.lnxyls.cn

[D08] 合并两个数组
来源：http://au.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://un.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://fh.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xf.hahajie.cn

TS:   [...a, ...b];
来源：http://qs.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iw.szsharing.cn

Go:   append(a, b...)
来源：http://fh.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://zo.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://re.hnjuh.cn

[D09] 排序（升序）
来源：http://yh.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ps.chemitech.net.cn

PHP:  sort($arr);
来源：http://wa.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mf.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tt.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uq.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ol.chemitech.net.cn

Ruby: arr.sort
来源：http://kp.asd995.cn

C#:   list.Sort();
来源：http://cc.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ac.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hd.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vt.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://az.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rj.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fn.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lg.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rs.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rp.gzmigu.cn

[D11] 反转数组
来源：http://lo.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bz.szsharing.cn

PHP:  array_reverse($arr);
来源：http://bz.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yp.9csxet.cn

TS:   [...arr].reverse();
来源：http://jp.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://jv.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://xn.9csxet.cn

Ruby: arr.reverse
来源：http://bi.nszjky.cn

C#:   list.Reverse();
来源：http://cl.lnxyls.cn

[D12] 查找元素下标
来源：http://ha.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://kk.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wd.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dw.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ji.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vi.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://ap.panjiajie.cn

Ruby: arr.index(x)
来源：http://iz.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://or.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://kf.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sm.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mi.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://ru.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ar.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cj.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://il.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vz.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bi.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://jg.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jz.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://na.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://gv.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://jj.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jj.panjiajie.cn

Go:   // 手写循环
来源：http://zp.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jt.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://il.bjjhwx.cn

[D15] 去重
来源：http://hm.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ij.colortex.cn

PHP:  array_unique($arr);
来源：http://pa.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://sx.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://pm.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lb.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zf.huixiangedu.cn

Ruby: arr.uniq
来源：http://nw.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://jz.haigaiapp.cn

[D16] 求和与平均值
来源：http://oc.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sg.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://na.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tv.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dq.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://le.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ps.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://in.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://kv.szsharing.cn

[D17] 最大值与最小值
来源：http://am.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://yy.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ro.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mj.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://sp.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iq.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://as.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://nr.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://nc.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://md.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cw.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://xs.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://do.yuexingan06.cn

TS:   nested.flat();
来源：http://zh.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sz.shxzukj.cn

Go:   // 手写双层循环
来源：http://oa.yuexingan06.cn

Ruby: nested.flatten
来源：http://pa.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ki.nicolike.cn

[D19] 按字段分组
来源：http://yo.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gr.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ur.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qh.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ug.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rb.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://tr.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bl.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ep.colortex.cn

[D20] 统计每个元素出现次数
来源：http://lk.huixiangedu.cn

Py:   Counter(arr)
来源：http://dy.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://jk.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pw.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rg.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ye.haigaiapp.cn

Ruby: arr.tally
来源：http://mq.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ge.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://rc.yuntaijiaju.cn

Py:   x in arr
来源：http://ws.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://go.nszjky.cn

JS:   arr.includes(x)
来源：http://gf.lnxyls.cn

TS:   arr.includes(x)
来源：http://tf.huixiangedu.cn

Java: list.contains(x)
来源：http://vu.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://vb.hnjuh.cn

Ruby: arr.include?(x)
来源：http://os.jctech888.com.cn

C#:   list.Contains(x)
来源：http://fg.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://ud.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xa.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gq.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dv.colortex.cn

TS:   [...arr];
来源：http://hx.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://hu.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ud.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://zt.huixiangedu.cn

C#:   new List<int>(list);
来源：http://mi.colortex.cn

[D23] reduce 累积计算
来源：http://fk.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://av.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fd.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ib.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mz.nicolike.cn

Go:   // 手写循环
来源：http://cq.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dn.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://te.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://ss.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uq.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://at.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oi.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ah.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://om.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vl.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://by.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lp.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://am.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qe.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oz.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jw.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oy.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nr.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lo.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tg.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hb.hahajie.cn

[D26] 数组转字符串
来源：http://hy.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://cx.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://pg.bjjhwx.cn

JS:   arr.join(", ")
来源：http://zq.newstarts.cn

TS:   arr.join(", ")
来源：http://qd.yuexingan06.cn

Java: String.join(", ", list)
来源：http://cb.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://ys.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://no.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://kb.yuntaijiaju.cn

================================================================================
来源：http://nx.colortex.cn

E. 字符串处理
来源：http://md.521024.cn

================================================================================
来源：http://vw.hnjuh.cn

[E01] 拼接字符串
来源：http://xu.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rs.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ok.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://on.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mr.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://us.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hf.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vj.haigaiapp.cn

[E02] 重复字符串
来源：http://nb.asd995.cn

Py:   "ab" * 3
来源：http://oj.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://yt.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ya.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://jo.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://xq.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://vd.panjiajie.cn

Ruby: "ab" * 3
来源：http://ox.jctech888.com.cn


<!-- 参考信息 -->