代发 wailian999

Py:   len(arr)
来源：http://xf.szsharing.cn

PHP:  count($arr);
来源：http://qo.hnjuh.cn

JS:   arr.length
来源：http://em.chemitech.net.cn

TS:   arr.length
来源：http://se.bookmarksfly.cn

Java: list.size();
来源：http://hf.521024.cn

Go:   len(arr)
来源：http://sv.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://xy.shxzskj.cn

C#:   list.Count;
来源：http://wc.asd995.cn

[D07] 切片 / 取子数组
来源：http://xg.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zq.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mi.colortex.cn

JS:   arr.slice(1, 4);
来源：http://br.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://wu.panjiajie.cn

Java: list.subList(1, 4);
来源：http://bn.nicolike.cn

Go:   arr[1:4]
来源：http://rz.asd995.cn

Ruby: arr[1, 3]
来源：http://lu.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ke.shtwfgs.cn

[D08] 合并两个数组
来源：http://ri.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://pd.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://qd.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ao.gzmigu.cn

TS:   [...a, ...b];
来源：http://rd.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kc.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://jh.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://vg.szsharing.cn

[D09] 排序（升序）
来源：http://tk.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://kq.lnxyls.cn

PHP:  sort($arr);
来源：http://xz.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rc.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tz.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vc.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rj.nszjky.cn

Ruby: arr.sort
来源：http://uv.gzmigu.cn

C#:   list.Sort();
来源：http://ka.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jq.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vy.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://at.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://um.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nx.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wz.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fo.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zw.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nr.yuntaijiaju.cn

[D11] 反转数组
来源：http://hg.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qv.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://nt.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lb.panjiajie.cn

TS:   [...arr].reverse();
来源：http://wf.asd995.cn

Java: Collections.reverse(list);
来源：http://xe.colortex.cn

Go:   slices.Reverse(arr)
来源：http://lk.gzmigu.cn

Ruby: arr.reverse
来源：http://nj.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://jw.szxytkj.cn

[D12] 查找元素下标
来源：http://uu.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ez.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mf.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oa.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nn.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oi.521024.cn

Go:   slices.Index(arr, x)
来源：http://bz.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ws.asd995.cn

C#:   list.IndexOf(x);
来源：http://up.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://jp.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cv.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nl.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://gm.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://km.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ua.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xx.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sv.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://me.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://ga.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qq.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://el.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://qr.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ak.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gq.hnjuh.cn

Go:   // 手写循环
来源：http://vl.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qa.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zy.521024.cn

[D15] 去重
来源：http://uv.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cx.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://bk.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ij.huanxung.cn

TS:   [...new Set(arr)]
来源：http://bt.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ul.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hs.shtwfgs.cn

Ruby: arr.uniq
来源：http://xn.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://vs.bookmarksfly.cn

[D16] 求和与平均值
来源：http://ii.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://db.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xa.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iu.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fy.huixiangedu.cn

Go:   // 手写循环累加
来源：http://za.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iv.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://sa.hahajie.cn

[D17] 最大值与最小值
来源：http://ns.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://xl.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://uw.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ci.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://xy.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bu.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vq.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://fz.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://lg.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://um.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jh.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://oo.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ds.bookmarksfly.cn

TS:   nested.flat();
来源：http://bt.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qv.shxzukj.cn

Go:   // 手写双层循环
来源：http://hv.muxihuayi.cn

Ruby: nested.flatten
来源：http://ep.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zg.jctech888.com.cn

[D19] 按字段分组
来源：http://it.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ps.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bw.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://an.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gw.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cg.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://ho.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zl.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sk.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://zt.wgjwhj.cn

Py:   Counter(arr)
来源：http://ci.szsharing.cn

PHP:  array_count_values($arr);
来源：http://gi.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qm.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vr.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zt.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://nl.lnxyls.cn

Ruby: arr.tally
来源：http://jz.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hw.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://qx.wgjwhj.cn

Py:   x in arr
来源：http://mv.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://kr.gzmigu.cn

JS:   arr.includes(x)
来源：http://ww.bjjhwx.cn

TS:   arr.includes(x)
来源：http://tj.nicolike.cn

Java: list.contains(x)
来源：http://sh.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://xu.shxzskj.cn

Ruby: arr.include?(x)
来源：http://tx.chemitech.net.cn

