代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gu.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://et.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fh.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kl.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yv.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lb.szxytkj.cn

[D05] 访问与修改元素
来源：http://wz.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vq.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pv.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mv.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://dw.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yn.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://fh.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nf.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ix.asd995.cn

[D06] 数组长度
来源：http://jz.hahajie.cn

Py:   len(arr)
来源：http://fv.lnxyls.cn

PHP:  count($arr);
来源：http://ah.nicolike.cn

JS:   arr.length
来源：http://tr.lnxyls.cn

TS:   arr.length
来源：http://dx.bookmarksfly.cn

Java: list.size();
来源：http://lf.hahajie.cn

Go:   len(arr)
来源：http://fx.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://fi.hnjuh.cn

C#:   list.Count;
来源：http://rt.nszjky.cn

[D07] 切片 / 取子数组
来源：http://uk.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xs.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://od.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://tg.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://gr.nszjky.cn

Java: list.subList(1, 4);
来源：http://sx.bjjhwx.cn

Go:   arr[1:4]
来源：http://yw.colortex.cn

Ruby: arr[1, 3]
来源：http://hc.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://xa.asd995.cn

[D08] 合并两个数组
来源：http://vt.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://uj.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://po.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sp.haigaiapp.cn

TS:   [...a, ...b];
来源：http://pd.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pp.haigaiapp.cn

Go:   append(a, b...)
来源：http://vm.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://rh.521024.cn

C#:   a.Concat(b).ToList()
来源：http://mh.521024.cn

[D09] 排序（升序）
来源：http://qs.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ry.szxytkj.cn

PHP:  sort($arr);
来源：http://wv.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tj.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wt.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://st.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yd.muxihuayi.cn

Ruby: arr.sort
来源：http://kh.panjiajie.cn

C#:   list.Sort();
来源：http://yc.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xs.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jm.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mb.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://px.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ij.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rh.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rx.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xj.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://va.colortex.cn

[D11] 反转数组
来源：http://fh.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qf.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://mk.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cw.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://jd.szxytkj.cn

Java: Collections.reverse(list);
来源：http://zw.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://jn.nicolike.cn

Ruby: arr.reverse
来源：http://wz.hahajie.cn

C#:   list.Reverse();
来源：http://ou.nszjky.cn

[D12] 查找元素下标
来源：http://xi.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://gz.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wo.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sb.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pj.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fo.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://gx.shtwfgs.cn

Ruby: arr.index(x)
来源：http://qv.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://ym.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://in.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qu.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qf.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://pa.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://vg.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ry.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vd.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wj.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oh.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://xq.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bq.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tx.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://vk.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://rr.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rz.szxytkj.cn

Go:   // 手写循环
来源：http://vw.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://at.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://um.nszjky.cn

[D15] 去重
来源：http://gs.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pl.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://dm.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://rm.9csxet.cn

TS:   [...new Set(arr)]
来源：http://zw.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zh.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qc.newstarts.cn

Ruby: arr.uniq
来源：http://hz.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://sn.colortex.cn

[D16] 求和与平均值
来源：http://co.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fa.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ls.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fb.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oe.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ye.jctech888.com.cn

Go:   // 手写循环累加
来源：http://xe.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ye.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://at.nszjky.cn

[D17] 最大值与最小值
来源：http://on.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://eo.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://sq.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mk.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://go.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rr.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://an.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://wp.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://sj.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://gj.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cy.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://fd.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qe.yuexingan06.cn

TS:   nested.flat();
来源：http://au.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bf.nicolike.cn

Go:   // 手写双层循环
来源：http://as.colortex.cn

Ruby: nested.flatten
来源：http://wy.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aq.nszjky.cn

[D19] 按字段分组
来源：http://xc.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rp.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dp.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gq.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tu.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://km.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://ta.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ki.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yu.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://xi.muxihuayi.cn

Py:   Counter(arr)
来源：http://ms.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://hw.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rz.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xm.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://pu.bjjhwx.cn

Ruby: arr.tally
来源：http://qe.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nl.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://qb.huixiangedu.cn

