代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://in.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kx.colortex.cn

JS:   arr.push(4);
来源：http://zm.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://xp.shxzskj.cn

Java: list.add(4);
来源：http://sd.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://fy.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://dr.nszjky.cn

C#:   list.Add(4);
来源：http://rs.nicolike.cn

[D03] 在指定位置插入元素
来源：http://rz.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://db.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fc.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wq.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://pz.nszjky.cn

Java: list.add(0, 0);
来源：http://ny.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xz.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wm.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ze.nszjky.cn

[D04] 删除元素
来源：http://yf.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vi.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tf.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ok.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ax.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bo.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qk.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://up.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ih.bjjhwx.cn

[D05] 访问与修改元素
来源：http://cd.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mh.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vn.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://au.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://iw.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yl.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://pk.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zb.shtwfgs.cn

[D06] 数组长度
来源：http://ck.yuntaijiaju.cn

Py:   len(arr)
来源：http://ty.hahajie.cn

PHP:  count($arr);
来源：http://ex.jianghongdianzi.cn

JS:   arr.length
来源：http://da.jianghongdianzi.cn

TS:   arr.length
来源：http://tm.szsharing.cn

Java: list.size();
来源：http://nw.szsharing.cn

Go:   len(arr)
来源：http://ym.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://mc.nszjky.cn

C#:   list.Count;
来源：http://jc.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://kk.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qa.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lk.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://if.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://id.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://ga.szxytkj.cn

Go:   arr[1:4]
来源：http://dg.nszjky.cn

Ruby: arr[1, 3]
来源：http://cq.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://hy.newstarts.cn

[D08] 合并两个数组
来源：http://pk.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://br.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://qa.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sf.chemitech.net.cn

TS:   [...a, ...b];
来源：http://dn.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ih.9csxet.cn

Go:   append(a, b...)
来源：http://fh.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://fb.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://oc.gzmigu.cn

[D09] 排序（升序）
来源：http://oz.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zb.jctech888.com.cn

PHP:  sort($arr);
来源：http://bs.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vs.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sn.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pm.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://se.lnxyls.cn

Ruby: arr.sort
来源：http://lg.lnxyls.cn

C#:   list.Sort();
来源：http://kr.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jc.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pg.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dt.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fj.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oi.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rb.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sa.wgjwhj.cn

[D11] 反转数组
来源：http://io.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uo.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://rp.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xb.nicolike.cn

TS:   [...arr].reverse();
来源：http://he.szxytkj.cn

Java: Collections.reverse(list);
来源：http://sc.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://mc.wgjwhj.cn

Ruby: arr.reverse
来源：http://xa.szsharing.cn

C#:   list.Reverse();
来源：http://rl.chemitech.net.cn

[D12] 查找元素下标
来源：http://gx.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://op.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wi.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://in.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rr.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xy.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://zm.chemitech.net.cn

Ruby: arr.index(x)
来源：http://rw.9csxet.cn

C#:   list.IndexOf(x);
来源：http://rs.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://dr.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gt.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pr.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://fl.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://xq.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://di.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://je.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nk.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://er.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://cf.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oe.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pk.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ry.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://gq.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ao.bookmarksfly.cn

Go:   // 手写循环
来源：http://ms.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qo.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pf.9csxet.cn

[D15] 去重
来源：http://gj.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wb.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://wh.hahajie.cn

JS:   [...new Set(arr)]
来源：http://ja.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://pl.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xw.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fr.521024.cn

Ruby: arr.uniq
来源：http://mf.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://qj.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://wb.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fw.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ii.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bh.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qw.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jl.yuexingan06.cn

Go:   // 手写循环累加
来源：http://qi.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://os.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://ia.nszjky.cn

[D17] 最大值与最小值
来源：http://sm.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://zg.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://gn.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wg.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ik.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zt.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ta.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://mb.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://bh.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ku.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vu.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://jv.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sk.huanxung.cn

TS:   nested.flat();
来源：http://of.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nb.jctech888.com.cn

Go:   // 手写双层循环
来源：http://db.newstarts.cn

