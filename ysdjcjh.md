代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ta.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ma.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ob.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nf.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://or.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tn.chemitech.net.cn

[D05] 访问与修改元素
来源：http://ts.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ov.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xq.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vl.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://ae.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://ai.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://mw.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hx.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://no.gzmigu.cn

[D06] 数组长度
来源：http://xc.huanxung.cn

Py:   len(arr)
来源：http://eq.shtwfgs.cn

PHP:  count($arr);
来源：http://rv.521024.cn

JS:   arr.length
来源：http://to.521024.cn

TS:   arr.length
来源：http://np.shxzukj.cn

Java: list.size();
来源：http://jp.panjiajie.cn

Go:   len(arr)
来源：http://sc.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://ld.hnjuh.cn

C#:   list.Count;
来源：http://qh.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://dn.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hu.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sj.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://vv.asd995.cn

TS:   arr.slice(1, 4);
来源：http://sf.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://qh.muxihuayi.cn

Go:   arr[1:4]
来源：http://cw.lnxyls.cn

Ruby: arr[1, 3]
来源：http://uh.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://uz.wgjwhj.cn

[D08] 合并两个数组
来源：http://pl.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://tr.asd995.cn

PHP:  array_merge($a, $b);
来源：http://kq.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eq.panjiajie.cn

TS:   [...a, ...b];
来源：http://ag.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zp.szxytkj.cn

Go:   append(a, b...)
来源：http://lr.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://kg.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://uq.haigaiapp.cn

[D09] 排序（升序）
来源：http://bc.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://cx.colortex.cn

PHP:  sort($arr);
来源：http://yd.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kq.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pj.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ra.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://im.hnjuh.cn

Ruby: arr.sort
来源：http://jj.hnjuh.cn

C#:   list.Sort();
来源：http://ki.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ml.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dk.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rj.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lx.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cm.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jn.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jz.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nh.yuntaijiaju.cn

[D11] 反转数组
来源：http://uc.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fz.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://hs.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lx.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://rw.newstarts.cn

Java: Collections.reverse(list);
来源：http://ma.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://lp.panjiajie.cn

Ruby: arr.reverse
来源：http://tr.shxzskj.cn

C#:   list.Reverse();
来源：http://kk.huixiangedu.cn

[D12] 查找元素下标
来源：http://wt.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://dt.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://no.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kd.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://en.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kx.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://km.yuexingan06.cn

Ruby: arr.index(x)
来源：http://cz.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://nd.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://gh.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ig.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uv.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://hr.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://nb.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sx.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bx.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cl.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zn.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://ug.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qo.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pj.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://aq.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ss.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ho.lnxyls.cn

Go:   // 手写循环
来源：http://mu.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ay.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tt.asd995.cn

[D15] 去重
来源：http://tw.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://om.gzmigu.cn

PHP:  array_unique($arr);
来源：http://gc.nszjky.cn

JS:   [...new Set(arr)]
来源：http://oz.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://xa.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yw.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ny.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://cw.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://bf.nszjky.cn

[D16] 求和与平均值
来源：http://rr.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ip.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gm.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oh.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ik.wgjwhj.cn

Go:   // 手写循环累加
来源：http://lk.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://do.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://oe.hnjuh.cn

[D17] 最大值与最小值
来源：http://nt.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://gg.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://ic.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ij.shxzukj.cn

TS:   Math.max(...arr);
来源：http://bs.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gg.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cd.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://vc.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://aw.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://oa.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://se.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://kb.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://va.huixiangedu.cn

TS:   nested.flat();
来源：http://pp.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qh.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://rj.shxzskj.cn

Ruby: nested.flatten
来源：http://sh.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mr.szxytkj.cn

[D19] 按字段分组
来源：http://ln.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pi.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://br.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pv.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ec.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jd.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://wt.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ch.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tq.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://qh.yuexingan06.cn

Py:   Counter(arr)
来源：http://vs.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://pl.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rr.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kj.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://po.shxzukj.cn

