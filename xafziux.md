代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lq.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dm.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ox.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://ux.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://yj.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vr.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mf.panjiajie.cn

[D06] 数组长度
来源：http://aa.jianghongdianzi.cn

Py:   len(arr)
来源：http://tj.shtwfgs.cn

PHP:  count($arr);
来源：http://kk.hahajie.cn

JS:   arr.length
来源：http://db.shtwfgs.cn

TS:   arr.length
来源：http://rc.haigaiapp.cn

Java: list.size();
来源：http://ei.panjiajie.cn

Go:   len(arr)
来源：http://nv.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://vi.asd995.cn

C#:   list.Count;
来源：http://en.hahajie.cn

[D07] 切片 / 取子数组
来源：http://cl.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pd.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sb.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://cf.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://qi.shxzskj.cn

Java: list.subList(1, 4);
来源：http://tk.9csxet.cn

Go:   arr[1:4]
来源：http://wj.521024.cn

Ruby: arr[1, 3]
来源：http://dt.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://hf.shxzskj.cn

[D08] 合并两个数组
来源：http://nm.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://bv.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://pl.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yo.521024.cn

TS:   [...a, ...b];
来源：http://wf.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vd.wgjwhj.cn

Go:   append(a, b...)
来源：http://gy.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://gj.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://nn.nszjky.cn

[D09] 排序（升序）
来源：http://wp.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ay.shxzukj.cn

PHP:  sort($arr);
来源：http://tq.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ad.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zq.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jq.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bd.hahajie.cn

Ruby: arr.sort
来源：http://pm.bjjhwx.cn

C#:   list.Sort();
来源：http://vk.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://or.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ig.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kf.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bs.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fz.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kt.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yu.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hc.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cq.colortex.cn

[D11] 反转数组
来源：http://ol.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ck.hahajie.cn

PHP:  array_reverse($arr);
来源：http://fy.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sk.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://sn.521024.cn

Java: Collections.reverse(list);
来源：http://tb.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ig.huanxung.cn

Ruby: arr.reverse
来源：http://ke.gzmigu.cn

C#:   list.Reverse();
来源：http://yw.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://mp.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://sf.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nk.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hj.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pk.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xc.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://lh.shxzskj.cn

Ruby: arr.index(x)
来源：http://wb.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://rm.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://kf.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://am.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zi.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://ky.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://cf.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jz.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://te.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cc.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tq.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://xz.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fg.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kw.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://cj.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://re.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xs.shtwfgs.cn

Go:   // 手写循环
来源：http://ye.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://co.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nj.hahajie.cn

[D15] 去重
来源：http://mc.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pt.huanxung.cn

PHP:  array_unique($arr);
来源：http://fo.nicolike.cn

JS:   [...new Set(arr)]
来源：http://nq.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://yk.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pg.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zx.hahajie.cn

Ruby: arr.uniq
来源：http://zi.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://rh.yuexingan06.cn

[D16] 求和与平均值
来源：http://no.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fp.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cw.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ed.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qz.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fk.nszjky.cn

Go:   // 手写循环累加
来源：http://ki.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ck.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://lo.hahajie.cn

[D17] 最大值与最小值
来源：http://bd.asd995.cn

Py:   max(arr);  min(arr)
来源：http://sh.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://zv.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://db.colortex.cn

TS:   Math.max(...arr);
来源：http://xl.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sp.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gv.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://xi.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://kz.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://mt.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jf.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ur.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tl.chemitech.net.cn

TS:   nested.flat();
来源：http://cn.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ow.muxihuayi.cn

Go:   // 手写双层循环
来源：http://bs.jctech888.com.cn

Ruby: nested.flatten
来源：http://rf.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sx.nicolike.cn

[D19] 按字段分组
来源：http://oo.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ds.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zo.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xe.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ln.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://mj.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mu.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://al.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://qp.panjiajie.cn

Py:   Counter(arr)
来源：http://rd.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://qz.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sq.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yf.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ae.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://xt.jctech888.com.cn

Ruby: arr.tally
来源：http://sj.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://op.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://lp.shxzskj.cn

Py:   x in arr
来源：http://gu.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://cx.521024.cn

