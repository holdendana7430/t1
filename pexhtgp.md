代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://up.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://zh.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vy.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sn.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mv.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nb.gzmigu.cn

[D05] 访问与修改元素
来源：http://nh.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lo.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wl.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ii.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://lv.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://mw.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://do.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yh.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nc.wgjwhj.cn

[D06] 数组长度
来源：http://xp.newstarts.cn

Py:   len(arr)
来源：http://wv.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ua.asd995.cn

JS:   arr.length
来源：http://bf.jianghongdianzi.cn

TS:   arr.length
来源：http://up.yuexingan06.cn

Java: list.size();
来源：http://ya.jctech888.com.cn

Go:   len(arr)
来源：http://uk.hahajie.cn

Ruby: arr.length; arr.size
来源：http://qx.yuexingan06.cn

C#:   list.Count;
来源：http://ar.szsharing.cn

[D07] 切片 / 取子数组
来源：http://qr.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vb.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cw.colortex.cn

JS:   arr.slice(1, 4);
来源：http://lt.colortex.cn

TS:   arr.slice(1, 4);
来源：http://cm.shxzskj.cn

Java: list.subList(1, 4);
来源：http://dn.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://go.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://ir.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://eh.yuexingan06.cn

[D08] 合并两个数组
来源：http://ui.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://vx.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://oj.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sc.colortex.cn

TS:   [...a, ...b];
来源：http://ou.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xy.9csxet.cn

Go:   append(a, b...)
来源：http://hw.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://sf.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://rp.huixiangedu.cn

[D09] 排序（升序）
来源：http://bt.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://hg.yuexingan06.cn

PHP:  sort($arr);
来源：http://wl.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://po.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mq.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tb.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fh.huixinmuqiang.cn

Ruby: arr.sort
来源：http://pu.chemitech.net.cn

C#:   list.Sort();
来源：http://hg.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ne.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ia.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ai.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kd.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://if.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qo.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://po.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cv.asd995.cn

[D11] 反转数组
来源：http://xp.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jo.colortex.cn

PHP:  array_reverse($arr);
来源：http://jh.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pq.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://ow.nicolike.cn

Java: Collections.reverse(list);
来源：http://mj.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://jg.shtwfgs.cn

Ruby: arr.reverse
来源：http://wm.haigaiapp.cn

C#:   list.Reverse();
来源：http://jo.lnxyls.cn

[D12] 查找元素下标
来源：http://ko.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://bi.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lf.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yn.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hl.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yr.colortex.cn

Go:   slices.Index(arr, x)
来源：http://jh.shxzskj.cn

Ruby: arr.index(x)
来源：http://pr.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://ap.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://pu.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ay.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://il.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://wb.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://xc.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hk.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sm.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wr.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://bz.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mb.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cl.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://sr.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://am.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ze.shxzskj.cn

Go:   // 手写循环
来源：http://tg.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lc.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sz.shxzskj.cn

[D15] 去重
来源：http://wm.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qi.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://mq.asd995.cn

JS:   [...new Set(arr)]
来源：http://ww.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://kg.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oo.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bd.muxihuayi.cn

Ruby: arr.uniq
来源：http://gz.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://pq.nicolike.cn

[D16] 求和与平均值
来源：http://mh.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lo.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yr.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://si.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jf.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oh.hahajie.cn

Go:   // 手写循环累加
来源：http://ib.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vj.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://it.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ry.colortex.cn

Py:   max(arr);  min(arr)
来源：http://qc.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ap.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ef.shxzskj.cn

TS:   Math.max(...arr);
来源：http://kd.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://te.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ay.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://ox.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://vk.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://dk.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ta.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://xb.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pp.yuexingan06.cn

TS:   nested.flat();
来源：http://rw.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fe.hnjuh.cn

Go:   // 手写双层循环
来源：http://xi.hahajie.cn

Ruby: nested.flatten
来源：http://kz.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hq.9csxet.cn

[D19] 按字段分组
来源：http://vc.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ex.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kh.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qz.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sw.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bp.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://hx.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eh.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qh.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://aj.wgjwhj.cn

Py:   Counter(arr)
来源：http://vl.colortex.cn

PHP:  array_count_values($arr);
来源：http://df.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kv.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ug.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ts.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://rz.gzmigu.cn

