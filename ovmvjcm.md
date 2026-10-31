代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ka.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pi.nicolike.cn

[D06] 数组长度
来源：http://jq.nszjky.cn

Py:   len(arr)
来源：http://qn.bjjhwx.cn

PHP:  count($arr);
来源：http://zv.shxzskj.cn

JS:   arr.length
来源：http://gu.bjjhwx.cn

TS:   arr.length
来源：http://zj.szsharing.cn

Java: list.size();
来源：http://yi.yuexingan06.cn

Go:   len(arr)
来源：http://jq.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://na.huanxung.cn

C#:   list.Count;
来源：http://ul.nszjky.cn

[D07] 切片 / 取子数组
来源：http://id.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mc.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fk.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://lg.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://hj.hahajie.cn

Java: list.subList(1, 4);
来源：http://cy.wgjwhj.cn

Go:   arr[1:4]
来源：http://lc.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://xe.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://nz.asd995.cn

[D08] 合并两个数组
来源：http://ef.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://ov.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://rm.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lc.shxzskj.cn

TS:   [...a, ...b];
来源：http://nj.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ad.bjjhwx.cn

Go:   append(a, b...)
来源：http://ml.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://ne.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ho.9csxet.cn

[D09] 排序（升序）
来源：http://tk.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://wp.asd995.cn

PHP:  sort($arr);
来源：http://dx.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qh.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ic.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ux.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ik.asd995.cn

Ruby: arr.sort
来源：http://sq.shxzukj.cn

C#:   list.Sort();
来源：http://my.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uv.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cb.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yb.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xi.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vf.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yd.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ux.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oz.huanxung.cn

[D11] 反转数组
来源：http://me.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zi.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://ow.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gc.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://so.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://vw.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://zq.huanxung.cn

Ruby: arr.reverse
来源：http://ts.huanxung.cn

C#:   list.Reverse();
来源：http://eq.huanxung.cn

[D12] 查找元素下标
来源：http://gv.521024.cn

Py:   arr.index(x);  x in arr
来源：http://it.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://is.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fy.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cy.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kp.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ct.bjjhwx.cn

Ruby: arr.index(x)
来源：http://vh.szsharing.cn

C#:   list.IndexOf(x);
来源：http://cm.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://ua.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pp.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ji.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://tm.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ud.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wu.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rp.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ag.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wd.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://rm.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tw.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://so.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://rz.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://hc.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bd.bjjhwx.cn

Go:   // 手写循环
来源：http://zr.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qb.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dw.gzmigu.cn

[D15] 去重
来源：http://zk.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sz.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://eu.newstarts.cn

JS:   [...new Set(arr)]
来源：http://wo.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://jz.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qz.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qk.asd995.cn

Ruby: arr.uniq
来源：http://gi.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://cu.shxzukj.cn

[D16] 求和与平均值
来源：http://hw.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lg.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ff.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://br.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vn.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vk.jctech888.com.cn

Go:   // 手写循环累加
来源：http://jq.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ta.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://kv.newstarts.cn

[D17] 最大值与最小值
来源：http://yw.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ot.521024.cn

PHP:  max($arr);  min($arr);
来源：http://pd.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zm.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://vu.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ee.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ii.asd995.cn

Ruby: arr.max;  arr.min
来源：http://ac.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://le.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://vp.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bt.colortex.cn

PHP:  array_merge(...$nested);
来源：http://yu.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fa.szsharing.cn

TS:   nested.flat();
来源：http://nq.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wd.panjiajie.cn

Go:   // 手写双层循环
来源：http://tq.nicolike.cn

Ruby: nested.flatten
来源：http://wp.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fg.yuntaijiaju.cn

[D19] 按字段分组
来源：http://px.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tu.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dq.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pr.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mh.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tc.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://vz.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wq.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oy.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://aj.wgjwhj.cn

Py:   Counter(arr)
来源：http://wf.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://kv.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fv.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cp.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wi.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://sb.shxzukj.cn

Ruby: arr.tally
来源：http://bb.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xo.szsharing.cn

[D21] 判断是否包含某元素
来源：http://dj.bjjhwx.cn

Py:   x in arr
来源：http://qj.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://sq.haigaiapp.cn

JS:   arr.includes(x)
来源：http://pv.huanxung.cn

