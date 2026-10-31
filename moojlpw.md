代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://bs.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://ns.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tp.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bb.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://wo.jianghongdianzi.cn

[D04] 删除元素
来源：http://oe.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://do.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xk.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eb.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://el.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://md.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wp.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://va.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://la.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://xa.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sv.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yf.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wm.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://di.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dq.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://vs.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://op.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iz.521024.cn

[D06] 数组长度
来源：http://oe.szsharing.cn

Py:   len(arr)
来源：http://eb.bjjhwx.cn

PHP:  count($arr);
来源：http://ky.nicolike.cn

JS:   arr.length
来源：http://zv.yuexingan06.cn

TS:   arr.length
来源：http://na.gzmigu.cn

Java: list.size();
来源：http://os.yuexingan06.cn

Go:   len(arr)
来源：http://qq.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://kd.newstarts.cn

C#:   list.Count;
来源：http://wc.9csxet.cn

[D07] 切片 / 取子数组
来源：http://qb.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ey.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ml.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://bn.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://zq.shxzskj.cn

Java: list.subList(1, 4);
来源：http://pz.szsharing.cn

Go:   arr[1:4]
来源：http://bs.szxytkj.cn

Ruby: arr[1, 3]
来源：http://fe.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ad.szsharing.cn

[D08] 合并两个数组
来源：http://te.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://nk.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://cs.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://no.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://gy.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://od.bjjhwx.cn

Go:   append(a, b...)
来源：http://qy.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://vr.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://na.jctech888.com.cn

[D09] 排序（升序）
来源：http://se.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zz.huanxung.cn

PHP:  sort($arr);
来源：http://vh.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fk.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fb.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fy.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lx.huixiangedu.cn

Ruby: arr.sort
来源：http://it.yuexingan06.cn

C#:   list.Sort();
来源：http://si.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mp.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ng.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sl.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zt.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ep.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yl.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uu.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qq.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mo.hahajie.cn

[D11] 反转数组
来源：http://et.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rg.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://sk.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uh.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://oj.szxytkj.cn

Java: Collections.reverse(list);
来源：http://cg.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://mx.huixiangedu.cn

Ruby: arr.reverse
来源：http://ob.bookmarksfly.cn

C#:   list.Reverse();
来源：http://ae.panjiajie.cn

[D12] 查找元素下标
来源：http://yo.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://hp.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://py.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mc.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hg.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ep.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://vz.panjiajie.cn

Ruby: arr.index(x)
来源：http://bo.szsharing.cn

C#:   list.IndexOf(x);
来源：http://js.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ua.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yr.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cc.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://fe.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://kh.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mi.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zr.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lm.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yo.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://zm.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oo.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vn.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://bd.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://cm.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rd.hahajie.cn

Go:   // 手写循环
来源：http://we.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cm.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zy.hnjuh.cn

[D15] 去重
来源：http://ie.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ga.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://oz.9csxet.cn

JS:   [...new Set(arr)]
来源：http://up.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ng.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://px.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hu.haigaiapp.cn

Ruby: arr.uniq
来源：http://ev.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://gh.bjjhwx.cn

[D16] 求和与平均值
来源：http://gk.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ng.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dg.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fp.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yi.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fb.shxzukj.cn

Go:   // 手写循环累加
来源：http://ak.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yr.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://ax.hahajie.cn

[D17] 最大值与最小值
来源：http://us.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://hh.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://fx.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zj.9csxet.cn

TS:   Math.max(...arr);
来源：http://oo.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dn.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zo.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://dr.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://ba.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://xa.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ie.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://qp.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mm.newstarts.cn

TS:   nested.flat();
来源：http://an.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zi.jctech888.com.cn

Go:   // 手写双层循环
来源：http://oe.bjjhwx.cn

Ruby: nested.flatten
来源：http://ni.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mo.gzmigu.cn

[D19] 按字段分组
来源：http://if.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kp.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wk.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nz.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ie.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://nz.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ll.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yc.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://pw.hahajie.cn

