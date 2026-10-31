代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dp.asd995.cn

[C15] 解构 / 展开参数
来源：http://dk.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yg.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://vy.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sy.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yd.szxytkj.cn

Java: // 无解构
来源：http://ln.lnxyls.cn

Go:   // 无解构
来源：http://qy.chemitech.net.cn

Ruby: a, b = pair
来源：http://hr.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://ox.huanxung.cn

[C16] 函数 / 方法重载
来源：http://xp.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yn.gzmigu.cn

PHP:  // 无重载
来源：http://bc.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wb.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://du.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mq.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://gn.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://wc.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://en.jianghongdianzi.cn

================================================================================
来源：http://zg.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://jl.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://df.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vt.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jf.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ro.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nl.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://in.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://hq.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://fs.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nq.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://ze.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dv.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hw.hahajie.cn

JS:   arr.push(4);
来源：http://cz.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://lu.bookmarksfly.cn

Java: list.add(4);
来源：http://gd.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://fg.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://np.szsharing.cn

C#:   list.Add(4);
来源：http://ki.colortex.cn

[D03] 在指定位置插入元素
来源：http://zf.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://xg.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qs.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fb.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://fr.9csxet.cn

Java: list.add(0, 0);
来源：http://ra.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mt.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bj.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://ae.hahajie.cn

[D04] 删除元素
来源：http://gy.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ra.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hw.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vl.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://tt.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ua.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rm.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rb.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://up.newstarts.cn

[D05] 访问与修改元素
来源：http://zi.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dx.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sa.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wx.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://wm.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://ee.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://gg.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qc.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sj.gzmigu.cn

[D06] 数组长度
来源：http://jx.shxzskj.cn

Py:   len(arr)
来源：http://lw.521024.cn

PHP:  count($arr);
来源：http://yv.jctech888.com.cn

JS:   arr.length
来源：http://xs.hnjuh.cn

TS:   arr.length
来源：http://dq.lnxyls.cn

Java: list.size();
来源：http://hm.nicolike.cn

Go:   len(arr)
来源：http://qq.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://nq.shxzukj.cn

C#:   list.Count;
来源：http://bf.szsharing.cn

[D07] 切片 / 取子数组
来源：http://tx.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ae.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yc.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://zr.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://mo.shxzskj.cn

Java: list.subList(1, 4);
来源：http://wt.hnjuh.cn

Go:   arr[1:4]
来源：http://ng.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://ep.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://rg.shtwfgs.cn

[D08] 合并两个数组
来源：http://bw.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://fx.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://qd.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pw.jctech888.com.cn

TS:   [...a, ...b];
来源：http://tj.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rk.asd995.cn

Go:   append(a, b...)
来源：http://gz.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://fw.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://yt.szxytkj.cn

[D09] 排序（升序）
来源：http://to.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jn.nicolike.cn

PHP:  sort($arr);
来源：http://js.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vu.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yr.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dy.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.shtwfgs.cn

Ruby: arr.sort
来源：http://cb.chemitech.net.cn

C#:   list.Sort();
来源：http://ox.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://og.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bi.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rw.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fl.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ey.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cn.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aq.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yb.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://en.jianghongdianzi.cn

[D11] 反转数组
来源：http://iq.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://je.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://pi.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kr.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://vh.asd995.cn

Java: Collections.reverse(list);
来源：http://sz.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://ik.haigaiapp.cn

Ruby: arr.reverse
来源：http://hc.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://wk.hahajie.cn

[D12] 查找元素下标
来源：http://lx.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://jc.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://je.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xh.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zg.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://hj.shxzukj.cn

Ruby: arr.index(x)
来源：http://rq.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://nu.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ku.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wv.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mp.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://mo.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://cx.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ts.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ka.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cc.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yk.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://lg.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tv.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eg.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://zh.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://ey.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dv.hahajie.cn

Go:   // 手写循环
来源：http://ix.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fo.lnxyls.cn

[D15] 去重
来源：http://ji.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rz.newstarts.cn

PHP:  array_unique($arr);
来源：http://xa.nicolike.cn

JS:   [...new Set(arr)]
来源：http://zq.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://dk.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rf.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mu.shtwfgs.cn

Ruby: arr.uniq
来源：http://am.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://bp.lnxyls.cn

