代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vk.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iz.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ik.hahajie.cn

Ruby: # 无泛型
来源：http://vb.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dl.nszjky.cn

[C15] 解构 / 展开参数
来源：http://if.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kd.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://ib.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ab.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aj.chemitech.net.cn

Java: // 无解构
来源：http://cg.nicolike.cn

Go:   // 无解构
来源：http://qp.bjjhwx.cn

Ruby: a, b = pair
来源：http://dc.huanxung.cn

C#:   var (a, b) = pair;
来源：http://yh.asd995.cn

[C16] 函数 / 方法重载
来源：http://yl.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zd.huixinmuqiang.cn

PHP:  // 无重载
来源：http://se.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://or.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://oz.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ju.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://wd.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://yq.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aa.asd995.cn

================================================================================
来源：http://qs.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://dw.521024.cn

================================================================================
来源：http://rp.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://lz.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yi.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jl.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jf.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rc.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tn.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://ed.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://uz.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kx.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://gc.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bb.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jp.shxzukj.cn

JS:   arr.push(4);
来源：http://wu.shxzukj.cn

TS:   arr.push(4);
来源：http://ux.hahajie.cn

Java: list.add(4);
来源：http://rg.colortex.cn

Go:   arr = append(arr, 4)
来源：http://kv.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://vj.hnjuh.cn

C#:   list.Add(4);
来源：http://fe.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://nl.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://nr.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vf.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bp.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://lo.huixiangedu.cn

Java: list.add(0, 0);
来源：http://qs.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ox.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ab.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://am.asd995.cn

[D04] 删除元素
来源：http://xr.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mr.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ml.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yr.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://xq.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wb.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nz.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ip.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fk.newstarts.cn

[D05] 访问与修改元素
来源：http://ng.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qb.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ph.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wh.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://uu.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://if.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://cb.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://is.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qi.bjjhwx.cn

[D06] 数组长度
来源：http://fc.huixinmuqiang.cn

Py:   len(arr)
来源：http://kd.szxytkj.cn

PHP:  count($arr);
来源：http://ue.huixiangedu.cn

JS:   arr.length
来源：http://vk.newstarts.cn

TS:   arr.length
来源：http://qp.newstarts.cn

Java: list.size();
来源：http://kk.wgjwhj.cn

Go:   len(arr)
来源：http://de.nszjky.cn

Ruby: arr.length; arr.size
来源：http://mi.hahajie.cn

C#:   list.Count;
来源：http://zx.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://td.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sg.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kp.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://uo.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://nz.panjiajie.cn

Java: list.subList(1, 4);
来源：http://fe.chemitech.net.cn

Go:   arr[1:4]
来源：http://az.szsharing.cn

Ruby: arr[1, 3]
来源：http://bf.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ct.szsharing.cn

[D08] 合并两个数组
来源：http://df.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://td.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://fe.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qv.panjiajie.cn

TS:   [...a, ...b];
来源：http://ku.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://av.muxihuayi.cn

Go:   append(a, b...)
来源：http://yx.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://nq.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://zn.lnxyls.cn

[D09] 排序（升序）
来源：http://bf.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kv.asd995.cn

PHP:  sort($arr);
来源：http://nd.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hu.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ih.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xh.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cg.nszjky.cn

Ruby: arr.sort
来源：http://pm.huanxung.cn

C#:   list.Sort();
来源：http://ov.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ca.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lx.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ef.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://da.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oa.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ih.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gl.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zz.521024.cn

[D11] 反转数组
来源：http://vo.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://ft.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lf.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://lz.colortex.cn

Java: Collections.reverse(list);
来源：http://ci.asd995.cn

Go:   slices.Reverse(arr)
来源：http://km.szxytkj.cn

Ruby: arr.reverse
来源：http://br.9csxet.cn

C#:   list.Reverse();
来源：http://ap.colortex.cn

[D12] 查找元素下标
来源：http://fm.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://eo.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uo.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gb.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rd.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ux.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://ou.shxzskj.cn

Ruby: arr.index(x)
来源：http://wf.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://rp.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://wj.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ow.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://be.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://zr.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://aa.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ie.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lh.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://se.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dy.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://sw.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hj.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cq.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://fd.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://jr.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pa.panjiajie.cn

