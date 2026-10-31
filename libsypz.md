代发 wailian999

C#:   list.Insert(0, 0);
来源：http://wp.yuntaijiaju.cn

[D04] 删除元素
来源：http://xo.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hv.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jr.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gd.521024.cn

TS:   arr.splice(0, 1);
来源：http://vi.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jl.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cc.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://st.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ab.gzmigu.cn

[D05] 访问与修改元素
来源：http://wi.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://st.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qu.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://vh.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://si.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ml.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lw.yuexingan06.cn

[D06] 数组长度
来源：http://wb.wgjwhj.cn

Py:   len(arr)
来源：http://yx.haigaiapp.cn

PHP:  count($arr);
来源：http://yn.yuntaijiaju.cn

JS:   arr.length
来源：http://rp.9csxet.cn

TS:   arr.length
来源：http://br.szsharing.cn

Java: list.size();
来源：http://zc.muxihuayi.cn

Go:   len(arr)
来源：http://dt.nszjky.cn

Ruby: arr.length; arr.size
来源：http://os.szxytkj.cn

C#:   list.Count;
来源：http://il.colortex.cn

[D07] 切片 / 取子数组
来源：http://dj.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ed.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ri.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://lm.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://pq.shxzukj.cn

Java: list.subList(1, 4);
来源：http://ur.bookmarksfly.cn

Go:   arr[1:4]
来源：http://ds.panjiajie.cn

Ruby: arr[1, 3]
来源：http://pp.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://cc.huanxung.cn

[D08] 合并两个数组
来源：http://br.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://kd.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://gg.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kf.yuexingan06.cn

TS:   [...a, ...b];
来源：http://ce.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fc.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://dk.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://gb.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://wa.shtwfgs.cn

[D09] 排序（升序）
来源：http://hr.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://tr.szxytkj.cn

PHP:  sort($arr);
来源：http://qr.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qc.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fx.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wp.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tc.lnxyls.cn

Ruby: arr.sort
来源：http://jz.hahajie.cn

C#:   list.Sort();
来源：http://id.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ce.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qc.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fm.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dx.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dq.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iu.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hy.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rr.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yh.chemitech.net.cn

[D11] 反转数组
来源：http://ol.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ns.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://sa.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ph.lnxyls.cn

TS:   [...arr].reverse();
来源：http://bb.szxytkj.cn

Java: Collections.reverse(list);
来源：http://lp.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://kn.gzmigu.cn

Ruby: arr.reverse
来源：http://fx.jctech888.com.cn

C#:   list.Reverse();
来源：http://gh.shxzukj.cn

[D12] 查找元素下标
来源：http://eh.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://al.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ku.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ni.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ok.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gr.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://xj.nicolike.cn

Ruby: arr.index(x)
来源：http://gi.nszjky.cn

C#:   list.IndexOf(x);
来源：http://iz.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://hy.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bj.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pg.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://ch.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://va.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qs.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wu.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uz.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rl.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://yj.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pk.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://ka.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://yc.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wm.jianghongdianzi.cn

Go:   // 手写循环
来源：http://bo.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wh.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hu.hnjuh.cn

[D15] 去重
来源：http://jg.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ms.9csxet.cn

PHP:  array_unique($arr);
来源：http://wq.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://gx.colortex.cn

TS:   [...new Set(arr)]
来源：http://dm.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://td.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zf.shxzskj.cn

Ruby: arr.uniq
来源：http://km.colortex.cn

C#:   list.Distinct().ToList()
来源：http://yk.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://of.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vg.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ax.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vj.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mm.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yt.asd995.cn

Go:   // 手写循环累加
来源：http://xh.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dw.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://gk.hahajie.cn

[D17] 最大值与最小值
来源：http://zv.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://cv.521024.cn

PHP:  max($arr);  min($arr);
来源：http://hr.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ki.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ua.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xr.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ya.521024.cn

Ruby: arr.max;  arr.min
来源：http://xg.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://jq.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ln.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vu.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://vi.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rx.asd995.cn

TS:   nested.flat();
来源：http://jo.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ta.colortex.cn

Go:   // 手写双层循环
来源：http://cz.haigaiapp.cn

Ruby: nested.flatten
来源：http://lc.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://um.shxzskj.cn

