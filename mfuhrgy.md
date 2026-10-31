代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yv.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://be.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ft.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://nu.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gg.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.muxihuayi.cn

Java: // 无解构
来源：http://zm.huixiangedu.cn

Go:   // 无解构
来源：http://ny.521024.cn

Ruby: a, b = pair
来源：http://nu.colortex.cn

C#:   var (a, b) = pair;
来源：http://zf.nicolike.cn

[C16] 函数 / 方法重载
来源：http://xj.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oe.lnxyls.cn

PHP:  // 无重载
来源：http://un.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lv.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://xm.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gg.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ty.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://mc.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rn.nicolike.cn

================================================================================
来源：http://az.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://lb.szsharing.cn

================================================================================
来源：http://sm.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://sk.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cc.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yr.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aj.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gq.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rp.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://qs.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://dg.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vo.colortex.cn

[D02] 追加元素到末尾
来源：http://od.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hn.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qf.panjiajie.cn

JS:   arr.push(4);
来源：http://tp.huixiangedu.cn

TS:   arr.push(4);
来源：http://hb.lnxyls.cn

Java: list.add(4);
来源：http://cv.asd995.cn

Go:   arr = append(arr, 4)
来源：http://pr.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://sh.521024.cn

C#:   list.Add(4);
来源：http://qz.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://nv.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://yh.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lj.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nz.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://tk.gzmigu.cn

Java: list.add(0, 0);
来源：http://gg.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xx.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://co.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://kh.bookmarksfly.cn

[D04] 删除元素
来源：http://rc.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lb.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cp.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://om.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://an.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xr.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rp.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qb.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qk.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://vn.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lw.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mk.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zy.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://bm.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://jz.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ln.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yx.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ph.colortex.cn

[D06] 数组长度
来源：http://sk.asd995.cn

Py:   len(arr)
来源：http://gz.shxzukj.cn

PHP:  count($arr);
来源：http://lv.hnjuh.cn

JS:   arr.length
来源：http://ni.yuexingan06.cn

TS:   arr.length
来源：http://ug.nicolike.cn

Java: list.size();
来源：http://td.jctech888.com.cn

Go:   len(arr)
来源：http://tc.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://sg.haigaiapp.cn

C#:   list.Count;
来源：http://sy.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://os.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ao.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qx.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://fs.521024.cn

TS:   arr.slice(1, 4);
来源：http://jx.gzmigu.cn

Java: list.subList(1, 4);
来源：http://kq.colortex.cn

Go:   arr[1:4]
来源：http://qq.panjiajie.cn

Ruby: arr[1, 3]
来源：http://yl.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://dy.haigaiapp.cn

[D08] 合并两个数组
来源：http://rz.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://ft.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://zv.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bh.521024.cn

TS:   [...a, ...b];
来源：http://lj.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ia.chemitech.net.cn

Go:   append(a, b...)
来源：http://tp.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://gw.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://ql.szsharing.cn

[D09] 排序（升序）
来源：http://uu.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://os.huanxung.cn

PHP:  sort($arr);
来源：http://ap.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uy.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xi.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tp.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://up.panjiajie.cn

Ruby: arr.sort
来源：http://fc.panjiajie.cn

C#:   list.Sort();
来源：http://go.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fx.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qt.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lu.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fe.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hy.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xt.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xg.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hh.shxzukj.cn

[D11] 反转数组
来源：http://vw.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lh.colortex.cn

PHP:  array_reverse($arr);
来源：http://xv.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hm.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ju.521024.cn

Java: Collections.reverse(list);
来源：http://ss.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://cy.shxzukj.cn

Ruby: arr.reverse
来源：http://gu.shtwfgs.cn

C#:   list.Reverse();
来源：http://nv.asd995.cn

[D12] 查找元素下标
来源：http://st.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://px.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cl.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gc.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jm.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://fn.muxihuayi.cn

Ruby: arr.index(x)
来源：http://oy.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://rk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://qy.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yn.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sv.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://vm.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://si.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sp.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://em.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tx.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qx.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://zd.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wm.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://li.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://lv.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ni.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wj.lnxyls.cn

Go:   // 手写循环
来源：http://ph.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jd.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lh.nicolike.cn

