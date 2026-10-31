代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ns.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ua.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jc.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cs.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://km.newstarts.cn

[D04] 删除元素
来源：http://dk.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://so.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bd.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xs.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://sn.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ua.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qq.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ru.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vo.huanxung.cn

[D05] 访问与修改元素
来源：http://in.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nn.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ht.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ld.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://zx.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://lf.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ew.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jx.szxytkj.cn

[D06] 数组长度
来源：http://wg.jctech888.com.cn

Py:   len(arr)
来源：http://pv.lnxyls.cn

PHP:  count($arr);
来源：http://kt.szsharing.cn

JS:   arr.length
来源：http://wn.szsharing.cn

TS:   arr.length
来源：http://ze.newstarts.cn

Java: list.size();
来源：http://cf.hahajie.cn

Go:   len(arr)
来源：http://yt.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://mk.huixiangedu.cn

C#:   list.Count;
来源：http://hl.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://lx.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wp.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gs.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://pp.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://bg.asd995.cn

Java: list.subList(1, 4);
来源：http://et.huixiangedu.cn

Go:   arr[1:4]
来源：http://ey.shxzskj.cn

Ruby: arr[1, 3]
来源：http://am.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://hi.chemitech.net.cn

[D08] 合并两个数组
来源：http://bf.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://am.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://eg.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tp.panjiajie.cn

TS:   [...a, ...b];
来源：http://wl.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nm.huanxung.cn

Go:   append(a, b...)
来源：http://qm.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://zj.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://ur.nszjky.cn

[D09] 排序（升序）
来源：http://on.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://hs.chemitech.net.cn

PHP:  sort($arr);
来源：http://zx.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ya.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hh.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rl.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sv.jctech888.com.cn

Ruby: arr.sort
来源：http://kt.huixiangedu.cn

C#:   list.Sort();
来源：http://fz.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ih.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bn.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ha.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uq.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iu.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pk.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fo.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kz.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cp.muxihuayi.cn

[D11] 反转数组
来源：http://xg.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cy.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://oc.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dp.huanxung.cn

TS:   [...arr].reverse();
来源：http://si.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://he.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://nx.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://rg.wgjwhj.cn

C#:   list.Reverse();
来源：http://mc.hnjuh.cn

[D12] 查找元素下标
来源：http://dm.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://dq.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vw.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://by.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jn.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ig.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://rz.521024.cn

Ruby: arr.index(x)
来源：http://up.szsharing.cn

C#:   list.IndexOf(x);
来源：http://al.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://am.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qf.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://of.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://tq.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://fn.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://se.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://od.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fq.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ni.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://sx.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://my.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bg.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://bm.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://au.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nt.gzmigu.cn

Go:   // 手写循环
来源：http://mv.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uw.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kz.shxzukj.cn

[D15] 去重
来源：http://pe.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pp.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://vd.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://sz.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://ez.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ff.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cu.colortex.cn

Ruby: arr.uniq
来源：http://re.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://wa.szsharing.cn

[D16] 求和与平均值
来源：http://nv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pg.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zs.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://od.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tr.hahajie.cn

Go:   // 手写循环累加
来源：http://qa.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://td.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://th.huanxung.cn

[D17] 最大值与最小值
来源：http://ez.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://ma.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://du.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://by.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://qy.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bc.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zz.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ah.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://yq.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://lf.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dw.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://jf.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dp.yuexingan06.cn

TS:   nested.flat();
来源：http://rq.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dz.muxihuayi.cn

Go:   // 手写双层循环
来源：http://ej.nicolike.cn

Ruby: nested.flatten
来源：http://zk.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dr.bookmarksfly.cn

[D19] 按字段分组
来源：http://kr.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://in.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://al.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://du.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ns.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bw.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://vk.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xp.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jm.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://vr.newstarts.cn

Py:   Counter(arr)
来源：http://vk.asd995.cn

