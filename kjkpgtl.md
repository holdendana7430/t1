代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cs.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ix.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://po.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sm.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://yw.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://xw.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fn.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://kn.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ur.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vc.shtwfgs.cn

JS:   arr.push(4);
来源：http://md.haigaiapp.cn

TS:   arr.push(4);
来源：http://dl.colortex.cn

Java: list.add(4);
来源：http://qn.colortex.cn

Go:   arr = append(arr, 4)
来源：http://jq.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://cd.muxihuayi.cn

C#:   list.Add(4);
来源：http://ll.szsharing.cn

[D03] 在指定位置插入元素
来源：http://en.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ty.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rr.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ea.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ji.jctech888.com.cn

Java: list.add(0, 0);
来源：http://kl.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jb.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zq.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://lh.shxzskj.cn

[D04] 删除元素
来源：http://xl.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vw.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dc.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ml.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://lk.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fg.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zf.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wm.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uh.wgjwhj.cn

[D05] 访问与修改元素
来源：http://qw.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mf.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uf.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ec.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://du.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://va.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://ur.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://of.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zq.chemitech.net.cn

[D06] 数组长度
来源：http://qz.shxzukj.cn

Py:   len(arr)
来源：http://id.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ic.newstarts.cn

JS:   arr.length
来源：http://jz.asd995.cn

TS:   arr.length
来源：http://yf.nicolike.cn

Java: list.size();
来源：http://xr.jctech888.com.cn

Go:   len(arr)
来源：http://fv.9csxet.cn

Ruby: arr.length; arr.size
来源：http://er.panjiajie.cn

C#:   list.Count;
来源：http://qy.szsharing.cn

[D07] 切片 / 取子数组
来源：http://yo.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vk.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://th.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://dn.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://wd.newstarts.cn

Java: list.subList(1, 4);
来源：http://ch.hnjuh.cn

Go:   arr[1:4]
来源：http://kb.hnjuh.cn

Ruby: arr[1, 3]
来源：http://tf.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ki.shxzukj.cn

[D08] 合并两个数组
来源：http://sq.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://jy.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://tn.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://go.hahajie.cn

TS:   [...a, ...b];
来源：http://tz.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hb.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ds.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://qb.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ny.szxytkj.cn

[D09] 排序（升序）
来源：http://ty.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://oc.shxzskj.cn

PHP:  sort($arr);
来源：http://xb.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qt.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://br.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wo.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qx.9csxet.cn

Ruby: arr.sort
来源：http://xf.muxihuayi.cn

C#:   list.Sort();
来源：http://kw.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sa.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rs.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sa.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vx.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dt.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://de.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yy.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ll.colortex.cn

[D11] 反转数组
来源：http://sy.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lr.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://ol.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hb.9csxet.cn

TS:   [...arr].reverse();
来源：http://xr.colortex.cn

Java: Collections.reverse(list);
来源：http://bu.colortex.cn

Go:   slices.Reverse(arr)
来源：http://ay.9csxet.cn

Ruby: arr.reverse
来源：http://hl.asd995.cn

C#:   list.Reverse();
来源：http://lk.nszjky.cn

[D12] 查找元素下标
来源：http://lz.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://fg.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cp.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://il.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gt.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nt.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://om.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ra.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://vp.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://yw.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ck.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bh.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://dd.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://dz.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xe.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nk.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mj.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ya.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://oa.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://et.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pu.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://ln.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://fb.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nt.wgjwhj.cn

Go:   // 手写循环
来源：http://jq.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zb.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aq.huixinmuqiang.cn

[D15] 去重
来源：http://nj.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pz.nszjky.cn

PHP:  array_unique($arr);
来源：http://vz.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://fj.nszjky.cn

TS:   [...new Set(arr)]
来源：http://vf.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xi.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ns.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://gk.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://up.lnxyls.cn

[D16] 求和与平均值
来源：http://zy.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dw.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zx.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wt.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nc.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://li.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://go.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ls.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://mf.panjiajie.cn

[D17] 最大值与最小值
来源：http://ci.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ok.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://pc.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qb.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://ds.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wn.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lk.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ys.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://pj.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://ax.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dz.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://fm.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://la.haigaiapp.cn

TS:   nested.flat();
来源：http://hl.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ac.wgjwhj.cn

