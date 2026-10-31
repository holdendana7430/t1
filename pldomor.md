代发 wailian999

Java: list.add(4);
来源：http://xq.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://lo.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://yb.jctech888.com.cn

C#:   list.Add(4);
来源：http://mz.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://xz.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://hq.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kc.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vs.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ea.szxytkj.cn

Java: list.add(0, 0);
来源：http://gc.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uc.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bd.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://hg.nicolike.cn

[D04] 删除元素
来源：http://rr.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zp.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ua.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qh.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ju.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pv.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tj.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xn.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gg.hnjuh.cn

[D05] 访问与修改元素
来源：http://um.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uj.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ky.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ns.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fh.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://jy.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://jv.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://so.nicolike.cn

[D06] 数组长度
来源：http://ho.yuexingan06.cn

Py:   len(arr)
来源：http://fy.hahajie.cn

PHP:  count($arr);
来源：http://oy.hnjuh.cn

JS:   arr.length
来源：http://co.szxytkj.cn

TS:   arr.length
来源：http://ot.lnxyls.cn

Java: list.size();
来源：http://kv.lnxyls.cn

Go:   len(arr)
来源：http://lu.nicolike.cn

Ruby: arr.length; arr.size
来源：http://ye.jianghongdianzi.cn

C#:   list.Count;
来源：http://ay.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://qt.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ea.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gv.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://zb.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://dq.szxytkj.cn

Java: list.subList(1, 4);
来源：http://qj.jctech888.com.cn

Go:   arr[1:4]
来源：http://ra.szsharing.cn

Ruby: arr[1, 3]
来源：http://uc.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://xx.521024.cn

[D08] 合并两个数组
来源：http://rt.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://gh.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://fu.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lz.bjjhwx.cn

TS:   [...a, ...b];
来源：http://sr.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bh.bookmarksfly.cn

Go:   append(a, b...)
来源：http://do.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://gz.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://on.bjjhwx.cn

[D09] 排序（升序）
来源：http://og.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ia.muxihuayi.cn

PHP:  sort($arr);
来源：http://zi.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yl.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mc.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wg.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fs.yuntaijiaju.cn

Ruby: arr.sort
来源：http://em.shtwfgs.cn

C#:   list.Sort();
来源：http://oo.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zv.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qm.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ha.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cn.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mc.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gd.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ck.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ef.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qf.huixiangedu.cn

[D11] 反转数组
来源：http://zw.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oh.hahajie.cn

PHP:  array_reverse($arr);
来源：http://pk.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zo.huanxung.cn

TS:   [...arr].reverse();
来源：http://sz.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://jc.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://ld.shtwfgs.cn

Ruby: arr.reverse
来源：http://yh.jctech888.com.cn

C#:   list.Reverse();
来源：http://au.9csxet.cn

[D12] 查找元素下标
来源：http://xx.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://dy.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dj.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yv.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rd.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ja.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://kn.huixiangedu.cn

Ruby: arr.index(x)
来源：http://uw.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://yd.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://db.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pk.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jr.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://tg.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://tb.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ld.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lb.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://of.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qp.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://jt.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ul.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://it.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://vj.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://iw.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sa.9csxet.cn

Go:   // 手写循环
来源：http://ak.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fw.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uy.bookmarksfly.cn

[D15] 去重
来源：http://bm.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pn.hahajie.cn

PHP:  array_unique($arr);
来源：http://pn.szsharing.cn

JS:   [...new Set(arr)]
来源：http://px.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ta.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://da.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bs.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://ea.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://yg.haigaiapp.cn

[D16] 求和与平均值
来源：http://nh.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://we.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fi.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hc.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mp.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wj.hahajie.cn

Go:   // 手写循环累加
来源：http://vq.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gl.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://gh.szsharing.cn

[D17] 最大值与最小值
来源：http://eg.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://ci.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://us.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ag.521024.cn

TS:   Math.max(...arr);
来源：http://il.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mo.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vc.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://fp.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ph.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://bq.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bc.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://hq.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qo.hahajie.cn

TS:   nested.flat();
来源：http://cu.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lx.szxytkj.cn

Go:   // 手写双层循环
来源：http://vk.asd995.cn

