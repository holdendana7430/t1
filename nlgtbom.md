代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://ft.bjjhwx.cn

C#:   using System.Text;
来源：http://nw.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://ak.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://hw.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://vn.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://mm.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://qo.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nu.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://fs.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ef.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fs.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://ao.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bm.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fx.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ah.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zs.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vc.colortex.cn

Go:   func add(a, b int) int
来源：http://uu.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ww.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bx.huanxung.cn

[C14] 泛型函数
来源：http://bu.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lx.gzmigu.cn

PHP:  // 无泛型
来源：http://ds.huixiangedu.cn

JS:   // 无泛型
来源：http://cn.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hy.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lr.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ik.asd995.cn

Ruby: # 无泛型
来源：http://es.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vn.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://eq.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lo.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://rr.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gg.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ot.wgjwhj.cn

Java: // 无解构
来源：http://mm.yuexingan06.cn

Go:   // 无解构
来源：http://hg.szxytkj.cn

Ruby: a, b = pair
来源：http://cv.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://xf.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://xg.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vl.nicolike.cn

PHP:  // 无重载
来源：http://zo.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lp.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://qv.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dn.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://wq.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://fr.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xo.shxzukj.cn

================================================================================
来源：http://zb.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://yg.yuexingan06.cn

================================================================================
来源：http://mu.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://qc.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sy.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ev.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kw.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mg.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xx.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://gh.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://bz.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nf.panjiajie.cn

[D02] 追加元素到末尾
来源：http://ui.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://en.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://db.shtwfgs.cn

JS:   arr.push(4);
来源：http://nr.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://rs.bookmarksfly.cn

Java: list.add(4);
来源：http://ta.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://jc.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ng.shtwfgs.cn

C#:   list.Add(4);
来源：http://rx.hahajie.cn

[D03] 在指定位置插入元素
来源：http://zc.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://qs.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://an.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tl.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://ky.newstarts.cn

Java: list.add(0, 0);
来源：http://ku.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fe.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wi.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://iu.haigaiapp.cn

[D04] 删除元素
来源：http://fi.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://si.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://il.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ks.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://md.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://am.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oi.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lq.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ly.szxytkj.cn

[D05] 访问与修改元素
来源：http://vo.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oc.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tc.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qj.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://sg.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ke.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://jd.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kp.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nx.chemitech.net.cn

[D06] 数组长度
来源：http://vt.bjjhwx.cn

Py:   len(arr)
来源：http://yq.hnjuh.cn

PHP:  count($arr);
来源：http://kh.hnjuh.cn

JS:   arr.length
来源：http://jg.bjjhwx.cn

TS:   arr.length
来源：http://ee.panjiajie.cn

Java: list.size();
来源：http://li.jctech888.com.cn

Go:   len(arr)
来源：http://gr.szsharing.cn

Ruby: arr.length; arr.size
来源：http://cv.hahajie.cn

C#:   list.Count;
来源：http://bp.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://sz.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://js.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fr.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ch.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://fw.gzmigu.cn

Java: list.subList(1, 4);
来源：http://wg.lnxyls.cn

Go:   arr[1:4]
来源：http://hi.gzmigu.cn

Ruby: arr[1, 3]
来源：http://fm.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://kk.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://na.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://xh.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://ib.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fe.huixiangedu.cn

TS:   [...a, ...b];
来源：http://ga.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vu.huixiangedu.cn

Go:   append(a, b...)
来源：http://kr.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://dk.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://nt.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ex.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lb.muxihuayi.cn

PHP:  sort($arr);
来源：http://fb.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xp.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oz.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yw.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://de.yuexingan06.cn

Ruby: arr.sort
来源：http://qi.huanxung.cn

C#:   list.Sort();
来源：http://hp.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ro.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jy.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jt.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ct.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qw.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hb.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bm.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fq.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sx.haigaiapp.cn

[D11] 反转数组
来源：http://bn.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xr.nszjky.cn

PHP:  array_reverse($arr);
来源：http://dq.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ju.lnxyls.cn

TS:   [...arr].reverse();
来源：http://hd.9csxet.cn

