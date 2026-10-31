代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mv.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qi.nicolike.cn

[D05] 访问与修改元素
来源：http://nf.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ac.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gu.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hg.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://jy.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://yq.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://ik.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dm.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eo.yuntaijiaju.cn

[D06] 数组长度
来源：http://jw.szxytkj.cn

Py:   len(arr)
来源：http://ku.bookmarksfly.cn

PHP:  count($arr);
来源：http://uz.nicolike.cn

JS:   arr.length
来源：http://tp.newstarts.cn

TS:   arr.length
来源：http://ya.hahajie.cn

Java: list.size();
来源：http://cl.9csxet.cn

Go:   len(arr)
来源：http://ld.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ha.haigaiapp.cn

C#:   list.Count;
来源：http://fl.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://hw.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cw.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oo.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://in.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ut.nszjky.cn

Java: list.subList(1, 4);
来源：http://pz.panjiajie.cn

Go:   arr[1:4]
来源：http://uh.9csxet.cn

Ruby: arr[1, 3]
来源：http://wc.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://oy.521024.cn

[D08] 合并两个数组
来源：http://ir.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://kc.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://gg.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bc.yuexingan06.cn

TS:   [...a, ...b];
来源：http://ht.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ou.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://ik.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://dn.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://eq.shxzukj.cn

[D09] 排序（升序）
来源：http://ke.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://gz.lnxyls.cn

PHP:  sort($arr);
来源：http://sz.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rq.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yu.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://co.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oc.shxzskj.cn

Ruby: arr.sort
来源：http://ny.jctech888.com.cn

C#:   list.Sort();
来源：http://ou.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vm.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wu.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ps.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eb.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ci.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zl.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kn.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wm.muxihuayi.cn

[D11] 反转数组
来源：http://mq.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wf.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://tj.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zw.szsharing.cn

TS:   [...arr].reverse();
来源：http://ot.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://wa.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ab.wgjwhj.cn

Ruby: arr.reverse
来源：http://uj.nicolike.cn

C#:   list.Reverse();
来源：http://ps.panjiajie.cn

[D12] 查找元素下标
来源：http://pw.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://yq.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dw.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yr.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qy.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://id.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://er.newstarts.cn

Ruby: arr.index(x)
来源：http://hp.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://wd.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://cc.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mk.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ne.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://lz.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ba.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ft.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hv.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sv.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hc.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://jo.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ho.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wj.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://vy.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://uy.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ne.colortex.cn

Go:   // 手写循环
来源：http://sa.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xz.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rl.newstarts.cn

[D15] 去重
来源：http://ic.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zz.nszjky.cn

PHP:  array_unique($arr);
来源：http://ar.nicolike.cn

JS:   [...new Set(arr)]
来源：http://hy.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://yl.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dx.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jx.chemitech.net.cn

Ruby: arr.uniq
来源：http://tb.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://zr.shxzukj.cn

[D16] 求和与平均值
来源：http://vv.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lo.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://td.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ge.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ja.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uw.nszjky.cn

Go:   // 手写循环累加
来源：http://ge.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nw.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://cs.yuexingan06.cn

[D17] 最大值与最小值
来源：http://rk.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://ig.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://lu.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hm.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://cm.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ub.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kw.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://cx.colortex.cn

C#:   list.Max();  list.Min()
来源：http://xq.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://pv.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ty.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://go.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yz.panjiajie.cn

TS:   nested.flat();
来源：http://sq.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://du.yuexingan06.cn

Go:   // 手写双层循环
来源：http://by.nszjky.cn

Ruby: nested.flatten
来源：http://fg.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://av.bookmarksfly.cn

[D19] 按字段分组
来源：http://ki.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://he.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cc.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vs.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qv.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fb.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://lu.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ny.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xv.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://jo.chemitech.net.cn

Py:   Counter(arr)
来源：http://vs.szsharing.cn

PHP:  array_count_values($arr);
来源：http://wn.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xf.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nb.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ww.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://mq.newstarts.cn

Ruby: arr.tally
来源：http://fm.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cd.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://cf.nszjky.cn

Py:   x in arr
来源：http://us.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://wo.huanxung.cn

JS:   arr.includes(x)
来源：http://ce.gzmigu.cn

TS:   arr.includes(x)
来源：http://sx.colortex.cn

Java: list.contains(x)
来源：http://iz.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://cx.huanxung.cn

Ruby: arr.include?(x)
来源：http://jv.panjiajie.cn

