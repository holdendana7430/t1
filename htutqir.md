代发 wailian999

D. 数组 / 列表 / 集合
来源：http://le.bjjhwx.cn

================================================================================
来源：http://zm.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ic.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ok.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vi.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jz.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://as.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nu.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://lp.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://zk.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kn.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://ie.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kl.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gy.521024.cn

JS:   arr.push(4);
来源：http://gj.asd995.cn

TS:   arr.push(4);
来源：http://cq.newstarts.cn

Java: list.add(4);
来源：http://hy.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://km.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://dq.521024.cn

C#:   list.Add(4);
来源：http://oz.colortex.cn

[D03] 在指定位置插入元素
来源：http://md.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://lh.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gh.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://es.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://uc.hnjuh.cn

Java: list.add(0, 0);
来源：http://bh.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iw.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hp.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://so.wgjwhj.cn

[D04] 删除元素
来源：http://yy.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jt.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dd.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eu.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://fq.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yl.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qm.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hn.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vk.lnxyls.cn

[D05] 访问与修改元素
来源：http://lx.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sc.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ec.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gq.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://gr.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://ce.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://wc.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ja.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sr.jianghongdianzi.cn

[D06] 数组长度
来源：http://gm.newstarts.cn

Py:   len(arr)
来源：http://ky.jianghongdianzi.cn

PHP:  count($arr);
来源：http://mv.haigaiapp.cn

JS:   arr.length
来源：http://fw.bookmarksfly.cn

TS:   arr.length
来源：http://fb.lnxyls.cn

Java: list.size();
来源：http://mv.gzmigu.cn

Go:   len(arr)
来源：http://uo.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://ho.wgjwhj.cn

C#:   list.Count;
来源：http://ky.521024.cn

[D07] 切片 / 取子数组
来源：http://ts.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cc.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xc.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://zj.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://md.hnjuh.cn

Java: list.subList(1, 4);
来源：http://tt.muxihuayi.cn

Go:   arr[1:4]
来源：http://jt.newstarts.cn

Ruby: arr[1, 3]
来源：http://jl.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://zu.shtwfgs.cn

[D08] 合并两个数组
来源：http://bb.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://bl.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://mu.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gp.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://cd.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yd.nicolike.cn

Go:   append(a, b...)
来源：http://qd.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://ej.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://sk.nszjky.cn

[D09] 排序（升序）
来源：http://ck.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://rz.jctech888.com.cn

PHP:  sort($arr);
来源：http://sr.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nw.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bl.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ja.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://co.shxzskj.cn

Ruby: arr.sort
来源：http://wx.bookmarksfly.cn

C#:   list.Sort();
来源：http://gz.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lf.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hy.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vn.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sk.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qb.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ig.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sw.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pu.shxzukj.cn

[D11] 反转数组
来源：http://lc.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qt.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://ij.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lg.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://hm.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://lr.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://gb.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://zh.lnxyls.cn

C#:   list.Reverse();
来源：http://wu.shtwfgs.cn

[D12] 查找元素下标
来源：http://hl.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://uh.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pf.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bo.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sy.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://au.colortex.cn

Go:   slices.Index(arr, x)
来源：http://vq.yuexingan06.cn

Ruby: arr.index(x)
来源：http://gn.huanxung.cn

C#:   list.IndexOf(x);
来源：http://lf.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://kh.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dw.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://od.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://wg.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ey.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eo.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kl.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://so.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ja.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://hr.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iq.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kc.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://bp.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://zv.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ud.huixiangedu.cn

Go:   // 手写循环
来源：http://ik.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aj.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wu.yuntaijiaju.cn

[D15] 去重
来源：http://dx.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rf.9csxet.cn

PHP:  array_unique($arr);
来源：http://sd.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://hg.hahajie.cn

TS:   [...new Set(arr)]
来源：http://yy.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bq.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vk.hahajie.cn

Ruby: arr.uniq
来源：http://xk.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://qi.wgjwhj.cn

[D16] 求和与平均值
来源：http://ro.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ji.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pb.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://av.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://po.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zm.shxzukj.cn

