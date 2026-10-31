代发 wailian999

C#:   list.Insert(0, 0);
来源：http://kr.wgjwhj.cn

[D04] 删除元素
来源：http://gs.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bt.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xb.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ug.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://yl.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vf.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://js.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vr.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fd.jctech888.com.cn

[D05] 访问与修改元素
来源：http://rk.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yo.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ox.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://so.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ov.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://nk.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://gc.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://az.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vm.jctech888.com.cn

[D06] 数组长度
来源：http://kz.huixiangedu.cn

Py:   len(arr)
来源：http://oi.newstarts.cn

PHP:  count($arr);
来源：http://az.shtwfgs.cn

JS:   arr.length
来源：http://ty.lnxyls.cn

TS:   arr.length
来源：http://vb.newstarts.cn

Java: list.size();
来源：http://ud.bookmarksfly.cn

Go:   len(arr)
来源：http://bf.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://fg.szsharing.cn

C#:   list.Count;
来源：http://vc.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://ye.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xm.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zq.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://wj.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://un.hahajie.cn

Java: list.subList(1, 4);
来源：http://bv.bookmarksfly.cn

Go:   arr[1:4]
来源：http://wm.hnjuh.cn

Ruby: arr[1, 3]
来源：http://ra.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://xu.panjiajie.cn

[D08] 合并两个数组
来源：http://jb.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://kp.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://nv.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tc.chemitech.net.cn

TS:   [...a, ...b];
来源：http://al.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dz.colortex.cn

Go:   append(a, b...)
来源：http://ut.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://wl.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://wt.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://zk.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://zg.huanxung.cn

PHP:  sort($arr);
来源：http://bn.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ay.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zj.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vz.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uh.chemitech.net.cn

Ruby: arr.sort
来源：http://pl.muxihuayi.cn

C#:   list.Sort();
来源：http://dg.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ze.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wi.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ig.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gs.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rh.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pw.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fz.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zj.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gj.gzmigu.cn

[D11] 反转数组
来源：http://mi.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ib.szsharing.cn

PHP:  array_reverse($arr);
来源：http://al.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ow.szxytkj.cn

TS:   [...arr].reverse();
来源：http://rk.asd995.cn

Java: Collections.reverse(list);
来源：http://va.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://hv.lnxyls.cn

Ruby: arr.reverse
来源：http://lo.521024.cn

C#:   list.Reverse();
来源：http://on.haigaiapp.cn

[D12] 查找元素下标
来源：http://fq.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://rn.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gx.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://os.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zl.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://rx.asd995.cn

Ruby: arr.index(x)
来源：http://mb.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ik.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://lw.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uy.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gx.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://oe.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qj.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rk.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rb.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qz.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zs.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://fu.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pq.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://el.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://df.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://hg.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://so.521024.cn

Go:   // 手写循环
来源：http://qx.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kk.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nv.shtwfgs.cn

[D15] 去重
来源：http://af.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hd.gzmigu.cn

PHP:  array_unique($arr);
来源：http://db.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://as.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://la.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://la.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xt.szsharing.cn

Ruby: arr.uniq
来源：http://fi.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://de.shxzskj.cn

[D16] 求和与平均值
来源：http://pq.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gd.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://il.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tc.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nf.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hb.hahajie.cn

Go:   // 手写循环累加
来源：http://ci.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pd.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://nr.newstarts.cn

[D17] 最大值与最小值
来源：http://kf.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://uk.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://ak.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ur.hahajie.cn

TS:   Math.max(...arr);
来源：http://nu.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://im.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mc.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://tu.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ek.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://sa.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ig.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://xt.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wy.panjiajie.cn

TS:   nested.flat();
来源：http://sv.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jf.panjiajie.cn

Go:   // 手写双层循环
来源：http://yn.huanxung.cn

Ruby: nested.flatten
来源：http://kn.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bh.gzmigu.cn

[D19] 按字段分组
来源：http://ml.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ky.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hk.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wo.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gv.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bu.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://el.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bo.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nc.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://vq.shxzskj.cn

Py:   Counter(arr)
来源：http://tl.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://jn.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nj.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qf.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qj.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://zk.huanxung.cn

