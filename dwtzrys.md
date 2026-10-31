代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qb.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://it.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nq.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://bm.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ks.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fm.newstarts.cn

Java: // 无解构
来源：http://am.huixiangedu.cn

Go:   // 无解构
来源：http://ft.yuexingan06.cn

Ruby: a, b = pair
来源：http://oz.hahajie.cn

C#:   var (a, b) = pair;
来源：http://rm.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://as.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pm.szxytkj.cn

PHP:  // 无重载
来源：http://gu.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mj.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://we.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://du.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://qm.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://lj.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zc.shtwfgs.cn

================================================================================
来源：http://mb.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://hw.haigaiapp.cn

================================================================================
来源：http://ih.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://dy.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cq.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kj.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ss.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pi.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lt.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://bz.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://wj.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tv.nicolike.cn

[D02] 追加元素到末尾
来源：http://nm.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oc.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wf.shtwfgs.cn

JS:   arr.push(4);
来源：http://oa.szxytkj.cn

TS:   arr.push(4);
来源：http://yg.lnxyls.cn

Java: list.add(4);
来源：http://za.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://gt.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://dr.colortex.cn

C#:   list.Add(4);
来源：http://wt.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ib.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://cz.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xy.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ce.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ya.hnjuh.cn

Java: list.add(0, 0);
来源：http://nc.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ll.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xe.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://hw.jianghongdianzi.cn

[D04] 删除元素
来源：http://go.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://am.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fg.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ah.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://xw.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ej.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pr.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mx.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eb.shxzukj.cn

[D05] 访问与修改元素
来源：http://wf.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kc.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://md.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bh.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://wp.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://dw.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ph.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nh.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xr.muxihuayi.cn

[D06] 数组长度
来源：http://gi.hnjuh.cn

Py:   len(arr)
来源：http://nv.huanxung.cn

PHP:  count($arr);
来源：http://gf.szxytkj.cn

JS:   arr.length
来源：http://gf.shxzukj.cn

TS:   arr.length
来源：http://wc.shtwfgs.cn

Java: list.size();
来源：http://fa.shtwfgs.cn

Go:   len(arr)
来源：http://te.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://hg.jctech888.com.cn

C#:   list.Count;
来源：http://fs.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://eo.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uk.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ye.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://sy.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://xs.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://yi.panjiajie.cn

Go:   arr[1:4]
来源：http://dw.lnxyls.cn

Ruby: arr[1, 3]
来源：http://jj.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://sg.nicolike.cn

[D08] 合并两个数组
来源：http://dq.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://zv.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://dk.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://st.panjiajie.cn

TS:   [...a, ...b];
来源：http://ps.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://at.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://fa.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ja.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://xq.shxzskj.cn

[D09] 排序（升序）
来源：http://xb.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mk.521024.cn

PHP:  sort($arr);
来源：http://vn.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qw.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lb.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cv.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zc.9csxet.cn

Ruby: arr.sort
来源：http://lu.colortex.cn

C#:   list.Sort();
来源：http://ty.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zl.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fv.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ry.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://az.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://al.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kq.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zu.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xc.bookmarksfly.cn

[D11] 反转数组
来源：http://fe.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ud.colortex.cn

PHP:  array_reverse($arr);
来源：http://iy.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cd.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ia.hnjuh.cn

Java: Collections.reverse(list);
来源：http://ks.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://pk.huanxung.cn

Ruby: arr.reverse
来源：http://zy.nicolike.cn

C#:   list.Reverse();
来源：http://wm.jctech888.com.cn

[D12] 查找元素下标
来源：http://xh.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ot.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://na.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mb.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cx.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aq.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://de.hnjuh.cn

Ruby: arr.index(x)
来源：http://xv.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://nt.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ap.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yv.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://my.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://sz.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://zq.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tm.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bw.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wc.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ry.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://vu.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ab.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xm.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://am.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://mi.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jl.bookmarksfly.cn

Go:   // 手写循环
来源：http://hd.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zi.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ju.bookmarksfly.cn

[D15] 去重
来源：http://mv.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://we.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://yy.nicolike.cn

JS:   [...new Set(arr)]
来源：http://tw.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://hl.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uv.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ki.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://oj.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://qh.chemitech.net.cn