Py:   x in arr
来源：http://ze.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://wj.chemitech.net.cn

JS:   arr.includes(x)
来源：http://ri.szsharing.cn

TS:   arr.includes(x)
来源：http://sr.szxytkj.cn

Java: list.contains(x)
来源：http://bl.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://fx.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://gl.gzmigu.cn

C#:   list.Contains(x)
来源：http://jl.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ql.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://te.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qu.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rx.jianghongdianzi.cn

TS:   [...arr];
来源：http://fj.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://zi.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wn.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://yw.gzmigu.cn

C#:   new List<int>(list);
来源：http://gq.yuexingan06.cn

[D23] reduce 累积计算
来源：http://rb.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ge.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xi.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dx.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qf.szsharing.cn

Go:   // 手写循环
来源：http://nb.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oy.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yi.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://ie.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rv.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://go.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jr.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bx.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ub.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gw.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://po.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://rh.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fs.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hw.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kf.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ub.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oq.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dc.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zb.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ot.wgjwhj.cn

[D26] 数组转字符串
来源：http://sg.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://fw.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://fu.521024.cn

JS:   arr.join(", ")
来源：http://bc.szxytkj.cn

TS:   arr.join(", ")
来源：http://ve.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://sb.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://to.9csxet.cn

Ruby: arr.join(", ")
来源：http://kj.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://do.huixinmuqiang.cn

================================================================================
来源：http://ka.nszjky.cn

E. 字符串处理
来源：http://gn.szsharing.cn

================================================================================
来源：http://ku.9csxet.cn

[E01] 拼接字符串
来源：http://ex.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bu.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dr.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qw.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nm.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vz.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yq.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ni.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://js.chemitech.net.cn

[E02] 重复字符串
来源：http://zn.shxzukj.cn

Py:   "ab" * 3
来源：http://sa.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://ch.hahajie.cn

JS:   "ab".repeat(3)
来源：http://vo.nicolike.cn

TS:   "ab".repeat(3)
来源：http://pz.shxzskj.cn

Java: "ab".repeat(3)
来源：http://jo.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://da.chemitech.net.cn

Ruby: "ab" * 3
来源：http://uw.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uo.newstarts.cn

[E03] 截取子串
来源：http://tj.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mn.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://us.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nw.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://vo.newstarts.cn

Java: s.substring(1, 4)
来源：http://xi.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cd.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lg.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://sv.lnxyls.cn

[E04] 查找子串位置
来源：http://mg.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://pv.nicolike.cn

PHP:  strpos($s, "x");
来源：http://uz.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mw.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://kb.huanxung.cn

Java: s.indexOf("x")
来源：http://qp.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://ya.nszjky.cn

Ruby: s.index("x")
来源：http://jw.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://yg.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sy.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uq.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bc.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uo.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rj.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qn.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zd.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kb.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pp.huixiangedu.cn

[E06] 替换子串
来源：http://wc.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hf.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://gn.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rr.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://bd.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ou.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cs.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ap.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ne.newstarts.cn

[E07] 按分隔符拆分
来源：http://kh.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fi.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://um.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wt.nszjky.cn

TS:   s.split(",")
来源：http://vn.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://el.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yd.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://ek.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ic.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://tl.chemitech.net.cn

Py:   ",".join(items)
来源：http://yz.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ny.yuntaijiaju.cn

JS:   items.join(",")
来源：http://ta.nszjky.cn

TS:   items.join(",")
来源：http://ze.nicolike.cn

Java: String.join(",", items)
来源：http://ep.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://mn.shxzskj.cn

Ruby: items.join(",")
来源：http://dv.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://pm.colortex.cn

[E09] 去除所有空白字符
来源：http://mf.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eq.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vu.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ps.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://cp.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://om.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vx.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ad.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://np.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://np.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aa.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iv.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://mu.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ib.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://or.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xv.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bg.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://do.newstarts.cn

[E11] 反转字符串
来源：http://xw.bookmarksfly.cn

Py:   s[::-1]
来源：http://nk.newstarts.cn

PHP:  strrev($s);
来源：http://eg.lnxyls.cn


<!-- 参考信息 -->