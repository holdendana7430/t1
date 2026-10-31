代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iv.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fc.asd995.cn

[D05] 访问与修改元素
来源：http://ef.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yf.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qz.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yu.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://hf.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://dy.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://uk.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dw.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://av.shxzukj.cn

[D06] 数组长度
来源：http://vs.huixiangedu.cn

Py:   len(arr)
来源：http://nx.newstarts.cn

PHP:  count($arr);
来源：http://ve.lnxyls.cn

JS:   arr.length
来源：http://co.gzmigu.cn

TS:   arr.length
来源：http://fl.hnjuh.cn

Java: list.size();
来源：http://mh.colortex.cn

Go:   len(arr)
来源：http://gd.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://es.shxzskj.cn

C#:   list.Count;
来源：http://sk.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://kb.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vy.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mu.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ht.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://zq.shxzskj.cn

Java: list.subList(1, 4);
来源：http://bp.chemitech.net.cn

Go:   arr[1:4]
来源：http://my.hnjuh.cn

Ruby: arr[1, 3]
来源：http://tl.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://kd.bjjhwx.cn

[D08] 合并两个数组
来源：http://ym.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://yt.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://ci.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://li.colortex.cn

TS:   [...a, ...b];
来源：http://wl.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eh.huanxung.cn

Go:   append(a, b...)
来源：http://ha.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://af.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://sp.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://kv.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ug.hahajie.cn

PHP:  sort($arr);
来源：http://lp.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ld.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tw.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://db.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rv.jianghongdianzi.cn

Ruby: arr.sort
来源：http://ei.szxytkj.cn

C#:   list.Sort();
来源：http://hk.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ww.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qt.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oz.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mk.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hk.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uc.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fu.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pv.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ky.yuexingan06.cn

[D11] 反转数组
来源：http://qt.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xk.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://lc.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wp.shxzukj.cn

TS:   [...arr].reverse();
来源：http://jb.gzmigu.cn

Java: Collections.reverse(list);
来源：http://gb.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://qn.szsharing.cn

Ruby: arr.reverse
来源：http://tl.lnxyls.cn

C#:   list.Reverse();
来源：http://xe.colortex.cn

[D12] 查找元素下标
来源：http://fu.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://bg.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aj.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dm.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kh.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cu.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ex.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ce.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ad.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://ls.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tn.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rg.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://yj.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://am.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yh.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qu.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cg.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gc.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://yi.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fb.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://we.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://kq.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://om.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mz.szxytkj.cn

Go:   // 手写循环
来源：http://gb.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vr.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cv.asd995.cn

[D15] 去重
来源：http://wf.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cg.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://pi.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ch.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://jy.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://px.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gn.nicolike.cn

Ruby: arr.uniq
来源：http://eu.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://nh.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://dk.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bk.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jk.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rg.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://io.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yu.chemitech.net.cn

Go:   // 手写循环累加
来源：http://tm.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ec.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://vm.wgjwhj.cn

[D17] 最大值与最小值
来源：http://ep.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://iu.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://ke.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vf.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ap.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rd.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nj.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://en.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://aj.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ww.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fo.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://bj.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cv.shxzskj.cn

TS:   nested.flat();
来源：http://mq.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ew.nicolike.cn

Go:   // 手写双层循环
来源：http://qp.521024.cn

Ruby: nested.flatten
来源：http://zp.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pm.asd995.cn

[D19] 按字段分组
来源：http://lc.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zl.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iu.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tr.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uk.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lj.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://th.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wr.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://et.521024.cn

[D20] 统计每个元素出现次数
来源：http://ph.shtwfgs.cn

Py:   Counter(arr)
来源：http://lp.asd995.cn

PHP:  array_count_values($arr);
来源：http://ss.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ii.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sd.9csxet.cn

Go:   // 手写 map[T]int
来源：http://ya.gzmigu.cn

Ruby: arr.tally
来源：http://vj.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://me.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://yh.lnxyls.cn

Py:   x in arr
来源：http://et.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ao.szxytkj.cn

JS:   arr.includes(x)
来源：http://ki.lnxyls.cn