Go:   // 手写循环累加
来源：http://om.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vd.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://zg.9csxet.cn

[D17] 最大值与最小值
来源：http://fs.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://hj.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://pn.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ju.panjiajie.cn

TS:   Math.max(...arr);
来源：http://le.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pu.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zf.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://cw.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://cv.521024.cn

[D18] 扁平化嵌套数组
来源：http://ev.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://he.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ec.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uf.hahajie.cn

TS:   nested.flat();
来源：http://gj.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://md.asd995.cn

Go:   // 手写双层循环
来源：http://cw.shxzukj.cn

Ruby: nested.flatten
来源：http://gv.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jc.muxihuayi.cn

[D19] 按字段分组
来源：http://pa.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nr.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://an.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sm.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lf.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fv.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://jj.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vf.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dd.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://lv.szxytkj.cn

Py:   Counter(arr)
来源：http://ft.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://wt.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uu.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vw.521024.cn

Go:   // 手写 map[T]int
来源：http://xb.shxzskj.cn

Ruby: arr.tally
来源：http://ho.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sf.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://bt.shtwfgs.cn

Py:   x in arr
来源：http://wm.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yj.shxzskj.cn

JS:   arr.includes(x)
来源：http://zv.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://xb.haigaiapp.cn

Java: list.contains(x)
来源：http://qu.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://ns.521024.cn

Ruby: arr.include?(x)
来源：http://sd.shxzskj.cn

C#:   list.Contains(x)
来源：http://ek.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xy.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hl.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ep.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rg.colortex.cn

TS:   [...arr];
来源：http://qd.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://ff.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hm.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://xy.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://bk.hnjuh.cn

[D23] reduce 累积计算
来源：http://gm.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tb.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uo.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bv.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://am.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://og.newstarts.cn

Go:   // 手写循环
来源：http://gu.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ol.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://to.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://cz.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eb.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wk.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qa.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qg.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dc.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ey.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pe.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ip.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ge.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://at.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gp.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vx.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pk.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vn.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mi.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rc.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gf.jctech888.com.cn

[D26] 数组转字符串
来源：http://ww.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://mq.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://mh.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://zt.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://hf.yuexingan06.cn

Java: String.join(", ", list)
来源：http://bt.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://ir.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://di.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://pn.shxzukj.cn

================================================================================
来源：http://bq.nicolike.cn

E. 字符串处理
来源：http://xk.huixinmuqiang.cn

================================================================================
来源：http://aj.521024.cn

[E01] 拼接字符串
来源：http://og.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xk.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dq.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yh.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vu.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ic.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ti.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zp.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wq.haigaiapp.cn

[E02] 重复字符串
来源：http://jw.chemitech.net.cn

Py:   "ab" * 3
来源：http://du.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://ef.newstarts.cn

JS:   "ab".repeat(3)
来源：http://av.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://pz.newstarts.cn

Java: "ab".repeat(3)
来源：http://pj.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://jy.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://bd.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oa.bjjhwx.cn

[E03] 截取子串
来源：http://ak.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nt.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ax.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://in.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://oz.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://jr.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qs.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dz.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://da.lnxyls.cn

[E04] 查找子串位置
来源：http://cv.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://uw.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://wy.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ut.gzmigu.cn

TS:   s.indexOf("x")
来源：http://qu.huixiangedu.cn

Java: s.indexOf("x")
来源：http://jc.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://jb.wgjwhj.cn

Ruby: s.index("x")
来源：http://qf.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://tb.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pm.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qu.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yi.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xr.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wh.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yw.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pa.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ee.nicolike.cn

[E06] 替换子串
来源：http://xm.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zh.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://pb.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wa.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://qw.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ad.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hn.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zd.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://zj.hnjuh.cn

[E07] 按分隔符拆分
来源：http://wm.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hg.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vz.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gp.hahajie.cn

TS:   s.split(",")
来源：http://vf.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mv.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nv.yuntaijiaju.cn


<!-- 参考信息 -->