C#:   list.Contains(x)
来源：http://xh.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://pv.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ar.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://md.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ar.yuntaijiaju.cn

TS:   [...arr];
来源：http://bz.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://dk.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jl.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://cr.muxihuayi.cn

C#:   new List<int>(list);
来源：http://fn.huanxung.cn

[D23] reduce 累积计算
来源：http://cb.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rp.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dx.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jo.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mp.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dq.hnjuh.cn

Go:   // 手写循环
来源：http://hu.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lc.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ix.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://qd.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ae.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gs.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sn.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aw.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bt.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ju.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://md.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jf.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://re.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fe.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sy.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fd.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wc.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xn.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nn.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zl.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jz.colortex.cn

[D26] 数组转字符串
来源：http://tf.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://xr.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://cq.521024.cn

JS:   arr.join(", ")
来源：http://sq.gzmigu.cn

TS:   arr.join(", ")
来源：http://uy.hnjuh.cn

Java: String.join(", ", list)
来源：http://uz.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://rl.newstarts.cn

Ruby: arr.join(", ")
来源：http://wc.colortex.cn

C#:   string.Join(", ", list)
来源：http://ym.jctech888.com.cn

================================================================================
来源：http://gp.muxihuayi.cn

E. 字符串处理
来源：http://hq.hahajie.cn

================================================================================
来源：http://ed.muxihuayi.cn

[E01] 拼接字符串
来源：http://qe.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fj.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hg.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hj.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gt.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ix.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xg.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mf.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wg.szsharing.cn

[E02] 重复字符串
来源：http://dj.chemitech.net.cn

Py:   "ab" * 3
来源：http://bs.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://hi.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://ds.asd995.cn

TS:   "ab".repeat(3)
来源：http://dh.gzmigu.cn

Java: "ab".repeat(3)
来源：http://bd.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://nw.shtwfgs.cn

Ruby: "ab" * 3
来源：http://oe.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xu.yuexingan06.cn

[E03] 截取子串
来源：http://em.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xs.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ql.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ff.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://bu.huanxung.cn

Java: s.substring(1, 4)
来源：http://cb.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uu.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qi.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://iy.muxihuayi.cn

[E04] 查找子串位置
来源：http://lb.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://qm.huanxung.cn

PHP:  strpos($s, "x");
来源：http://ln.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://df.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ru.shxzukj.cn

Java: s.indexOf("x")
来源：http://sm.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://jn.lnxyls.cn

Ruby: s.index("x")
来源：http://ht.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://ok.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ib.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hq.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kg.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hk.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cd.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ec.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ue.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sa.huanxung.cn

[E06] 替换子串
来源：http://rl.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fz.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://ry.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rq.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://nh.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ca.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wh.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rf.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://vy.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://eo.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gj.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vt.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tz.gzmigu.cn

TS:   s.split(",")
来源：http://ep.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dl.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iv.asd995.cn

Ruby: s.split(",");  s.split
来源：http://rl.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dj.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://cv.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://hg.panjiajie.cn

PHP:  implode(",", $items);
来源：http://wc.wgjwhj.cn

JS:   items.join(",")
来源：http://en.shxzukj.cn

TS:   items.join(",")
来源：http://nl.wgjwhj.cn

Java: String.join(",", items)
来源：http://ws.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://ta.shtwfgs.cn

Ruby: items.join(",")
来源：http://mb.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://xb.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://pk.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bd.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yk.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kh.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://js.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://uw.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bi.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wc.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cv.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://ln.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pg.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://km.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://jo.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ez.colortex.cn

Java: String.format("%03d", 7)
来源：http://ix.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ib.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wl.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dx.shxzukj.cn

[E11] 反转字符串
来源：http://kv.asd995.cn

Py:   s[::-1]
来源：http://ur.9csxet.cn

PHP:  strrev($s);
来源：http://dw.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://wz.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://mb.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ys.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vt.gzmigu.cn

Ruby: s.reverse
来源：http://ly.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ia.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://mx.shxzukj.cn

Py:   s.count("a")
来源：http://tw.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://xf.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ui.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://mp.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yl.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://tc.shtwfgs.cn

Ruby: s.count("a")
来源：http://cx.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://np.colortex.cn

[E13] 逐字符遍历
来源：http://bb.hahajie.cn


<!-- 参考信息 -->