TS:   arr.includes(x)
来源：http://yo.bjjhwx.cn

Java: list.contains(x)
来源：http://fy.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://zs.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://fm.jctech888.com.cn

C#:   list.Contains(x)
来源：http://on.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://ne.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ec.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xq.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dz.asd995.cn

TS:   [...arr];
来源：http://pd.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://dv.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ws.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://oa.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://ka.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://zm.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xu.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fs.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ty.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yb.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lz.gzmigu.cn

Go:   // 手写循环
来源：http://hh.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://li.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ty.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://cy.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iz.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fj.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://go.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vf.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qz.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eg.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fo.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://be.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://qj.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rx.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rh.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://en.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gw.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vc.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hd.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iu.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://se.521024.cn

[D26] 数组转字符串
来源：http://id.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://ro.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://ji.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://lw.nicolike.cn

TS:   arr.join(", ")
来源：http://xm.huanxung.cn

Java: String.join(", ", list)
来源：http://eg.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://we.521024.cn

Ruby: arr.join(", ")
来源：http://be.newstarts.cn

C#:   string.Join(", ", list)
来源：http://pq.panjiajie.cn

================================================================================
来源：http://sn.huanxung.cn

E. 字符串处理
来源：http://na.shxzukj.cn

================================================================================
来源：http://bq.szxytkj.cn

[E01] 拼接字符串
来源：http://xa.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jc.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tg.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fo.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ur.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ef.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yq.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qc.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wm.panjiajie.cn

[E02] 重复字符串
来源：http://zt.lnxyls.cn

Py:   "ab" * 3
来源：http://za.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://ay.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://sy.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://kq.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://de.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://rq.lnxyls.cn

Ruby: "ab" * 3
来源：http://zn.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lm.gzmigu.cn

[E03] 截取子串
来源：http://ej.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qu.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ms.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sm.9csxet.cn

TS:   s.slice(1, 4)
来源：http://eb.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://yu.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cg.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vs.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://vg.shxzskj.cn

[E04] 查找子串位置
来源：http://ba.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://pq.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ch.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wa.huanxung.cn

TS:   s.indexOf("x")
来源：http://ch.shxzskj.cn

Java: s.indexOf("x")
来源：http://qh.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://oy.haigaiapp.cn

Ruby: s.index("x")
来源：http://hn.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://le.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ec.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://md.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ic.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qx.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cq.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hc.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ap.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vm.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zu.panjiajie.cn

[E06] 替换子串
来源：http://fc.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ed.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ie.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lj.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://uo.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kj.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rf.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sd.colortex.cn

C#:   s.Replace("a", "b")
来源：http://po.gzmigu.cn

[E07] 按分隔符拆分
来源：http://ey.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iu.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fi.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wl.nszjky.cn

TS:   s.split(",")
来源：http://ei.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xg.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qs.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://aa.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yk.asd995.cn

[E08] 数组按分隔符合并
来源：http://pj.asd995.cn

Py:   ",".join(items)
来源：http://as.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://ku.asd995.cn

JS:   items.join(",")
来源：http://zi.shtwfgs.cn

TS:   items.join(",")
来源：http://up.newstarts.cn

Java: String.join(",", items)
来源：http://cx.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://la.lnxyls.cn

Ruby: items.join(",")
来源：http://sn.panjiajie.cn

C#:   string.Join(",", items)
来源：http://rl.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://lk.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nw.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qx.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ec.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://tw.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gn.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mi.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://to.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ok.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://wc.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ye.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qa.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://iu.521024.cn

TS:   "7".padStart(3, "0")
来源：http://mw.asd995.cn

Java: String.format("%03d", 7)
来源：http://wj.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://do.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ts.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hv.9csxet.cn

[E11] 反转字符串
来源：http://lr.yuexingan06.cn

Py:   s[::-1]
来源：http://rm.jctech888.com.cn

PHP:  strrev($s);
来源：http://oa.521024.cn

JS:   [...s].reverse().join("")
来源：http://me.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://qy.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dk.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hp.lnxyls.cn

Ruby: s.reverse
来源：http://it.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dg.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://cy.colortex.cn

Py:   s.count("a")
来源：http://nt.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://di.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ry.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://el.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gt.hnjuh.cn


<!-- 参考信息 -->