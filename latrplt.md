代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qk.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hw.szsharing.cn

JS:   arr.push(4);
来源：http://lf.wgjwhj.cn

TS:   arr.push(4);
来源：http://ej.panjiajie.cn

Java: list.add(4);
来源：http://dz.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://nz.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://yr.muxihuayi.cn

C#:   list.Add(4);
来源：http://mw.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://yn.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://oa.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gt.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ko.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://wn.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://oy.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tu.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dn.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ys.shtwfgs.cn

[D04] 删除元素
来源：http://se.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dv.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dg.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jv.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ne.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://en.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dv.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kk.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hp.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://os.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kn.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pp.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ho.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://bv.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://tn.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://iy.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nm.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bg.521024.cn

[D06] 数组长度
来源：http://xs.asd995.cn

Py:   len(arr)
来源：http://ff.nszjky.cn

PHP:  count($arr);
来源：http://lb.colortex.cn

JS:   arr.length
来源：http://bq.haigaiapp.cn

TS:   arr.length
来源：http://ba.jianghongdianzi.cn

Java: list.size();
来源：http://be.nicolike.cn

Go:   len(arr)
来源：http://hu.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://yh.huixiangedu.cn

C#:   list.Count;
来源：http://wr.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://mh.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ey.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lm.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://uy.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://ej.gzmigu.cn

Java: list.subList(1, 4);
来源：http://oo.9csxet.cn

Go:   arr[1:4]
来源：http://df.szxytkj.cn

Ruby: arr[1, 3]
来源：http://bs.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://xr.hahajie.cn

[D08] 合并两个数组
来源：http://mf.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://xj.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://ca.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xp.yuexingan06.cn

TS:   [...a, ...b];
来源：http://nx.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qy.hahajie.cn

Go:   append(a, b...)
来源：http://gs.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://uv.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://sr.9csxet.cn

[D09] 排序（升序）
来源：http://pl.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ni.521024.cn

PHP:  sort($arr);
来源：http://lw.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://df.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xp.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sy.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bc.szxytkj.cn

Ruby: arr.sort
来源：http://tu.jianghongdianzi.cn

C#:   list.Sort();
来源：http://fw.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bo.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ch.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vj.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pl.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ys.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ue.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bg.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vt.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://be.muxihuayi.cn

[D11] 反转数组
来源：http://xw.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hq.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://oz.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rs.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://jt.asd995.cn

Java: Collections.reverse(list);
来源：http://yd.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ml.hahajie.cn

Ruby: arr.reverse
来源：http://gj.muxihuayi.cn

C#:   list.Reverse();
来源：http://fi.asd995.cn

[D12] 查找元素下标
来源：http://np.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://es.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://px.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fe.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mq.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pp.colortex.cn

Go:   slices.Index(arr, x)
来源：http://nr.hahajie.cn

Ruby: arr.index(x)
来源：http://hw.521024.cn

C#:   list.IndexOf(x);
来源：http://tu.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://og.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wi.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hw.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://fy.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://xj.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vp.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cm.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vk.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fi.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://iv.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pe.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qw.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://wb.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://rs.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://er.asd995.cn

Go:   // 手写循环
来源：http://si.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://js.huanxung.cn

[D15] 去重
来源：http://br.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cf.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://yq.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://dh.newstarts.cn

TS:   [...new Set(arr)]
来源：http://vj.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zu.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hh.yuexingan06.cn

Ruby: arr.uniq
来源：http://uh.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://nf.huanxung.cn

[D16] 求和与平均值
来源：http://jz.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nh.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oy.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qn.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mf.gzmigu.cn

Go:   // 手写循环累加
来源：http://pt.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uk.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://yy.shtwfgs.cn

[D17] 最大值与最小值
来源：http://qg.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ak.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://rn.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://og.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://xs.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lr.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cw.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://zb.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://qh.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://ep.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dl.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://gf.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ei.521024.cn

TS:   nested.flat();
来源：http://hd.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tb.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://nq.nicolike.cn

