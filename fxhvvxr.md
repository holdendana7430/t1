代发 wailian999

[D03] 在指定位置插入元素
来源：http://gr.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ea.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yz.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zr.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://um.nszjky.cn

Java: list.add(0, 0);
来源：http://hg.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bp.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xi.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://hm.newstarts.cn

[D04] 删除元素
来源：http://xm.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wy.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qs.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lp.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://fs.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sc.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ha.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tn.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gx.szsharing.cn

[D05] 访问与修改元素
来源：http://cc.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wm.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cy.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sf.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://qw.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://zt.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://bu.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xv.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nj.haigaiapp.cn

[D06] 数组长度
来源：http://eo.yuexingan06.cn

Py:   len(arr)
来源：http://ax.jctech888.com.cn

PHP:  count($arr);
来源：http://hl.huanxung.cn

JS:   arr.length
来源：http://vf.huanxung.cn

TS:   arr.length
来源：http://mi.colortex.cn

Java: list.size();
来源：http://si.wgjwhj.cn

Go:   len(arr)
来源：http://xq.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://jn.szxytkj.cn

C#:   list.Count;
来源：http://ih.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://bw.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yt.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kt.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://xo.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://xv.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://im.panjiajie.cn

Go:   arr[1:4]
来源：http://qa.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://yx.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://lo.muxihuayi.cn

[D08] 合并两个数组
来源：http://eh.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://kb.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://kv.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oc.shxzukj.cn

TS:   [...a, ...b];
来源：http://zc.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oq.shxzukj.cn

Go:   append(a, b...)
来源：http://zm.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://xi.521024.cn

C#:   a.Concat(b).ToList()
来源：http://tl.shxzskj.cn

[D09] 排序（升序）
来源：http://yh.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://cs.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://fd.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://up.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ru.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ch.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kt.asd995.cn

Ruby: arr.sort
来源：http://bu.huixiangedu.cn

C#:   list.Sort();
来源：http://oo.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wc.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cr.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://di.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pd.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ex.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vn.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yh.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zy.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lw.nicolike.cn

[D11] 反转数组
来源：http://hr.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ie.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://xo.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lg.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://vg.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://pe.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://yc.bookmarksfly.cn

Ruby: arr.reverse
来源：http://xy.shtwfgs.cn

C#:   list.Reverse();
来源：http://yo.521024.cn

[D12] 查找元素下标
来源：http://kv.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://nx.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://my.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eb.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mr.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lu.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://ya.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ze.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://vg.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://nl.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rg.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fp.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://cv.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://sr.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bd.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xq.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wt.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kf.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ua.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ca.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vr.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://tz.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://ix.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ma.colortex.cn

Go:   // 手写循环
来源：http://hm.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gk.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zb.lnxyls.cn

[D15] 去重
来源：http://zo.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wm.szxytkj.cn

PHP:  array_unique($arr);
来源：http://rg.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://ml.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://aq.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oh.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lo.lnxyls.cn

Ruby: arr.uniq
来源：http://ne.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://im.9csxet.cn

[D16] 求和与平均值
来源：http://rh.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ji.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hg.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dl.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ya.huixiangedu.cn

Go:   // 手写循环累加
来源：http://yh.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cp.521024.cn

C#:   list.Sum();  list.Average()
来源：http://hw.huixiangedu.cn

[D17] 最大值与最小值
来源：http://xe.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://fr.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://gv.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zn.521024.cn

TS:   Math.max(...arr);
来源：http://pe.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sm.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qy.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ws.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://rj.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://kb.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vp.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://gc.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qh.jctech888.com.cn

TS:   nested.flat();
来源：http://je.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://te.shtwfgs.cn

Go:   // 手写双层循环
来源：http://yu.hnjuh.cn

Ruby: nested.flatten
来源：http://ol.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://et.nicolike.cn

[D19] 按字段分组
来源：http://er.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dd.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rx.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bt.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qf.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fw.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://px.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nu.colortex.cn

