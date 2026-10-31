代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://jo.nicolike.cn

Java: list.add(0, 0);
来源：http://uq.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wl.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gr.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://je.yuexingan06.cn

[D04] 删除元素
来源：http://bo.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xo.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://in.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fa.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://tz.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fw.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xb.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wg.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ws.nszjky.cn

[D05] 访问与修改元素
来源：http://oe.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://an.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gf.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bi.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://mg.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://sh.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://hu.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pi.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gh.muxihuayi.cn

[D06] 数组长度
来源：http://se.huanxung.cn

Py:   len(arr)
来源：http://jb.jianghongdianzi.cn

PHP:  count($arr);
来源：http://vo.yuntaijiaju.cn

JS:   arr.length
来源：http://ya.jianghongdianzi.cn

TS:   arr.length
来源：http://oh.nicolike.cn

Java: list.size();
来源：http://qp.nicolike.cn

Go:   len(arr)
来源：http://lj.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://re.bjjhwx.cn

C#:   list.Count;
来源：http://ae.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ro.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ja.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hv.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://xb.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://pw.521024.cn

Java: list.subList(1, 4);
来源：http://oo.nicolike.cn

Go:   arr[1:4]
来源：http://lb.newstarts.cn

Ruby: arr[1, 3]
来源：http://jg.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://go.521024.cn

[D08] 合并两个数组
来源：http://of.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://cc.521024.cn

PHP:  array_merge($a, $b);
来源：http://rd.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bu.hahajie.cn

TS:   [...a, ...b];
来源：http://fk.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zu.muxihuayi.cn

Go:   append(a, b...)
来源：http://ag.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://uw.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://av.bookmarksfly.cn

[D09] 排序（升序）
来源：http://nn.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://hz.jctech888.com.cn

PHP:  sort($arr);
来源：http://xe.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yt.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wc.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fi.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gl.521024.cn

Ruby: arr.sort
来源：http://sh.chemitech.net.cn

C#:   list.Sort();
来源：http://ub.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pe.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fs.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ql.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://os.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kh.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ia.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cg.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ix.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kn.huixinmuqiang.cn

[D11] 反转数组
来源：http://ia.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ow.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ip.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yw.panjiajie.cn

TS:   [...arr].reverse();
来源：http://fu.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://le.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://si.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://xs.nszjky.cn

C#:   list.Reverse();
来源：http://jd.chemitech.net.cn

[D12] 查找元素下标
来源：http://xp.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://nu.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lr.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://so.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uk.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nt.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://cy.hnjuh.cn

Ruby: arr.index(x)
来源：http://ch.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://fg.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://fq.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://np.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://at.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://zk.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://mn.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yo.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nu.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qj.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://na.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://oq.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mq.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ln.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://ph.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://qp.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wh.yuexingan06.cn

Go:   // 手写循环
来源：http://tm.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ab.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ws.colortex.cn

[D15] 去重
来源：http://we.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dt.asd995.cn

PHP:  array_unique($arr);
来源：http://uo.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://gc.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://mi.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cq.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fq.panjiajie.cn

Ruby: arr.uniq
来源：http://pt.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://lr.colortex.cn

[D16] 求和与平均值
来源：http://ou.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://km.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zp.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rn.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pv.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oj.panjiajie.cn

Go:   // 手写循环累加
来源：http://tu.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wa.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://ag.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://nk.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://il.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://io.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pi.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ua.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://co.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zs.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://pl.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://nj.521024.cn

[D18] 扁平化嵌套数组
来源：http://iw.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qd.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://fd.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ll.newstarts.cn

TS:   nested.flat();
来源：http://fi.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gt.yuexingan06.cn

Go:   // 手写双层循环
来源：http://bw.nszjky.cn

Ruby: nested.flatten
来源：http://cu.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kl.muxihuayi.cn

[D19] 按字段分组
来源：http://na.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jb.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qx.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nz.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cw.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kx.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://if.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uj.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eq.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://pk.9csxet.cn

Py:   Counter(arr)
来源：http://vt.asd995.cn

PHP:  array_count_values($arr);
来源：http://xl.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sj.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qt.szsharing.cn

