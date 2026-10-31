代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wg.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://af.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://iu.muxihuayi.cn

TS:   arr.push(4);
来源：http://ch.huanxung.cn

Java: list.add(4);
来源：http://qz.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://fb.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://rb.huixiangedu.cn

C#:   list.Add(4);
来源：http://yx.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ba.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://cb.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mx.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zx.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://rg.shtwfgs.cn

Java: list.add(0, 0);
来源：http://hb.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ef.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://av.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ya.shtwfgs.cn

[D04] 删除元素
来源：http://iq.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aq.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ut.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xo.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://zw.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ci.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yj.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ix.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sp.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://rc.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bo.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sm.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://di.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://au.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://cz.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://qu.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nk.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sx.yuntaijiaju.cn

[D06] 数组长度
来源：http://yn.bjjhwx.cn

Py:   len(arr)
来源：http://nx.521024.cn

PHP:  count($arr);
来源：http://cs.9csxet.cn

JS:   arr.length
来源：http://lv.muxihuayi.cn

TS:   arr.length
来源：http://ay.shtwfgs.cn

Java: list.size();
来源：http://rc.lnxyls.cn

Go:   len(arr)
来源：http://ix.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ne.hahajie.cn

C#:   list.Count;
来源：http://du.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://bz.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qh.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vd.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://dn.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://en.newstarts.cn

Java: list.subList(1, 4);
来源：http://ta.shxzskj.cn

Go:   arr[1:4]
来源：http://bl.szsharing.cn

Ruby: arr[1, 3]
来源：http://er.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://ip.lnxyls.cn

[D08] 合并两个数组
来源：http://df.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://la.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://wd.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://og.9csxet.cn

TS:   [...a, ...b];
来源：http://fi.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pi.lnxyls.cn

Go:   append(a, b...)
来源：http://cx.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://av.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://xh.shxzskj.cn

[D09] 排序（升序）
来源：http://ab.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://wm.chemitech.net.cn

PHP:  sort($arr);
来源：http://nm.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vz.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ki.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ex.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gv.yuexingan06.cn

Ruby: arr.sort
来源：http://ea.newstarts.cn

C#:   list.Sort();
来源：http://bu.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qw.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ko.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yo.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ld.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bq.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pt.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lz.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tv.nszjky.cn

[D11] 反转数组
来源：http://mr.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bp.huanxung.cn

PHP:  array_reverse($arr);
来源：http://zx.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://gp.panjiajie.cn

Java: Collections.reverse(list);
来源：http://aw.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://em.muxihuayi.cn

Ruby: arr.reverse
来源：http://np.szxytkj.cn

C#:   list.Reverse();
来源：http://iv.shxzukj.cn

[D12] 查找元素下标
来源：http://df.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://nw.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jd.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wm.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://we.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://go.colortex.cn

Go:   slices.Index(arr, x)
来源：http://yr.shtwfgs.cn

Ruby: arr.index(x)
来源：http://dt.szsharing.cn

C#:   list.IndexOf(x);
来源：http://hd.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://xu.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sc.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bj.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://sn.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://xt.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ef.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://az.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gi.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://on.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://dt.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yc.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jn.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://aa.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://bk.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fc.newstarts.cn

Go:   // 手写循环
来源：http://lt.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ts.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://du.yuexingan06.cn

[D15] 去重
来源：http://ks.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ue.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://br.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://iy.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://hq.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://om.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ia.yuexingan06.cn

Ruby: arr.uniq
来源：http://mp.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ma.newstarts.cn

[D16] 求和与平均值
来源：http://vv.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qa.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ng.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xa.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iv.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sb.gzmigu.cn

Go:   // 手写循环累加
来源：http://jg.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sc.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://qs.shtwfgs.cn

[D17] 最大值与最小值
来源：http://we.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://af.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://ec.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nc.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://it.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mt.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ag.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://fg.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://vv.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://tk.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lk.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://dv.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vm.jctech888.com.cn

TS:   nested.flat();
来源：http://xf.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yd.yuexingan06.cn

Go:   // 手写双层循环
来源：http://rc.jctech888.com.cn

Ruby: nested.flatten
来源：http://oh.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ye.yuexingan06.cn