[D20] 统计每个元素出现次数
来源：http://nb.muxihuayi.cn

Py:   Counter(arr)
来源：http://vw.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://fe.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qa.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hv.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dz.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://dg.szsharing.cn

Ruby: arr.tally
来源：http://qe.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://st.asd995.cn

[D21] 判断是否包含某元素
来源：http://uz.hnjuh.cn

Py:   x in arr
来源：http://pc.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://si.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://qk.hahajie.cn

TS:   arr.includes(x)
来源：http://qe.panjiajie.cn

Java: list.contains(x)
来源：http://vy.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://al.colortex.cn

Ruby: arr.include?(x)
来源：http://tq.huixiangedu.cn

C#:   list.Contains(x)
来源：http://tb.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ks.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hf.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nk.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xz.shxzukj.cn

TS:   [...arr];
来源：http://qa.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://sm.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zp.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://gw.haigaiapp.cn

C#:   new List<int>(list);
来源：http://vz.huanxung.cn

[D23] reduce 累积计算
来源：http://rs.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zd.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ii.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pz.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yu.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fg.yuexingan06.cn

Go:   // 手写循环
来源：http://bu.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xa.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://al.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://an.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fl.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fz.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lm.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dh.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sr.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ql.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ve.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rl.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://cp.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eo.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ng.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sy.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jx.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cw.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lk.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nk.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://em.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://ah.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://aw.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://cm.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://cp.521024.cn

TS:   arr.join(", ")
来源：http://sf.shtwfgs.cn

Java: String.join(", ", list)
来源：http://lz.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://lh.hnjuh.cn

Ruby: arr.join(", ")
来源：http://bn.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://gm.nszjky.cn

================================================================================
来源：http://pn.huanxung.cn

E. 字符串处理
来源：http://cz.jianghongdianzi.cn

================================================================================
来源：http://gd.shxzukj.cn

[E01] 拼接字符串
来源：http://kt.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tq.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://be.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uo.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oh.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nb.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tz.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zw.9csxet.cn

[E02] 重复字符串
来源：http://dh.newstarts.cn

Py:   "ab" * 3
来源：http://mp.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://dz.9csxet.cn

JS:   "ab".repeat(3)
来源：http://pv.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://mp.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ms.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://md.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://qo.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ri.chemitech.net.cn

[E03] 截取子串
来源：http://gf.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ct.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mv.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cg.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ee.colortex.cn

Java: s.substring(1, 4)
来源：http://ln.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xe.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://si.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://rz.nicolike.cn

[E04] 查找子串位置
来源：http://uj.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://qr.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://il.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tp.colortex.cn

TS:   s.indexOf("x")
来源：http://kc.nszjky.cn

Java: s.indexOf("x")
来源：http://rp.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://zb.szxytkj.cn

Ruby: s.index("x")
来源：http://ny.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://rx.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sf.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://by.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eu.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ka.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qh.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fe.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ga.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xx.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gs.huixiangedu.cn

[E06] 替换子串
来源：http://pb.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dc.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ma.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rw.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://iw.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vf.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ss.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://da.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://bu.521024.cn

[E07] 按分隔符拆分
来源：http://dt.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jl.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wp.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eh.521024.cn

TS:   s.split(",")
来源：http://ff.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vz.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nk.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://xe.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yd.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://if.szsharing.cn

Py:   ",".join(items)
来源：http://no.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://as.szxytkj.cn

JS:   items.join(",")
来源：http://dm.huixinmuqiang.cn

TS:   items.join(",")
来源：http://nx.9csxet.cn

Java: String.join(",", items)
来源：http://fc.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://hr.szxytkj.cn

Ruby: items.join(",")
来源：http://lb.shxzskj.cn

C#:   string.Join(",", items)
来源：http://vd.huanxung.cn

[E09] 去除所有空白字符
来源：http://ry.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://st.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rx.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ah.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://do.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://au.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uy.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bs.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.nicolike.cn


<!-- 参考信息 -->