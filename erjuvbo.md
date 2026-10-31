代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://jg.chemitech.net.cn

C#:   using System.Text;
来源：http://lb.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ue.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://co.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://uq.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://cu.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://dg.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mg.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://kb.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://pf.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jg.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://yk.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kz.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ir.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aa.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://bq.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dv.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gf.panjiajie.cn

[C14] 泛型函数
来源：http://zd.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://un.colortex.cn

PHP:  // 无泛型
来源：http://py.bjjhwx.cn

JS:   // 无泛型
来源：http://xt.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fn.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ss.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vw.yuexingan06.cn

Ruby: # 无泛型
来源：http://rg.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://js.nicolike.cn

[C15] 解构 / 展开参数
来源：http://xt.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hl.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://fg.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://za.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hv.asd995.cn

Java: // 无解构
来源：http://qc.bjjhwx.cn

Go:   // 无解构
来源：http://hs.lnxyls.cn

Ruby: a, b = pair
来源：http://pb.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://yl.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ps.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://if.bjjhwx.cn

PHP:  // 无重载
来源：http://cm.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pb.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://rf.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://go.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://jy.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://xw.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ac.haigaiapp.cn

================================================================================
来源：http://gv.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://fq.shtwfgs.cn

================================================================================
来源：http://fs.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://kp.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ng.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ck.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fl.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ed.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kf.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://hm.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://wf.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ui.huanxung.cn

[D02] 追加元素到末尾
来源：http://cm.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nv.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hi.hnjuh.cn

JS:   arr.push(4);
来源：http://zn.huixiangedu.cn

TS:   arr.push(4);
来源：http://zp.bjjhwx.cn

Java: list.add(4);
来源：http://ya.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://xp.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://mn.hnjuh.cn

C#:   list.Add(4);
来源：http://hm.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://ud.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://qp.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tu.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ho.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://gr.panjiajie.cn

Java: list.add(0, 0);
来源：http://jw.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://op.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://da.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://rs.szsharing.cn

[D04] 删除元素
来源：http://hn.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wa.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://js.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://is.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://fp.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yg.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wz.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gw.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qz.huanxung.cn

[D05] 访问与修改元素
来源：http://nk.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mt.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yd.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tq.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://cs.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://vp.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://eh.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sv.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cv.9csxet.cn

[D06] 数组长度
来源：http://nq.lnxyls.cn

Py:   len(arr)
来源：http://hh.colortex.cn

PHP:  count($arr);
来源：http://fe.wgjwhj.cn

JS:   arr.length
来源：http://ov.bjjhwx.cn

TS:   arr.length
来源：http://iv.yuntaijiaju.cn

Java: list.size();
来源：http://kr.newstarts.cn

Go:   len(arr)
来源：http://pz.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://ff.bookmarksfly.cn

C#:   list.Count;
来源：http://um.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://fa.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kq.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yq.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://jx.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://qw.nicolike.cn

Java: list.subList(1, 4);
来源：http://lh.muxihuayi.cn

Go:   arr[1:4]
来源：http://qt.shxzukj.cn

Ruby: arr[1, 3]
来源：http://tn.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://qu.bookmarksfly.cn

[D08] 合并两个数组
来源：http://os.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://rz.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://en.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yw.hahajie.cn

TS:   [...a, ...b];
来源：http://bp.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cq.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://dz.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://tk.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://cy.9csxet.cn

[D09] 排序（升序）
来源：http://kh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://rs.yuexingan06.cn

PHP:  sort($arr);
来源：http://pn.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zm.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://md.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dm.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lg.wgjwhj.cn

Ruby: arr.sort
来源：http://hh.chemitech.net.cn

C#:   list.Sort();
来源：http://pf.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sn.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tl.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://px.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pj.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zb.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sc.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://un.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vh.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gh.hahajie.cn

[D11] 反转数组
来源：http://mu.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rc.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://pz.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ur.gzmigu.cn