Go:   // 手写双层循环
来源：http://va.9csxet.cn

Ruby: nested.flatten
来源：http://mb.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iu.hnjuh.cn

[D19] 按字段分组
来源：http://yq.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bm.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zq.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lp.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://de.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://an.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://uq.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rs.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oh.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://cw.gzmigu.cn

Py:   Counter(arr)
来源：http://dx.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://ui.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kp.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pd.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tq.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://tk.muxihuayi.cn

Ruby: arr.tally
来源：http://zb.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://te.huanxung.cn

[D21] 判断是否包含某元素
来源：http://sq.shxzukj.cn

Py:   x in arr
来源：http://qw.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://eq.hnjuh.cn

JS:   arr.includes(x)
来源：http://se.szxytkj.cn

TS:   arr.includes(x)
来源：http://je.hnjuh.cn

Java: list.contains(x)
来源：http://oq.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://af.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://zu.jctech888.com.cn

C#:   list.Contains(x)
来源：http://gp.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://om.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zy.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oo.huixiangedu.cn

TS:   [...arr];
来源：http://qn.hahajie.cn

Java: new ArrayList<>(list);
来源：http://au.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xo.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.newstarts.cn

C#:   new List<int>(list);
来源：http://rj.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ui.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ym.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ta.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ik.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://it.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hy.muxihuayi.cn

Go:   // 手写循环
来源：http://tr.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ff.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fp.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://uo.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wa.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ky.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mh.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ne.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gj.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pr.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://br.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iy.521024.cn

[D25] Set 集合去重与交并差
来源：http://ph.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ht.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vr.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ul.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fl.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xg.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tc.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tm.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ii.hahajie.cn

[D26] 数组转字符串
来源：http://lz.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://rj.colortex.cn

PHP:  implode(", ", $arr);
来源：http://hb.huanxung.cn

JS:   arr.join(", ")
来源：http://pd.yuexingan06.cn

TS:   arr.join(", ")
来源：http://fi.shxzukj.cn

Java: String.join(", ", list)
来源：http://kd.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://br.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://cl.9csxet.cn

C#:   string.Join(", ", list)
来源：http://wl.szxytkj.cn

================================================================================
来源：http://un.521024.cn

E. 字符串处理
来源：http://dq.bjjhwx.cn

================================================================================
来源：http://sx.jctech888.com.cn

[E01] 拼接字符串
来源：http://of.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rp.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yj.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qg.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hp.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uv.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hd.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lh.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vt.gzmigu.cn

[E02] 重复字符串
来源：http://ru.huixiangedu.cn

Py:   "ab" * 3
来源：http://tp.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://ce.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://oe.asd995.cn

TS:   "ab".repeat(3)
来源：http://ae.szxytkj.cn

Java: "ab".repeat(3)
来源：http://lt.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://qv.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://as.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fh.huixinmuqiang.cn

[E03] 截取子串
来源：http://yf.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ly.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lo.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ig.521024.cn

TS:   s.slice(1, 4)
来源：http://oh.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://yu.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vb.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sv.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://gy.colortex.cn

[E04] 查找子串位置
来源：http://wq.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://mb.nszjky.cn

PHP:  strpos($s, "x");
来源：http://fj.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qw.colortex.cn

TS:   s.indexOf("x")
来源：http://ar.huixiangedu.cn

Java: s.indexOf("x")
来源：http://vv.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://kk.newstarts.cn

Ruby: s.index("x")
来源：http://et.nszjky.cn

C#:   s.IndexOf("x")
来源：http://cq.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wg.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://no.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hn.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uk.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ug.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://je.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kv.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cw.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gt.shxzskj.cn

[E06] 替换子串
来源：http://mk.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fs.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://qr.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ui.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://yh.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mc.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://he.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kj.521024.cn

C#:   s.Replace("a", "b")
来源：http://nk.szxytkj.cn

[E07] 按分隔符拆分
来源：http://wz.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dn.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xz.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rg.yuntaijiaju.cn

TS:   s.split(",")
来源：http://oy.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pe.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sv.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://lz.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qg.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ln.shtwfgs.cn

Py:   ",".join(items)
来源：http://gx.haigaiapp.cn


<!-- 参考信息 -->