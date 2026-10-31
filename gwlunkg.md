代发 wailian999

[D03] 在指定位置插入元素
来源：http://me.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://yn.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hg.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jt.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://fg.jctech888.com.cn

Java: list.add(0, 0);
来源：http://ov.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jc.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fj.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://nx.haigaiapp.cn

[D04] 删除元素
来源：http://ku.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ha.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bh.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pz.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://we.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zl.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bq.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ne.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sd.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ub.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dx.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pj.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gk.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ci.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://tp.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://dd.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mf.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://va.nicolike.cn

[D06] 数组长度
来源：http://ah.hnjuh.cn

Py:   len(arr)
来源：http://yr.nszjky.cn

PHP:  count($arr);
来源：http://ny.nicolike.cn

JS:   arr.length
来源：http://cv.newstarts.cn

TS:   arr.length
来源：http://at.wgjwhj.cn

Java: list.size();
来源：http://uy.haigaiapp.cn

Go:   len(arr)
来源：http://wl.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://ks.yuexingan06.cn

C#:   list.Count;
来源：http://si.szsharing.cn

[D07] 切片 / 取子数组
来源：http://xt.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qy.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oa.asd995.cn

JS:   arr.slice(1, 4);
来源：http://hf.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://iz.colortex.cn

Java: list.subList(1, 4);
来源：http://kp.521024.cn

Go:   arr[1:4]
来源：http://hn.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://xc.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://vi.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://up.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://gu.colortex.cn

PHP:  array_merge($a, $b);
来源：http://fg.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xb.yuexingan06.cn

TS:   [...a, ...b];
来源：http://dx.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://if.shxzskj.cn

Go:   append(a, b...)
来源：http://tg.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://qv.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://lx.haigaiapp.cn

[D09] 排序（升序）
来源：http://vi.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ru.szsharing.cn

PHP:  sort($arr);
来源：http://tw.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://as.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://le.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ts.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wy.yuexingan06.cn

Ruby: arr.sort
来源：http://mr.yuexingan06.cn

C#:   list.Sort();
来源：http://rv.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rw.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yf.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rm.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cq.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ud.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zz.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ee.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rm.panjiajie.cn

[D11] 反转数组
来源：http://af.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hb.newstarts.cn

PHP:  array_reverse($arr);
来源：http://cy.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hp.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://we.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://fu.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://lj.asd995.cn

Ruby: arr.reverse
来源：http://lp.shxzukj.cn

C#:   list.Reverse();
来源：http://is.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://rn.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://fi.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rr.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wm.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ri.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qo.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://gz.nicolike.cn

Ruby: arr.index(x)
来源：http://hj.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ml.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://av.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jc.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://me.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://ip.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://zz.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ct.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mh.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vb.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://ih.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eg.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jd.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ad.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://mq.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://is.nicolike.cn

Go:   // 手写循环
来源：http://op.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ry.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hi.9csxet.cn

[D15] 去重
来源：http://nx.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gz.hnjuh.cn

PHP:  array_unique($arr);
来源：http://gd.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://ax.colortex.cn

TS:   [...new Set(arr)]
来源：http://mg.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nw.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zh.521024.cn

Ruby: arr.uniq
来源：http://ll.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ip.colortex.cn

[D16] 求和与平均值
来源：http://ty.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dz.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nd.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ae.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kl.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sf.muxihuayi.cn

Go:   // 手写循环累加
来源：http://os.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ad.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://qf.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ri.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ni.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://yl.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ss.newstarts.cn

TS:   Math.max(...arr);
来源：http://nq.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qh.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gz.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://kt.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://tz.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://cw.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fk.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://io.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jw.huixiangedu.cn

TS:   nested.flat();
来源：http://ey.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hr.jctech888.com.cn

Go:   // 手写双层循环
来源：http://ym.asd995.cn

Ruby: nested.flatten
来源：http://by.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fn.gzmigu.cn

[D19] 按字段分组
来源：http://el.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ct.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zh.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://he.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dj.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ga.asd995.cn

Go:   // 手写 map[string][]T
来源：http://tz.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sp.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gi.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://iv.nicolike.cn