Ruby: nested.flatten
来源：http://lk.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ma.lnxyls.cn

[D19] 按字段分组
来源：http://zz.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://td.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://we.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vj.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jp.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pa.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://er.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yv.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dy.asd995.cn

[D20] 统计每个元素出现次数
来源：http://dx.szxytkj.cn

Py:   Counter(arr)
来源：http://oq.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ph.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oj.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jh.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://er.szsharing.cn

Go:   // 手写 map[T]int
来源：http://qk.gzmigu.cn

Ruby: arr.tally
来源：http://ek.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zc.colortex.cn

[D21] 判断是否包含某元素
来源：http://qn.muxihuayi.cn

Py:   x in arr
来源：http://kt.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://wg.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://sx.gzmigu.cn

TS:   arr.includes(x)
来源：http://cj.jctech888.com.cn

Java: list.contains(x)
来源：http://fi.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://gm.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://vy.hahajie.cn

C#:   list.Contains(x)
来源：http://im.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://rh.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gf.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sa.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xk.huixiangedu.cn

TS:   [...arr];
来源：http://eu.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://ex.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://le.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://vw.shxzukj.cn

C#:   new List<int>(list);
来源：http://gv.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ui.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://np.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://td.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mo.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://as.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lr.haigaiapp.cn

Go:   // 手写循环
来源：http://ni.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wc.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mx.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://rz.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zo.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ix.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qt.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wg.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ci.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://my.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rv.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jl.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://wh.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qn.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ay.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wj.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tu.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aw.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ko.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://df.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qq.nicolike.cn

[D26] 数组转字符串
来源：http://pq.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://np.asd995.cn

PHP:  implode(", ", $arr);
来源：http://do.panjiajie.cn

JS:   arr.join(", ")
来源：http://as.szsharing.cn

TS:   arr.join(", ")
来源：http://ru.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://pa.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://rh.colortex.cn

Ruby: arr.join(", ")
来源：http://yb.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://hz.nszjky.cn

================================================================================
来源：http://hm.szsharing.cn

E. 字符串处理
来源：http://sr.huanxung.cn

================================================================================
来源：http://pg.asd995.cn

[E01] 拼接字符串
来源：http://ut.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hb.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tm.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oy.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fn.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://po.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iq.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lv.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ga.asd995.cn

[E02] 重复字符串
来源：http://tb.haigaiapp.cn

Py:   "ab" * 3
来源：http://ft.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://lo.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://mt.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://jd.shxzskj.cn

Java: "ab".repeat(3)
来源：http://km.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://vo.panjiajie.cn

Ruby: "ab" * 3
来源：http://cy.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pr.hnjuh.cn

[E03] 截取子串
来源：http://dk.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kj.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vg.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fb.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://va.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://cw.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ha.521024.cn

C#:   s.Substring(1, 3)
来源：http://td.szxytkj.cn

[E04] 查找子串位置
来源：http://sd.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://pi.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://pp.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ul.lnxyls.cn

TS:   s.indexOf("x")
来源：http://vi.9csxet.cn

Java: s.indexOf("x")
来源：http://yl.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://nd.shtwfgs.cn

Ruby: s.index("x")
来源：http://qq.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://qx.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ew.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qe.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xn.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vq.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bs.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ww.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tm.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jl.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ap.wgjwhj.cn

[E06] 替换子串
来源：http://oz.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://if.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://og.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kh.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ea.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uy.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nu.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zd.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://ud.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://kx.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ux.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bj.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ip.shtwfgs.cn

TS:   s.split(",")
来源：http://rl.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ur.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hg.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://dw.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mr.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ia.szxytkj.cn

Py:   ",".join(items)
来源：http://hv.nicolike.cn

PHP:  implode(",", $items);
来源：http://wt.muxihuayi.cn

JS:   items.join(",")
来源：http://jf.haigaiapp.cn

TS:   items.join(",")
来源：http://nl.chemitech.net.cn

Java: String.join(",", items)
来源：http://uq.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://ez.chemitech.net.cn

Ruby: items.join(",")
来源：http://zv.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://hd.lnxyls.cn

[E09] 去除所有空白字符
来源：http://tc.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xt.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hp.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://bc.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://wo.9csxet.cn


<!-- 参考信息 -->