PHP:  array_count_values($arr);
来源：http://kh.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ol.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ht.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wf.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://vp.bjjhwx.cn

Ruby: arr.tally
来源：http://yq.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yd.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://ub.shtwfgs.cn

Py:   x in arr
来源：http://ov.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://eo.shtwfgs.cn

JS:   arr.includes(x)
来源：http://eo.yuexingan06.cn

TS:   arr.includes(x)
来源：http://zu.szsharing.cn

Java: list.contains(x)
来源：http://ad.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://rk.huanxung.cn

Ruby: arr.include?(x)
来源：http://vv.newstarts.cn

C#:   list.Contains(x)
来源：http://fc.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://jt.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jp.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zw.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kh.jctech888.com.cn

TS:   [...arr];
来源：http://ob.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://jq.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hd.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ib.panjiajie.cn

C#:   new List<int>(list);
来源：http://yw.jctech888.com.cn

[D23] reduce 累积计算
来源：http://ou.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://az.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eh.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bg.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rp.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rj.hnjuh.cn

Go:   // 手写循环
来源：http://df.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ud.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rk.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://wh.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ui.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ps.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tf.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wa.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pm.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oz.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gn.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gn.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://wo.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yf.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fz.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vp.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bg.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hq.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fa.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dn.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ly.huixiangedu.cn

[D26] 数组转字符串
来源：http://ah.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://go.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://qw.huixiangedu.cn

JS:   arr.join(", ")
来源：http://vb.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ip.szsharing.cn

Java: String.join(", ", list)
来源：http://im.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://dg.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://kw.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://dx.muxihuayi.cn

================================================================================
来源：http://zv.panjiajie.cn

E. 字符串处理
来源：http://xk.huixinmuqiang.cn

================================================================================
来源：http://cq.haigaiapp.cn

[E01] 拼接字符串
来源：http://es.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://om.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ya.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uv.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lc.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hf.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dc.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wx.szxytkj.cn

[E02] 重复字符串
来源：http://qr.yuexingan06.cn

Py:   "ab" * 3
来源：http://kx.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://yx.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://fn.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://td.newstarts.cn

Java: "ab".repeat(3)
来源：http://hs.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://jp.panjiajie.cn

Ruby: "ab" * 3
来源：http://py.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hp.haigaiapp.cn

[E03] 截取子串
来源：http://er.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://je.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dc.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kb.nszjky.cn

TS:   s.slice(1, 4)
来源：http://uq.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://tz.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ut.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://km.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://jh.lnxyls.cn

[E04] 查找子串位置
来源：http://bm.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://hl.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fz.hahajie.cn

TS:   s.indexOf("x")
来源：http://ah.521024.cn

Java: s.indexOf("x")
来源：http://zj.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://ey.hahajie.cn

Ruby: s.index("x")
来源：http://jr.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://oh.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://md.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gz.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ps.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sr.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tc.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oz.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zw.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mh.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pd.huixiangedu.cn

[E06] 替换子串
来源：http://rr.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ov.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://an.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zi.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://tw.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wb.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://db.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xy.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ou.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://jo.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://di.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://as.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zc.huanxung.cn

TS:   s.split(",")
来源：http://hx.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://um.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ih.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://az.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mg.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://jy.szsharing.cn

Py:   ",".join(items)
来源：http://ij.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://fa.yuntaijiaju.cn

JS:   items.join(",")
来源：http://va.lnxyls.cn

TS:   items.join(",")
来源：http://zc.haigaiapp.cn

Java: String.join(",", items)
来源：http://qy.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://bj.bookmarksfly.cn

Ruby: items.join(",")
来源：http://fs.hahajie.cn

C#:   string.Join(",", items)
来源：http://pe.panjiajie.cn

[E09] 去除所有空白字符
来源：http://ph.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ap.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hn.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://gv.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://is.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://un.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ws.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ex.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://po.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://pn.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uc.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gf.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://oi.nszjky.cn


<!-- 参考信息 -->