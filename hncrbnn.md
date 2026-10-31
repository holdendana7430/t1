代发 wailian999

PHP:  // 无重载
来源：http://af.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tt.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://to.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rp.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://xi.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://gp.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sy.lnxyls.cn

================================================================================
来源：http://jc.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ab.asd995.cn

================================================================================
来源：http://rs.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://be.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zy.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vd.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ds.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://du.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uc.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://fa.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://iv.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://st.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://rr.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gg.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fi.lnxyls.cn

JS:   arr.push(4);
来源：http://vk.nicolike.cn

TS:   arr.push(4);
来源：http://qr.yuexingan06.cn

Java: list.add(4);
来源：http://wt.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://pi.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://je.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ql.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://bm.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://ih.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nm.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://je.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://oo.bjjhwx.cn

Java: list.add(0, 0);
来源：http://ti.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jy.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pj.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://mk.hnjuh.cn

[D04] 删除元素
来源：http://il.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xh.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mp.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://mo.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jh.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://if.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zi.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gg.wgjwhj.cn

[D05] 访问与修改元素
来源：http://mt.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gj.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ai.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ip.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://hr.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://kh.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pd.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zq.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lr.nszjky.cn

[D06] 数组长度
来源：http://zn.huanxung.cn

Py:   len(arr)
来源：http://mz.shxzskj.cn

PHP:  count($arr);
来源：http://vj.lnxyls.cn

JS:   arr.length
来源：http://fq.panjiajie.cn

TS:   arr.length
来源：http://pp.wgjwhj.cn

Java: list.size();
来源：http://ir.yuntaijiaju.cn

Go:   len(arr)
来源：http://kw.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://eo.huanxung.cn

C#:   list.Count;
来源：http://gm.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://un.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xr.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eo.colortex.cn

JS:   arr.slice(1, 4);
来源：http://pe.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://lo.nicolike.cn

Java: list.subList(1, 4);
来源：http://gk.gzmigu.cn

Go:   arr[1:4]
来源：http://gz.szsharing.cn

Ruby: arr[1, 3]
来源：http://uj.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://yz.shxzskj.cn

[D08] 合并两个数组
来源：http://dr.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://rz.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://aq.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bn.szsharing.cn

TS:   [...a, ...b];
来源：http://wx.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qy.colortex.cn

Go:   append(a, b...)
来源：http://lm.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://rg.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://gb.haigaiapp.cn

[D09] 排序（升序）
来源：http://xy.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://uy.jctech888.com.cn

PHP:  sort($arr);
来源：http://ly.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jn.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xh.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qg.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://du.521024.cn

Ruby: arr.sort
来源：http://eo.shxzukj.cn

C#:   list.Sort();
来源：http://ya.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://he.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wz.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zo.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eq.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mo.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kl.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tk.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bs.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bm.nicolike.cn

[D11] 反转数组
来源：http://gd.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fl.hahajie.cn

PHP:  array_reverse($arr);
来源：http://oq.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sf.521024.cn

TS:   [...arr].reverse();
来源：http://tf.colortex.cn

Java: Collections.reverse(list);
来源：http://ca.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://nv.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ew.asd995.cn

C#:   list.Reverse();
来源：http://ay.wgjwhj.cn

[D12] 查找元素下标
来源：http://sn.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://bl.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lv.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wa.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://le.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fx.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://qp.jctech888.com.cn

Ruby: arr.index(x)
来源：http://ko.newstarts.cn

C#:   list.IndexOf(x);
来源：http://rr.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://xo.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sr.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ng.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://uq.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://lg.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nn.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gh.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ax.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vf.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://ae.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yu.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nu.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://pu.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://dm.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.colortex.cn

Go:   // 手写循环
来源：http://kk.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cu.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ol.shxzskj.cn

[D15] 去重
来源：http://be.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lj.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://oz.colortex.cn

JS:   [...new Set(arr)]
来源：http://ws.szsharing.cn

TS:   [...new Set(arr)]
来源：http://bl.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fe.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aa.haigaiapp.cn

Ruby: arr.uniq
来源：http://sp.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://bu.nicolike.cn