[D16] 求和与平均值
来源：http://mw.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mh.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oo.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uk.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://da.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://di.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://xv.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ga.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://zw.lnxyls.cn

[D17] 最大值与最小值
来源：http://xt.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://xc.521024.cn

PHP:  max($arr);  min($arr);
来源：http://sp.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zr.panjiajie.cn

TS:   Math.max(...arr);
来源：http://hm.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ux.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ab.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://qt.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ir.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://cs.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://je.asd995.cn

PHP:  array_merge(...$nested);
来源：http://zz.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sd.shtwfgs.cn

TS:   nested.flat();
来源：http://zz.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jm.shxzskj.cn

Go:   // 手写双层循环
来源：http://ft.bjjhwx.cn

Ruby: nested.flatten
来源：http://uz.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://le.colortex.cn

[D19] 按字段分组
来源：http://ld.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qm.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kq.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mr.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://am.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kk.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://yd.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hg.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ko.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://hq.haigaiapp.cn

Py:   Counter(arr)
来源：http://hf.newstarts.cn

PHP:  array_count_values($arr);
来源：http://uu.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wd.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vb.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jn.521024.cn

Go:   // 手写 map[T]int
来源：http://ku.hahajie.cn

Ruby: arr.tally
来源：http://pa.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xi.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ld.muxihuayi.cn

Py:   x in arr
来源：http://nv.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://wn.shxzukj.cn

JS:   arr.includes(x)
来源：http://ug.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ra.shxzskj.cn

Java: list.contains(x)
来源：http://jr.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://uj.colortex.cn

Ruby: arr.include?(x)
来源：http://lv.muxihuayi.cn

C#:   list.Contains(x)
来源：http://vz.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://we.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xz.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://og.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lp.bookmarksfly.cn

TS:   [...arr];
来源：http://zp.9csxet.cn

Java: new ArrayList<>(list);
来源：http://fq.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ir.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://cg.panjiajie.cn

C#:   new List<int>(list);
来源：http://vk.chemitech.net.cn

[D23] reduce 累积计算
来源：http://zn.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yh.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ak.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fv.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gh.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jx.szsharing.cn

Go:   // 手写循环
来源：http://jz.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rd.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xm.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://qi.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ea.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://so.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vd.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hb.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tr.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cv.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xs.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ty.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://cp.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iw.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vr.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tg.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yb.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jt.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://da.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ka.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ns.bookmarksfly.cn

[D26] 数组转字符串
来源：http://vb.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://ei.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://ow.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://gu.huixiangedu.cn

TS:   arr.join(", ")
来源：http://nb.shxzskj.cn

Java: String.join(", ", list)
来源：http://mv.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://uh.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://aq.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://hk.hahajie.cn

================================================================================
来源：http://pa.shxzskj.cn

E. 字符串处理
来源：http://if.colortex.cn

================================================================================
来源：http://hs.hahajie.cn

[E01] 拼接字符串
来源：http://rw.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qj.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oy.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gw.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bm.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cz.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ef.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yi.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qb.9csxet.cn

[E02] 重复字符串
来源：http://ku.huanxung.cn

Py:   "ab" * 3
来源：http://zk.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://fr.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://vz.huanxung.cn

TS:   "ab".repeat(3)
来源：http://ro.huanxung.cn

Java: "ab".repeat(3)
来源：http://oi.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://cm.shxzskj.cn

Ruby: "ab" * 3
来源：http://zh.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qs.newstarts.cn

[E03] 截取子串
来源：http://va.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yl.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://go.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uv.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://ys.9csxet.cn

Java: s.substring(1, 4)
来源：http://sw.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xd.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://op.521024.cn

C#:   s.Substring(1, 3)
来源：http://kt.jctech888.com.cn

[E04] 查找子串位置
来源：http://vf.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://mh.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://oo.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bn.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://zr.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://bm.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://it.bjjhwx.cn

Ruby: s.index("x")
来源：http://zm.9csxet.cn

C#:   s.IndexOf("x")
来源：http://dx.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://si.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wk.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rz.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lt.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xh.huanxung.cn


<!-- 参考信息 -->