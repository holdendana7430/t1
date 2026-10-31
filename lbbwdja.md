代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wh.asd995.cn

[C15] 解构 / 展开参数
来源：http://fn.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mb.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://vy.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bb.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fd.jianghongdianzi.cn

Java: // 无解构
来源：http://bs.9csxet.cn

Go:   // 无解构
来源：http://pr.wgjwhj.cn

Ruby: a, b = pair
来源：http://tr.szsharing.cn

C#:   var (a, b) = pair;
来源：http://gi.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://wn.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://td.shtwfgs.cn

PHP:  // 无重载
来源：http://xs.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://it.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://xw.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tm.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://dl.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://vw.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ti.lnxyls.cn

================================================================================
来源：http://qt.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ou.huanxung.cn

================================================================================
来源：http://jt.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://ju.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ic.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gi.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bf.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vm.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hs.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://oa.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://al.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vx.panjiajie.cn

[D02] 追加元素到末尾
来源：http://zq.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zn.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vv.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://tf.panjiajie.cn

TS:   arr.push(4);
来源：http://uq.521024.cn

Java: list.add(4);
来源：http://fo.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ju.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://yd.huanxung.cn

C#:   list.Add(4);
来源：http://pz.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://qd.asd995.cn

Py:   arr.insert(0, 0)
来源：http://zj.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zl.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ac.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://sa.wgjwhj.cn

Java: list.add(0, 0);
来源：http://gr.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fu.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fa.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://is.hahajie.cn

[D04] 删除元素
来源：http://wt.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ne.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iz.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fk.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ep.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bt.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://po.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://br.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fv.panjiajie.cn

[D05] 访问与修改元素
来源：http://ei.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hi.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nq.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zj.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://rt.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://an.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://jn.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bu.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ya.muxihuayi.cn

[D06] 数组长度
来源：http://et.521024.cn

Py:   len(arr)
来源：http://si.yuntaijiaju.cn

PHP:  count($arr);
来源：http://bj.huanxung.cn

JS:   arr.length
来源：http://tm.wgjwhj.cn

TS:   arr.length
来源：http://lt.szxytkj.cn

Java: list.size();
来源：http://kz.newstarts.cn

Go:   len(arr)
来源：http://ex.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ei.gzmigu.cn

C#:   list.Count;
来源：http://fk.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://tj.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ik.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tb.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ns.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://it.asd995.cn

Java: list.subList(1, 4);
来源：http://cd.hahajie.cn

Go:   arr[1:4]
来源：http://sa.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://xe.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://sz.huixiangedu.cn

[D08] 合并两个数组
来源：http://wd.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://jw.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://fw.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ce.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://kh.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oc.huanxung.cn

Go:   append(a, b...)
来源：http://fx.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://lw.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://on.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://ag.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ov.szsharing.cn

PHP:  sort($arr);
来源：http://uj.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cq.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zs.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jy.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ky.panjiajie.cn

Ruby: arr.sort
来源：http://sn.muxihuayi.cn

C#:   list.Sort();
来源：http://wv.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xs.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tf.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vu.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qb.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dg.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lq.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sm.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ir.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qn.hnjuh.cn

[D11] 反转数组
来源：http://sj.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ev.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://cy.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ep.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://gk.shxzskj.cn

Java: Collections.reverse(list);
来源：http://sr.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://nb.colortex.cn

Ruby: arr.reverse
来源：http://ya.bjjhwx.cn

C#:   list.Reverse();
来源：http://ln.huanxung.cn

[D12] 查找元素下标
来源：http://lc.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://vj.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fz.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eh.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://by.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://on.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://sm.chemitech.net.cn

Ruby: arr.index(x)
来源：http://qf.nszjky.cn

C#:   list.IndexOf(x);
来源：http://so.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://gr.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nr.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eb.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://mo.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://cv.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pv.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ow.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ew.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ge.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://cs.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cb.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pb.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://nq.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://qz.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mq.chemitech.net.cn

Go:   // 手写循环
来源：http://ww.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://od.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://my.chemitech.net.cn

[D15] 去重
来源：http://hd.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ko.panjiajie.cn

