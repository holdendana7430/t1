代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xb.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://dd.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vf.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://dt.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hw.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zq.jianghongdianzi.cn

Java: // 无解构
来源：http://im.colortex.cn

Go:   // 无解构
来源：http://lo.newstarts.cn

Ruby: a, b = pair
来源：http://ri.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://wt.nicolike.cn

[C16] 函数 / 方法重载
来源：http://kj.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bd.huixiangedu.cn

PHP:  // 无重载
来源：http://zt.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cr.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://gv.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fs.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://jt.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://fi.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://js.szsharing.cn

================================================================================
来源：http://pj.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://la.521024.cn

================================================================================
来源：http://iu.nszjky.cn

[D01] 创建数组 / 列表
来源：http://nc.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pe.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bp.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://la.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mh.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tq.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ig.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://lm.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xp.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://sl.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dp.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ny.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ul.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://jr.521024.cn

Java: list.add(4);
来源：http://gd.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://ih.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://fa.bjjhwx.cn

C#:   list.Add(4);
来源：http://pk.colortex.cn

[D03] 在指定位置插入元素
来源：http://tt.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://ju.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pt.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wk.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://sr.szsharing.cn

Java: list.add(0, 0);
来源：http://nw.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vv.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ob.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://jy.jctech888.com.cn

[D04] 删除元素
来源：http://jb.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rn.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ay.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vx.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://bp.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wf.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cw.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tc.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ah.newstarts.cn

[D05] 访问与修改元素
来源：http://ua.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kx.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fu.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zk.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://qv.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://je.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://xw.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ng.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://az.wgjwhj.cn

[D06] 数组长度
来源：http://aw.yuntaijiaju.cn

Py:   len(arr)
来源：http://gs.bjjhwx.cn

PHP:  count($arr);
来源：http://wa.shxzukj.cn

JS:   arr.length
来源：http://ap.jianghongdianzi.cn

TS:   arr.length
来源：http://tk.huanxung.cn

Java: list.size();
来源：http://ha.bjjhwx.cn

Go:   len(arr)
来源：http://pd.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://td.yuntaijiaju.cn

C#:   list.Count;
来源：http://as.colortex.cn

[D07] 切片 / 取子数组
来源：http://or.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oh.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://az.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://cc.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://nj.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://gz.yuexingan06.cn

Go:   arr[1:4]
来源：http://wp.panjiajie.cn

Ruby: arr[1, 3]
来源：http://sj.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://oj.shxzukj.cn

[D08] 合并两个数组
来源：http://zn.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://yo.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://fq.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wl.newstarts.cn

TS:   [...a, ...b];
来源：http://kg.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bl.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://bo.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://tr.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://ah.huanxung.cn

[D09] 排序（升序）
来源：http://si.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ej.shxzskj.cn

PHP:  sort($arr);
来源：http://eo.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zz.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pi.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rl.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nd.bjjhwx.cn

Ruby: arr.sort
来源：http://qq.shxzukj.cn

C#:   list.Sort();
来源：http://xu.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nk.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xl.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xy.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zb.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hq.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eb.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bt.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hm.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oz.jctech888.com.cn

[D11] 反转数组
来源：http://ay.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://at.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://xs.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pz.lnxyls.cn

TS:   [...arr].reverse();
来源：http://wv.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://vw.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://hu.lnxyls.cn

Ruby: arr.reverse
来源：http://cs.huanxung.cn

C#:   list.Reverse();
来源：http://ed.muxihuayi.cn

[D12] 查找元素下标
来源：http://qh.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://yu.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://js.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bd.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hc.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://le.asd995.cn

Go:   slices.Index(arr, x)
来源：http://gw.huixiangedu.cn

Ruby: arr.index(x)
来源：http://re.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://nx.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://lf.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fw.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bu.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://kz.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ji.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lq.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hq.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qw.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ea.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://hz.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cj.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sl.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://zz.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://yf.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rx.nicolike.cn

Go:   // 手写循环
来源：http://ys.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lk.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xo.szsharing.cn

[D15] 去重
来源：http://jo.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rf.szsharing.cn

