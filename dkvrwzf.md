代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://si.nicolike.cn

Java: list.add(0, 0);
来源：http://yk.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bb.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ta.colortex.cn

C#:   list.Insert(0, 0);
来源：http://bz.szsharing.cn

[D04] 删除元素
来源：http://ry.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bn.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nq.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xy.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://kb.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mn.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uj.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xc.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jl.nszjky.cn

[D05] 访问与修改元素
来源：http://xm.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yy.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://as.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://im.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ot.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://in.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://eo.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zv.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rf.521024.cn

[D06] 数组长度
来源：http://im.colortex.cn

Py:   len(arr)
来源：http://nq.szxytkj.cn

PHP:  count($arr);
来源：http://om.bjjhwx.cn

JS:   arr.length
来源：http://xa.wgjwhj.cn

TS:   arr.length
来源：http://fx.nszjky.cn

Java: list.size();
来源：http://fp.newstarts.cn

Go:   len(arr)
来源：http://yf.nicolike.cn

Ruby: arr.length; arr.size
来源：http://re.shtwfgs.cn

C#:   list.Count;
来源：http://hn.huanxung.cn

[D07] 切片 / 取子数组
来源：http://sr.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wz.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tx.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ms.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://do.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://kk.newstarts.cn

Go:   arr[1:4]
来源：http://hu.hnjuh.cn

Ruby: arr[1, 3]
来源：http://kl.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://js.shxzskj.cn

[D08] 合并两个数组
来源：http://nq.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://hx.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://zi.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uo.wgjwhj.cn

TS:   [...a, ...b];
来源：http://vp.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ti.gzmigu.cn

Go:   append(a, b...)
来源：http://zi.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://qm.521024.cn

C#:   a.Concat(b).ToList()
来源：http://fz.nicolike.cn

[D09] 排序（升序）
来源：http://cw.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://xt.521024.cn

PHP:  sort($arr);
来源：http://rd.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kp.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nt.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://on.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ba.nszjky.cn

Ruby: arr.sort
来源：http://hr.haigaiapp.cn

C#:   list.Sort();
来源：http://pz.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rz.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tl.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ex.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ml.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mu.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ta.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pl.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ij.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://az.panjiajie.cn

[D11] 反转数组
来源：http://dc.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sw.nicolike.cn

PHP:  array_reverse($arr);
来源：http://yl.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://el.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://hf.szsharing.cn

Java: Collections.reverse(list);
来源：http://qk.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://wq.muxihuayi.cn

Ruby: arr.reverse
来源：http://vt.shxzskj.cn

C#:   list.Reverse();
来源：http://fp.bookmarksfly.cn

[D12] 查找元素下标
来源：http://qp.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://ej.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uw.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yj.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nm.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tv.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://yb.nicolike.cn

Ruby: arr.index(x)
来源：http://dr.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ic.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://vk.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ej.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wv.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://nx.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://iy.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mc.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pv.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ka.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zp.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://lk.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wz.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eh.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://ly.521024.cn

TS:   arr.map(x => x * 2)
来源：http://pq.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://si.jctech888.com.cn

Go:   // 手写循环
来源：http://qv.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bi.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://li.shxzskj.cn

[D15] 去重
来源：http://dw.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ep.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://qs.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://hc.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://bv.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wl.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sd.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://nb.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://qm.shxzukj.cn

[D16] 求和与平均值
来源：http://pe.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cz.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xm.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rq.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qw.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cy.521024.cn

Go:   // 手写循环累加
来源：http://kv.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vp.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://va.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ys.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://hu.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://mj.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ee.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://iu.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bm.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fk.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://qp.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://rf.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ko.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pg.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://ee.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vj.muxihuayi.cn

TS:   nested.flat();
来源：http://gr.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qf.nicolike.cn

Go:   // 手写双层循环
来源：http://tc.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://wa.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zu.bjjhwx.cn

[D19] 按字段分组
来源：http://au.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dm.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yd.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dz.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jh.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://al.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://fs.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yk.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vp.521024.cn