PHP:  array_unique($arr);
来源：http://oj.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ee.nszjky.cn

TS:   [...new Set(arr)]
来源：http://mo.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kt.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bu.jctech888.com.cn

Ruby: arr.uniq
来源：http://ne.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://xv.hnjuh.cn

[D16] 求和与平均值
来源：http://pr.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://as.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cy.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gt.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fx.jctech888.com.cn

Go:   // 手写循环累加
来源：http://pq.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mk.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://kz.lnxyls.cn

[D17] 最大值与最小值
来源：http://xx.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ck.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ju.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nb.szsharing.cn

TS:   Math.max(...arr);
来源：http://hr.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uh.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rh.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://ry.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://yc.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://hr.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wc.521024.cn

PHP:  array_merge(...$nested);
来源：http://hh.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sm.9csxet.cn

TS:   nested.flat();
来源：http://wc.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ia.wgjwhj.cn

Go:   // 手写双层循环
来源：http://wd.jctech888.com.cn

Ruby: nested.flatten
来源：http://hd.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gq.9csxet.cn

[D19] 按字段分组
来源：http://el.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gm.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tp.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vd.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bk.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://hf.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jc.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zo.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://vx.shtwfgs.cn

Py:   Counter(arr)
来源：http://dg.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://fh.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bt.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xq.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vg.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://tr.521024.cn

Ruby: arr.tally
来源：http://bo.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fp.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://kl.nicolike.cn

Py:   x in arr
来源：http://xn.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://hk.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://zv.haigaiapp.cn

TS:   arr.includes(x)
来源：http://dd.yuexingan06.cn

Java: list.contains(x)
来源：http://fw.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://eu.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://dp.szsharing.cn

C#:   list.Contains(x)
来源：http://px.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://om.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://it.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jq.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jt.nszjky.cn

TS:   [...arr];
来源：http://zu.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://qb.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://so.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://am.hnjuh.cn

C#:   new List<int>(list);
来源：http://ka.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ry.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lu.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vy.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fi.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jd.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uu.nicolike.cn

Go:   // 手写循环
来源：http://kw.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sr.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ow.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://nh.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xw.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ee.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xo.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yx.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fr.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hi.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://az.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hq.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://rd.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wl.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yz.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uy.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hv.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rs.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hr.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bg.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jn.yuexingan06.cn

[D26] 数组转字符串
来源：http://id.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://ci.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://js.asd995.cn

JS:   arr.join(", ")
来源：http://kc.panjiajie.cn

TS:   arr.join(", ")
来源：http://ka.muxihuayi.cn

Java: String.join(", ", list)
来源：http://vw.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://rz.shxzskj.cn

Ruby: arr.join(", ")
来源：http://ua.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://jp.nicolike.cn

================================================================================
来源：http://zv.shtwfgs.cn

E. 字符串处理
来源：http://iq.bookmarksfly.cn

================================================================================
来源：http://vi.panjiajie.cn

[E01] 拼接字符串
来源：http://tx.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yq.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gj.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bu.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oj.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ey.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jw.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qn.szsharing.cn

[E02] 重复字符串
来源：http://tg.jctech888.com.cn

Py:   "ab" * 3
来源：http://ug.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://fl.huanxung.cn

JS:   "ab".repeat(3)
来源：http://pm.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://jn.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://hb.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://sz.newstarts.cn

Ruby: "ab" * 3
来源：http://wv.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zu.gzmigu.cn

[E03] 截取子串
来源：http://dn.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yb.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jf.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://av.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://rp.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://zx.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ah.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bz.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://rt.nicolike.cn

[E04] 查找子串位置
来源：http://ho.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ve.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://af.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gi.9csxet.cn

TS:   s.indexOf("x")
来源：http://is.shtwfgs.cn

Java: s.indexOf("x")
来源：http://gy.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://vi.hnjuh.cn

Ruby: s.index("x")
来源：http://is.nicolike.cn

C#:   s.IndexOf("x")
来源：http://dj.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qa.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vn.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xa.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lt.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vi.haigaiapp.cn


<!-- 参考信息 -->