Py:   Counter(arr)
来源：http://yh.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://cu.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mh.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lo.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sv.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://hx.szsharing.cn

Ruby: arr.tally
来源：http://ea.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ur.hahajie.cn

[D21] 判断是否包含某元素
来源：http://uw.shxzskj.cn

Py:   x in arr
来源：http://iu.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://fw.lnxyls.cn

JS:   arr.includes(x)
来源：http://ur.shxzukj.cn

TS:   arr.includes(x)
来源：http://yn.gzmigu.cn

Java: list.contains(x)
来源：http://em.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ta.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ja.szsharing.cn

C#:   list.Contains(x)
来源：http://qx.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://em.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ox.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pq.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ly.huixiangedu.cn

TS:   [...arr];
来源：http://nf.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ul.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wf.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://yz.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://nm.muxihuayi.cn

[D23] reduce 累积计算
来源：http://ej.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jg.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eo.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kh.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lr.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fi.panjiajie.cn

Go:   // 手写循环
来源：http://nz.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ft.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aw.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://gx.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wb.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bq.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rh.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gm.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dm.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dg.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lf.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fw.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://lb.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ee.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qc.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xp.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zz.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jh.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pu.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hx.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ez.nicolike.cn

[D26] 数组转字符串
来源：http://jl.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://te.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://xg.521024.cn

JS:   arr.join(", ")
来源：http://gc.colortex.cn

TS:   arr.join(", ")
来源：http://iy.bjjhwx.cn

Java: String.join(", ", list)
来源：http://kw.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://ax.shxzskj.cn

Ruby: arr.join(", ")
来源：http://dr.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://tb.asd995.cn

================================================================================
来源：http://uw.shxzskj.cn

E. 字符串处理
来源：http://gn.nszjky.cn

================================================================================
来源：http://kg.nszjky.cn

[E01] 拼接字符串
来源：http://cv.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qd.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kk.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ui.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ab.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jf.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gn.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fc.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qz.gzmigu.cn

[E02] 重复字符串
来源：http://ho.hahajie.cn

Py:   "ab" * 3
来源：http://qx.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://ah.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://ha.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://ld.shxzskj.cn

Java: "ab".repeat(3)
来源：http://uk.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ah.newstarts.cn

Ruby: "ab" * 3
来源：http://bn.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://we.huixiangedu.cn

[E03] 截取子串
来源：http://js.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lq.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yb.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tu.colortex.cn

TS:   s.slice(1, 4)
来源：http://sq.521024.cn

Java: s.substring(1, 4)
来源：http://xa.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nc.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dy.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://yz.jctech888.com.cn

[E04] 查找子串位置
来源：http://ec.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://nr.asd995.cn

PHP:  strpos($s, "x");
来源：http://gq.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hd.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://hb.nszjky.cn

Java: s.indexOf("x")
来源：http://rj.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ev.panjiajie.cn

Ruby: s.index("x")
来源：http://kt.huanxung.cn

C#:   s.IndexOf("x")
来源：http://wt.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mn.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lw.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ho.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qo.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cp.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sk.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ej.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lm.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hp.nszjky.cn

[E06] 替换子串
来源：http://ov.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mz.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://vc.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://zl.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zn.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://if.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ys.521024.cn

C#:   s.Replace("a", "b")
来源：http://nc.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://le.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nn.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jo.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rl.shxzukj.cn

TS:   s.split(",")
来源：http://xi.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vd.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xl.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://nk.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xd.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ky.jctech888.com.cn

Py:   ",".join(items)
来源：http://tl.hahajie.cn

PHP:  implode(",", $items);
来源：http://rl.9csxet.cn

JS:   items.join(",")
来源：http://lk.newstarts.cn

TS:   items.join(",")
来源：http://il.asd995.cn

Java: String.join(",", items)
来源：http://xj.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ih.hahajie.cn

Ruby: items.join(",")
来源：http://ql.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://gn.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://kn.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sk.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yx.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://gp.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://vn.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://gm.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fo.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ie.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kc.asd995.cn


<!-- 参考信息 -->