Java: Collections.reverse(list);
来源：http://uk.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://kc.huanxung.cn

Ruby: arr.reverse
来源：http://yp.chemitech.net.cn

C#:   list.Reverse();
来源：http://qr.521024.cn

[D12] 查找元素下标
来源：http://kz.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://ca.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hp.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mq.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fn.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ye.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://us.nicolike.cn

Ruby: arr.index(x)
来源：http://sy.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://dp.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://iv.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://te.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ji.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://gv.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://kw.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zy.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pg.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bq.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jf.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://ou.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hf.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vz.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://os.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://th.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zu.muxihuayi.cn

Go:   // 手写循环
来源：http://ec.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xl.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ou.chemitech.net.cn

[D15] 去重
来源：http://bz.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uy.hahajie.cn

PHP:  array_unique($arr);
来源：http://hx.hahajie.cn

JS:   [...new Set(arr)]
来源：http://jq.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://wo.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qv.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gq.9csxet.cn

Ruby: arr.uniq
来源：http://yc.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://to.shxzukj.cn

[D16] 求和与平均值
来源：http://kp.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gs.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yd.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ds.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rf.nicolike.cn

Go:   // 手写循环累加
来源：http://yy.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ng.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://wi.szsharing.cn

[D17] 最大值与最小值
来源：http://iz.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://sp.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://nv.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yv.newstarts.cn

TS:   Math.max(...arr);
来源：http://ar.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zo.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jg.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://dz.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://oi.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://vc.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ja.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://gp.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nn.shtwfgs.cn

TS:   nested.flat();
来源：http://ac.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oo.nicolike.cn

Go:   // 手写双层循环
来源：http://xq.bjjhwx.cn

Ruby: nested.flatten
来源：http://vq.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mk.panjiajie.cn

[D19] 按字段分组
来源：http://fi.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fn.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yz.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ni.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zq.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tt.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://tp.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ba.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sd.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://dx.haigaiapp.cn

Py:   Counter(arr)
来源：http://bu.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://gi.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nf.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://it.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cq.nicolike.cn

Go:   // 手写 map[T]int
来源：http://pa.gzmigu.cn

Ruby: arr.tally
来源：http://rz.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kr.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://js.wgjwhj.cn

Py:   x in arr
来源：http://ey.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://zf.lnxyls.cn

JS:   arr.includes(x)
来源：http://of.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://og.bookmarksfly.cn

Java: list.contains(x)
来源：http://jm.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://dn.shxzskj.cn

Ruby: arr.include?(x)
来源：http://gq.shxzskj.cn

C#:   list.Contains(x)
来源：http://al.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ct.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ue.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://db.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oo.haigaiapp.cn

TS:   [...arr];
来源：http://eq.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ci.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ty.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://tp.nszjky.cn

C#:   new List<int>(list);
来源：http://uw.panjiajie.cn

[D23] reduce 累积计算
来源：http://vn.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xs.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zf.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ol.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rf.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fd.huixiangedu.cn

Go:   // 手写循环
来源：http://kj.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bk.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mr.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://yw.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://px.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mq.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vp.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ok.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zi.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vr.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ta.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ri.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://kt.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qi.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fs.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hg.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://va.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://so.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://be.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aq.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yy.shtwfgs.cn

[D26] 数组转字符串
来源：http://jr.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://ue.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://bl.muxihuayi.cn

JS:   arr.join(", ")
来源：http://wy.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://pw.szsharing.cn

Java: String.join(", ", list)
来源：http://aq.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://in.shxzskj.cn

Ruby: arr.join(", ")
来源：http://jl.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://qi.haigaiapp.cn

================================================================================
来源：http://su.szsharing.cn

E. 字符串处理
来源：http://tu.hnjuh.cn

================================================================================
来源：http://bo.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://lv.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uf.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wc.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nu.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hf.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iw.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mx.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lp.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://df.521024.cn

[E02] 重复字符串
来源：http://yp.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://nd.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://fk.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://iu.bookmarksfly.cn


<!-- 参考信息 -->