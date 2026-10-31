代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ok.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ra.muxihuayi.cn

[D05] 访问与修改元素
来源：http://vc.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gb.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dm.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jv.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://mp.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://iu.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ep.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gs.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dg.yuntaijiaju.cn

[D06] 数组长度
来源：http://mj.huixinmuqiang.cn

Py:   len(arr)
来源：http://hi.panjiajie.cn

PHP:  count($arr);
来源：http://kr.shtwfgs.cn

JS:   arr.length
来源：http://if.wgjwhj.cn

TS:   arr.length
来源：http://dk.wgjwhj.cn

Java: list.size();
来源：http://uc.shtwfgs.cn

Go:   len(arr)
来源：http://pm.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://am.521024.cn

C#:   list.Count;
来源：http://yb.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://oj.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://at.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ig.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ew.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://kj.colortex.cn

Java: list.subList(1, 4);
来源：http://xx.newstarts.cn

Go:   arr[1:4]
来源：http://oy.nicolike.cn

Ruby: arr[1, 3]
来源：http://ls.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://it.panjiajie.cn

[D08] 合并两个数组
来源：http://vv.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://uu.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://ru.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rg.lnxyls.cn

TS:   [...a, ...b];
来源：http://ap.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vs.nszjky.cn

Go:   append(a, b...)
来源：http://by.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ce.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://mi.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://tz.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://qi.nicolike.cn

PHP:  sort($arr);
来源：http://zl.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oj.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jr.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gq.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nj.panjiajie.cn

Ruby: arr.sort
来源：http://jl.szsharing.cn

C#:   list.Sort();
来源：http://bc.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ml.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zk.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sm.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gm.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vv.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yk.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vn.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ek.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oa.gzmigu.cn

[D11] 反转数组
来源：http://fv.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kg.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://pi.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ir.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ss.colortex.cn

Java: Collections.reverse(list);
来源：http://zz.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://cl.newstarts.cn

Ruby: arr.reverse
来源：http://xq.nicolike.cn

C#:   list.Reverse();
来源：http://yy.yuexingan06.cn

[D12] 查找元素下标
来源：http://fh.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://na.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dh.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://on.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uq.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bw.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://iu.bjjhwx.cn

Ruby: arr.index(x)
来源：http://ey.521024.cn

C#:   list.IndexOf(x);
来源：http://jl.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://op.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jx.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sn.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://il.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://bq.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qp.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pa.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yt.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bn.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://dx.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gt.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ft.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://rt.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://th.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kr.chemitech.net.cn

Go:   // 手写循环
来源：http://ml.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ck.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xy.szxytkj.cn

[D15] 去重
来源：http://kr.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://me.nszjky.cn

PHP:  array_unique($arr);
来源：http://qk.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://us.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://di.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pj.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ss.9csxet.cn

Ruby: arr.uniq
来源：http://nv.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://hm.gzmigu.cn

[D16] 求和与平均值
来源：http://ez.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ha.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iq.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dr.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tw.nszjky.cn

Go:   // 手写循环累加
来源：http://qf.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uk.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://ul.hahajie.cn

[D17] 最大值与最小值
来源：http://fg.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://sq.521024.cn

PHP:  max($arr);  min($arr);
来源：http://en.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ts.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://dw.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ge.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ay.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://xp.521024.cn

C#:   list.Max();  list.Min()
来源：http://jq.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://ew.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fl.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://hz.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hu.shtwfgs.cn

TS:   nested.flat();
来源：http://an.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gt.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://zu.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://ul.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://he.bjjhwx.cn

[D19] 按字段分组
来源：http://qp.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mm.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qr.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oi.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://en.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ae.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://kq.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bo.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kp.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://oj.yuexingan06.cn

Py:   Counter(arr)
来源：http://mm.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://hc.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://au.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pq.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pj.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://be.panjiajie.cn

