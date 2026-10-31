代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://te.nszjky.cn

Java: list.add(0, 0);
来源：http://vw.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://di.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rq.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://qi.nszjky.cn

[D04] 删除元素
来源：http://vt.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ra.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ku.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qp.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://qm.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lt.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jo.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mn.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gz.shtwfgs.cn

[D05] 访问与修改元素
来源：http://uj.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yh.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dx.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sz.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ze.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ag.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://dj.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dj.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ht.newstarts.cn

[D06] 数组长度
来源：http://va.shtwfgs.cn

Py:   len(arr)
来源：http://kc.haigaiapp.cn

PHP:  count($arr);
来源：http://pi.bookmarksfly.cn

JS:   arr.length
来源：http://rq.bookmarksfly.cn

TS:   arr.length
来源：http://go.shxzskj.cn

Java: list.size();
来源：http://no.newstarts.cn

Go:   len(arr)
来源：http://qw.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ze.yuexingan06.cn

C#:   list.Count;
来源：http://be.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://jh.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hd.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jn.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://kg.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://fv.521024.cn

Java: list.subList(1, 4);
来源：http://ef.shxzskj.cn

Go:   arr[1:4]
来源：http://wz.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://hj.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://aq.szsharing.cn

[D08] 合并两个数组
来源：http://mq.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://pg.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://pn.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yi.newstarts.cn

TS:   [...a, ...b];
来源：http://oa.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nq.lnxyls.cn

Go:   append(a, b...)
来源：http://if.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://fe.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://wm.colortex.cn

[D09] 排序（升序）
来源：http://db.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://nt.shxzskj.cn

PHP:  sort($arr);
来源：http://as.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rn.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fz.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://io.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nc.gzmigu.cn

Ruby: arr.sort
来源：http://hp.szsharing.cn

C#:   list.Sort();
来源：http://dw.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ge.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cm.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zl.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sr.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://be.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ah.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://es.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kb.gzmigu.cn

[D11] 反转数组
来源：http://eb.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dv.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://qc.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kq.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://qy.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://rh.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://dq.jctech888.com.cn

Ruby: arr.reverse
来源：http://wb.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://eu.bjjhwx.cn

[D12] 查找元素下标
来源：http://ig.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://sa.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oj.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tf.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cg.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://zr.szxytkj.cn

Ruby: arr.index(x)
来源：http://nh.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://uw.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://ph.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ax.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uj.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://ey.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://hp.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kq.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hx.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yg.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ls.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bx.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mp.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://gx.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://ah.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wh.jctech888.com.cn

Go:   // 手写循环
来源：http://tk.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lb.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yg.muxihuayi.cn

[D15] 去重
来源：http://mw.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rs.9csxet.cn

PHP:  array_unique($arr);
来源：http://pe.hahajie.cn

JS:   [...new Set(arr)]
来源：http://wd.colortex.cn

TS:   [...new Set(arr)]
来源：http://df.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rk.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ss.colortex.cn

Ruby: arr.uniq
来源：http://ep.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://us.9csxet.cn

[D16] 求和与平均值
来源：http://ya.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bw.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vc.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ki.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://za.haigaiapp.cn

Go:   // 手写循环累加
来源：http://vq.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gj.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://ph.szxytkj.cn

[D17] 最大值与最小值
来源：http://fa.asd995.cn

Py:   max(arr);  min(arr)
来源：http://va.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://vg.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lk.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://kq.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gd.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yu.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://wm.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://ng.521024.cn

[D18] 扁平化嵌套数组
来源：http://ny.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zn.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://hp.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fm.huixinmuqiang.cn

TS:   nested.flat();
来源：http://lb.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://og.szsharing.cn

Go:   // 手写双层循环
来源：http://wc.colortex.cn

Ruby: nested.flatten
来源：http://as.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zb.yuntaijiaju.cn

[D19] 按字段分组
来源：http://yx.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://be.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://id.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://un.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uv.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ju.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://gf.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xb.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vn.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ao.hnjuh.cn

Py:   Counter(arr)
来源：http://yk.newstarts.cn

