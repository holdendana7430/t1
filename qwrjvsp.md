代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://db.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://er.szxytkj.cn

JS:   arr.push(4);
来源：http://oo.haigaiapp.cn

TS:   arr.push(4);
来源：http://bs.szsharing.cn

Java: list.add(4);
来源：http://qt.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ez.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://pt.wgjwhj.cn

C#:   list.Add(4);
来源：http://al.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://tu.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://jb.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mv.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hv.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://xq.nszjky.cn

Java: list.add(0, 0);
来源：http://ol.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fc.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yr.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ia.jianghongdianzi.cn

[D04] 删除元素
来源：http://rv.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vd.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oa.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pg.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://er.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eg.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ox.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nd.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tl.huixiangedu.cn

[D05] 访问与修改元素
来源：http://pd.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ft.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ue.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tn.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://aw.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://bn.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://bk.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ck.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qo.nszjky.cn

[D06] 数组长度
来源：http://md.huixiangedu.cn

Py:   len(arr)
来源：http://gt.haigaiapp.cn

PHP:  count($arr);
来源：http://tm.shxzskj.cn

JS:   arr.length
来源：http://zs.hnjuh.cn

TS:   arr.length
来源：http://jw.panjiajie.cn

Java: list.size();
来源：http://sb.colortex.cn

Go:   len(arr)
来源：http://qp.szsharing.cn

Ruby: arr.length; arr.size
来源：http://td.nszjky.cn

C#:   list.Count;
来源：http://aj.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://qn.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lk.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xh.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://dz.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://cr.9csxet.cn

Java: list.subList(1, 4);
来源：http://gj.bookmarksfly.cn

Go:   arr[1:4]
来源：http://sg.hnjuh.cn

Ruby: arr[1, 3]
来源：http://ht.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://gz.gzmigu.cn

[D08] 合并两个数组
来源：http://yb.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://in.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://fj.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mz.521024.cn

TS:   [...a, ...b];
来源：http://mc.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ea.huixiangedu.cn

Go:   append(a, b...)
来源：http://mj.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://jj.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://gj.hahajie.cn

[D09] 排序（升序）
来源：http://je.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://np.newstarts.cn

PHP:  sort($arr);
来源：http://nq.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wk.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rv.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://et.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iu.nicolike.cn

Ruby: arr.sort
来源：http://eb.hnjuh.cn

C#:   list.Sort();
来源：http://oh.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aj.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wd.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ng.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ne.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fi.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tc.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jd.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ub.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cg.szsharing.cn

[D11] 反转数组
来源：http://pk.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lu.hahajie.cn

PHP:  array_reverse($arr);
来源：http://mm.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xd.gzmigu.cn

TS:   [...arr].reverse();
来源：http://fj.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://nd.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ob.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ik.asd995.cn

C#:   list.Reverse();
来源：http://hi.jctech888.com.cn

[D12] 查找元素下标
来源：http://bs.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://pw.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pi.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jf.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nc.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://kx.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://ck.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://jl.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://dz.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qe.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wi.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://bg.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://sk.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yv.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ip.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kd.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://px.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://qw.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jb.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uq.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://de.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://hy.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ul.521024.cn

Go:   // 手写循环
来源：http://ld.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mb.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://au.szxytkj.cn

[D15] 去重
来源：http://rk.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://js.panjiajie.cn

PHP:  array_unique($arr);
来源：http://es.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://tl.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://ep.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uf.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ja.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://ih.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://ke.jctech888.com.cn

[D16] 求和与平均值
来源：http://bd.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://do.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://if.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kd.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zf.hnjuh.cn

Go:   // 手写循环累加
来源：http://zo.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rn.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://no.muxihuayi.cn

[D17] 最大值与最小值
来源：http://rq.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://lm.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://qz.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sp.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://qd.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sc.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ld.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://iu.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://bw.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://mz.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mc.colortex.cn

PHP:  array_merge(...$nested);
来源：http://yu.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jy.muxihuayi.cn

TS:   nested.flat();
来源：http://lj.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ry.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ez.huixiangedu.cn

