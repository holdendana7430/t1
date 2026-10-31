代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://wv.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ni.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bm.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bt.521024.cn

C#:   list.Insert(0, 0);
来源：http://sr.szxytkj.cn

[D04] 删除元素
来源：http://rv.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ry.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ov.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://po.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://sw.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ti.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qp.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vk.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mt.panjiajie.cn

[D05] 访问与修改元素
来源：http://qt.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ss.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qr.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lz.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://nm.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ff.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://rj.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fn.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yl.9csxet.cn

[D06] 数组长度
来源：http://ty.colortex.cn

Py:   len(arr)
来源：http://ph.gzmigu.cn

PHP:  count($arr);
来源：http://yn.newstarts.cn

JS:   arr.length
来源：http://ym.huixinmuqiang.cn

TS:   arr.length
来源：http://yi.wgjwhj.cn

Java: list.size();
来源：http://vw.asd995.cn

Go:   len(arr)
来源：http://yp.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ak.hnjuh.cn

C#:   list.Count;
来源：http://hb.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://lr.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ny.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bl.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://ba.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://jq.asd995.cn

Java: list.subList(1, 4);
来源：http://aw.hnjuh.cn

Go:   arr[1:4]
来源：http://bl.521024.cn

Ruby: arr[1, 3]
来源：http://gg.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://fx.lnxyls.cn

[D08] 合并两个数组
来源：http://on.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://vl.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://jd.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wc.panjiajie.cn

TS:   [...a, ...b];
来源：http://md.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gk.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ml.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://pm.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://ny.shtwfgs.cn

[D09] 排序（升序）
来源：http://dy.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ac.bookmarksfly.cn

PHP:  sort($arr);
来源：http://gi.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ef.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yb.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://td.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ey.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ub.szxytkj.cn

C#:   list.Sort();
来源：http://zw.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iz.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qe.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://me.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qr.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wf.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sa.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vm.szxytkj.cn

[D11] 反转数组
来源：http://ij.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dq.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://mm.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jk.nicolike.cn

TS:   [...arr].reverse();
来源：http://jh.szxytkj.cn

Java: Collections.reverse(list);
来源：http://ng.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://xl.huanxung.cn

Ruby: arr.reverse
来源：http://nv.newstarts.cn

C#:   list.Reverse();
来源：http://yy.jctech888.com.cn

[D12] 查找元素下标
来源：http://fq.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ht.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fw.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sk.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mc.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dm.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://op.nszjky.cn

Ruby: arr.index(x)
来源：http://as.asd995.cn

C#:   list.IndexOf(x);
来源：http://ui.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://zo.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zw.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qp.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://fq.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ub.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ir.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lg.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nr.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cv.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://mc.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zs.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kg.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://cr.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://fp.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xb.9csxet.cn

Go:   // 手写循环
来源：http://ek.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hx.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ho.huanxung.cn

[D15] 去重
来源：http://sm.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gl.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://sy.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://qo.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://wm.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jx.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vk.szsharing.cn

Ruby: arr.uniq
来源：http://ev.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://ki.jctech888.com.cn

[D16] 求和与平均值
来源：http://pd.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ug.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ft.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yb.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rp.shxzskj.cn

Go:   // 手写循环累加
来源：http://cf.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://do.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://bl.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://az.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://qx.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://sn.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.huanxung.cn

TS:   Math.max(...arr);
来源：http://fz.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qo.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://io.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://rz.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://bu.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://zy.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xd.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://pp.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eh.huanxung.cn

TS:   nested.flat();
来源：http://ci.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hy.muxihuayi.cn

Go:   // 手写双层循环
来源：http://dn.asd995.cn

Ruby: nested.flatten
来源：http://ig.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ae.gzmigu.cn

[D19] 按字段分组
来源：http://kc.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gc.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ys.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sk.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jw.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qh.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://vh.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://az.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dv.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ne.nszjky.cn

Py:   Counter(arr)
来源：http://gn.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://zp.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ba.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fv.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oj.colortex.cn

Go:   // 手写 map[T]int
来源：http://gv.hahajie.cn

Ruby: arr.tally
来源：http://pd.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vy.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://ol.jianghongdianzi.cn

Py:   x in arr
来源：http://zs.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://jq.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ru.9csxet.cn

TS:   arr.includes(x)
来源：http://yu.szsharing.cn

Java: list.contains(x)
来源：http://tl.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://od.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://uw.jctech888.com.cn

C#:   list.Contains(x)
来源：http://kt.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://db.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://su.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fp.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mj.gzmigu.cn

TS:   [...arr];
来源：http://eh.nicolike.cn

Java: new ArrayList<>(list);
来源：http://ho.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qv.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://vq.shxzukj.cn

C#:   new List<int>(list);
来源：http://bv.shxzukj.cn

[D23] reduce 累积计算
来源：http://gp.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://er.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qg.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://al.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sd.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ej.szsharing.cn

Go:   // 手写循环
来源：http://ff.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cf.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ti.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://hs.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vp.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ga.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cf.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zk.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kv.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yg.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ke.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gx.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://hf.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rf.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://em.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mg.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pk.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zm.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yd.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mj.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yz.521024.cn

[D26] 数组转字符串
来源：http://xm.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ea.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://uc.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://dh.colortex.cn

TS:   arr.join(", ")
来源：http://rh.jctech888.com.cn

Java: String.join(", ", list)
来源：http://sp.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://ui.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://xp.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://vj.9csxet.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

E. 字符串处理
来源：http://sj.9csxet.cn

================================================================================
来源：http://tu.nszjky.cn

[E01] 拼接字符串
来源：http://np.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cy.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dh.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nl.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ym.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://md.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://go.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yg.asd995.cn

[E02] 重复字符串
来源：http://id.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://tq.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://dc.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://hm.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://zr.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://oo.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://tt.chemitech.net.cn

Ruby: "ab" * 3
来源：http://ta.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aj.nicolike.cn

[E03] 截取子串
来源：http://fw.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rg.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wt.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jz.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://ar.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://ll.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kl.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xz.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://zx.huanxung.cn

[E04] 查找子串位置
来源：http://xn.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://az.521024.cn

PHP:  strpos($s, "x");
来源：http://rn.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yi.szxytkj.cn

TS:   s.indexOf("x")
来源：http://wy.szxytkj.cn

Java: s.indexOf("x")
来源：http://tc.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://jt.hnjuh.cn

Ruby: s.index("x")
来源：http://rc.521024.cn

C#:   s.IndexOf("x")
来源：http://ft.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tb.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ac.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rr.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rr.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cu.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tg.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sb.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ap.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pe.nicolike.cn

[E06] 替换子串
来源：http://lg.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nj.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ja.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sc.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://im.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ys.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gg.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hw.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://yx.shxzukj.cn

[E07] 按分隔符拆分
来源：http://uq.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cf.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://op.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uj.newstarts.cn

TS:   s.split(",")
来源：http://wy.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xo.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tf.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://hv.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jo.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://sq.haigaiapp.cn

Py:   ",".join(items)
来源：http://eu.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ut.chemitech.net.cn

JS:   items.join(",")
来源：http://sx.huixinmuqiang.cn

TS:   items.join(",")
来源：http://eo.muxihuayi.cn

Java: String.join(",", items)
来源：http://pt.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://lr.9csxet.cn

Ruby: items.join(",")
来源：http://pc.521024.cn

C#:   string.Join(",", items)
来源：http://jn.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://he.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pm.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ta.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://gy.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://fp.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://pq.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hw.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xi.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kk.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://ku.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sv.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tb.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://vx.huixinmuqiang.cn


<!-- 参考信息 -->