[D19] 按字段分组
来源：http://sb.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nm.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oj.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vk.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://th.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sk.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://qw.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lw.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xs.521024.cn

[D20] 统计每个元素出现次数
来源：http://ls.shxzukj.cn

Py:   Counter(arr)
来源：http://bi.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://el.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tl.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://va.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://py.huixinmuqiang.cn

Ruby: arr.tally
来源：http://wg.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ds.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://cu.9csxet.cn

Py:   x in arr
来源：http://rp.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://wt.panjiajie.cn

JS:   arr.includes(x)
来源：http://bj.huixiangedu.cn

TS:   arr.includes(x)
来源：http://bf.szxytkj.cn

Java: list.contains(x)
来源：http://bz.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://ci.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://wm.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://ij.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://ch.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ry.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uo.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xp.muxihuayi.cn

TS:   [...arr];
来源：http://ap.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://iq.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://so.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://rm.hahajie.cn

C#:   new List<int>(list);
来源：http://ap.hnjuh.cn

[D23] reduce 累积计算
来源：http://zm.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dp.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dv.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ht.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gg.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hf.panjiajie.cn

Go:   // 手写循环
来源：http://cn.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fm.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kw.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://aq.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gs.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qa.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ui.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ds.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ov.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rr.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://so.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lb.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://da.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://if.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tm.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wk.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ec.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rd.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qw.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qc.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dw.jctech888.com.cn

[D26] 数组转字符串
来源：http://lg.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://tz.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://jw.newstarts.cn

JS:   arr.join(", ")
来源：http://oa.haigaiapp.cn

TS:   arr.join(", ")
来源：http://qd.panjiajie.cn

Java: String.join(", ", list)
来源：http://vx.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://ud.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://wy.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://qc.shxzskj.cn

================================================================================
来源：http://sd.lnxyls.cn

E. 字符串处理
来源：http://pk.yuntaijiaju.cn

================================================================================
来源：http://pe.shxzukj.cn

[E01] 拼接字符串
来源：http://ic.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cb.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ah.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gq.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pm.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iv.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bs.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cl.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mo.shxzukj.cn

[E02] 重复字符串
来源：http://ql.huanxung.cn

Py:   "ab" * 3
来源：http://lw.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://fx.newstarts.cn

JS:   "ab".repeat(3)
来源：http://dj.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://cl.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://cc.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://id.9csxet.cn

Ruby: "ab" * 3
来源：http://xm.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xx.shtwfgs.cn

[E03] 截取子串
来源：http://wi.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oa.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gx.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cg.nicolike.cn

TS:   s.slice(1, 4)
来源：http://jb.nszjky.cn

Java: s.substring(1, 4)
来源：http://lq.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qo.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hx.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://bv.haigaiapp.cn

[E04] 查找子串位置
来源：http://jf.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://ze.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://gx.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mb.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ni.nszjky.cn

Java: s.indexOf("x")
来源：http://bz.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://ng.nicolike.cn

Ruby: s.index("x")
来源：http://ln.newstarts.cn

C#:   s.IndexOf("x")
来源：http://vx.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gz.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ly.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xd.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uc.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://da.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kk.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ju.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wp.lnxyls.cn

[E06] 替换子串
来源：http://lv.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ht.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://up.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://re.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ip.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wo.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kg.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ot.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://wr.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://tq.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ha.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yu.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oo.jctech888.com.cn

TS:   s.split(",")
来源：http://ce.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://si.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yr.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://mc.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qh.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://nn.colortex.cn

Py:   ",".join(items)
来源：http://eb.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://jo.huanxung.cn

JS:   items.join(",")
来源：http://eo.nicolike.cn

TS:   items.join(",")
来源：http://gy.9csxet.cn

Java: String.join(",", items)
来源：http://cq.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://wi.colortex.cn

Ruby: items.join(",")
来源：http://ye.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://vb.lnxyls.cn

[E09] 去除所有空白字符
来源：http://ie.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bs.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jx.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://mw.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://ak.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://sw.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tc.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vb.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://st.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://hm.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lf.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fu.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://bd.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://sd.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://aq.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://la.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sh.colortex.cn


<!-- 参考信息 -->