Ruby: nested.flatten
来源：http://gg.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hf.hahajie.cn

[D19] 按字段分组
来源：http://yk.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sl.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yp.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pz.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tu.521024.cn

Go:   // 手写 map[string][]T
来源：http://ja.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qu.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://as.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://jg.shtwfgs.cn

Py:   Counter(arr)
来源：http://gj.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://tf.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ld.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ix.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://wp.hahajie.cn

Ruby: arr.tally
来源：http://fr.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sw.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://tz.wgjwhj.cn

Py:   x in arr
来源：http://gd.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://sm.colortex.cn

JS:   arr.includes(x)
来源：http://oy.huixiangedu.cn

TS:   arr.includes(x)
来源：http://mo.newstarts.cn

Java: list.contains(x)
来源：http://ga.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://cy.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://fg.9csxet.cn

C#:   list.Contains(x)
来源：http://ht.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ly.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ho.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://el.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kq.9csxet.cn

TS:   [...arr];
来源：http://xj.nszjky.cn

Java: new ArrayList<>(list);
来源：http://sl.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zd.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ac.nszjky.cn

C#:   new List<int>(list);
来源：http://zj.yuexingan06.cn

[D23] reduce 累积计算
来源：http://pp.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zr.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mj.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gx.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rc.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pq.shtwfgs.cn

Go:   // 手写循环
来源：http://oi.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vt.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mf.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://hi.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://su.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sl.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://za.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://in.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tq.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nr.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eq.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://dj.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qk.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kj.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jw.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jq.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uw.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nn.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ku.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dk.bookmarksfly.cn

[D26] 数组转字符串
来源：http://eb.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://km.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://xm.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://us.colortex.cn

TS:   arr.join(", ")
来源：http://cj.haigaiapp.cn

Java: String.join(", ", list)
来源：http://du.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://fd.9csxet.cn

Ruby: arr.join(", ")
来源：http://sa.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://gv.yuntaijiaju.cn

================================================================================
来源：http://ri.lnxyls.cn

E. 字符串处理
来源：http://lv.chemitech.net.cn

================================================================================
来源：http://gh.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://vh.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rl.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hh.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://do.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mz.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zf.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yc.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ja.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://io.muxihuayi.cn

[E02] 重复字符串
来源：http://mv.szsharing.cn

Py:   "ab" * 3
来源：http://fx.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.colortex.cn

JS:   "ab".repeat(3)
来源：http://os.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://if.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://bt.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://gl.huanxung.cn

Ruby: "ab" * 3
来源：http://tp.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ab.bookmarksfly.cn

[E03] 截取子串
来源：http://qa.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ns.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cv.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yf.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://cx.nicolike.cn

Java: s.substring(1, 4)
来源：http://dh.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qa.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dk.asd995.cn

C#:   s.Substring(1, 3)
来源：http://jj.lnxyls.cn

[E04] 查找子串位置
来源：http://tn.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://us.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://dk.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ib.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ld.szxytkj.cn

Java: s.indexOf("x")
来源：http://qc.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://iz.521024.cn

Ruby: s.index("x")
来源：http://lf.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://ss.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bx.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ye.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fb.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://me.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zb.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tt.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ep.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yf.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ur.lnxyls.cn

[E06] 替换子串
来源：http://wv.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mv.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://fc.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kj.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://ow.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zr.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://km.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://th.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://ew.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://cu.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kn.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lc.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hk.lnxyls.cn

TS:   s.split(",")
来源：http://dy.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dc.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://za.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://md.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dg.asd995.cn

[E08] 数组按分隔符合并
来源：http://nk.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://zb.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://xf.bjjhwx.cn

JS:   items.join(",")
来源：http://oz.colortex.cn

TS:   items.join(",")
来源：http://qu.newstarts.cn

Java: String.join(",", items)
来源：http://xx.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://cg.chemitech.net.cn

Ruby: items.join(",")
来源：http://jr.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://yy.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://xf.colortex.cn


<!-- 参考信息 -->