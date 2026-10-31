代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://pb.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://nm.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wj.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ik.panjiajie.cn

[C14] 泛型函数
来源：http://kh.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uq.521024.cn

PHP:  // 无泛型
来源：http://px.asd995.cn

JS:   // 无泛型
来源：http://zz.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ii.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nm.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xo.szsharing.cn

Ruby: # 无泛型
来源：http://qh.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kj.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ir.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lu.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://uo.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pa.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jk.bjjhwx.cn

Java: // 无解构
来源：http://kk.newstarts.cn

Go:   // 无解构
来源：http://hw.shxzukj.cn

Ruby: a, b = pair
来源：http://pp.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://uk.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://bj.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sh.asd995.cn

PHP:  // 无重载
来源：http://af.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hq.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://hy.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nr.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ew.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://gh.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ul.asd995.cn

================================================================================
来源：http://vh.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://nz.hnjuh.cn

================================================================================
来源：http://fr.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://rf.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xp.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://br.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pb.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ux.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://un.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://er.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://nj.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sq.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://rx.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kn.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ba.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ft.9csxet.cn

TS:   arr.push(4);
来源：http://eu.shxzukj.cn

Java: list.add(4);
来源：http://be.asd995.cn

Go:   arr = append(arr, 4)
来源：http://vd.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://is.haigaiapp.cn

C#:   list.Add(4);
来源：http://sd.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://bt.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://yg.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nx.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sr.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ya.jctech888.com.cn

Java: list.add(0, 0);
来源：http://jb.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://id.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ay.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://oz.yuntaijiaju.cn

[D04] 删除元素
来源：http://ra.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://no.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ar.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iu.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://tj.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kf.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hu.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lf.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wk.shxzukj.cn

[D05] 访问与修改元素
来源：http://zm.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://th.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hl.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iz.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://xy.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://fd.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://tw.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vo.shxzskj.cn

[D06] 数组长度
来源：http://tk.muxihuayi.cn

Py:   len(arr)
来源：http://zj.chemitech.net.cn

PHP:  count($arr);
来源：http://rr.lnxyls.cn

JS:   arr.length
来源：http://bh.hahajie.cn

TS:   arr.length
来源：http://lg.jianghongdianzi.cn

Java: list.size();
来源：http://ol.huixiangedu.cn

Go:   len(arr)
来源：http://pg.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://vz.jctech888.com.cn

C#:   list.Count;
来源：http://lp.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://zm.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ns.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://md.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://bk.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://xw.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ah.bookmarksfly.cn

Go:   arr[1:4]
来源：http://ah.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://ie.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ak.521024.cn

[D08] 合并两个数组
来源：http://kt.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://mu.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://yc.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gs.muxihuayi.cn

TS:   [...a, ...b];
来源：http://dr.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gr.muxihuayi.cn

Go:   append(a, b...)
来源：http://oc.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://vz.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://mq.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://bf.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://rb.bjjhwx.cn

PHP:  sort($arr);
来源：http://ls.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://as.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vx.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ty.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://db.jctech888.com.cn

Ruby: arr.sort
来源：http://jl.gzmigu.cn

C#:   list.Sort();
来源：http://lc.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lm.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oc.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ai.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hf.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hg.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ou.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ag.huanxung.cn

[D11] 反转数组
来源：http://gz.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kx.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://fi.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gq.gzmigu.cn

TS:   [...arr].reverse();
来源：http://nk.hahajie.cn

Java: Collections.reverse(list);
来源：http://cs.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://dw.newstarts.cn

Ruby: arr.reverse
来源：http://va.huixiangedu.cn

C#:   list.Reverse();
来源：http://wk.lnxyls.cn

[D12] 查找元素下标
来源：http://mk.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://sb.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sy.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ys.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tg.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uq.521024.cn

Go:   slices.Index(arr, x)
来源：http://vk.asd995.cn

Ruby: arr.index(x)
来源：http://fc.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://xa.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://zz.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zr.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xc.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://hl.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://tt.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mm.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pq.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ve.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tj.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://zj.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yt.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xz.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://pc.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://ni.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sh.szsharing.cn