Ruby: arr.tally
来源：http://pm.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ml.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://eg.hahajie.cn

Py:   x in arr
来源：http://fy.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://zx.colortex.cn

JS:   arr.includes(x)
来源：http://fu.wgjwhj.cn

TS:   arr.includes(x)
来源：http://pa.muxihuayi.cn

Java: list.contains(x)
来源：http://pd.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://dt.nszjky.cn

Ruby: arr.include?(x)
来源：http://gi.jctech888.com.cn

C#:   list.Contains(x)
来源：http://sz.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ql.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xw.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tk.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bs.hnjuh.cn

TS:   [...arr];
来源：http://rm.hahajie.cn

Java: new ArrayList<>(list);
来源：http://vk.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gw.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://xb.gzmigu.cn

C#:   new List<int>(list);
来源：http://zk.newstarts.cn

[D23] reduce 累积计算
来源：http://mk.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yx.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://di.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ro.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vg.shxzskj.cn

Go:   // 手写循环
来源：http://gw.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tz.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ab.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://xv.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ou.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sm.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gr.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://di.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lh.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jq.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ie.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fw.colortex.cn

[D25] Set 集合去重与交并差
来源：http://nd.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gh.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ie.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fh.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cx.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uv.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nu.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ho.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yk.huixiangedu.cn

[D26] 数组转字符串
来源：http://ly.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ih.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://me.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://ss.shxzskj.cn

TS:   arr.join(", ")
来源：http://zw.nszjky.cn

Java: String.join(", ", list)
来源：http://xd.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://ps.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://hh.nszjky.cn

C#:   string.Join(", ", list)
来源：http://di.bjjhwx.cn

================================================================================
来源：http://xj.huixiangedu.cn

E. 字符串处理
来源：http://tq.nszjky.cn

================================================================================
来源：http://qz.yuexingan06.cn

[E01] 拼接字符串
来源：http://xi.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://by.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ep.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://df.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qc.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cu.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sv.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://do.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cf.szxytkj.cn

[E02] 重复字符串
来源：http://md.asd995.cn

Py:   "ab" * 3
来源：http://tz.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://fh.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://cn.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://sy.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://nx.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://kg.lnxyls.cn

Ruby: "ab" * 3
来源：http://ae.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mr.haigaiapp.cn

[E03] 截取子串
来源：http://ti.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sv.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fl.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sz.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://te.shxzskj.cn

Java: s.substring(1, 4)
来源：http://de.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ny.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://va.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ej.szsharing.cn

[E04] 查找子串位置
来源：http://la.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ts.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://zq.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ph.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://jf.huanxung.cn

Java: s.indexOf("x")
来源：http://gq.asd995.cn

Go:   strings.Index(s, "x")
来源：http://dy.9csxet.cn

Ruby: s.index("x")
来源：http://ww.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://ch.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fv.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vh.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yn.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://um.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cd.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ky.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mz.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://di.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://df.huixinmuqiang.cn

[E06] 替换子串
来源：http://zq.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ka.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://mg.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jl.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://as.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dm.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oi.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pc.521024.cn

C#:   s.Replace("a", "b")
来源：http://bf.gzmigu.cn

[E07] 按分隔符拆分
来源：http://iv.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ro.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tu.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pu.jianghongdianzi.cn

TS:   s.split(",")
来源：http://wx.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qy.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mk.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://iv.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ke.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://sw.wgjwhj.cn

Py:   ",".join(items)
来源：http://oh.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://rn.newstarts.cn

JS:   items.join(",")
来源：http://li.jianghongdianzi.cn

TS:   items.join(",")
来源：http://to.szsharing.cn

Java: String.join(",", items)
来源：http://xk.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://an.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://zl.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://gi.szxytkj.cn

[E09] 去除所有空白字符
来源：http://mm.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dv.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hn.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://nw.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://sk.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://mu.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fs.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hn.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://op.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://bm.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rc.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mp.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://cv.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ha.nicolike.cn

Java: String.format("%03d", 7)
来源：http://bx.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oy.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ie.huixinmuqiang.cn


<!-- 参考信息 -->