Py:   Counter(arr)
来源：http://gn.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ti.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fp.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vh.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pr.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://uh.shtwfgs.cn

Ruby: arr.tally
来源：http://mz.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yv.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://rf.shxzukj.cn

Py:   x in arr
来源：http://sk.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://pl.nicolike.cn

JS:   arr.includes(x)
来源：http://bp.shxzskj.cn

TS:   arr.includes(x)
来源：http://jo.szxytkj.cn

Java: list.contains(x)
来源：http://kn.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://bi.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://ca.newstarts.cn

C#:   list.Contains(x)
来源：http://or.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://wb.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cr.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://br.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bz.9csxet.cn

TS:   [...arr];
来源：http://rq.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://sn.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xu.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://ru.shxzukj.cn

C#:   new List<int>(list);
来源：http://aj.hnjuh.cn

[D23] reduce 累积计算
来源：http://bt.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gi.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iv.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lw.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yk.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dw.wgjwhj.cn

Go:   // 手写循环
来源：http://ds.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://io.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ww.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://ma.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tt.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gr.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xm.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lc.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xz.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yb.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xx.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rv.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://wn.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oc.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pk.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://me.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gk.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xn.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xa.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dl.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wx.lnxyls.cn

[D26] 数组转字符串
来源：http://bs.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://ji.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://qn.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://un.521024.cn

TS:   arr.join(", ")
来源：http://kc.asd995.cn

Java: String.join(", ", list)
来源：http://vn.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://dk.colortex.cn

Ruby: arr.join(", ")
来源：http://nw.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://fy.521024.cn

================================================================================
来源：http://xh.newstarts.cn

E. 字符串处理
来源：http://ys.shtwfgs.cn

================================================================================
来源：http://xr.shxzskj.cn

[E01] 拼接字符串
来源：http://iu.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://au.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gg.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jf.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kh.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gw.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qo.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://af.bjjhwx.cn

[E02] 重复字符串
来源：http://ek.yuexingan06.cn

Py:   "ab" * 3
来源：http://ym.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://vp.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://hg.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ii.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://jb.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://co.shtwfgs.cn

Ruby: "ab" * 3
来源：http://fm.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lx.9csxet.cn

[E03] 截取子串
来源：http://di.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fk.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qe.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ks.colortex.cn

TS:   s.slice(1, 4)
来源：http://wx.panjiajie.cn

Java: s.substring(1, 4)
来源：http://lt.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rt.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://py.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://mx.jctech888.com.cn

[E04] 查找子串位置
来源：http://gj.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://qi.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://hv.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xn.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://tz.bjjhwx.cn

Java: s.indexOf("x")
来源：http://yx.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://uu.newstarts.cn

Ruby: s.index("x")
来源：http://yk.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://rj.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pw.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vx.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qr.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wr.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ne.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lq.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ka.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bh.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vj.asd995.cn

[E06] 替换子串
来源：http://rm.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://me.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://es.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://vx.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://to.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bf.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jo.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://so.9csxet.cn

[E07] 按分隔符拆分
来源：http://hi.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gm.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yp.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cr.chemitech.net.cn

TS:   s.split(",")
来源：http://ge.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tk.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lb.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://fp.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bk.nicolike.cn

[E08] 数组按分隔符合并
来源：http://dl.shxzukj.cn

Py:   ",".join(items)
来源：http://uh.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://vg.huixinmuqiang.cn

JS:   items.join(",")
来源：http://yq.jianghongdianzi.cn

TS:   items.join(",")
来源：http://kw.chemitech.net.cn

Java: String.join(",", items)
来源：http://fr.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://gc.colortex.cn

Ruby: items.join(",")
来源：http://gp.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://sb.9csxet.cn

[E09] 去除所有空白字符
来源：http://hf.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ao.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ff.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://rl.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://wh.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://qz.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yt.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nb.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ch.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://ch.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eb.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zq.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://am.bjjhwx.cn


<!-- 参考信息 -->