Ruby: arr.tally
来源：http://ak.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yt.nicolike.cn

[D21] 判断是否包含某元素
来源：http://bn.jctech888.com.cn

Py:   x in arr
来源：http://we.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://lb.newstarts.cn

JS:   arr.includes(x)
来源：http://fv.shxzskj.cn

TS:   arr.includes(x)
来源：http://tb.lnxyls.cn

Java: list.contains(x)
来源：http://hi.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://nc.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://sv.nicolike.cn

C#:   list.Contains(x)
来源：http://me.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://jn.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ng.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://se.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fo.bookmarksfly.cn

TS:   [...arr];
来源：http://zo.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://fg.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bv.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://wt.hahajie.cn

C#:   new List<int>(list);
来源：http://ag.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://jv.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://td.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ky.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jx.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zs.huanxung.cn

Go:   // 手写循环
来源：http://bg.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bg.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hv.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://qa.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ry.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ss.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qo.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pu.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ho.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ew.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eq.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://bq.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ci.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zu.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uw.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zr.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rw.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tz.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zp.chemitech.net.cn

[D26] 数组转字符串
来源：http://oj.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://rr.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://gp.521024.cn

JS:   arr.join(", ")
来源：http://ix.gzmigu.cn

TS:   arr.join(", ")
来源：http://by.yuexingan06.cn

Java: String.join(", ", list)
来源：http://cr.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://yf.colortex.cn

Ruby: arr.join(", ")
来源：http://pi.9csxet.cn

C#:   string.Join(", ", list)
来源：http://nq.gzmigu.cn

================================================================================
来源：http://ko.asd995.cn

E. 字符串处理
来源：http://qe.shxzukj.cn

================================================================================
来源：http://pe.lnxyls.cn

[E01] 拼接字符串
来源：http://ov.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cj.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://th.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ms.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gz.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ny.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://in.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gv.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ge.hnjuh.cn

[E02] 重复字符串
来源：http://db.yuexingan06.cn

Py:   "ab" * 3
来源：http://rq.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://jv.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://nf.huanxung.cn

TS:   "ab".repeat(3)
来源：http://ax.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://st.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://bw.gzmigu.cn

Ruby: "ab" * 3
来源：http://uw.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gc.shxzukj.cn

[E03] 截取子串
来源：http://ky.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qe.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ai.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sc.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://hf.nicolike.cn

Java: s.substring(1, 4)
来源：http://iw.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ku.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kf.colortex.cn

C#:   s.Substring(1, 3)
来源：http://ai.colortex.cn

[E04] 查找子串位置
来源：http://mh.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ff.asd995.cn

PHP:  strpos($s, "x");
来源：http://gd.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nm.szxytkj.cn

TS:   s.indexOf("x")
来源：http://eg.haigaiapp.cn

Java: s.indexOf("x")
来源：http://xx.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://cr.huixiangedu.cn

Ruby: s.index("x")
来源：http://tl.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://az.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gr.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ty.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vb.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rh.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mu.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gn.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ne.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wl.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nj.newstarts.cn

[E06] 替换子串
来源：http://om.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aw.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://yf.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fc.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://xn.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ne.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qt.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fc.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://uj.hnjuh.cn

[E07] 按分隔符拆分
来源：http://fm.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fc.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://og.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wt.muxihuayi.cn

TS:   s.split(",")
来源：http://jy.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jz.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sc.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://am.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mh.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://ep.nicolike.cn

Py:   ",".join(items)
来源：http://tp.colortex.cn

PHP:  implode(",", $items);
来源：http://vj.hnjuh.cn

JS:   items.join(",")
来源：http://hp.hnjuh.cn

TS:   items.join(",")
来源：http://yd.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ll.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://wy.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://zx.nszjky.cn

C#:   string.Join(",", items)
来源：http://ox.szsharing.cn

[E09] 去除所有空白字符
来源：http://ew.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xm.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ib.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://am.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://fa.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://mh.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nj.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ss.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pp.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://of.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xa.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yx.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://pu.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://gk.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://xm.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lh.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hu.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dl.wgjwhj.cn

[E11] 反转字符串
来源：http://kq.hahajie.cn

Py:   s[::-1]
来源：http://yx.jctech888.com.cn

PHP:  strrev($s);
来源：http://th.hahajie.cn


<!-- 参考信息 -->