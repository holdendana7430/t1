代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://gh.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://tc.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://an.lnxyls.cn

================================================================================
来源：http://me.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://nf.panjiajie.cn

================================================================================
来源：http://tr.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://el.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nv.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qz.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ny.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xu.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zw.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://kd.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ec.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xw.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://gt.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nq.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dy.shtwfgs.cn

JS:   arr.push(4);
来源：http://kd.wgjwhj.cn

TS:   arr.push(4);
来源：http://tx.hahajie.cn

Java: list.add(4);
来源：http://fc.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://xi.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://sc.shtwfgs.cn

C#:   list.Add(4);
来源：http://pq.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://by.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://sp.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qh.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ma.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://nq.newstarts.cn

Java: list.add(0, 0);
来源：http://gs.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bt.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ji.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ll.9csxet.cn

[D04] 删除元素
来源：http://ai.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pc.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wh.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ow.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://qb.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wg.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yg.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://si.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ef.szsharing.cn

[D05] 访问与修改元素
来源：http://ml.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://co.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yi.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wp.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://uf.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://ym.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://cl.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://st.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pp.szxytkj.cn

[D06] 数组长度
来源：http://zh.huanxung.cn

Py:   len(arr)
来源：http://wu.lnxyls.cn

PHP:  count($arr);
来源：http://sm.nicolike.cn

JS:   arr.length
来源：http://yk.hahajie.cn

TS:   arr.length
来源：http://zo.asd995.cn

Java: list.size();
来源：http://jx.lnxyls.cn

Go:   len(arr)
来源：http://dw.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://vv.bookmarksfly.cn

C#:   list.Count;
来源：http://au.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://uq.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nf.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nn.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://lg.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://kx.lnxyls.cn

Java: list.subList(1, 4);
来源：http://mt.nicolike.cn

Go:   arr[1:4]
来源：http://hu.colortex.cn

Ruby: arr[1, 3]
来源：http://xo.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://eq.huanxung.cn

[D08] 合并两个数组
来源：http://qk.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://io.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://sq.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rb.haigaiapp.cn

TS:   [...a, ...b];
来源：http://nx.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://og.szsharing.cn

Go:   append(a, b...)
来源：http://to.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://nu.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://go.yuexingan06.cn

[D09] 排序（升序）
来源：http://ei.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://qd.asd995.cn

PHP:  sort($arr);
来源：http://dq.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cc.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fk.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ve.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pc.jctech888.com.cn

Ruby: arr.sort
来源：http://ua.colortex.cn

C#:   list.Sort();
来源：http://xd.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fu.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ao.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fi.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://or.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nk.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xt.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lk.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qt.hnjuh.cn

[D11] 反转数组
来源：http://ng.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oc.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://va.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ji.lnxyls.cn

TS:   [...arr].reverse();
来源：http://vu.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://vm.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://mc.9csxet.cn

Ruby: arr.reverse
来源：http://fh.nszjky.cn

C#:   list.Reverse();
来源：http://fw.szxytkj.cn

[D12] 查找元素下标
来源：http://fv.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://qm.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bq.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ab.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sy.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xh.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://jh.hnjuh.cn

Ruby: arr.index(x)
来源：http://nn.asd995.cn

C#:   list.IndexOf(x);
来源：http://er.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://rc.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uw.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aa.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://iv.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://ah.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ne.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vn.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://of.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lk.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://ur.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jo.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jr.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://ml.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://zh.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dm.521024.cn

Go:   // 手写循环
来源：http://ar.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://el.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dd.shxzskj.cn

[D15] 去重
来源：http://pk.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pn.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://qz.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://gv.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://lh.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ph.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lz.colortex.cn

Ruby: arr.uniq
来源：http://xy.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://eb.nszjky.cn

[D16] 求和与平均值
来源：http://os.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://no.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wo.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gs.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ux.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cs.shxzskj.cn

Go:   // 手写循环累加
来源：http://np.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bc.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://cl.lnxyls.cn