[D16] 求和与平均值
来源：http://bv.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vs.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fn.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hy.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://de.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sa.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://zj.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zc.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://vk.jctech888.com.cn

[D17] 最大值与最小值
来源：http://cd.colortex.cn

Py:   max(arr);  min(arr)
来源：http://kn.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://vf.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nd.huanxung.cn

TS:   Math.max(...arr);
来源：http://gh.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gt.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mr.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://wc.asd995.cn

C#:   list.Max();  list.Min()
来源：http://pw.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://kc.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ru.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://fb.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pc.hnjuh.cn

TS:   nested.flat();
来源：http://tz.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yz.colortex.cn

Go:   // 手写双层循环
来源：http://fz.haigaiapp.cn

Ruby: nested.flatten
来源：http://pi.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qb.bookmarksfly.cn

[D19] 按字段分组
来源：http://hq.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bl.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tv.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ad.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nj.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://me.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://xu.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tn.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ou.521024.cn

[D20] 统计每个元素出现次数
来源：http://ak.newstarts.cn

Py:   Counter(arr)
来源：http://dg.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://lm.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tv.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nc.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kz.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://od.lnxyls.cn

Ruby: arr.tally
来源：http://cu.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jq.hahajie.cn

[D21] 判断是否包含某元素
来源：http://sd.asd995.cn

Py:   x in arr
来源：http://iz.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://pn.colortex.cn

JS:   arr.includes(x)
来源：http://ud.haigaiapp.cn

TS:   arr.includes(x)
来源：http://pt.colortex.cn

Java: list.contains(x)
来源：http://vk.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://bx.asd995.cn

Ruby: arr.include?(x)
来源：http://mz.hahajie.cn

C#:   list.Contains(x)
来源：http://cf.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://yg.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://df.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qv.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ui.huanxung.cn

TS:   [...arr];
来源：http://si.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://ej.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xv.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://ub.lnxyls.cn

C#:   new List<int>(list);
来源：http://uu.haigaiapp.cn

[D23] reduce 累积计算
来源：http://nw.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yj.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iv.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tq.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://we.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pa.muxihuayi.cn

Go:   // 手写循环
来源：http://dn.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lr.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cc.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://tp.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ed.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://af.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ay.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://se.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lx.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ax.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jv.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yw.asd995.cn

[D25] Set 集合去重与交并差
来源：http://bu.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ez.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dm.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qm.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oe.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://il.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vp.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ae.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ap.asd995.cn

[D26] 数组转字符串
来源：http://zl.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://sa.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://yk.9csxet.cn

JS:   arr.join(", ")
来源：http://pf.jctech888.com.cn

TS:   arr.join(", ")
来源：http://fb.yuexingan06.cn

Java: String.join(", ", list)
来源：http://iv.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://pm.nicolike.cn

Ruby: arr.join(", ")
来源：http://om.szsharing.cn

C#:   string.Join(", ", list)
来源：http://vx.bookmarksfly.cn

================================================================================
来源：http://lq.jctech888.com.cn

E. 字符串处理
来源：http://qo.asd995.cn

================================================================================
来源：http://ie.haigaiapp.cn

[E01] 拼接字符串
来源：http://qh.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://id.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pk.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ld.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sg.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rs.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uo.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zq.521024.cn

[E02] 重复字符串
来源：http://jp.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://hz.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://dj.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://to.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://ay.asd995.cn

Java: "ab".repeat(3)
来源：http://lb.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://mc.9csxet.cn

Ruby: "ab" * 3
来源：http://pm.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kp.colortex.cn

[E03] 截取子串
来源：http://ly.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lw.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qy.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sw.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://xb.szsharing.cn

Java: s.substring(1, 4)
来源：http://va.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eb.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://sy.nicolike.cn

[E04] 查找子串位置
来源：http://kr.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://me.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://qj.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vm.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://po.lnxyls.cn

Java: s.indexOf("x")
来源：http://my.colortex.cn

Go:   strings.Index(s, "x")
来源：http://wb.asd995.cn

Ruby: s.index("x")
来源：http://qr.hahajie.cn

C#:   s.IndexOf("x")
来源：http://jf.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uu.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tz.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xa.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ro.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pg.nicolike.cn


<!-- 参考信息 -->