Ruby: nested.flatten
来源：http://se.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://or.wgjwhj.cn

[D19] 按字段分组
来源：http://mg.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fg.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lu.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sh.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://en.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ig.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://qa.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zs.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://he.shxzskj.cn

Py:   Counter(arr)
来源：http://zc.szsharing.cn

PHP:  array_count_values($arr);
来源：http://fq.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mm.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fr.nszjky.cn

Go:   // 手写 map[T]int
来源：http://kf.hnjuh.cn

Ruby: arr.tally
来源：http://wj.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mo.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://ok.yuntaijiaju.cn

Py:   x in arr
来源：http://qo.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://vf.asd995.cn

JS:   arr.includes(x)
来源：http://py.muxihuayi.cn

TS:   arr.includes(x)
来源：http://hf.shxzukj.cn

Java: list.contains(x)
来源：http://pc.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://cb.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://sy.szsharing.cn

C#:   list.Contains(x)
来源：http://fm.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://ww.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yp.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lo.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hw.521024.cn

TS:   [...arr];
来源：http://ea.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://uh.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cx.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://jo.szsharing.cn

C#:   new List<int>(list);
来源：http://yj.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://cw.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://su.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xy.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yk.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kc.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oy.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ms.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cy.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://jo.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ix.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vf.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://um.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hs.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aa.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aj.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rz.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ec.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://um.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gi.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oe.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yu.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ci.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yl.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vt.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mr.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ob.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://fx.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://jq.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ij.hnjuh.cn

JS:   arr.join(", ")
来源：http://bx.shxzskj.cn

TS:   arr.join(", ")
来源：http://fp.nszjky.cn

Java: String.join(", ", list)
来源：http://fz.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://uo.9csxet.cn

Ruby: arr.join(", ")
来源：http://ew.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://gn.shtwfgs.cn

================================================================================
来源：http://vi.haigaiapp.cn

E. 字符串处理
来源：http://kg.colortex.cn

================================================================================
来源：http://jn.chemitech.net.cn

[E01] 拼接字符串
来源：http://ab.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ve.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dd.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://si.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vs.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wz.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tz.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vm.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bl.huanxung.cn

[E02] 重复字符串
来源：http://ki.9csxet.cn

Py:   "ab" * 3
来源：http://bj.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://gg.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://go.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://dq.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ac.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://kc.szsharing.cn

Ruby: "ab" * 3
来源：http://hr.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xw.haigaiapp.cn

[E03] 截取子串
来源：http://qk.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fm.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ni.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yh.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://vq.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://gc.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://of.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xc.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://wy.colortex.cn

[E04] 查找子串位置
来源：http://uy.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://bj.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://br.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qr.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://aw.hnjuh.cn

Java: s.indexOf("x")
来源：http://uj.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://zm.hnjuh.cn

Ruby: s.index("x")
来源：http://qv.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ey.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qy.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ah.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wv.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hw.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://di.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ht.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pk.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xi.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ue.nszjky.cn

[E06] 替换子串
来源：http://hm.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://st.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ke.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wi.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://zj.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gd.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lf.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ar.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://of.nszjky.cn

[E07] 按分隔符拆分
来源：http://cj.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zk.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pw.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bf.huixinmuqiang.cn

TS:   s.split(",")
来源：http://lw.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ap.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bg.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://yy.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gb.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://kn.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://wn.newstarts.cn

PHP:  implode(",", $items);
来源：http://au.chemitech.net.cn

JS:   items.join(",")
来源：http://lx.panjiajie.cn

TS:   items.join(",")
来源：http://td.bjjhwx.cn

Java: String.join(",", items)
来源：http://lc.colortex.cn

Go:   strings.Join(items, ",")
来源：http://qj.shtwfgs.cn

Ruby: items.join(",")
来源：http://rb.panjiajie.cn

C#:   string.Join(",", items)
来源：http://xa.hnjuh.cn

[E09] 去除所有空白字符
来源：http://oy.jctech888.com.cn


<!-- 参考信息 -->