TS:   [...arr].reverse();
来源：http://pk.shxzskj.cn

Java: Collections.reverse(list);
来源：http://sa.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://fm.wgjwhj.cn

Ruby: arr.reverse
来源：http://cc.panjiajie.cn

C#:   list.Reverse();
来源：http://gz.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://yo.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://zq.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xn.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ul.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bm.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dz.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://tv.shxzukj.cn

Ruby: arr.index(x)
来源：http://xz.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://yr.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://pu.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cs.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kv.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://zx.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://me.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ly.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vi.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oi.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ad.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://od.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://th.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yh.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://fx.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://lj.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pc.gzmigu.cn

Go:   // 手写循环
来源：http://sk.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ri.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hp.9csxet.cn

[D15] 去重
来源：http://ha.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ti.9csxet.cn

PHP:  array_unique($arr);
来源：http://xo.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://jd.szsharing.cn

TS:   [...new Set(arr)]
来源：http://qo.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sc.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pa.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://br.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://jd.shxzskj.cn

[D16] 求和与平均值
来源：http://lx.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://us.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ym.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ut.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cd.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ox.newstarts.cn

Go:   // 手写循环累加
来源：http://wi.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yt.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://se.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://os.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://ys.521024.cn

PHP:  max($arr);  min($arr);
来源：http://gw.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ft.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://rs.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bi.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dr.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://hj.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://az.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://as.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fi.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://nx.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ae.huanxung.cn

TS:   nested.flat();
来源：http://tg.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ob.yuexingan06.cn

Go:   // 手写双层循环
来源：http://qb.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://ew.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xh.jctech888.com.cn

[D19] 按字段分组
来源：http://ki.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uh.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ug.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gi.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pc.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://td.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://vu.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ez.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://se.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://so.shxzukj.cn

Py:   Counter(arr)
来源：http://yc.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://dz.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jh.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fi.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vt.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://uf.hnjuh.cn

Ruby: arr.tally
来源：http://me.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cq.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://mz.9csxet.cn

Py:   x in arr
来源：http://zc.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://od.nszjky.cn

JS:   arr.includes(x)
来源：http://kf.asd995.cn

TS:   arr.includes(x)
来源：http://el.panjiajie.cn

Java: list.contains(x)
来源：http://wb.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://qc.hnjuh.cn

Ruby: arr.include?(x)
来源：http://sr.yuexingan06.cn

C#:   list.Contains(x)
来源：http://za.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://lp.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yg.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ce.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://li.nicolike.cn

TS:   [...arr];
来源：http://os.nicolike.cn

Java: new ArrayList<>(list);
来源：http://eo.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xl.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://qv.shxzukj.cn

C#:   new List<int>(list);
来源：http://bt.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://qp.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dp.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ag.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dk.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rt.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ey.szxytkj.cn

Go:   // 手写循环
来源：http://in.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lr.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pz.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://ml.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sd.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lx.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ay.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pa.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ej.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zv.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aw.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sf.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://nx.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xe.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mo.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nx.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zt.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cz.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zf.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ep.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jp.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://aa.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://gr.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://wd.lnxyls.cn

JS:   arr.join(", ")
来源：http://lh.shtwfgs.cn

TS:   arr.join(", ")
来源：http://oz.huanxung.cn

Java: String.join(", ", list)
来源：http://gd.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://yb.nszjky.cn

Ruby: arr.join(", ")
来源：http://yp.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://up.huanxung.cn

================================================================================
来源：http://lx.nszjky.cn

E. 字符串处理
来源：http://sr.colortex.cn

================================================================================
来源：http://xi.lnxyls.cn

[E01] 拼接字符串
来源：http://ou.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rk.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nm.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iw.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://un.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://us.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xq.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oc.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xg.wgjwhj.cn

[E02] 重复字符串
来源：http://ky.asd995.cn

Py:   "ab" * 3
来源：http://oq.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ao.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://bs.bookmarksfly.cn


<!-- 参考信息 -->