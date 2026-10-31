代发 wailian999

[D03] 在指定位置插入元素
来源：http://ba.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://dm.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dp.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gi.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://jx.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://gm.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yn.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sf.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://zo.wgjwhj.cn

[D04] 删除元素
来源：http://qo.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mw.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ts.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lt.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://ou.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vc.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ty.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bg.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://de.muxihuayi.cn

[D05] 访问与修改元素
来源：http://bf.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://td.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ne.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sy.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ug.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://yt.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://de.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kv.asd995.cn

[D06] 数组长度
来源：http://ry.nszjky.cn

Py:   len(arr)
来源：http://ju.jctech888.com.cn

PHP:  count($arr);
来源：http://kq.colortex.cn

JS:   arr.length
来源：http://vd.panjiajie.cn

TS:   arr.length
来源：http://bq.yuntaijiaju.cn

Java: list.size();
来源：http://wf.huixiangedu.cn

Go:   len(arr)
来源：http://bj.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://eq.bjjhwx.cn

C#:   list.Count;
来源：http://gk.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://yp.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ih.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xw.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://ag.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://bq.panjiajie.cn

Java: list.subList(1, 4);
来源：http://bq.colortex.cn

Go:   arr[1:4]
来源：http://hp.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://uk.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://zj.haigaiapp.cn

[D08] 合并两个数组
来源：http://hn.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://xj.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://qb.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gl.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://jo.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://di.huanxung.cn

Go:   append(a, b...)
来源：http://ee.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://xl.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://ec.wgjwhj.cn

[D09] 排序（升序）
来源：http://jm.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.colortex.cn

PHP:  sort($arr);
来源：http://pv.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rd.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lr.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dl.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oa.huixinmuqiang.cn

Ruby: arr.sort
来源：http://af.hnjuh.cn

C#:   list.Sort();
来源：http://qw.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://em.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wl.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zy.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qn.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ye.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fn.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rl.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qd.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://up.yuntaijiaju.cn

[D11] 反转数组
来源：http://zu.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qa.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://jz.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wy.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://ex.lnxyls.cn

Java: Collections.reverse(list);
来源：http://vf.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://xb.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://uu.nicolike.cn

C#:   list.Reverse();
来源：http://yl.colortex.cn

[D12] 查找元素下标
来源：http://zg.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://kg.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ij.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hp.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gh.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yj.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://pz.panjiajie.cn

Ruby: arr.index(x)
来源：http://sp.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://vp.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://on.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oh.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qr.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://xz.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://vf.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://su.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rt.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://im.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mh.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://lx.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ba.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xt.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://zf.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://uh.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zh.jianghongdianzi.cn

Go:   // 手写循环
来源：http://nm.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ux.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://et.jianghongdianzi.cn

[D15] 去重
来源：http://uk.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wq.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://pn.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ih.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://al.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ob.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bv.nicolike.cn

Ruby: arr.uniq
来源：http://qa.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://nz.lnxyls.cn

[D16] 求和与平均值
来源：http://wi.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oq.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rm.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pm.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kc.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://al.9csxet.cn

Go:   // 手写循环累加
来源：http://bp.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xz.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://fo.bjjhwx.cn

[D17] 最大值与最小值
来源：http://uf.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://vh.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://cs.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pq.asd995.cn

TS:   Math.max(...arr);
来源：http://on.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uw.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vq.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://kz.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://lg.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://zj.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ab.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://tx.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://er.huixinmuqiang.cn

TS:   nested.flat();
来源：http://bg.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ut.huixiangedu.cn

Go:   // 手写双层循环
来源：http://pw.yuexingan06.cn

Ruby: nested.flatten
来源：http://lp.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://va.jctech888.com.cn

[D19] 按字段分组
来源：http://zw.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ic.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aj.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tu.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://da.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hd.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://yl.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eb.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fx.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://ko.szxytkj.cn

Py:   Counter(arr)
来源：http://op.asd995.cn

