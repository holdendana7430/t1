代发 wailian999

Java: list.add(4);
来源：http://dm.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://ax.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://yl.bjjhwx.cn

C#:   list.Add(4);
来源：http://jt.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ed.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://pb.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cv.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://so.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ek.panjiajie.cn

Java: list.add(0, 0);
来源：http://cm.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wb.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mk.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://sn.nszjky.cn

[D04] 删除元素
来源：http://tp.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hh.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xq.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oa.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://cs.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zq.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wx.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nw.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cq.colortex.cn

[D05] 访问与修改元素
来源：http://by.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oa.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jr.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zg.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://is.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://fy.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://qg.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tv.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uu.bjjhwx.cn

[D06] 数组长度
来源：http://oi.9csxet.cn

Py:   len(arr)
来源：http://ag.shxzukj.cn

PHP:  count($arr);
来源：http://uw.bookmarksfly.cn

JS:   arr.length
来源：http://hs.gzmigu.cn

TS:   arr.length
来源：http://gb.huixiangedu.cn

Java: list.size();
来源：http://mf.panjiajie.cn

Go:   len(arr)
来源：http://qs.newstarts.cn

Ruby: arr.length; arr.size
来源：http://if.lnxyls.cn

C#:   list.Count;
来源：http://sb.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://yg.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iv.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ab.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://nx.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://mw.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://qz.9csxet.cn

Go:   arr[1:4]
来源：http://sl.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://eu.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://cf.szsharing.cn

[D08] 合并两个数组
来源：http://tv.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://jq.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://gd.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xc.newstarts.cn

TS:   [...a, ...b];
来源：http://zx.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nu.shtwfgs.cn

Go:   append(a, b...)
来源：http://md.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://xk.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ne.szsharing.cn

[D09] 排序（升序）
来源：http://gn.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://rs.newstarts.cn

PHP:  sort($arr);
来源：http://tm.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cw.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zc.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lu.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ak.shtwfgs.cn

Ruby: arr.sort
来源：http://vq.gzmigu.cn

C#:   list.Sort();
来源：http://ja.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oq.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ec.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kx.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wk.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xi.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yq.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fo.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kv.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ya.lnxyls.cn

[D11] 反转数组
来源：http://pr.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://da.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://he.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vs.521024.cn

TS:   [...arr].reverse();
来源：http://pb.shxzskj.cn

Java: Collections.reverse(list);
来源：http://lc.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://ba.chemitech.net.cn

Ruby: arr.reverse
来源：http://js.szsharing.cn

C#:   list.Reverse();
来源：http://ac.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://os.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://gq.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ex.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iy.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kr.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dm.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://wg.9csxet.cn

Ruby: arr.index(x)
来源：http://ib.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ck.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://kz.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sc.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gi.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://bx.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://vg.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mg.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ni.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ak.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ak.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://wu.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fk.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tk.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://zs.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://al.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ds.hahajie.cn

Go:   // 手写循环
来源：http://vt.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ie.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wa.huixinmuqiang.cn

[D15] 去重
来源：http://yg.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://to.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://cv.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://lx.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://dt.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ot.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sc.huanxung.cn

Ruby: arr.uniq
来源：http://ie.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://vp.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://jj.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sk.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sj.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ko.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vk.hnjuh.cn

Go:   // 手写循环累加
来源：http://rz.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ri.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ql.521024.cn

[D17] 最大值与最小值
来源：http://uz.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://nv.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://lq.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bm.hahajie.cn

TS:   Math.max(...arr);
来源：http://dr.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ee.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fj.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://pr.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://ve.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://fv.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mr.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://me.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gi.yuntaijiaju.cn

TS:   nested.flat();
来源：http://cx.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cr.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://dy.szsharing.cn

Ruby: nested.flatten
来源：http://vm.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vf.szsharing.cn

[D19] 按字段分组
来源：http://dd.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qz.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ug.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ik.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qu.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dp.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://mb.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vv.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wr.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://uu.521024.cn

