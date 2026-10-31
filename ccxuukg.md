代发 wailian999

C#:   list.Insert(0, 0);
来源：http://fm.huixiangedu.cn

[D04] 删除元素
来源：http://be.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rd.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rx.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tr.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://pd.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ru.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yy.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rh.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gz.shtwfgs.cn

[D05] 访问与修改元素
来源：http://kf.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lv.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hq.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://el.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://kt.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ia.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://uh.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vi.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dq.bookmarksfly.cn

[D06] 数组长度
来源：http://bt.haigaiapp.cn

Py:   len(arr)
来源：http://vx.9csxet.cn

PHP:  count($arr);
来源：http://nx.asd995.cn

JS:   arr.length
来源：http://oy.lnxyls.cn

TS:   arr.length
来源：http://oj.huanxung.cn

Java: list.size();
来源：http://eo.hahajie.cn

Go:   len(arr)
来源：http://me.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://xq.521024.cn

C#:   list.Count;
来源：http://yh.huanxung.cn

[D07] 切片 / 取子数组
来源：http://yt.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cn.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bc.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://xk.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://tp.newstarts.cn

Java: list.subList(1, 4);
来源：http://vd.shxzskj.cn

Go:   arr[1:4]
来源：http://ad.shxzukj.cn

Ruby: arr[1, 3]
来源：http://as.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://nh.9csxet.cn

[D08] 合并两个数组
来源：http://bh.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ql.asd995.cn

PHP:  array_merge($a, $b);
来源：http://oo.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://de.hahajie.cn

TS:   [...a, ...b];
来源：http://cm.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lh.bookmarksfly.cn

Go:   append(a, b...)
来源：http://no.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://jd.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://xy.hnjuh.cn

[D09] 排序（升序）
来源：http://ce.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://gs.bjjhwx.cn

PHP:  sort($arr);
来源：http://oh.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ak.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://md.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uv.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nz.nicolike.cn

Ruby: arr.sort
来源：http://eb.jianghongdianzi.cn

C#:   list.Sort();
来源：http://da.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xr.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fe.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ge.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gb.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://no.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://go.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qj.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://li.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lw.wgjwhj.cn

[D11] 反转数组
来源：http://eu.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://be.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://dn.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zz.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ks.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://hr.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://ck.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://tc.haigaiapp.cn

C#:   list.Reverse();
来源：http://vu.521024.cn

[D12] 查找元素下标
来源：http://io.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ax.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zt.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dc.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://di.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dr.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://sc.nicolike.cn

Ruby: arr.index(x)
来源：http://dz.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://yk.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://zs.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qi.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ui.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://vd.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://wo.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kr.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nv.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://le.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tb.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://sr.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tu.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pz.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://ro.521024.cn

TS:   arr.map(x => x * 2)
来源：http://he.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ms.szxytkj.cn

Go:   // 手写循环
来源：http://vm.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://us.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sm.muxihuayi.cn

[D15] 去重
来源：http://tw.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tq.szsharing.cn

PHP:  array_unique($arr);
来源：http://fj.9csxet.cn

JS:   [...new Set(arr)]
来源：http://io.nszjky.cn

TS:   [...new Set(arr)]
来源：http://fq.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cd.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ee.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://oc.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://bb.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://tj.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gv.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://il.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://id.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yx.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ml.haigaiapp.cn

Go:   // 手写循环累加
来源：http://qh.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ut.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://dz.shxzskj.cn

[D17] 最大值与最小值
来源：http://oh.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://jr.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ry.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://un.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://ka.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kw.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ns.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://pi.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://xm.colortex.cn

[D18] 扁平化嵌套数组
来源：http://kn.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://um.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://og.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://my.hnjuh.cn

TS:   nested.flat();
来源：http://ag.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yt.huixiangedu.cn

Go:   // 手写双层循环
来源：http://tg.shtwfgs.cn

Ruby: nested.flatten
来源：http://qc.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zy.wgjwhj.cn

[D19] 按字段分组
来源：http://as.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rs.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vh.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://na.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qb.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nk.colortex.cn