[D20] 统计每个元素出现次数
来源：http://sd.muxihuayi.cn

Py:   Counter(arr)
来源：http://wp.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://xz.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wc.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ra.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zb.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://io.szxytkj.cn

Ruby: arr.tally
来源：http://ol.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://za.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://sy.nicolike.cn

Py:   x in arr
来源：http://oi.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://zu.shtwfgs.cn

JS:   arr.includes(x)
来源：http://ez.lnxyls.cn

TS:   arr.includes(x)
来源：http://dp.shxzukj.cn

Java: list.contains(x)
来源：http://mj.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://uc.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://kq.haigaiapp.cn

C#:   list.Contains(x)
来源：http://ii.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://xj.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jx.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ka.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://id.yuexingan06.cn

TS:   [...arr];
来源：http://eb.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://wk.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yp.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://rp.nicolike.cn

C#:   new List<int>(list);
来源：http://vu.szsharing.cn

[D23] reduce 累积计算
来源：http://gr.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tn.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ig.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pk.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cl.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qg.lnxyls.cn

Go:   // 手写循环
来源：http://rc.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uc.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://df.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://jt.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bs.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cr.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zm.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nc.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vb.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://or.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ac.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vs.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://gm.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xp.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mu.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://az.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mm.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zq.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mm.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ck.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qx.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://hu.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://ck.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://vq.shxzukj.cn

JS:   arr.join(", ")
来源：http://hl.wgjwhj.cn

TS:   arr.join(", ")
来源：http://yt.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hc.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bd.panjiajie.cn

Ruby: arr.join(", ")
来源：http://ms.huanxung.cn

C#:   string.Join(", ", list)
来源：http://bp.szsharing.cn

================================================================================
来源：http://vy.newstarts.cn

E. 字符串处理
来源：http://bn.szxytkj.cn

================================================================================
来源：http://ea.jctech888.com.cn

[E01] 拼接字符串
来源：http://rx.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sb.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ae.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pp.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gf.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hq.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yh.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://va.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ic.hnjuh.cn

[E02] 重复字符串
来源：http://ak.hahajie.cn

Py:   "ab" * 3
来源：http://pp.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://so.nicolike.cn

JS:   "ab".repeat(3)
来源：http://aq.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://sr.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://dl.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://jr.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://lx.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wg.gzmigu.cn

[E03] 截取子串
来源：http://cl.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gk.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aj.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xf.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://xt.9csxet.cn

Java: s.substring(1, 4)
来源：http://ee.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hg.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sj.521024.cn

C#:   s.Substring(1, 3)
来源：http://xk.szsharing.cn

[E04] 查找子串位置
来源：http://yt.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://xj.newstarts.cn

PHP:  strpos($s, "x");
来源：http://kb.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ss.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://fl.nicolike.cn

Java: s.indexOf("x")
来源：http://pq.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://ej.jctech888.com.cn

Ruby: s.index("x")
来源：http://xg.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://fb.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kv.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://me.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bj.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wo.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qy.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zr.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://le.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jc.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ak.colortex.cn

[E06] 替换子串
来源：http://pz.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dd.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://pi.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gd.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://es.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qx.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dp.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yz.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://bs.huanxung.cn

[E07] 按分隔符拆分
来源：http://zj.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zi.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kv.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rr.gzmigu.cn

TS:   s.split(",")
来源：http://wj.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rk.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gu.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://cz.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sy.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ox.huanxung.cn

Py:   ",".join(items)
来源：http://gs.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://xj.yuexingan06.cn

JS:   items.join(",")
来源：http://ab.newstarts.cn

TS:   items.join(",")
来源：http://qk.asd995.cn

Java: String.join(",", items)
来源：http://ac.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://py.gzmigu.cn

Ruby: items.join(",")
来源：http://eh.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://pu.lnxyls.cn

[E09] 去除所有空白字符
来源：http://uf.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mc.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vi.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://ov.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://dq.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://yu.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ca.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gd.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wv.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://tx.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bv.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dn.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://uu.wgjwhj.cn


<!-- 参考信息 -->