JS:   arr.includes(x)
来源：http://fz.huixiangedu.cn

TS:   arr.includes(x)
来源：http://nu.yuntaijiaju.cn

Java: list.contains(x)
来源：http://em.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://cj.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://nu.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://ff.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://hx.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ff.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hp.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yz.asd995.cn

TS:   [...arr];
来源：http://av.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://hv.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://du.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://rh.hnjuh.cn

C#:   new List<int>(list);
来源：http://qs.newstarts.cn

[D23] reduce 累积计算
来源：http://rs.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cw.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zp.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://is.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://la.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eh.gzmigu.cn

Go:   // 手写循环
来源：http://yu.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qt.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ks.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://in.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rj.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ak.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jv.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wt.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lh.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hm.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fq.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gs.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://nu.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gz.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vd.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jt.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ug.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xy.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ot.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mh.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ib.huixiangedu.cn

[D26] 数组转字符串
来源：http://qa.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://lp.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://jw.panjiajie.cn

JS:   arr.join(", ")
来源：http://fu.szxytkj.cn

TS:   arr.join(", ")
来源：http://mv.huixiangedu.cn

Java: String.join(", ", list)
来源：http://gn.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ev.colortex.cn

Ruby: arr.join(", ")
来源：http://qx.9csxet.cn

C#:   string.Join(", ", list)
来源：http://dq.bookmarksfly.cn

================================================================================
来源：http://vk.shtwfgs.cn

E. 字符串处理
来源：http://ox.hnjuh.cn

================================================================================
来源：http://et.huixiangedu.cn

[E01] 拼接字符串
来源：http://ij.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fw.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tt.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mb.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dk.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gv.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gd.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://re.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hf.szxytkj.cn

[E02] 重复字符串
来源：http://jo.huixiangedu.cn

Py:   "ab" * 3
来源：http://zw.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://op.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://jq.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://vu.nszjky.cn

Java: "ab".repeat(3)
来源：http://fb.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://kn.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://hd.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gq.9csxet.cn

[E03] 截取子串
来源：http://ki.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fd.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yf.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://to.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://wf.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://ar.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ba.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ba.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://az.shxzskj.cn

[E04] 查找子串位置
来源：http://zl.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://fd.nszjky.cn

PHP:  strpos($s, "x");
来源：http://pu.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bd.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://mc.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ov.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://rb.nicolike.cn

Ruby: s.index("x")
来源：http://cm.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://vx.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sn.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://im.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fd.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kx.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mt.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zv.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qp.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ug.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qf.yuexingan06.cn

[E06] 替换子串
来源：http://sc.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ai.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://cy.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mq.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://gp.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yv.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lh.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gz.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://wm.szsharing.cn

[E07] 按分隔符拆分
来源：http://nb.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fu.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ls.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fr.chemitech.net.cn

TS:   s.split(",")
来源：http://fn.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mh.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ka.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://hm.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xk.colortex.cn

[E08] 数组按分隔符合并
来源：http://co.szxytkj.cn

Py:   ",".join(items)
来源：http://ek.9csxet.cn

PHP:  implode(",", $items);
来源：http://hd.shxzukj.cn

JS:   items.join(",")
来源：http://ce.9csxet.cn

TS:   items.join(",")
来源：http://rp.bookmarksfly.cn

Java: String.join(",", items)
来源：http://lw.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ll.haigaiapp.cn

Ruby: items.join(",")
来源：http://aj.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://pt.shxzskj.cn

[E09] 去除所有空白字符
来源：http://fw.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ty.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gi.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://py.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://dm.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://in.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gs.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bx.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rs.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://qv.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ye.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://az.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://ff.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ym.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://wj.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://di.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yr.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ec.newstarts.cn

[E11] 反转字符串
来源：http://iw.newstarts.cn

Py:   s[::-1]
来源：http://gh.nicolike.cn

PHP:  strrev($s);
来源：http://yz.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://xu.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://xb.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tu.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ep.huixiangedu.cn

Ruby: s.reverse
来源：http://ix.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wc.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://nu.jctech888.com.cn

Py:   s.count("a")
来源：http://bb.gzmigu.cn


<!-- 参考信息 -->