Ruby: nested.flatten
来源：http://df.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xk.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ed.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kp.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tb.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jk.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dt.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://st.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://ii.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sq.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lh.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://an.chemitech.net.cn

Py:   Counter(arr)
来源：http://rb.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ni.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cn.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qa.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://yk.shxzukj.cn

Ruby: arr.tally
来源：http://tc.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iq.nszjky.cn

[D21] 判断是否包含某元素
来源：http://ud.wgjwhj.cn

Py:   x in arr
来源：http://tz.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://va.huanxung.cn

JS:   arr.includes(x)
来源：http://pu.521024.cn

TS:   arr.includes(x)
来源：http://fo.shxzskj.cn

Java: list.contains(x)
来源：http://gi.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://sb.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://aq.9csxet.cn

C#:   list.Contains(x)
来源：http://nf.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ft.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hp.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://az.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jp.huanxung.cn

TS:   [...arr];
来源：http://nh.9csxet.cn

Java: new ArrayList<>(list);
来源：http://zh.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tg.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://pu.panjiajie.cn

C#:   new List<int>(list);
来源：http://kv.gzmigu.cn

[D23] reduce 累积计算
来源：http://jd.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kl.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yp.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://na.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gb.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vp.newstarts.cn

Go:   // 手写循环
来源：http://ep.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cb.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sk.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://gv.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dz.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bl.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hc.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fy.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dg.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wv.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ye.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uo.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://kp.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gt.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nd.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mm.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://da.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zw.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ba.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ti.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uc.shxzskj.cn

[D26] 数组转字符串
来源：http://lb.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://fz.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://od.nszjky.cn

JS:   arr.join(", ")
来源：http://bp.hahajie.cn

TS:   arr.join(", ")
来源：http://jd.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://os.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://mp.521024.cn

Ruby: arr.join(", ")
来源：http://zn.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://we.panjiajie.cn

================================================================================
来源：http://bq.wgjwhj.cn

E. 字符串处理
来源：http://zk.haigaiapp.cn

================================================================================
来源：http://da.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://ks.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kl.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gu.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xk.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dt.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iw.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fw.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://js.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.nicolike.cn

[E02] 重复字符串
来源：http://go.gzmigu.cn

Py:   "ab" * 3
来源：http://hs.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://rh.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://ap.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ti.newstarts.cn

Java: "ab".repeat(3)
来源：http://qs.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://bb.huanxung.cn

Ruby: "ab" * 3
来源：http://iy.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ji.521024.cn

[E03] 截取子串
来源：http://wl.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gq.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yn.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zw.huanxung.cn

TS:   s.slice(1, 4)
来源：http://xl.lnxyls.cn

Java: s.substring(1, 4)
来源：http://tz.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kl.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zx.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://qc.shtwfgs.cn

[E04] 查找子串位置
来源：http://nn.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://gk.nicolike.cn

PHP:  strpos($s, "x");
来源：http://lg.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zd.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://zz.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://su.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://wg.nszjky.cn

Ruby: s.index("x")
来源：http://js.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://ki.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uc.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lv.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gh.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bv.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fu.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mj.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gn.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cc.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wm.huixiangedu.cn

[E06] 替换子串
来源：http://rq.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tg.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://fu.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://za.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://xg.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bk.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kr.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iy.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://it.521024.cn

[E07] 按分隔符拆分
来源：http://tm.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://js.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ob.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pa.szxytkj.cn

TS:   s.split(",")
来源：http://ac.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wo.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fu.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://dx.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://if.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://ep.521024.cn

Py:   ",".join(items)
来源：http://lc.szsharing.cn

PHP:  implode(",", $items);
来源：http://fr.newstarts.cn

JS:   items.join(",")
来源：http://ph.9csxet.cn

TS:   items.join(",")
来源：http://jk.colortex.cn

Java: String.join(",", items)
来源：http://dl.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://vo.hnjuh.cn

Ruby: items.join(",")
来源：http://fb.szxytkj.cn

C#:   string.Join(",", items)
来源：http://nm.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://eq.hahajie.cn


<!-- 参考信息 -->