Ruby: arr.tally
来源：http://te.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oi.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://xl.colortex.cn

Py:   x in arr
来源：http://zf.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://zd.muxihuayi.cn

JS:   arr.includes(x)
来源：http://jr.gzmigu.cn

TS:   arr.includes(x)
来源：http://db.yuexingan06.cn

Java: list.contains(x)
来源：http://fn.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ka.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://mu.asd995.cn

C#:   list.Contains(x)
来源：http://se.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://vr.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ee.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pt.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uy.shxzskj.cn

TS:   [...arr];
来源：http://wh.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://tp.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ku.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://az.chemitech.net.cn

C#:   new List<int>(list);
来源：http://cp.newstarts.cn

[D23] reduce 累积计算
来源：http://au.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ji.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fs.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jm.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zq.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ym.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ft.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://et.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jn.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://nd.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://om.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qv.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cu.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kv.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kk.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vw.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://il.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hl.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://yp.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bq.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vl.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tm.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xt.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sm.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://za.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rl.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zs.hahajie.cn

[D26] 数组转字符串
来源：http://ue.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://lf.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://aw.9csxet.cn

JS:   arr.join(", ")
来源：http://jf.colortex.cn

TS:   arr.join(", ")
来源：http://wj.yuexingan06.cn

Java: String.join(", ", list)
来源：http://es.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://te.521024.cn

Ruby: arr.join(", ")
来源：http://lr.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://nu.haigaiapp.cn

================================================================================
来源：http://hf.lnxyls.cn

E. 字符串处理
来源：http://ec.muxihuayi.cn

================================================================================
来源：http://vl.9csxet.cn

[E01] 拼接字符串
来源：http://jm.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mo.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rv.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uv.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://su.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ht.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bl.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rq.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gs.shxzskj.cn

[E02] 重复字符串
来源：http://gp.jctech888.com.cn

Py:   "ab" * 3
来源：http://rp.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://eu.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://wb.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://lo.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ck.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://is.szsharing.cn

Ruby: "ab" * 3
来源：http://md.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.szsharing.cn

[E03] 截取子串
来源：http://dq.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://or.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ol.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://he.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://ut.lnxyls.cn

Java: s.substring(1, 4)
来源：http://nl.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://es.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ib.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://vy.gzmigu.cn

[E04] 查找子串位置
来源：http://mf.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://bs.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ud.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zy.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://yo.shxzskj.cn

Java: s.indexOf("x")
来源：http://oy.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://cg.haigaiapp.cn

Ruby: s.index("x")
来源：http://wv.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://si.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mm.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iz.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uh.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mn.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eh.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://il.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xi.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ym.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kg.huixinmuqiang.cn

[E06] 替换子串
来源：http://ew.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ax.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://yz.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://km.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://dx.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kc.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rl.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bu.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://in.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://yw.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xy.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rt.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dw.bjjhwx.cn

TS:   s.split(",")
来源：http://jh.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://db.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jw.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://vz.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mu.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://tg.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://jk.asd995.cn

PHP:  implode(",", $items);
来源：http://or.521024.cn

JS:   items.join(",")
来源：http://ww.newstarts.cn

TS:   items.join(",")
来源：http://wb.szsharing.cn

Java: String.join(",", items)
来源：http://kg.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://gb.jctech888.com.cn

Ruby: items.join(",")
来源：http://rh.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://cb.hnjuh.cn

[E09] 去除所有空白字符
来源：http://ws.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bj.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mw.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://nl.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ev.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://em.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cw.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ke.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qh.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ua.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ho.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aj.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://sr.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://tk.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://bv.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yw.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://in.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lu.9csxet.cn

[E11] 反转字符串
来源：http://eg.nszjky.cn

Py:   s[::-1]
来源：http://rr.hahajie.cn

PHP:  strrev($s);
来源：http://oa.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://pn.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://ff.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://na.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yp.huanxung.cn


<!-- 参考信息 -->