PHP:  array_unique($arr);
来源：http://sw.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://ha.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://uf.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://av.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vs.wgjwhj.cn

Ruby: arr.uniq
来源：http://zw.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://ni.szsharing.cn

[D16] 求和与平均值
来源：http://vv.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qg.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rn.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rx.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iy.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oc.jctech888.com.cn

Go:   // 手写循环累加
来源：http://cp.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://co.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://po.gzmigu.cn

[D17] 最大值与最小值
来源：http://gt.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://pj.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://bh.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ln.hahajie.cn

TS:   Math.max(...arr);
来源：http://rs.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://td.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pd.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://kg.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://yg.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://zj.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ue.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://sy.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cr.nszjky.cn

TS:   nested.flat();
来源：http://cb.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rs.521024.cn

Go:   // 手写双层循环
来源：http://li.lnxyls.cn

Ruby: nested.flatten
来源：http://wv.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://no.huixiangedu.cn

[D19] 按字段分组
来源：http://dj.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://we.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mw.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ym.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://um.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qs.521024.cn

Go:   // 手写 map[string][]T
来源：http://tz.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ig.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gx.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://kk.bjjhwx.cn

Py:   Counter(arr)
来源：http://qj.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://jf.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wi.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zi.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ju.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ok.bjjhwx.cn

Ruby: arr.tally
来源：http://ps.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://it.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://qc.huixiangedu.cn

Py:   x in arr
来源：http://de.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://lr.jctech888.com.cn

JS:   arr.includes(x)
来源：http://bs.shtwfgs.cn

TS:   arr.includes(x)
来源：http://gu.wgjwhj.cn

Java: list.contains(x)
来源：http://ur.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://xn.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://sl.521024.cn

C#:   list.Contains(x)
来源：http://mg.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://bh.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ly.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kw.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dt.szxytkj.cn

TS:   [...arr];
来源：http://au.colortex.cn

Java: new ArrayList<>(list);
来源：http://oc.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iu.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://yf.yuexingan06.cn

C#:   new List<int>(list);
来源：http://wx.colortex.cn

[D23] reduce 累积计算
来源：http://xj.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lr.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rj.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ta.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gl.szxytkj.cn

Go:   // 手写循环
来源：http://yy.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://de.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://li.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://xe.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wz.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wn.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ya.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zr.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://co.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://na.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bz.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dl.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://qt.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mh.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fx.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wm.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hs.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wh.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ib.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://du.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://td.521024.cn

[D26] 数组转字符串
来源：http://my.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://jp.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://os.colortex.cn

JS:   arr.join(", ")
来源：http://oq.colortex.cn

TS:   arr.join(", ")
来源：http://zm.huixiangedu.cn

Java: String.join(", ", list)
来源：http://lk.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://xs.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://es.newstarts.cn

C#:   string.Join(", ", list)
来源：http://zo.jianghongdianzi.cn

================================================================================
来源：http://su.huixiangedu.cn

E. 字符串处理
来源：http://mo.shtwfgs.cn

================================================================================
来源：http://so.nszjky.cn

[E01] 拼接字符串
来源：http://nr.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nv.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vm.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ji.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pj.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sn.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jo.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rl.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yo.newstarts.cn

[E02] 重复字符串
来源：http://la.colortex.cn

Py:   "ab" * 3
来源：http://dh.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://xu.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://mf.hahajie.cn

TS:   "ab".repeat(3)
来源：http://we.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://sv.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://pa.lnxyls.cn

Ruby: "ab" * 3
来源：http://je.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nb.yuexingan06.cn

[E03] 截取子串
来源：http://ts.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fp.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xd.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ds.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://pt.shxzukj.cn

Java: s.substring(1, 4)
来源：http://wq.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bu.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qx.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://wc.shxzskj.cn

[E04] 查找子串位置
来源：http://zy.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ea.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://cm.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vp.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://xx.nszjky.cn

Java: s.indexOf("x")
来源：http://ku.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://kt.szsharing.cn

Ruby: s.index("x")
来源：http://zp.nszjky.cn

C#:   s.IndexOf("x")
来源：http://rb.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oz.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mp.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eb.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.szsharing.cn


<!-- 参考信息 -->