PHP:  array_count_values($arr);
来源：http://be.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vf.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pe.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mf.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ve.jianghongdianzi.cn

Ruby: arr.tally
来源：http://dh.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pc.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://zq.yuntaijiaju.cn

Py:   x in arr
来源：http://qv.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://bz.jctech888.com.cn

JS:   arr.includes(x)
来源：http://ha.shxzukj.cn

TS:   arr.includes(x)
来源：http://rm.newstarts.cn

Java: list.contains(x)
来源：http://ze.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://my.shxzukj.cn

Ruby: arr.include?(x)
来源：http://hf.chemitech.net.cn

C#:   list.Contains(x)
来源：http://zs.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://ne.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ds.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ca.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jq.yuexingan06.cn

TS:   [...arr];
来源：http://mx.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://el.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yd.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://iq.521024.cn

C#:   new List<int>(list);
来源：http://ce.shtwfgs.cn

[D23] reduce 累积计算
来源：http://lg.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eo.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aw.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dk.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mt.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lp.9csxet.cn

Go:   // 手写循环
来源：http://bd.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ph.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ge.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://vm.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://za.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vk.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ij.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pt.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://st.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://am.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tm.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://or.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ff.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nu.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nm.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cw.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://me.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wl.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xy.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xd.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://td.huixiangedu.cn

[D26] 数组转字符串
来源：http://zb.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://qd.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://vi.szsharing.cn

JS:   arr.join(", ")
来源：http://ll.colortex.cn

TS:   arr.join(", ")
来源：http://yj.wgjwhj.cn

Java: String.join(", ", list)
来源：http://na.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://jc.asd995.cn

Ruby: arr.join(", ")
来源：http://yk.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://oq.shtwfgs.cn

================================================================================
来源：http://uk.bjjhwx.cn

E. 字符串处理
来源：http://dv.chemitech.net.cn

================================================================================
来源：http://gb.lnxyls.cn

[E01] 拼接字符串
来源：http://ml.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://im.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xq.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ov.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rg.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nq.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gk.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vm.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://of.shxzukj.cn

[E02] 重复字符串
来源：http://as.colortex.cn

Py:   "ab" * 3
来源：http://ja.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://xf.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://vm.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://sw.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://vy.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://hw.chemitech.net.cn

Ruby: "ab" * 3
来源：http://xw.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://en.muxihuayi.cn

[E03] 截取子串
来源：http://no.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sf.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ts.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ea.9csxet.cn

TS:   s.slice(1, 4)
来源：http://hb.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://ww.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ry.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rx.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://gb.9csxet.cn

[E04] 查找子串位置
来源：http://aa.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://co.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://re.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yc.gzmigu.cn

TS:   s.indexOf("x")
来源：http://sr.colortex.cn

Java: s.indexOf("x")
来源：http://gt.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://hg.haigaiapp.cn

Ruby: s.index("x")
来源：http://cf.szsharing.cn

C#:   s.IndexOf("x")
来源：http://fu.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xf.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://de.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://au.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nc.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fx.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kk.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rr.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gx.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mu.szsharing.cn

[E06] 替换子串
来源：http://hm.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ir.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ju.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://lg.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ok.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kx.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xg.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://xl.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://vb.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uj.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vp.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mh.yuntaijiaju.cn

TS:   s.split(",")
来源：http://yg.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://br.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gs.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://vf.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ps.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://xi.haigaiapp.cn

Py:   ",".join(items)
来源：http://nx.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://ey.shxzukj.cn

JS:   items.join(",")
来源：http://mj.nszjky.cn

TS:   items.join(",")
来源：http://aa.gzmigu.cn

Java: String.join(",", items)
来源：http://bc.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://gh.szsharing.cn

Ruby: items.join(",")
来源：http://iu.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://kq.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://xk.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://af.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xz.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://qj.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://yi.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ba.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bh.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ty.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gj.bjjhwx.cn


<!-- 参考信息 -->