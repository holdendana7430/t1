代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://oy.shxzskj.cn

C#:   using System.Text;
来源：http://ev.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://py.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://re.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://en.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://rr.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://bz.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dw.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://jn.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ks.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jr.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://tw.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fg.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lq.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ki.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rh.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yw.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://bu.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://no.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mh.shxzskj.cn

[C14] 泛型函数
来源：http://su.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zk.szsharing.cn

PHP:  // 无泛型
来源：http://vq.muxihuayi.cn

JS:   // 无泛型
来源：http://rq.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xc.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tf.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://me.jctech888.com.cn

Ruby: # 无泛型
来源：http://mz.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zq.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://oq.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zb.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://er.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://re.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ce.wgjwhj.cn

Java: // 无解构
来源：http://yc.asd995.cn

Go:   // 无解构
来源：http://gr.bookmarksfly.cn

Ruby: a, b = pair
来源：http://jh.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ht.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ih.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qi.shxzukj.cn

PHP:  // 无重载
来源：http://ch.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pt.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://hw.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sa.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://wy.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://kt.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.huixinmuqiang.cn

================================================================================
来源：http://wb.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://po.shtwfgs.cn

================================================================================
来源：http://wb.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://jp.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vt.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mb.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wy.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://od.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vw.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://dr.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://aa.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bg.szsharing.cn

[D02] 追加元素到末尾
来源：http://jb.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yk.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yc.shtwfgs.cn

JS:   arr.push(4);
来源：http://vu.hahajie.cn

TS:   arr.push(4);
来源：http://fl.hnjuh.cn

Java: list.add(4);
来源：http://ne.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://kl.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://mx.newstarts.cn

C#:   list.Add(4);
来源：http://wd.521024.cn

[D03] 在指定位置插入元素
来源：http://ec.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://or.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jo.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fq.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://py.9csxet.cn

Java: list.add(0, 0);
来源：http://pg.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xx.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://st.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://cy.jianghongdianzi.cn

[D04] 删除元素
来源：http://xc.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ps.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pr.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sm.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://mc.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ms.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mb.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mb.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bk.nicolike.cn

[D05] 访问与修改元素
来源：http://op.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://be.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uj.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://xp.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://sq.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://vq.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lo.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lp.asd995.cn

[D06] 数组长度
来源：http://qe.lnxyls.cn

Py:   len(arr)
来源：http://ng.haigaiapp.cn

PHP:  count($arr);
来源：http://pe.huixinmuqiang.cn

JS:   arr.length
来源：http://he.nszjky.cn

TS:   arr.length
来源：http://nu.szsharing.cn

Java: list.size();
来源：http://sz.panjiajie.cn

Go:   len(arr)
来源：http://ce.asd995.cn

Ruby: arr.length; arr.size
来源：http://sm.jctech888.com.cn

C#:   list.Count;
来源：http://jy.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://vl.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rn.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zs.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ii.asd995.cn

TS:   arr.slice(1, 4);
来源：http://dn.hahajie.cn

Java: list.subList(1, 4);
来源：http://li.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://or.9csxet.cn

Ruby: arr[1, 3]
来源：http://rq.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://iv.asd995.cn

[D08] 合并两个数组
来源：http://ss.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://fm.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://rr.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://di.szsharing.cn

TS:   [...a, ...b];
来源：http://mt.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zx.szsharing.cn

Go:   append(a, b...)
来源：http://hd.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://fa.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ts.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://te.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://rj.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://qp.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xm.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sm.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yp.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gp.bookmarksfly.cn

Ruby: arr.sort
来源：http://kl.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ws.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qj.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ow.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://il.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mh.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yj.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://st.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ds.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ze.muxihuayi.cn

[D11] 反转数组
来源：http://pa.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ai.asd995.cn

PHP:  array_reverse($arr);
来源：http://el.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ka.lnxyls.cn

TS:   [...arr].reverse();
来源：http://oy.panjiajie.cn

Java: Collections.reverse(list);
来源：http://jz.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://wo.hahajie.cn