[D15] 去重
来源：http://tz.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jj.newstarts.cn

PHP:  array_unique($arr);
来源：http://wt.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://yn.nicolike.cn

TS:   [...new Set(arr)]
来源：http://ww.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fq.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yd.asd995.cn

Ruby: arr.uniq
来源：http://sy.colortex.cn

C#:   list.Distinct().ToList()
来源：http://yf.colortex.cn

[D16] 求和与平均值
来源：http://uw.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ap.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eq.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ou.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://km.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ad.szxytkj.cn

Go:   // 手写循环累加
来源：http://ks.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nm.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://gz.shxzukj.cn

[D17] 最大值与最小值
来源：http://cy.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://if.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://vn.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://le.521024.cn

TS:   Math.max(...arr);
来源：http://tb.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uo.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sc.colortex.cn

Ruby: arr.max;  arr.min
来源：http://ez.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://zm.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://hx.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ll.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ks.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fc.hahajie.cn

TS:   nested.flat();
来源：http://cm.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iq.nszjky.cn

Go:   // 手写双层循环
来源：http://tm.nicolike.cn

Ruby: nested.flatten
来源：http://lc.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://by.huixinmuqiang.cn

[D19] 按字段分组
来源：http://mh.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pi.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://is.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ug.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ho.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kf.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://gu.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yo.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ob.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://vz.9csxet.cn

Py:   Counter(arr)
来源：http://fg.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://pm.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wd.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vk.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://ak.bookmarksfly.cn

Ruby: arr.tally
来源：http://gt.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sy.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://sj.shxzskj.cn

Py:   x in arr
来源：http://on.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://zy.huixiangedu.cn

JS:   arr.includes(x)
来源：http://hk.lnxyls.cn

TS:   arr.includes(x)
来源：http://hw.hahajie.cn

Java: list.contains(x)
来源：http://yg.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://vq.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://zm.nicolike.cn

C#:   list.Contains(x)
来源：http://id.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ho.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nj.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sp.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oa.asd995.cn

TS:   [...arr];
来源：http://yf.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://ac.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rw.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://un.panjiajie.cn

C#:   new List<int>(list);
来源：http://uf.huanxung.cn

[D23] reduce 累积计算
来源：http://ro.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cp.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yw.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cy.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://id.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xh.yuexingan06.cn

Go:   // 手写循环
来源：http://am.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jc.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gw.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ki.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qw.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lt.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lm.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zn.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bf.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gn.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mz.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wc.521024.cn

[D25] Set 集合去重与交并差
来源：http://th.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dk.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ut.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jl.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ug.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ea.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fw.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ty.huanxung.cn

[D26] 数组转字符串
来源：http://cy.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://cr.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://fi.nicolike.cn

JS:   arr.join(", ")
来源：http://yw.hahajie.cn

TS:   arr.join(", ")
来源：http://ti.nicolike.cn

Java: String.join(", ", list)
来源：http://wn.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://kk.newstarts.cn

Ruby: arr.join(", ")
来源：http://eq.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://ge.huanxung.cn

================================================================================
来源：http://td.huanxung.cn

E. 字符串处理
来源：http://jy.huixiangedu.cn

================================================================================
来源：http://be.huixiangedu.cn

[E01] 拼接字符串
来源：http://xd.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nu.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cl.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bg.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kv.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://md.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ge.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hy.huixinmuqiang.cn

[E02] 重复字符串
来源：http://hi.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://lu.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://zy.colortex.cn

JS:   "ab".repeat(3)
来源：http://bl.hahajie.cn

TS:   "ab".repeat(3)
来源：http://eq.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ul.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://wt.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://up.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wz.9csxet.cn

[E03] 截取子串
来源：http://yy.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xh.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gb.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hq.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://pu.gzmigu.cn

Java: s.substring(1, 4)
来源：http://nw.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hj.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xf.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://sp.521024.cn

[E04] 查找子串位置
来源：http://gz.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://zg.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://bl.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jg.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ja.muxihuayi.cn

Java: s.indexOf("x")
来源：http://je.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://gk.szxytkj.cn

Ruby: s.index("x")
来源：http://fk.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://yc.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gg.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tj.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bu.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aq.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pf.yuntaijiaju.cn


<!-- 参考信息 -->