Go:   // 手写 map[string][]T
来源：http://mz.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hr.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vh.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://rk.shtwfgs.cn

Py:   Counter(arr)
来源：http://zs.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://kk.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lt.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ow.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eh.asd995.cn

Go:   // 手写 map[T]int
来源：http://jz.521024.cn

Ruby: arr.tally
来源：http://mp.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vz.nszjky.cn

[D21] 判断是否包含某元素
来源：http://rc.nszjky.cn

Py:   x in arr
来源：http://cc.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://lj.hahajie.cn

JS:   arr.includes(x)
来源：http://sc.panjiajie.cn

TS:   arr.includes(x)
来源：http://on.huixinmuqiang.cn

Java: list.contains(x)
来源：http://nx.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://ev.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://xn.panjiajie.cn

C#:   list.Contains(x)
来源：http://ff.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://vs.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wh.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kj.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yl.yuntaijiaju.cn

TS:   [...arr];
来源：http://em.asd995.cn

Java: new ArrayList<>(list);
来源：http://rp.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mc.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://rt.wgjwhj.cn

C#:   new List<int>(list);
来源：http://yc.521024.cn

[D23] reduce 累积计算
来源：http://zq.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dw.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hx.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tz.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kw.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zt.hahajie.cn

Go:   // 手写循环
来源：http://ee.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://py.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vq.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://yn.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xw.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bt.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jg.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bg.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ol.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ek.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eu.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vb.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://hx.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nr.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xs.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://av.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qa.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ue.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mu.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://an.nszjky.cn

[D26] 数组转字符串
来源：http://vu.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://mx.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://gq.szxytkj.cn

JS:   arr.join(", ")
来源：http://fj.shxzskj.cn

TS:   arr.join(", ")
来源：http://xx.newstarts.cn

Java: String.join(", ", list)
来源：http://ae.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://mt.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://ml.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://bf.yuexingan06.cn

================================================================================
来源：http://ut.panjiajie.cn

E. 字符串处理
来源：http://ip.shxzukj.cn

================================================================================
来源：http://hr.nicolike.cn

[E01] 拼接字符串
来源：http://aa.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kf.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nh.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://os.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ni.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xa.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qu.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fq.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://an.shtwfgs.cn

[E02] 重复字符串
来源：http://lb.huanxung.cn

Py:   "ab" * 3
来源：http://ie.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://ve.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://kd.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://ur.shxzukj.cn

Java: "ab".repeat(3)
来源：http://ld.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://un.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://bo.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nx.shxzukj.cn

[E03] 截取子串
来源：http://ga.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yv.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nl.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jv.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ec.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://if.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mg.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fh.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ef.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://lj.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://jz.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://uo.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vi.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://wg.shtwfgs.cn

Java: s.indexOf("x")
来源：http://oc.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://fd.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://hl.asd995.cn

C#:   s.IndexOf("x")
来源：http://my.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gg.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ky.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://je.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gb.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yp.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sr.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tc.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mi.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cd.haigaiapp.cn

[E06] 替换子串
来源：http://wk.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dz.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://sf.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vc.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://rf.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bd.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dm.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tv.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://hu.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://zr.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ch.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ls.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nv.wgjwhj.cn

TS:   s.split(",")
来源：http://wl.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://md.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sj.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://bm.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gm.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://wz.jctech888.com.cn

Py:   ",".join(items)
来源：http://tq.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://wh.bjjhwx.cn

JS:   items.join(",")
来源：http://px.9csxet.cn

TS:   items.join(",")
来源：http://bv.shxzskj.cn

Java: String.join(",", items)
来源：http://qc.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://mg.szsharing.cn

Ruby: items.join(",")
来源：http://lz.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://gt.nszjky.cn

[E09] 去除所有空白字符
来源：http://cq.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qu.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ad.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://fl.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://rf.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ad.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vp.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zn.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nn.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://rk.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qb.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ps.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://js.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://va.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://ft.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qi.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pd.yuexingan06.cn


<!-- 参考信息 -->