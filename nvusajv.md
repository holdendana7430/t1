代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://cx.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gz.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kw.521024.cn

[D06] 数组长度
来源：http://gm.yuntaijiaju.cn

Py:   len(arr)
来源：http://fj.szxytkj.cn

PHP:  count($arr);
来源：http://jw.shxzskj.cn

JS:   arr.length
来源：http://se.colortex.cn

TS:   arr.length
来源：http://sb.521024.cn

Java: list.size();
来源：http://mf.hahajie.cn

Go:   len(arr)
来源：http://rl.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://dc.bookmarksfly.cn

C#:   list.Count;
来源：http://mn.nicolike.cn

[D07] 切片 / 取子数组
来源：http://fn.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pf.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yk.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://kt.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://tv.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://yf.bookmarksfly.cn

Go:   arr[1:4]
来源：http://xm.shxzukj.cn

Ruby: arr[1, 3]
来源：http://vi.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://lc.nszjky.cn

[D08] 合并两个数组
来源：http://ok.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://ef.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://nu.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rf.asd995.cn

TS:   [...a, ...b];
来源：http://um.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pp.bjjhwx.cn

Go:   append(a, b...)
来源：http://dy.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://uk.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://od.nszjky.cn

[D09] 排序（升序）
来源：http://mp.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://is.chemitech.net.cn

PHP:  sort($arr);
来源：http://xx.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yt.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fq.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qd.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nm.yuntaijiaju.cn

Ruby: arr.sort
来源：http://mv.haigaiapp.cn

C#:   list.Sort();
来源：http://ou.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lw.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ou.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jb.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kj.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rd.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gc.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aj.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yr.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ec.muxihuayi.cn

[D11] 反转数组
来源：http://zi.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vp.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://mw.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rv.panjiajie.cn

TS:   [...arr].reverse();
来源：http://gn.panjiajie.cn

Java: Collections.reverse(list);
来源：http://hc.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://yv.panjiajie.cn

Ruby: arr.reverse
来源：http://fb.bjjhwx.cn

C#:   list.Reverse();
来源：http://wm.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://xe.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://xi.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mz.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hh.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kl.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ts.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://sp.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://lf.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://qb.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://na.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nb.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oz.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://yx.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ih.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pc.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iu.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gg.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ec.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://fe.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cc.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://as.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://cs.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://st.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ss.haigaiapp.cn

Go:   // 手写循环
来源：http://xz.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rx.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sa.colortex.cn

[D15] 去重
来源：http://nx.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ss.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://qg.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://yk.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rm.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ak.asd995.cn

Ruby: arr.uniq
来源：http://jd.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://bi.bjjhwx.cn

[D16] 求和与平均值
来源：http://nc.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://di.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xs.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kk.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ff.chemitech.net.cn

Go:   // 手写循环累加
来源：http://ic.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ei.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://fp.asd995.cn

[D17] 最大值与最小值
来源：http://th.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://wv.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://ao.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kp.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ic.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nx.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uf.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://sd.521024.cn

C#:   list.Max();  list.Min()
来源：http://cz.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://vw.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mw.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://cx.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jk.yuexingan06.cn

TS:   nested.flat();
来源：http://ya.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jp.9csxet.cn

Go:   // 手写双层循环
来源：http://wo.wgjwhj.cn

Ruby: nested.flatten
来源：http://gj.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qi.huanxung.cn

[D19] 按字段分组
来源：http://bl.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bc.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uk.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://az.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cr.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iz.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://gs.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ye.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vh.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://td.chemitech.net.cn

Py:   Counter(arr)
来源：http://vv.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://ya.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://np.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vg.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fk.nszjky.cn

Go:   // 手写 map[T]int
来源：http://yt.haigaiapp.cn

Ruby: arr.tally
来源：http://re.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lc.huanxung.cn

[D21] 判断是否包含某元素
来源：http://gn.hnjuh.cn

Py:   x in arr
来源：http://rh.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://lw.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://ed.gzmigu.cn

TS:   arr.includes(x)
来源：http://if.jianghongdianzi.cn

Java: list.contains(x)
来源：http://sv.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://ao.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://fp.gzmigu.cn

