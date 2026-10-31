代发 wailian999

PHP:  // 无重载
来源：http://vr.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://re.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://dv.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dv.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://yz.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://vi.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cj.yuexingan06.cn

================================================================================
来源：http://yg.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://oa.huixiangedu.cn

================================================================================
来源：http://vl.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://gf.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hq.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zg.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mu.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gl.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://th.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://lq.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://uz.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ia.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://xd.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wf.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pj.huanxung.cn

JS:   arr.push(4);
来源：http://jb.nszjky.cn

TS:   arr.push(4);
来源：http://ii.bjjhwx.cn

Java: list.add(4);
来源：http://hu.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://so.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://nk.colortex.cn

C#:   list.Add(4);
来源：http://ph.nicolike.cn

[D03] 在指定位置插入元素
来源：http://hm.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ym.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ck.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lg.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://um.bjjhwx.cn

Java: list.add(0, 0);
来源：http://sr.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ij.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cr.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://kk.szsharing.cn

[D04] 删除元素
来源：http://qr.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ng.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gr.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bd.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://dm.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bq.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jn.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fc.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vx.newstarts.cn

[D05] 访问与修改元素
来源：http://tu.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ea.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fe.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xy.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://pb.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://sz.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://nu.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ng.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vz.huixiangedu.cn

[D06] 数组长度
来源：http://fw.yuexingan06.cn

Py:   len(arr)
来源：http://on.szxytkj.cn

PHP:  count($arr);
来源：http://dm.jctech888.com.cn

JS:   arr.length
来源：http://gg.szsharing.cn

TS:   arr.length
来源：http://yd.huixinmuqiang.cn

Java: list.size();
来源：http://dz.nicolike.cn

Go:   len(arr)
来源：http://tf.huanxung.cn

Ruby: arr.length; arr.size
来源：http://yt.shtwfgs.cn

C#:   list.Count;
来源：http://xc.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ny.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lz.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dc.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://fv.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://em.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://wf.asd995.cn

Go:   arr[1:4]
来源：http://cs.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://bx.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://iu.huixiangedu.cn

[D08] 合并两个数组
来源：http://gq.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ie.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://cp.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ak.wgjwhj.cn

TS:   [...a, ...b];
来源：http://av.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sv.wgjwhj.cn

Go:   append(a, b...)
来源：http://mx.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ge.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://hf.asd995.cn

[D09] 排序（升序）
来源：http://hc.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://iz.nszjky.cn

PHP:  sort($arr);
来源：http://fe.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sh.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cg.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tk.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://so.bookmarksfly.cn

Ruby: arr.sort
来源：http://jf.521024.cn

C#:   list.Sort();
来源：http://jq.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fo.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dm.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ns.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mh.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jc.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ul.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dy.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://es.jctech888.com.cn

[D11] 反转数组
来源：http://jt.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wd.newstarts.cn

PHP:  array_reverse($arr);
来源：http://qp.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ci.nicolike.cn

TS:   [...arr].reverse();
来源：http://uq.gzmigu.cn

Java: Collections.reverse(list);
来源：http://lu.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://ce.shxzukj.cn

Ruby: arr.reverse
来源：http://gs.szxytkj.cn

C#:   list.Reverse();
来源：http://at.shxzukj.cn

[D12] 查找元素下标
来源：http://zw.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://nr.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ad.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xu.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fw.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://sg.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://hw.newstarts.cn

C#:   list.IndexOf(x);
来源：http://tl.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://ya.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gk.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ui.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://zg.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://gk.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://up.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tg.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://je.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qm.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://nx.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kv.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wg.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://nk.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://nn.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://no.nicolike.cn

Go:   // 手写循环
来源：http://bo.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rl.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sd.shxzukj.cn

[D15] 去重
来源：http://ys.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ae.hahajie.cn

PHP:  array_unique($arr);
来源：http://kt.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://rq.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://eo.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mb.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sy.shxzskj.cn

Ruby: arr.uniq
来源：http://ac.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://zv.bjjhwx.cn

[D16] 求和与平均值
来源：http://pd.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fl.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://az.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ni.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yy.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lv.bjjhwx.cn

