代发 wailian999

Ruby: a, b = pair
来源：http://br.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://ah.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://dt.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bc.asd995.cn

PHP:  // 无重载
来源：http://sb.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ba.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://vm.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tu.521024.cn

Go:   // 无重载：用不同函数名
来源：http://ay.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://nn.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sf.asd995.cn

================================================================================
来源：http://dy.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://gt.haigaiapp.cn

================================================================================
来源：http://rw.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://si.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qp.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://id.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bg.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xa.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fe.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ph.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://ht.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ss.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://lh.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xk.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pc.shxzukj.cn

JS:   arr.push(4);
来源：http://kt.nszjky.cn

TS:   arr.push(4);
来源：http://au.hahajie.cn

Java: list.add(4);
来源：http://zv.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://wq.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://no.huixiangedu.cn

C#:   list.Add(4);
来源：http://to.colortex.cn

[D03] 在指定位置插入元素
来源：http://ed.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://wm.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cc.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wf.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://wi.muxihuayi.cn

Java: list.add(0, 0);
来源：http://sj.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://no.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nb.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://fc.yuntaijiaju.cn

[D04] 删除元素
来源：http://kd.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qj.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pa.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dn.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://sc.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ch.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nt.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gx.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wi.nicolike.cn

[D05] 访问与修改元素
来源：http://tz.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yy.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uq.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tn.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://mi.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://fy.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ep.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cz.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ql.nszjky.cn

[D06] 数组长度
来源：http://qs.szsharing.cn

Py:   len(arr)
来源：http://yi.chemitech.net.cn

PHP:  count($arr);
来源：http://ly.hnjuh.cn

JS:   arr.length
来源：http://ft.chemitech.net.cn

TS:   arr.length
来源：http://zv.huixiangedu.cn

Java: list.size();
来源：http://ho.panjiajie.cn

Go:   len(arr)
来源：http://hy.szsharing.cn

Ruby: arr.length; arr.size
来源：http://we.521024.cn

C#:   list.Count;
来源：http://nr.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://se.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fe.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://va.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://sl.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://km.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://dk.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://hj.newstarts.cn

Ruby: arr[1, 3]
来源：http://df.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://ip.yuexingan06.cn

[D08] 合并两个数组
来源：http://ea.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://tc.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://zh.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zq.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ze.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ys.newstarts.cn

Go:   append(a, b...)
来源：http://py.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://tl.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://cu.shxzukj.cn

[D09] 排序（升序）
来源：http://ct.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://rn.muxihuayi.cn

PHP:  sort($arr);
来源：http://ld.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://td.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ow.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nw.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://va.szxytkj.cn

Ruby: arr.sort
来源：http://ak.shtwfgs.cn

C#:   list.Sort();
来源：http://ho.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cr.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://od.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yt.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://co.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vf.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ql.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tr.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://np.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oy.jianghongdianzi.cn

[D11] 反转数组
来源：http://io.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eh.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://gq.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ay.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://vc.huanxung.cn

Java: Collections.reverse(list);
来源：http://bq.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://fo.panjiajie.cn

Ruby: arr.reverse
来源：http://jl.hahajie.cn

C#:   list.Reverse();
来源：http://hk.gzmigu.cn

[D12] 查找元素下标
来源：http://yq.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://df.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tm.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eg.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ym.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xr.521024.cn

Go:   slices.Index(arr, x)
来源：http://as.colortex.cn

Ruby: arr.index(x)
来源：http://js.hahajie.cn

C#:   list.IndexOf(x);
来源：http://qn.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://tp.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://as.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ub.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://uc.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://tb.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iv.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://df.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ga.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ly.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://jv.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nq.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nn.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ld.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://hz.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ns.nszjky.cn

Go:   // 手写循环
来源：http://kb.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qv.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oa.szxytkj.cn

[D15] 去重
来源：http://cm.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vv.colortex.cn

PHP:  array_unique($arr);
来源：http://yv.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://gg.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://vl.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xb.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://py.lnxyls.cn