TS:   arr.includes(x)
来源：http://yz.huixiangedu.cn

Java: list.contains(x)
来源：http://cb.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://tr.newstarts.cn

Ruby: arr.include?(x)
来源：http://gr.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://un.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://oc.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tb.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gd.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bo.newstarts.cn

TS:   [...arr];
来源：http://me.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://pw.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://em.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://in.szxytkj.cn

C#:   new List<int>(list);
来源：http://lr.colortex.cn

[D23] reduce 累积计算
来源：http://hb.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mi.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uj.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uo.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://du.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pw.muxihuayi.cn

Go:   // 手写循环
来源：http://zc.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jj.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jz.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://ww.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dq.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bz.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kn.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cl.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xw.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eh.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tq.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://he.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ff.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gk.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sb.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://av.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ho.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mw.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://he.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rv.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fo.newstarts.cn

[D26] 数组转字符串
来源：http://qv.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://cz.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://gp.gzmigu.cn

JS:   arr.join(", ")
来源：http://ku.jctech888.com.cn

TS:   arr.join(", ")
来源：http://xh.hnjuh.cn

Java: String.join(", ", list)
来源：http://lh.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://ms.521024.cn

Ruby: arr.join(", ")
来源：http://jz.asd995.cn

C#:   string.Join(", ", list)
来源：http://eo.gzmigu.cn

================================================================================
来源：http://wq.jctech888.com.cn

E. 字符串处理
来源：http://ts.yuexingan06.cn

================================================================================
来源：http://mi.shxzskj.cn

[E01] 拼接字符串
来源：http://vi.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vu.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nl.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zx.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://il.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://br.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://be.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lp.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sh.szxytkj.cn

[E02] 重复字符串
来源：http://zb.hnjuh.cn

Py:   "ab" * 3
来源：http://xs.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://dj.asd995.cn

JS:   "ab".repeat(3)
来源：http://ej.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://jv.lnxyls.cn

Java: "ab".repeat(3)
来源：http://vy.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ay.muxihuayi.cn

Ruby: "ab" * 3
来源：http://hr.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qq.shxzukj.cn

[E03] 截取子串
来源：http://jv.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wz.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rh.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yn.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://fg.gzmigu.cn

Java: s.substring(1, 4)
来源：http://ud.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://om.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ak.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://sh.bookmarksfly.cn

[E04] 查找子串位置
来源：http://gx.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://pw.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://yg.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bh.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ch.gzmigu.cn

Java: s.indexOf("x")
来源：http://sx.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://ts.9csxet.cn

Ruby: s.index("x")
来源：http://wd.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://hi.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xn.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lk.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pt.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fd.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fk.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xx.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oq.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cb.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rt.lnxyls.cn

[E06] 替换子串
来源：http://vp.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kn.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://rd.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ps.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://fq.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fv.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://na.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zf.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://rj.9csxet.cn

[E07] 按分隔符拆分
来源：http://qi.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pt.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wl.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gy.jctech888.com.cn

TS:   s.split(",")
来源：http://tr.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yr.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sm.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://es.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dw.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://lz.yuexingan06.cn

Py:   ",".join(items)
来源：http://xe.shxzukj.cn

PHP:  implode(",", $items);
来源：http://nq.wgjwhj.cn

JS:   items.join(",")
来源：http://aq.huixinmuqiang.cn

TS:   items.join(",")
来源：http://xh.521024.cn

Java: String.join(",", items)
来源：http://eu.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://fq.shxzukj.cn

Ruby: items.join(",")
来源：http://gl.colortex.cn

C#:   string.Join(",", items)
来源：http://zr.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://eo.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ji.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vd.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://tm.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://af.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ly.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hs.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sb.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ip.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://zb.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wo.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oq.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://dq.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://bk.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ib.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hp.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tu.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mo.panjiajie.cn

[E11] 反转字符串
来源：http://kl.colortex.cn

Py:   s[::-1]
来源：http://pc.panjiajie.cn

PHP:  strrev($s);
来源：http://ap.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://yy.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://zx.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zv.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ym.szsharing.cn


<!-- 参考信息 -->