[D17] 最大值与最小值
来源：http://pu.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://lg.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://xh.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oq.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://vo.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bc.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jf.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://xd.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://ah.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ba.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hu.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://hz.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lw.panjiajie.cn

TS:   nested.flat();
来源：http://mi.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uw.wgjwhj.cn

Go:   // 手写双层循环
来源：http://gs.szsharing.cn

Ruby: nested.flatten
来源：http://ge.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rg.wgjwhj.cn

[D19] 按字段分组
来源：http://iz.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vt.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ho.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://av.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xr.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pe.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://ki.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fz.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xh.asd995.cn

[D20] 统计每个元素出现次数
来源：http://yq.jctech888.com.cn

Py:   Counter(arr)
来源：http://pc.521024.cn

PHP:  array_count_values($arr);
来源：http://ic.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jo.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tx.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jq.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://to.nszjky.cn

Ruby: arr.tally
来源：http://kd.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vr.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://zn.gzmigu.cn

Py:   x in arr
来源：http://yc.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://nh.newstarts.cn

JS:   arr.includes(x)
来源：http://qf.haigaiapp.cn

TS:   arr.includes(x)
来源：http://ix.9csxet.cn

Java: list.contains(x)
来源：http://kt.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://fo.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ix.colortex.cn

C#:   list.Contains(x)
来源：http://ti.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://xd.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gb.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://le.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ku.asd995.cn

TS:   [...arr];
来源：http://qq.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://wc.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bq.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://iu.szsharing.cn

C#:   new List<int>(list);
来源：http://oy.huanxung.cn

[D23] reduce 累积计算
来源：http://wz.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zj.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fc.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://od.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nb.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ma.521024.cn

Go:   // 手写循环
来源：http://wb.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://az.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qg.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ar.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wc.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ud.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://le.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nq.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xv.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kh.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bm.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tr.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://fs.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mj.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ol.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ih.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vn.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://en.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wi.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ft.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ly.shxzskj.cn

[D26] 数组转字符串
来源：http://fu.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://bi.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://je.yuexingan06.cn

JS:   arr.join(", ")
来源：http://yn.asd995.cn

TS:   arr.join(", ")
来源：http://mp.shxzukj.cn

Java: String.join(", ", list)
来源：http://ej.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://wg.hahajie.cn

Ruby: arr.join(", ")
来源：http://zb.huanxung.cn

C#:   string.Join(", ", list)
来源：http://xg.haigaiapp.cn

================================================================================
来源：http://ig.asd995.cn

E. 字符串处理
来源：http://un.bjjhwx.cn

================================================================================
来源：http://gt.haigaiapp.cn

[E01] 拼接字符串
来源：http://po.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yr.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yk.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zr.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dd.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oy.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ly.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nd.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kc.9csxet.cn

[E02] 重复字符串
来源：http://lz.huixiangedu.cn

Py:   "ab" * 3
来源：http://jt.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ie.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://bh.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ga.szsharing.cn

Java: "ab".repeat(3)
来源：http://jv.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://uc.shxzukj.cn

Ruby: "ab" * 3
来源：http://ju.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kk.lnxyls.cn

[E03] 截取子串
来源：http://xo.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rq.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ur.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sd.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://hi.szsharing.cn

Java: s.substring(1, 4)
来源：http://ed.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nw.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ov.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://lx.szsharing.cn

[E04] 查找子串位置
来源：http://lg.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://gv.newstarts.cn

PHP:  strpos($s, "x");
来源：http://xf.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://by.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://pw.wgjwhj.cn

Java: s.indexOf("x")
来源：http://jv.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://gc.szsharing.cn

Ruby: s.index("x")
来源：http://vd.9csxet.cn

C#:   s.IndexOf("x")
来源：http://gc.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pm.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jk.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qj.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rj.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wa.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mw.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ir.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xv.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qb.chemitech.net.cn

[E06] 替换子串
来源：http://wz.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gd.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://vg.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://va.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://vw.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ie.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tk.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nh.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://ge.nicolike.cn

[E07] 按分隔符拆分
来源：http://yy.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lr.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://im.gzmigu.cn


<!-- 参考信息 -->