[D19] 按字段分组
来源：http://df.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://md.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iz.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ae.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ew.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ix.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://kv.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ek.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://in.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://kv.shxzukj.cn

Py:   Counter(arr)
来源：http://ry.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://yq.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yu.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bg.9csxet.cn

Go:   // 手写 map[T]int
来源：http://jt.nszjky.cn

Ruby: arr.tally
来源：http://tg.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qk.colortex.cn

[D21] 判断是否包含某元素
来源：http://ge.huanxung.cn

Py:   x in arr
来源：http://ud.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://vy.lnxyls.cn

JS:   arr.includes(x)
来源：http://pb.jctech888.com.cn

TS:   arr.includes(x)
来源：http://vo.gzmigu.cn

Java: list.contains(x)
来源：http://az.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://bn.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://yt.szsharing.cn

C#:   list.Contains(x)
来源：http://qc.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://tk.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zx.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wp.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vp.wgjwhj.cn

TS:   [...arr];
来源：http://io.521024.cn

Java: new ArrayList<>(list);
来源：http://qg.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mx.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://nj.wgjwhj.cn

C#:   new List<int>(list);
来源：http://fq.shtwfgs.cn

[D23] reduce 累积计算
来源：http://nw.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ji.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uc.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zf.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jx.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://im.yuexingan06.cn

Go:   // 手写循环
来源：http://yd.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mg.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bg.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://gg.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ke.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ep.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zm.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lj.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cs.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eu.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mv.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ya.colortex.cn

[D25] Set 集合去重与交并差
来源：http://wt.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ji.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yg.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fq.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://us.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bm.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sq.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oe.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gs.szxytkj.cn

[D26] 数组转字符串
来源：http://rw.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://xx.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://od.hnjuh.cn

JS:   arr.join(", ")
来源：http://er.yuexingan06.cn

TS:   arr.join(", ")
来源：http://mi.bjjhwx.cn

Java: String.join(", ", list)
来源：http://en.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://nj.colortex.cn

Ruby: arr.join(", ")
来源：http://rz.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://be.bookmarksfly.cn

================================================================================
来源：http://zx.muxihuayi.cn

E. 字符串处理
来源：http://qk.nicolike.cn

================================================================================
来源：http://wp.nszjky.cn

[E01] 拼接字符串
来源：http://oa.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jr.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://os.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lp.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://os.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jm.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sx.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kc.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tr.huixiangedu.cn

[E02] 重复字符串
来源：http://te.asd995.cn

Py:   "ab" * 3
来源：http://tr.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ln.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://or.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://hu.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://la.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://et.huanxung.cn

Ruby: "ab" * 3
来源：http://oy.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sv.jctech888.com.cn

[E03] 截取子串
来源：http://hl.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://am.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ce.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vk.hahajie.cn

TS:   s.slice(1, 4)
来源：http://nx.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://sr.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uj.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rs.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://gw.szsharing.cn

[E04] 查找子串位置
来源：http://qf.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://xg.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://nx.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://la.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://jb.colortex.cn

Java: s.indexOf("x")
来源：http://xy.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://ft.szxytkj.cn

Ruby: s.index("x")
来源：http://nc.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://tc.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bl.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ko.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vm.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sp.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zv.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nt.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://le.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vd.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wk.huixiangedu.cn

[E06] 替换子串
来源：http://nn.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://om.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://br.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ku.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://og.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lj.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uw.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hn.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://wj.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://xf.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ys.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gb.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zi.hnjuh.cn

TS:   s.split(",")
来源：http://ef.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ah.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://se.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://wn.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uu.nszjky.cn

[E08] 数组按分隔符合并
来源：http://uy.bjjhwx.cn

Py:   ",".join(items)
来源：http://nt.9csxet.cn

PHP:  implode(",", $items);
来源：http://vk.jctech888.com.cn

JS:   items.join(",")
来源：http://hw.chemitech.net.cn

TS:   items.join(",")
来源：http://vq.lnxyls.cn

Java: String.join(",", items)
来源：http://ly.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://og.szsharing.cn

Ruby: items.join(",")
来源：http://vf.szxytkj.cn

C#:   string.Join(",", items)
来源：http://pm.shxzskj.cn

[E09] 去除所有空白字符
来源：http://gm.yuexingan06.cn


<!-- 参考信息 -->