Go:   // 手写循环
来源：http://qe.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vm.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lv.nszjky.cn

[D15] 去重
来源：http://dk.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://av.nicolike.cn

PHP:  array_unique($arr);
来源：http://lz.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://pd.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://fr.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://du.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cj.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://az.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://nx.shtwfgs.cn

[D16] 求和与平均值
来源：http://cl.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nj.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uc.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fe.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xd.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wf.szxytkj.cn

Go:   // 手写循环累加
来源：http://zv.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qj.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://pq.gzmigu.cn

[D17] 最大值与最小值
来源：http://az.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ns.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://bq.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pp.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://hp.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ma.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fh.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://ym.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://yz.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://sb.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pz.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://xj.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dl.huanxung.cn

TS:   nested.flat();
来源：http://wh.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gc.bjjhwx.cn

Go:   // 手写双层循环
来源：http://me.bjjhwx.cn

Ruby: nested.flatten
来源：http://wy.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xa.newstarts.cn

[D19] 按字段分组
来源：http://bh.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vs.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fu.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bp.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ro.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vf.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://zm.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cx.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://za.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://rk.chemitech.net.cn

Py:   Counter(arr)
来源：http://rd.asd995.cn

PHP:  array_count_values($arr);
来源：http://xk.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ma.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jy.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xk.asd995.cn

Go:   // 手写 map[T]int
来源：http://yl.muxihuayi.cn

Ruby: arr.tally
来源：http://gs.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tv.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://lv.jianghongdianzi.cn

Py:   x in arr
来源：http://pl.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://bc.lnxyls.cn

JS:   arr.includes(x)
来源：http://se.haigaiapp.cn

TS:   arr.includes(x)
来源：http://cw.shxzukj.cn

Java: list.contains(x)
来源：http://ty.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://yq.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://jd.521024.cn

C#:   list.Contains(x)
来源：http://tc.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://hj.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ue.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pg.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hh.shxzskj.cn

TS:   [...arr];
来源：http://es.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://vp.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://da.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://io.yuexingan06.cn

C#:   new List<int>(list);
来源：http://jn.9csxet.cn

[D23] reduce 累积计算
来源：http://an.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pd.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zm.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mv.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://at.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rs.shtwfgs.cn

Go:   // 手写循环
来源：http://ku.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://av.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uz.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ug.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bk.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kg.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://df.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qv.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://or.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sl.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vr.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cd.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://uy.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ey.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ew.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oj.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mp.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ib.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ba.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ng.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ie.jctech888.com.cn

[D26] 数组转字符串
来源：http://ga.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://iz.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://nt.9csxet.cn

JS:   arr.join(", ")
来源：http://fg.9csxet.cn

TS:   arr.join(", ")
来源：http://ue.hahajie.cn

Java: String.join(", ", list)
来源：http://yp.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://jz.panjiajie.cn

Ruby: arr.join(", ")
来源：http://pn.521024.cn

C#:   string.Join(", ", list)
来源：http://yt.panjiajie.cn

================================================================================
来源：http://vr.szsharing.cn

E. 字符串处理
来源：http://wf.bjjhwx.cn

================================================================================
来源：http://hs.haigaiapp.cn

[E01] 拼接字符串
来源：http://ux.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yw.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ao.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iw.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ph.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://di.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tp.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ge.bookmarksfly.cn

[E02] 重复字符串
来源：http://ym.bookmarksfly.cn

Py:   "ab" * 3
来源：http://lw.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://us.colortex.cn

JS:   "ab".repeat(3)
来源：http://xj.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://lu.lnxyls.cn

Java: "ab".repeat(3)
来源：http://up.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://qb.yuexingan06.cn

Ruby: "ab" * 3
来源：http://cd.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cy.wgjwhj.cn

[E03] 截取子串
来源：http://zc.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pd.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uj.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pz.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://vs.newstarts.cn

Java: s.substring(1, 4)
来源：http://do.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wu.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uo.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://na.newstarts.cn

[E04] 查找子串位置
来源：http://ct.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://dg.nicolike.cn


<!-- 参考信息 -->