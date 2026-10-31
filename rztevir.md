代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://pf.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fl.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tq.wgjwhj.cn

[D06] 数组长度
来源：http://qv.szsharing.cn

Py:   len(arr)
来源：http://gl.nicolike.cn

PHP:  count($arr);
来源：http://xj.huixinmuqiang.cn

JS:   arr.length
来源：http://gl.yuntaijiaju.cn

TS:   arr.length
来源：http://ed.huixinmuqiang.cn

Java: list.size();
来源：http://wk.shxzskj.cn

Go:   len(arr)
来源：http://jf.szsharing.cn

Ruby: arr.length; arr.size
来源：http://gh.yuntaijiaju.cn

C#:   list.Count;
来源：http://dl.521024.cn

[D07] 切片 / 取子数组
来源：http://cn.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vv.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ll.521024.cn

JS:   arr.slice(1, 4);
来源：http://qv.521024.cn

TS:   arr.slice(1, 4);
来源：http://qe.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://vd.hahajie.cn

Go:   arr[1:4]
来源：http://bn.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://hz.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://wx.shtwfgs.cn

[D08] 合并两个数组
来源：http://sa.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://gg.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://rs.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wg.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://cn.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ml.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://eb.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://jo.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://fd.haigaiapp.cn

[D09] 排序（升序）
来源：http://ba.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://vh.huixiangedu.cn

PHP:  sort($arr);
来源：http://nv.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ga.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uz.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vx.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ly.colortex.cn

Ruby: arr.sort
来源：http://ys.yuexingan06.cn

C#:   list.Sort();
来源：http://wj.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mr.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ld.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tk.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ue.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sj.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yk.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uc.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sk.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://su.shtwfgs.cn

[D11] 反转数组
来源：http://ke.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://po.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://pr.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rm.nszjky.cn

TS:   [...arr].reverse();
来源：http://cz.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://so.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://kf.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://jl.szxytkj.cn

C#:   list.Reverse();
来源：http://wd.bookmarksfly.cn

[D12] 查找元素下标
来源：http://gm.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://tw.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rv.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qp.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bj.521024.cn

Go:   slices.Index(arr, x)
来源：http://uf.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://bp.521024.cn

C#:   list.IndexOf(x);
来源：http://ab.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://xv.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yj.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cb.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://ls.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://cn.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qi.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ka.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ud.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cf.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://dl.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uf.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yi.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://vi.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://eu.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jb.nszjky.cn

Go:   // 手写循环
来源：http://nj.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://am.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lx.wgjwhj.cn

[D15] 去重
来源：http://cn.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sx.asd995.cn

PHP:  array_unique($arr);
来源：http://dc.colortex.cn

JS:   [...new Set(arr)]
来源：http://dl.hahajie.cn

TS:   [...new Set(arr)]
来源：http://vc.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://il.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ga.hnjuh.cn

Ruby: arr.uniq
来源：http://xj.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://de.nicolike.cn

[D16] 求和与平均值
来源：http://xu.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bf.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ap.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xs.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yb.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qe.newstarts.cn

Go:   // 手写循环累加
来源：http://ki.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ua.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://df.colortex.cn

[D17] 最大值与最小值
来源：http://xm.asd995.cn

Py:   max(arr);  min(arr)
来源：http://hi.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://bk.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sm.shxzskj.cn

TS:   Math.max(...arr);
来源：http://qu.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qq.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uf.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://cl.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://vt.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://er.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kj.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://ii.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gm.bjjhwx.cn

TS:   nested.flat();
来源：http://uh.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qt.panjiajie.cn

Go:   // 手写双层循环
来源：http://du.shtwfgs.cn

Ruby: nested.flatten
来源：http://vw.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://im.nszjky.cn

[D19] 按字段分组
来源：http://mq.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jj.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oc.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://su.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cn.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yu.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://sm.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ao.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jz.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://xx.wgjwhj.cn

Py:   Counter(arr)
来源：http://ic.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://xv.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jj.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qz.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jl.colortex.cn

Go:   // 手写 map[T]int
来源：http://ll.lnxyls.cn

Ruby: arr.tally
来源：http://wy.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rm.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://fq.yuexingan06.cn

Py:   x in arr
来源：http://fg.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ag.521024.cn