Ruby: arr.uniq
来源：http://id.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://pt.nicolike.cn

[D16] 求和与平均值
来源：http://fe.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ly.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ci.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ql.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ap.shxzskj.cn

Go:   // 手写循环累加
来源：http://jh.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://at.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://tu.521024.cn

[D17] 最大值与最小值
来源：http://zd.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://kb.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://wj.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uq.hahajie.cn

TS:   Math.max(...arr);
来源：http://xh.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zu.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://df.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://tf.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://da.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://sh.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sm.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://kv.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vk.colortex.cn

TS:   nested.flat();
来源：http://ky.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ag.hnjuh.cn

Go:   // 手写双层循环
来源：http://gy.yuexingan06.cn

Ruby: nested.flatten
来源：http://lq.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zg.panjiajie.cn

[D19] 按字段分组
来源：http://mi.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kf.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ok.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ev.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pt.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aw.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://zw.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ry.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gw.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://vj.haigaiapp.cn

Py:   Counter(arr)
来源：http://sc.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://fz.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rl.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kf.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hj.colortex.cn

Go:   // 手写 map[T]int
来源：http://ib.shtwfgs.cn

Ruby: arr.tally
来源：http://zv.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ib.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://sl.huixiangedu.cn

Py:   x in arr
来源：http://th.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ni.nicolike.cn

JS:   arr.includes(x)
来源：http://dt.hahajie.cn

TS:   arr.includes(x)
来源：http://sh.shxzskj.cn

Java: list.contains(x)
来源：http://gu.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://cm.panjiajie.cn

Ruby: arr.include?(x)
来源：http://fe.jctech888.com.cn

C#:   list.Contains(x)
来源：http://nc.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://fy.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gz.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cs.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mk.hahajie.cn

TS:   [...arr];
来源：http://ou.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://og.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rz.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://nz.nicolike.cn

C#:   new List<int>(list);
来源：http://mc.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://tn.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://be.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://om.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sk.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://we.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pr.colortex.cn

Go:   // 手写循环
来源：http://cf.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ir.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://et.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://tn.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ov.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ss.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jf.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dd.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bo.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ya.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bg.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dm.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://eq.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kf.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mb.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yi.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kl.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sx.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://et.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oq.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://an.wgjwhj.cn

[D26] 数组转字符串
来源：http://xn.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://gh.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://rm.shxzukj.cn

JS:   arr.join(", ")
来源：http://ix.bjjhwx.cn

TS:   arr.join(", ")
来源：http://iw.huixiangedu.cn

Java: String.join(", ", list)
来源：http://jz.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://bx.hahajie.cn

Ruby: arr.join(", ")
来源：http://gr.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://dz.yuexingan06.cn

================================================================================
来源：http://as.colortex.cn

E. 字符串处理
来源：http://uc.asd995.cn

================================================================================
来源：http://gp.shtwfgs.cn

[E01] 拼接字符串
来源：http://ck.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://le.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ul.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vx.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ey.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://at.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xo.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tp.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bh.huixiangedu.cn

[E02] 重复字符串
来源：http://aw.hnjuh.cn

Py:   "ab" * 3
来源：http://tf.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://mh.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://ae.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://jn.gzmigu.cn

Java: "ab".repeat(3)
来源：http://oc.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://su.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://xs.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vy.jianghongdianzi.cn

[E03] 截取子串
来源：http://ve.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ei.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lr.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bx.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ri.lnxyls.cn

Java: s.substring(1, 4)
来源：http://na.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xm.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wl.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://vg.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ni.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://eu.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://zk.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kk.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ga.newstarts.cn

Java: s.indexOf("x")
来源：http://tr.colortex.cn

Go:   strings.Index(s, "x")
来源：http://oq.szsharing.cn

Ruby: s.index("x")
来源：http://zq.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://nl.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tv.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xf.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bw.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tx.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://io.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ew.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ri.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://me.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eb.colortex.cn

[E06] 替换子串
来源：http://jc.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oz.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://lm.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xc.wgjwhj.cn


<!-- 参考信息 -->