Ruby: arr.reverse
来源：http://rl.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://vp.wgjwhj.cn

[D12] 查找元素下标
来源：http://pf.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://mp.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bl.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://di.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mj.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://om.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://jc.521024.cn

Ruby: arr.index(x)
来源：http://yn.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://dd.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://iy.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ti.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jv.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://hs.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://vi.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ue.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uv.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jr.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ot.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://mf.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uv.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qs.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://cw.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://sn.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ud.521024.cn

Go:   // 手写循环
来源：http://xo.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ye.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dw.yuntaijiaju.cn

[D15] 去重
来源：http://mh.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vl.huanxung.cn

PHP:  array_unique($arr);
来源：http://ae.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://gv.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://tf.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rn.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xc.nicolike.cn

Ruby: arr.uniq
来源：http://qa.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://nj.asd995.cn

[D16] 求和与平均值
来源：http://dr.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ke.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zj.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ct.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ys.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uv.hnjuh.cn

Go:   // 手写循环累加
来源：http://eq.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wf.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://so.muxihuayi.cn

[D17] 最大值与最小值
来源：http://so.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://kg.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://nm.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pw.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://lx.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jd.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mr.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://cg.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://te.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://yk.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ih.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://pf.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fv.lnxyls.cn

TS:   nested.flat();
来源：http://sm.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tx.huixiangedu.cn

Go:   // 手写双层循环
来源：http://fm.521024.cn

Ruby: nested.flatten
来源：http://yv.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://du.bookmarksfly.cn

[D19] 按字段分组
来源：http://yh.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ac.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wi.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ip.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yz.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hv.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://lv.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aj.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://od.521024.cn

[D20] 统计每个元素出现次数
来源：http://at.shtwfgs.cn

Py:   Counter(arr)
来源：http://ps.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://px.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mn.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bx.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yw.newstarts.cn

Go:   // 手写 map[T]int
来源：http://km.panjiajie.cn

Ruby: arr.tally
来源：http://kj.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gc.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://ri.chemitech.net.cn

Py:   x in arr
来源：http://jy.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ve.shxzukj.cn

JS:   arr.includes(x)
来源：http://pr.huanxung.cn

TS:   arr.includes(x)
来源：http://ix.9csxet.cn

Java: list.contains(x)
来源：http://ls.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://bl.nszjky.cn

Ruby: arr.include?(x)
来源：http://tb.gzmigu.cn

C#:   list.Contains(x)
来源：http://pg.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://so.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ud.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vk.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ls.szsharing.cn

TS:   [...arr];
来源：http://lr.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ao.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kq.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://mc.panjiajie.cn

C#:   new List<int>(list);
来源：http://ji.haigaiapp.cn

[D23] reduce 累积计算
来源：http://pl.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sw.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://te.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yi.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sc.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vr.huixiangedu.cn

Go:   // 手写循环
来源：http://hr.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wd.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cg.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://md.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ls.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jw.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tg.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ke.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sw.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kr.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oh.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wn.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://hf.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tl.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xz.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fn.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hv.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uk.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ku.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hq.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zj.nicolike.cn

[D26] 数组转字符串
来源：http://as.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://ph.colortex.cn

PHP:  implode(", ", $arr);
来源：http://lv.nicolike.cn

JS:   arr.join(", ")
来源：http://dh.colortex.cn

TS:   arr.join(", ")
来源：http://lx.wgjwhj.cn

Java: String.join(", ", list)
来源：http://im.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://pp.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://yo.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://yo.wgjwhj.cn

================================================================================
来源：http://lv.shxzskj.cn

E. 字符串处理
来源：http://fo.9csxet.cn

================================================================================
来源：http://pz.huanxung.cn

[E01] 拼接字符串
来源：http://on.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ae.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bl.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pe.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ay.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vm.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://be.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hv.9csxet.cn

[E02] 重复字符串
来源：http://ac.muxihuayi.cn

Py:   "ab" * 3
来源：http://hp.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://aw.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://nd.nicolike.cn


<!-- 参考信息 -->