Go:   // 手写循环
来源：http://hd.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kb.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sg.nszjky.cn

[D15] 去重
来源：http://jx.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bk.colortex.cn

PHP:  array_unique($arr);
来源：http://vz.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://tv.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://pa.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://it.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://it.gzmigu.cn

Ruby: arr.uniq
来源：http://hi.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ph.panjiajie.cn

[D16] 求和与平均值
来源：http://xr.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xe.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xw.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://it.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://br.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://at.shxzukj.cn

Go:   // 手写循环累加
来源：http://gp.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ip.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://as.newstarts.cn

[D17] 最大值与最小值
来源：http://ss.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://uv.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://gt.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gg.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://lq.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pj.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zr.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://jw.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ku.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://lb.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lg.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://me.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bb.bjjhwx.cn

TS:   nested.flat();
来源：http://mu.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hx.9csxet.cn

Go:   // 手写双层循环
来源：http://lm.colortex.cn

Ruby: nested.flatten
来源：http://ml.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eq.nicolike.cn

[D19] 按字段分组
来源：http://ci.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tg.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vr.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ul.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ix.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://op.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ia.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cj.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jb.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://ny.panjiajie.cn

Py:   Counter(arr)
来源：http://ic.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://au.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mg.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ns.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sd.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://el.huixinmuqiang.cn

Ruby: arr.tally
来源：http://lq.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eo.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://ea.gzmigu.cn

Py:   x in arr
来源：http://pa.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://mf.szsharing.cn

JS:   arr.includes(x)
来源：http://jy.hnjuh.cn

TS:   arr.includes(x)
来源：http://ug.bjjhwx.cn

Java: list.contains(x)
来源：http://gx.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://se.9csxet.cn

Ruby: arr.include?(x)
来源：http://id.newstarts.cn

C#:   list.Contains(x)
来源：http://hb.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://zl.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pk.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ku.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uq.yuntaijiaju.cn

TS:   [...arr];
来源：http://ou.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ki.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://og.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://um.huanxung.cn

C#:   new List<int>(list);
来源：http://gl.9csxet.cn

[D23] reduce 累积计算
来源：http://zn.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mr.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uz.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fu.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jo.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ko.nszjky.cn

Go:   // 手写循环
来源：http://ve.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xo.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lq.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://pm.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rg.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xc.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gc.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://go.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://it.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zu.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wg.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ui.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://ub.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uy.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tw.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sr.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vq.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nn.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gv.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cz.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nc.yuexingan06.cn

[D26] 数组转字符串
来源：http://mo.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://lu.asd995.cn

PHP:  implode(", ", $arr);
来源：http://sx.wgjwhj.cn

JS:   arr.join(", ")
来源：http://gl.nszjky.cn

TS:   arr.join(", ")
来源：http://ro.shxzukj.cn

Java: String.join(", ", list)
来源：http://vc.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://gx.newstarts.cn

Ruby: arr.join(", ")
来源：http://ze.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://jo.shxzskj.cn

================================================================================
来源：http://pw.newstarts.cn

E. 字符串处理
来源：http://zs.muxihuayi.cn

================================================================================
来源：http://oe.haigaiapp.cn

[E01] 拼接字符串
来源：http://rp.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bx.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tg.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fz.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nm.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hm.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ei.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cm.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vg.colortex.cn

[E02] 重复字符串
来源：http://oq.chemitech.net.cn

Py:   "ab" * 3
来源：http://nx.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://af.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://dc.colortex.cn

TS:   "ab".repeat(3)
来源：http://hn.521024.cn

Java: "ab".repeat(3)
来源：http://zc.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ge.colortex.cn

Ruby: "ab" * 3
来源：http://ir.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ij.yuntaijiaju.cn

[E03] 截取子串
来源：http://sc.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hw.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ld.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jv.nszjky.cn

TS:   s.slice(1, 4)
来源：http://qb.nicolike.cn

Java: s.substring(1, 4)
来源：http://tj.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xz.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oj.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ku.jctech888.com.cn

[E04] 查找子串位置
来源：http://lj.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://sv.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://hl.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kn.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://oa.huanxung.cn

Java: s.indexOf("x")
来源：http://eg.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://om.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://rq.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://py.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rc.nszjky.cn


<!-- 参考信息 -->