Py:   Counter(arr)
来源：http://gq.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://ph.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://an.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vl.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dn.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://bw.bookmarksfly.cn

Ruby: arr.tally
来源：http://lj.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eu.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://eo.shxzukj.cn

Py:   x in arr
来源：http://rj.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://bg.newstarts.cn

JS:   arr.includes(x)
来源：http://ks.shtwfgs.cn

TS:   arr.includes(x)
来源：http://rd.shxzskj.cn

Java: list.contains(x)
来源：http://ma.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://pu.gzmigu.cn

Ruby: arr.include?(x)
来源：http://pv.jctech888.com.cn

C#:   list.Contains(x)
来源：http://rl.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://tm.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bj.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tg.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cb.colortex.cn

TS:   [...arr];
来源：http://bn.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://rb.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fw.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://fr.panjiajie.cn

C#:   new List<int>(list);
来源：http://qh.wgjwhj.cn

[D23] reduce 累积计算
来源：http://os.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gq.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mo.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kq.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://un.shxzukj.cn

Go:   // 手写循环
来源：http://ny.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zu.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oi.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://lk.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jf.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kb.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zn.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nv.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vo.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kz.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jl.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fe.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://qy.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oi.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ij.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lq.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lf.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://er.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://re.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bk.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ha.nicolike.cn

[D26] 数组转字符串
来源：http://lb.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://yf.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://mn.nicolike.cn

JS:   arr.join(", ")
来源：http://tb.wgjwhj.cn

TS:   arr.join(", ")
来源：http://tr.chemitech.net.cn

Java: String.join(", ", list)
来源：http://xw.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://tm.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://nh.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://pp.szxytkj.cn

================================================================================
来源：http://es.shxzskj.cn

E. 字符串处理
来源：http://aq.hahajie.cn

================================================================================
来源：http://qv.9csxet.cn

[E01] 拼接字符串
来源：http://hn.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sg.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wi.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ym.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ez.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kn.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://je.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dz.szxytkj.cn

[E02] 重复字符串
来源：http://fk.bjjhwx.cn

Py:   "ab" * 3
来源：http://qe.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://tv.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://fb.newstarts.cn

TS:   "ab".repeat(3)
来源：http://ra.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://jc.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://ja.jctech888.com.cn

Ruby: "ab" * 3
来源：http://xg.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sm.huanxung.cn

[E03] 截取子串
来源：http://gm.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fm.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://td.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xr.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://hi.huanxung.cn

Java: s.substring(1, 4)
来源：http://qd.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fe.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eg.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://vc.huanxung.cn

[E04] 查找子串位置
来源：http://vx.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://sj.newstarts.cn

PHP:  strpos($s, "x");
来源：http://sy.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ka.huanxung.cn

TS:   s.indexOf("x")
来源：http://ad.haigaiapp.cn

Java: s.indexOf("x")
来源：http://vw.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://ys.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://cg.nszjky.cn

C#:   s.IndexOf("x")
来源：http://km.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yy.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dm.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oq.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bu.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vm.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mg.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xs.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://df.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qp.521024.cn

[E06] 替换子串
来源：http://yb.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lb.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://mg.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lv.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://ag.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lb.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dc.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ug.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://aw.panjiajie.cn

[E07] 按分隔符拆分
来源：http://gs.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://td.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sz.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dx.muxihuayi.cn

TS:   s.split(",")
来源：http://bl.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xo.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wr.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://kv.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yu.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://vc.lnxyls.cn

Py:   ",".join(items)
来源：http://ue.lnxyls.cn

PHP:  implode(",", $items);
来源：http://lx.colortex.cn

JS:   items.join(",")
来源：http://kq.huixiangedu.cn

TS:   items.join(",")
来源：http://mp.huanxung.cn

Java: String.join(",", items)
来源：http://dx.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://yn.gzmigu.cn

Ruby: items.join(",")
来源：http://nf.hnjuh.cn

C#:   string.Join(",", items)
来源：http://rw.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://cw.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dg.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zt.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://jz.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://bg.shxzukj.cn


<!-- 参考信息 -->