C#:   list.Contains(x)
来源：http://is.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://vw.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pt.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sl.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bb.bjjhwx.cn

TS:   [...arr];
来源：http://qk.asd995.cn

Java: new ArrayList<>(list);
来源：http://wp.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gi.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://wn.newstarts.cn

C#:   new List<int>(list);
来源：http://lw.bjjhwx.cn

[D23] reduce 累积计算
来源：http://pp.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bd.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jt.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rc.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xr.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gd.newstarts.cn

Go:   // 手写循环
来源：http://je.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zy.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hf.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://gi.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pj.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://et.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ci.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ga.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gd.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yi.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://go.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fb.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://er.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ma.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://of.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nc.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fm.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kn.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fw.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ui.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://za.panjiajie.cn

[D26] 数组转字符串
来源：http://sa.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://lo.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://xi.asd995.cn

JS:   arr.join(", ")
来源：http://zw.panjiajie.cn

TS:   arr.join(", ")
来源：http://gh.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://cz.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://eb.521024.cn

Ruby: arr.join(", ")
来源：http://ix.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://nz.shtwfgs.cn

================================================================================
来源：http://sn.hnjuh.cn

E. 字符串处理
来源：http://kp.bjjhwx.cn

================================================================================
来源：http://yv.haigaiapp.cn

[E01] 拼接字符串
来源：http://gf.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://en.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://am.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ct.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pz.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gp.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xb.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kg.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://re.shxzskj.cn

[E02] 重复字符串
来源：http://kc.huanxung.cn

Py:   "ab" * 3
来源：http://go.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://ae.521024.cn

JS:   "ab".repeat(3)
来源：http://ls.9csxet.cn

TS:   "ab".repeat(3)
来源：http://kc.hnjuh.cn

Java: "ab".repeat(3)
来源：http://rx.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://ks.shxzukj.cn

Ruby: "ab" * 3
来源：http://sc.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ah.szsharing.cn

[E03] 截取子串
来源：http://mv.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tu.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ds.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ku.newstarts.cn

TS:   s.slice(1, 4)
来源：http://vr.newstarts.cn

Java: s.substring(1, 4)
来源：http://we.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ny.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jb.colortex.cn

C#:   s.Substring(1, 3)
来源：http://yf.chemitech.net.cn

[E04] 查找子串位置
来源：http://ya.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://lw.hahajie.cn

PHP:  strpos($s, "x");
来源：http://hh.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bd.newstarts.cn

TS:   s.indexOf("x")
来源：http://ew.9csxet.cn

Java: s.indexOf("x")
来源：http://sg.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://as.chemitech.net.cn

Ruby: s.index("x")
来源：http://ed.nicolike.cn

C#:   s.IndexOf("x")
来源：http://lq.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eb.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wi.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kk.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ev.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vp.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tx.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nr.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://la.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ra.hahajie.cn

[E06] 替换子串
来源：http://hd.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uq.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://dp.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tq.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ek.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xc.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cj.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dk.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://yc.lnxyls.cn

[E07] 按分隔符拆分
来源：http://tw.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gl.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ps.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hs.newstarts.cn

TS:   s.split(",")
来源：http://rk.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mi.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fz.colortex.cn

Ruby: s.split(",");  s.split
来源：http://gz.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xi.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://fb.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://co.szxytkj.cn

PHP:  implode(",", $items);
来源：http://st.jianghongdianzi.cn

JS:   items.join(",")
来源：http://vs.nszjky.cn

TS:   items.join(",")
来源：http://id.asd995.cn

Java: String.join(",", items)
来源：http://ly.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://tq.bookmarksfly.cn

Ruby: items.join(",")
来源：http://kp.szxytkj.cn

C#:   string.Join(",", items)
来源：http://lp.shxzukj.cn

[E09] 去除所有空白字符
来源：http://jf.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sp.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sz.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wi.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://rk.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://jg.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ml.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hs.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://en.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://ol.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ob.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kj.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://cm.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://wa.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://qv.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ya.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oj.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kf.huixiangedu.cn

[E11] 反转字符串
来源：http://gb.hahajie.cn

Py:   s[::-1]
来源：http://fn.colortex.cn

PHP:  strrev($s);
来源：http://ov.colortex.cn

JS:   [...s].reverse().join("")
来源：http://gu.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://mz.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ih.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ja.jctech888.com.cn


<!-- 参考信息 -->