C#:   list.Contains(x)
来源：http://ch.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://oq.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sb.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ia.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kx.jianghongdianzi.cn

TS:   [...arr];
来源：http://lx.huanxung.cn

Java: new ArrayList<>(list);
来源：http://kj.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qb.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://tr.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ck.szsharing.cn

[D23] reduce 累积计算
来源：http://ww.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lw.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ww.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cm.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://id.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fx.huixiangedu.cn

Go:   // 手写循环
来源：http://ki.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nm.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ny.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://fh.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ta.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iw.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rx.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gv.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zr.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bh.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://er.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://os.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://bt.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yx.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qu.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ml.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rs.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jm.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nj.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pu.szsharing.cn

[D26] 数组转字符串
来源：http://vu.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://yu.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://el.huixiangedu.cn

JS:   arr.join(", ")
来源：http://lk.asd995.cn

TS:   arr.join(", ")
来源：http://ym.yuexingan06.cn

Java: String.join(", ", list)
来源：http://jh.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://er.szxytkj.cn

Ruby: arr.join(", ")
来源：http://kj.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://dl.shxzskj.cn

================================================================================
来源：http://ke.bjjhwx.cn

E. 字符串处理
来源：http://md.jctech888.com.cn

================================================================================
来源：http://dq.muxihuayi.cn

[E01] 拼接字符串
来源：http://px.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gg.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mp.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pb.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dg.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sy.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fy.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://up.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gy.asd995.cn

[E02] 重复字符串
来源：http://ug.newstarts.cn

Py:   "ab" * 3
来源：http://ve.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://hu.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://zj.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://wu.asd995.cn

Java: "ab".repeat(3)
来源：http://zn.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://lx.colortex.cn

Ruby: "ab" * 3
来源：http://zu.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://al.bjjhwx.cn

[E03] 截取子串
来源：http://de.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dj.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pz.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cu.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://eu.521024.cn

Java: s.substring(1, 4)
来源：http://bf.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zb.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://os.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://pq.szsharing.cn

[E04] 查找子串位置
来源：http://ae.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://dt.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://sg.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ix.huanxung.cn

TS:   s.indexOf("x")
来源：http://va.muxihuayi.cn

Java: s.indexOf("x")
来源：http://rr.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://fz.szxytkj.cn

Ruby: s.index("x")
来源：http://gl.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://jl.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sb.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ck.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iw.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ls.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ca.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gf.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gp.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pp.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hj.asd995.cn

[E06] 替换子串
来源：http://pg.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yg.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://mm.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://di.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://iz.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eh.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://il.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fd.colortex.cn

C#:   s.Replace("a", "b")
来源：http://lh.shxzskj.cn

[E07] 按分隔符拆分
来源：http://np.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wi.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://os.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ec.shxzskj.cn

TS:   s.split(",")
来源：http://im.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://az.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ne.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://jc.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ux.szsharing.cn

[E08] 数组按分隔符合并
来源：http://kq.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://jb.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://jr.jianghongdianzi.cn

JS:   items.join(",")
来源：http://ag.chemitech.net.cn

TS:   items.join(",")
来源：http://rs.szsharing.cn

Java: String.join(",", items)
来源：http://uh.521024.cn

Go:   strings.Join(items, ",")
来源：http://xe.haigaiapp.cn

Ruby: items.join(",")
来源：http://lu.gzmigu.cn

C#:   string.Join(",", items)
来源：http://os.nicolike.cn

[E09] 去除所有空白字符
来源：http://gr.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hx.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hj.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wf.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://wh.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ed.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pd.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cl.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vx.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ml.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nh.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qv.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://yf.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://oh.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://ya.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kv.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uj.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ly.hahajie.cn

[E11] 反转字符串
来源：http://pi.shxzukj.cn

Py:   s[::-1]
来源：http://gx.szxytkj.cn

PHP:  strrev($s);
来源：http://mm.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://fi.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://lw.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tw.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jv.shtwfgs.cn

Ruby: s.reverse
来源：http://wr.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cq.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://hr.huanxung.cn

Py:   s.count("a")
来源：http://xk.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://gt.nszjky.cn

JS:   s.split("a").length - 1
来源：http://mx.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://xw.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kt.chemitech.net.cn


<!-- 参考信息 -->