JS:   arr.includes(x)
来源：http://ua.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://rl.wgjwhj.cn

Java: list.contains(x)
来源：http://ol.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://jo.shxzukj.cn

Ruby: arr.include?(x)
来源：http://qc.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://gi.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ji.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xk.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ss.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lc.bjjhwx.cn

TS:   [...arr];
来源：http://rc.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://xt.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qc.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://dc.szsharing.cn

C#:   new List<int>(list);
来源：http://dv.hahajie.cn

[D23] reduce 累积计算
来源：http://yz.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uo.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ep.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xz.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uo.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dq.shxzukj.cn

Go:   // 手写循环
来源：http://vp.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hb.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://iv.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://we.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bp.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mp.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://va.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mv.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hr.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rs.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xi.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://pf.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://if.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ty.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jw.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dl.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mn.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://py.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tj.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mi.nicolike.cn

[D26] 数组转字符串
来源：http://ts.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://qf.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://cp.9csxet.cn

JS:   arr.join(", ")
来源：http://jo.bjjhwx.cn

TS:   arr.join(", ")
来源：http://rl.yuexingan06.cn

Java: String.join(", ", list)
来源：http://jj.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://py.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://kr.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://hf.lnxyls.cn

================================================================================
来源：http://ju.newstarts.cn

E. 字符串处理
来源：http://za.asd995.cn

================================================================================
来源：http://ld.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://th.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ov.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://do.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dl.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dj.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eu.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ni.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ly.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cx.huanxung.cn

[E02] 重复字符串
来源：http://nr.shtwfgs.cn

Py:   "ab" * 3
来源：http://sl.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ki.nicolike.cn

JS:   "ab".repeat(3)
来源：http://bo.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://vf.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://uu.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://xn.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://gd.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wy.yuexingan06.cn

[E03] 截取子串
来源：http://qp.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bi.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xd.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pc.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://xz.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://sy.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ly.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vf.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ei.yuexingan06.cn

[E04] 查找子串位置
来源：http://sr.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://uf.asd995.cn

PHP:  strpos($s, "x");
来源：http://jz.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fp.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://un.chemitech.net.cn

Java: s.indexOf("x")
来源：http://pv.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://ov.chemitech.net.cn

Ruby: s.index("x")
来源：http://ai.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://pk.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sa.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kk.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ge.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ec.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uv.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zm.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vf.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wt.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://il.hahajie.cn

[E06] 替换子串
来源：http://bc.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hf.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ke.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vr.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://xk.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vv.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jw.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nc.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://nz.newstarts.cn

[E07] 按分隔符拆分
来源：http://cp.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ju.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hh.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fe.nszjky.cn

TS:   s.split(",")
来源：http://vh.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ys.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cv.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://ww.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://et.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://zg.muxihuayi.cn

Py:   ",".join(items)
来源：http://tq.gzmigu.cn

PHP:  implode(",", $items);
来源：http://bc.colortex.cn

JS:   items.join(",")
来源：http://tg.chemitech.net.cn

TS:   items.join(",")
来源：http://ka.lnxyls.cn

Java: String.join(",", items)
来源：http://ad.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://sn.huanxung.cn

Ruby: items.join(",")
来源：http://cp.huanxung.cn

C#:   string.Join(",", items)
来源：http://lx.hnjuh.cn

[E09] 去除所有空白字符
来源：http://hk.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wc.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://je.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://fh.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://fb.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://gb.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://an.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eq.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ca.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://ma.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://is.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uo.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://qc.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://dj.szsharing.cn

Java: String.format("%03d", 7)
来源：http://cs.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rb.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cb.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gf.jctech888.com.cn

[E11] 反转字符串
来源：http://rd.shtwfgs.cn

Py:   s[::-1]
来源：http://ut.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://tx.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://th.521024.cn

TS:   [...s].reverse().join("")
来源：http://ng.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wd.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wf.bjjhwx.cn

Ruby: s.reverse
来源：http://la.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wr.szsharing.cn

[E12] 统计某字符出现次数
来源：http://yh.shxzskj.cn

Py:   s.count("a")
来源：http://jw.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://og.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://fd.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://ds.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ij.muxihuayi.cn


<!-- 参考信息 -->