Go:   // 手写 map[T]int
来源：http://gk.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ef.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fs.nicolike.cn

[D21] 判断是否包含某元素
来源：http://dp.huanxung.cn

Py:   x in arr
来源：http://ul.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://rk.nszjky.cn

JS:   arr.includes(x)
来源：http://bh.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://zo.jctech888.com.cn

Java: list.contains(x)
来源：http://nw.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://uj.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://md.muxihuayi.cn

C#:   list.Contains(x)
来源：http://nh.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://it.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dw.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kz.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cq.shtwfgs.cn

TS:   [...arr];
来源：http://ux.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://xj.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bh.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://nj.muxihuayi.cn

C#:   new List<int>(list);
来源：http://ty.9csxet.cn

[D23] reduce 累积计算
来源：http://vt.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hi.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cy.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pc.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hu.wgjwhj.cn

Go:   // 手写循环
来源：http://ap.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vp.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rs.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://tt.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rh.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cx.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://un.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://su.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jm.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://em.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pq.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ba.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://fh.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ya.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ms.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gi.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fg.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ac.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ow.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rb.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bz.shtwfgs.cn

[D26] 数组转字符串
来源：http://te.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://ec.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://jq.nszjky.cn

JS:   arr.join(", ")
来源：http://vi.bjjhwx.cn

TS:   arr.join(", ")
来源：http://um.bjjhwx.cn

Java: String.join(", ", list)
来源：http://gu.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://ka.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://oc.colortex.cn

C#:   string.Join(", ", list)
来源：http://bi.9csxet.cn

================================================================================
来源：http://iv.nszjky.cn

E. 字符串处理
来源：http://bt.yuntaijiaju.cn

================================================================================
来源：http://aj.bookmarksfly.cn

[E01] 拼接字符串
来源：http://th.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jp.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uv.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://de.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oo.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ei.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://te.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ar.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ko.bookmarksfly.cn

[E02] 重复字符串
来源：http://fz.hnjuh.cn

Py:   "ab" * 3
来源：http://ib.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://pj.521024.cn

JS:   "ab".repeat(3)
来源：http://bi.hahajie.cn

TS:   "ab".repeat(3)
来源：http://hy.szsharing.cn

Java: "ab".repeat(3)
来源：http://hx.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://nf.colortex.cn

Ruby: "ab" * 3
来源：http://tm.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ng.nszjky.cn

[E03] 截取子串
来源：http://ex.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ab.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sc.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iv.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://rf.lnxyls.cn

Java: s.substring(1, 4)
来源：http://ok.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uz.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://em.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://al.szsharing.cn

[E04] 查找子串位置
来源：http://um.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://lw.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://lg.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://li.newstarts.cn

TS:   s.indexOf("x")
来源：http://hd.shxzukj.cn

Java: s.indexOf("x")
来源：http://qa.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://dp.muxihuayi.cn

Ruby: s.index("x")
来源：http://ie.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://az.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fs.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ve.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ay.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yp.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ri.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jd.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yb.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wa.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zf.9csxet.cn

[E06] 替换子串
来源：http://uy.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yj.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ts.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iu.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://qx.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://as.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iv.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qj.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://uj.huanxung.cn

[E07] 按分隔符拆分
来源：http://xe.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qk.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yo.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ym.bjjhwx.cn

TS:   s.split(",")
来源：http://bw.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://up.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://df.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://fh.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wv.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://wg.panjiajie.cn

Py:   ",".join(items)
来源：http://na.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://ve.szsharing.cn

JS:   items.join(",")
来源：http://je.521024.cn

TS:   items.join(",")
来源：http://iq.jctech888.com.cn

Java: String.join(",", items)
来源：http://hl.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ve.shtwfgs.cn

Ruby: items.join(",")
来源：http://dx.colortex.cn

C#:   string.Join(",", items)
来源：http://fr.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://lb.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jn.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://th.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://gk.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://ji.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://fv.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cz.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eq.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cg.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://wa.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ud.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xb.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://xv.lnxyls.cn


<!-- 参考信息 -->