Go:   // 手写循环累加
来源：http://ss.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ht.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://cb.yuexingan06.cn

[D17] 最大值与最小值
来源：http://dl.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://pl.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://yh.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://em.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://gv.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ve.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://il.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://zr.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ht.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://rr.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ab.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://ro.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sk.chemitech.net.cn

TS:   nested.flat();
来源：http://rz.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qk.muxihuayi.cn

Go:   // 手写双层循环
来源：http://kl.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://gy.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tl.shxzukj.cn

[D19] 按字段分组
来源：http://ie.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://up.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fv.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cw.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pn.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ro.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://xl.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mc.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wz.colortex.cn

[D20] 统计每个元素出现次数
来源：http://qa.asd995.cn

Py:   Counter(arr)
来源：http://im.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://hk.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eq.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://py.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mz.9csxet.cn

Go:   // 手写 map[T]int
来源：http://lb.521024.cn

Ruby: arr.tally
来源：http://rp.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://za.hahajie.cn

[D21] 判断是否包含某元素
来源：http://lk.nicolike.cn

Py:   x in arr
来源：http://ih.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://oz.hnjuh.cn

JS:   arr.includes(x)
来源：http://eq.colortex.cn

TS:   arr.includes(x)
来源：http://mg.huixinmuqiang.cn

Java: list.contains(x)
来源：http://lg.521024.cn

Go:   slices.Contains(arr, x)
来源：http://ns.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://my.haigaiapp.cn

C#:   list.Contains(x)
来源：http://rw.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://cp.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vw.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://le.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sl.shtwfgs.cn

TS:   [...arr];
来源：http://ny.hahajie.cn

Java: new ArrayList<>(list);
来源：http://bo.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jn.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://og.newstarts.cn

C#:   new List<int>(list);
来源：http://pi.shxzskj.cn

[D23] reduce 累积计算
来源：http://ff.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dj.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://es.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mk.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rl.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pa.huixiangedu.cn

Go:   // 手写循环
来源：http://kd.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lv.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qf.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://on.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ss.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eq.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dn.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ia.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bu.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wi.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fh.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zb.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://rw.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ov.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rk.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vh.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cr.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xi.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cu.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rw.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ew.chemitech.net.cn

[D26] 数组转字符串
来源：http://hz.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://rx.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://rs.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://uj.szxytkj.cn

TS:   arr.join(", ")
来源：http://nz.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://lq.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ax.gzmigu.cn

Ruby: arr.join(", ")
来源：http://nq.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://zt.bjjhwx.cn

================================================================================
来源：http://gx.chemitech.net.cn

E. 字符串处理
来源：http://oy.bjjhwx.cn

================================================================================
来源：http://ui.huanxung.cn

[E01] 拼接字符串
来源：http://bz.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lp.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://av.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qx.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rz.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pw.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ve.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nm.panjiajie.cn

[E02] 重复字符串
来源：http://bx.asd995.cn

Py:   "ab" * 3
来源：http://zi.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ft.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://ug.colortex.cn

TS:   "ab".repeat(3)
来源：http://en.9csxet.cn

Java: "ab".repeat(3)
来源：http://nn.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://eb.gzmigu.cn

Ruby: "ab" * 3
来源：http://hs.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ao.chemitech.net.cn

[E03] 截取子串
来源：http://pg.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dm.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ni.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xl.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://hk.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://dx.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pj.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mc.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://mr.colortex.cn

[E04] 查找子串位置
来源：http://qd.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://yo.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://li.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bh.9csxet.cn

TS:   s.indexOf("x")
来源：http://dv.haigaiapp.cn

Java: s.indexOf("x")
来源：http://ex.521024.cn

Go:   strings.Index(s, "x")
来源：http://jm.colortex.cn

Ruby: s.index("x")
来源：http://ab.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://hh.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bq.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qc.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ue.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gn.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uh.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ld.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bc.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kz.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yt.yuexingan06.cn

[E06] 替换子串
来源：http://aw.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jq.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ly.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pc.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://qf.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://an.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://us.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eu.gzmigu.cn


<!-- 参考信息 -->