[D16] 求和与平均值
来源：http://ln.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cj.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ne.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zl.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://do.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ss.lnxyls.cn

Go:   // 手写循环累加
来源：http://pz.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://df.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://ss.shxzskj.cn

[D17] 最大值与最小值
来源：http://fv.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://le.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://jf.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ex.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://mn.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pg.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dw.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://id.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://vx.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://vh.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xq.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://no.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sf.panjiajie.cn

TS:   nested.flat();
来源：http://kp.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vu.panjiajie.cn

Go:   // 手写双层循环
来源：http://rp.huixiangedu.cn

Ruby: nested.flatten
来源：http://pr.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mf.wgjwhj.cn

[D19] 按字段分组
来源：http://ly.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://we.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jj.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hw.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bz.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dn.521024.cn

Go:   // 手写 map[string][]T
来源：http://nd.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ao.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://vf.asd995.cn

Py:   Counter(arr)
来源：http://gc.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ww.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ai.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mg.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bs.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ek.muxihuayi.cn

Ruby: arr.tally
来源：http://vc.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jj.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://by.newstarts.cn

Py:   x in arr
来源：http://iy.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://yp.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://tm.yuexingan06.cn

TS:   arr.includes(x)
来源：http://uh.asd995.cn

Java: list.contains(x)
来源：http://qk.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://tc.hahajie.cn

Ruby: arr.include?(x)
来源：http://ru.muxihuayi.cn

C#:   list.Contains(x)
来源：http://qd.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ns.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mo.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gl.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zf.shtwfgs.cn

TS:   [...arr];
来源：http://no.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://dp.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bv.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://um.newstarts.cn

C#:   new List<int>(list);
来源：http://ny.gzmigu.cn

[D23] reduce 累积计算
来源：http://of.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hf.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gj.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hx.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vi.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lu.521024.cn

Go:   // 手写循环
来源：http://km.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tf.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://st.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://kp.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ln.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mp.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ip.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wu.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ti.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wy.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qh.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ej.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://ts.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nt.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jj.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ij.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xj.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://do.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lx.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wo.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nh.shxzukj.cn

[D26] 数组转字符串
来源：http://om.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://pp.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://ba.huixiangedu.cn

JS:   arr.join(", ")
来源：http://xf.chemitech.net.cn

TS:   arr.join(", ")
来源：http://iw.wgjwhj.cn

Java: String.join(", ", list)
来源：http://na.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://sf.panjiajie.cn

Ruby: arr.join(", ")
来源：http://qb.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://wc.asd995.cn

================================================================================
来源：http://zs.nicolike.cn

E. 字符串处理
来源：http://iy.yuntaijiaju.cn

================================================================================
来源：http://ds.hnjuh.cn

[E01] 拼接字符串
来源：http://oe.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lp.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://js.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rr.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qd.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ay.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ok.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fl.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fm.huanxung.cn

[E02] 重复字符串
来源：http://sb.newstarts.cn

Py:   "ab" * 3
来源：http://zg.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://nz.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://jj.nicolike.cn

TS:   "ab".repeat(3)
来源：http://ky.hahajie.cn

Java: "ab".repeat(3)
来源：http://ng.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://rr.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://mr.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ys.hnjuh.cn

[E03] 截取子串
来源：http://ru.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tv.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fj.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nd.hahajie.cn

TS:   s.slice(1, 4)
来源：http://wt.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://qj.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dz.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yf.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://jo.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://ij.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://oh.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://pr.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qt.lnxyls.cn

TS:   s.indexOf("x")
来源：http://dh.shxzskj.cn

Java: s.indexOf("x")
来源：http://cx.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://fg.huanxung.cn

Ruby: s.index("x")
来源：http://za.newstarts.cn

C#:   s.IndexOf("x")
来源：http://vj.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tj.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ge.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://og.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rr.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ye.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://te.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://or.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://je.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pc.shxzskj.cn

[E06] 替换子串
来源：http://sy.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yk.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://zm.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ef.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://dc.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mf.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gb.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xn.hahajie.cn


<!-- 参考信息 -->