Ruby: arr.tally
来源：http://hl.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cm.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://jm.yuntaijiaju.cn

Py:   x in arr
来源：http://hi.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://ts.gzmigu.cn

JS:   arr.includes(x)
来源：http://ns.yuexingan06.cn

TS:   arr.includes(x)
来源：http://ui.muxihuayi.cn

Java: list.contains(x)
来源：http://ru.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://rr.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://gx.shxzskj.cn

C#:   list.Contains(x)
来源：http://rp.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://qm.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rd.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ok.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://om.huanxung.cn

TS:   [...arr];
来源：http://cp.newstarts.cn

Java: new ArrayList<>(list);
来源：http://hb.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://el.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://ho.newstarts.cn

C#:   new List<int>(list);
来源：http://jc.521024.cn

[D23] reduce 累积计算
来源：http://dn.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pz.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pn.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ol.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pn.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ue.yuexingan06.cn

Go:   // 手写循环
来源：http://uy.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sv.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ju.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://sj.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sw.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://og.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xo.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oq.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sv.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mw.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ul.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wn.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://xx.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ea.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nf.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wq.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bt.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lt.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ho.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ys.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pw.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://zd.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://gn.colortex.cn

PHP:  implode(", ", $arr);
来源：http://er.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://wu.yuexingan06.cn

TS:   arr.join(", ")
来源：http://pq.yuexingan06.cn

Java: String.join(", ", list)
来源：http://zm.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://gn.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://rc.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://vw.huanxung.cn

================================================================================
来源：http://jg.nszjky.cn

E. 字符串处理
来源：http://ls.chemitech.net.cn

================================================================================
来源：http://yy.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://pr.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ht.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ig.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wa.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tt.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ww.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oa.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xh.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pr.asd995.cn

[E02] 重复字符串
来源：http://in.haigaiapp.cn

Py:   "ab" * 3
来源：http://ba.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://qj.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://qv.521024.cn

TS:   "ab".repeat(3)
来源：http://hi.gzmigu.cn

Java: "ab".repeat(3)
来源：http://np.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://sw.bjjhwx.cn

Ruby: "ab" * 3
来源：http://jb.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tk.shxzukj.cn

[E03] 截取子串
来源：http://hk.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bz.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pf.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ms.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://is.shxzukj.cn

Java: s.substring(1, 4)
来源：http://vz.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ie.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kr.colortex.cn

C#:   s.Substring(1, 3)
来源：http://nz.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://vq.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://lm.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://mh.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bw.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ua.huanxung.cn

Java: s.indexOf("x")
来源：http://xr.asd995.cn

Go:   strings.Index(s, "x")
来源：http://yu.szxytkj.cn

Ruby: s.index("x")
来源：http://qu.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://db.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wa.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pr.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cg.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qv.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eo.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yf.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dc.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cc.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xw.panjiajie.cn

[E06] 替换子串
来源：http://ud.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://df.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://oi.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xb.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://vd.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wh.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cc.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kv.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://va.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://oy.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jj.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zu.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rc.asd995.cn

TS:   s.split(",")
来源：http://jj.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ug.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mi.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://cn.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zs.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://ug.lnxyls.cn

Py:   ",".join(items)
来源：http://bh.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://nx.colortex.cn

JS:   items.join(",")
来源：http://om.shxzukj.cn

TS:   items.join(",")
来源：http://yr.colortex.cn

Java: String.join(",", items)
来源：http://lp.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://fj.shxzukj.cn

Ruby: items.join(",")
来源：http://ag.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ti.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://uw.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jw.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://na.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://gc.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://yk.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://pf.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qi.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mk.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ti.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://wh.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qj.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qu.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://jm.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://kx.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ht.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ne.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jt.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jp.szxytkj.cn

[E11] 反转字符串
来源：http://tr.shxzskj.cn

Py:   s[::-1]
来源：http://ma.nicolike.cn

PHP:  strrev($s);
来源：http://ew.huixiangedu.cn


<!-- 参考信息 -->