PHP:  array_count_values($arr);
来源：http://ip.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cp.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://al.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vi.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://co.wgjwhj.cn

Ruby: arr.tally
来源：http://sz.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gs.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://vj.yuntaijiaju.cn

Py:   x in arr
来源：http://hb.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://nv.yuexingan06.cn

JS:   arr.includes(x)
来源：http://ar.hnjuh.cn

TS:   arr.includes(x)
来源：http://bb.newstarts.cn

Java: list.contains(x)
来源：http://wc.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://ih.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://gp.hahajie.cn

C#:   list.Contains(x)
来源：http://bf.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://lg.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vy.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wg.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://df.yuntaijiaju.cn

TS:   [...arr];
来源：http://eb.szsharing.cn

Java: new ArrayList<>(list);
来源：http://ik.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ww.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://um.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://qk.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://tz.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ar.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cp.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bw.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jp.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oo.jctech888.com.cn

Go:   // 手写循环
来源：http://vh.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qp.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jn.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://dq.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qc.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iy.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://es.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dd.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ce.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xl.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wc.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ux.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://sv.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nf.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xa.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ya.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://af.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cj.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pa.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nv.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rn.jctech888.com.cn

[D26] 数组转字符串
来源：http://fp.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://kl.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://sm.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://rb.hnjuh.cn

TS:   arr.join(", ")
来源：http://ch.nszjky.cn

Java: String.join(", ", list)
来源：http://qt.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://zz.colortex.cn

Ruby: arr.join(", ")
来源：http://lb.hahajie.cn

C#:   string.Join(", ", list)
来源：http://ld.haigaiapp.cn

================================================================================
来源：http://kd.hahajie.cn

E. 字符串处理
来源：http://jc.huixinmuqiang.cn

================================================================================
来源：http://ge.521024.cn

[E01] 拼接字符串
来源：http://js.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zb.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uq.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jx.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ic.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ht.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lt.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wj.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lt.yuexingan06.cn

[E02] 重复字符串
来源：http://di.muxihuayi.cn

Py:   "ab" * 3
来源：http://of.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://mx.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://dq.asd995.cn

TS:   "ab".repeat(3)
来源：http://kk.colortex.cn

Java: "ab".repeat(3)
来源：http://cw.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://db.hahajie.cn

Ruby: "ab" * 3
来源：http://nf.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gt.muxihuayi.cn

[E03] 截取子串
来源：http://jf.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uz.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bf.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ev.9csxet.cn

TS:   s.slice(1, 4)
来源：http://uw.hnjuh.cn

Java: s.substring(1, 4)
来源：http://ac.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xz.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tb.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://hb.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://fe.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://iy.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://gg.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pv.9csxet.cn

TS:   s.indexOf("x")
来源：http://cp.szsharing.cn

Java: s.indexOf("x")
来源：http://bd.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://fc.hahajie.cn

Ruby: s.index("x")
来源：http://gv.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://iq.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ji.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ua.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://to.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dr.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ly.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tn.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tc.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ez.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ts.hahajie.cn

[E06] 替换子串
来源：http://dm.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nn.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://zg.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://sv.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jw.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tr.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gm.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://vg.nszjky.cn

[E07] 按分隔符拆分
来源：http://ob.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://za.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ao.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ey.nicolike.cn

TS:   s.split(",")
来源：http://ju.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rn.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zg.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://be.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fx.nicolike.cn

[E08] 数组按分隔符合并
来源：http://jh.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://hy.colortex.cn

PHP:  implode(",", $items);
来源：http://fl.asd995.cn

JS:   items.join(",")
来源：http://nq.jianghongdianzi.cn

TS:   items.join(",")
来源：http://oi.haigaiapp.cn

Java: String.join(",", items)
来源：http://bq.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://rj.shxzskj.cn

Ruby: items.join(",")
来源：http://hg.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://tt.shxzskj.cn

[E09] 去除所有空白字符
来源：http://br.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bq.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wy.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://cy.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fr.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://bm.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uf.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ru.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ck.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://ke.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xl.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://in.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://vr.szsharing.cn


<!-- 参考信息 -->