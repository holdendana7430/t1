代发 wailian999

[D03] 在指定位置插入元素
来源：http://qv.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://cd.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bg.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jb.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://cv.9csxet.cn

Java: list.add(0, 0);
来源：http://hk.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nw.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://op.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://gc.shxzskj.cn

[D04] 删除元素
来源：http://hs.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qk.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xe.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wm.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://qo.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rl.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ux.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rm.hahajie.cn

[D05] 访问与修改元素
来源：http://ub.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://la.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aa.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vi.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://hs.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://nl.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://ys.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yp.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lk.szsharing.cn

[D06] 数组长度
来源：http://od.chemitech.net.cn

Py:   len(arr)
来源：http://yy.yuntaijiaju.cn

PHP:  count($arr);
来源：http://yi.bjjhwx.cn

JS:   arr.length
来源：http://va.jianghongdianzi.cn

TS:   arr.length
来源：http://pj.gzmigu.cn

Java: list.size();
来源：http://qw.nszjky.cn

Go:   len(arr)
来源：http://oj.szsharing.cn

Ruby: arr.length; arr.size
来源：http://jp.nszjky.cn

C#:   list.Count;
来源：http://ad.asd995.cn

[D07] 切片 / 取子数组
来源：http://dl.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uj.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gy.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://ep.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://va.9csxet.cn

Java: list.subList(1, 4);
来源：http://km.yuexingan06.cn

Go:   arr[1:4]
来源：http://gm.nicolike.cn

Ruby: arr[1, 3]
来源：http://fw.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ri.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ex.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://mh.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://km.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vl.huixiangedu.cn

TS:   [...a, ...b];
来源：http://gh.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jr.wgjwhj.cn

Go:   append(a, b...)
来源：http://os.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://xc.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://jn.nszjky.cn

[D09] 排序（升序）
来源：http://sk.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qp.huanxung.cn

PHP:  sort($arr);
来源：http://ev.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ur.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cv.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cb.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bo.haigaiapp.cn

Ruby: arr.sort
来源：http://kp.panjiajie.cn

C#:   list.Sort();
来源：http://ne.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yd.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qn.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wo.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yq.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ch.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ng.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sw.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://el.521024.cn

[D11] 反转数组
来源：http://ne.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xg.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://tk.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ch.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://bf.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://nl.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://sy.shxzskj.cn

Ruby: arr.reverse
来源：http://wy.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://dj.wgjwhj.cn

[D12] 查找元素下标
来源：http://fm.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://kq.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zu.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qd.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dn.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qc.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://yt.lnxyls.cn

Ruby: arr.index(x)
来源：http://wp.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ar.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ar.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bd.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gl.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://jb.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://lp.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qd.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ts.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qs.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tl.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://rm.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xw.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gs.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://iw.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://ie.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hq.9csxet.cn

Go:   // 手写循环
来源：http://rx.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ya.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jj.muxihuayi.cn

[D15] 去重
来源：http://ec.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ii.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://ez.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://ye.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://qp.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bq.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ag.huixiangedu.cn

Ruby: arr.uniq
来源：http://xd.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://oi.asd995.cn

[D16] 求和与平均值
来源：http://my.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vd.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kj.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fi.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bn.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wg.szxytkj.cn

Go:   // 手写循环累加
来源：http://ti.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fl.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://iq.nicolike.cn

[D17] 最大值与最小值
来源：http://uz.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://va.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://gl.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rg.521024.cn

TS:   Math.max(...arr);
来源：http://kl.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uk.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rz.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://at.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ac.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://ym.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qu.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://pe.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wg.newstarts.cn

TS:   nested.flat();
来源：http://sg.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://as.huixiangedu.cn

Go:   // 手写双层循环
来源：http://en.colortex.cn

Ruby: nested.flatten
来源：http://bm.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tb.521024.cn

[D19] 按字段分组
来源：http://rs.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ph.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://so.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hc.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ta.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kk.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://dd.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ho.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://md.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://mc.jctech888.com.cn

Py:   Counter(arr)
来源：http://gm.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://hb.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ma.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wp.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://es.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://sf.gzmigu.cn

Ruby: arr.tally
来源：http://rp.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mm.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://zv.huixinmuqiang.cn

Py:   x in arr
来源：http://jz.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://wp.hnjuh.cn

JS:   arr.includes(x)
来源：http://aa.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://us.szsharing.cn

Java: list.contains(x)
来源：http://gk.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://zp.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ec.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://nt.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://kz.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ak.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aa.bookmarksfly.cn

TS:   [...arr];
来源：http://zv.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://pc.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://on.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://cl.yuexingan06.cn

C#:   new List<int>(list);
来源：http://ui.szsharing.cn

[D23] reduce 累积计算
来源：http://ww.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tq.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wo.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xy.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://up.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ux.lnxyls.cn

Go:   // 手写循环
来源：http://yc.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vl.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ug.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://dl.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pa.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xd.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ub.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nu.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zo.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bk.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kl.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dk.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://px.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ig.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fy.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tq.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gi.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cp.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nz.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cd.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dw.huixiangedu.cn

[D26] 数组转字符串
来源：http://mg.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://vn.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://lg.gzmigu.cn

JS:   arr.join(", ")
来源：http://xm.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ae.hahajie.cn

Java: String.join(", ", list)
来源：http://tu.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://sg.9csxet.cn

Ruby: arr.join(", ")
来源：http://dz.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://xl.panjiajie.cn

================================================================================
来源：http://ul.shxzukj.cn

E. 字符串处理
来源：http://xh.huanxung.cn

================================================================================
来源：http://ix.bookmarksfly.cn

[E01] 拼接字符串
来源：http://kn.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://np.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ee.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qo.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dp.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dv.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sm.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dm.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fr.hnjuh.cn

[E02] 重复字符串
来源：http://xk.hnjuh.cn

Py:   "ab" * 3
来源：http://wf.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://od.colortex.cn

JS:   "ab".repeat(3)
来源：http://cy.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://oc.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://tk.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://fg.hahajie.cn

Ruby: "ab" * 3
来源：http://pr.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ns.hahajie.cn

[E03] 截取子串
来源：http://zr.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zq.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ku.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eq.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://ch.huanxung.cn

Java: s.substring(1, 4)
来源：http://sr.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kk.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dl.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://ms.nicolike.cn

[E04] 查找子串位置
来源：http://ys.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://vz.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://ms.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rn.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ue.yuexingan06.cn

Java: s.indexOf("x")
来源：http://va.asd995.cn

Go:   strings.Index(s, "x")
来源：http://gv.yuexingan06.cn

Ruby: s.index("x")
来源：http://as.nicolike.cn

C#:   s.IndexOf("x")
来源：http://rj.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ct.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pf.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jf.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zi.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yx.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ij.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aj.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vj.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qh.muxihuayi.cn

[E06] 替换子串
来源：http://ew.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bu.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ut.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ku.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://ix.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nt.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iv.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xi.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://cy.lnxyls.cn

[E07] 按分隔符拆分
来源：http://dg.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uy.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sk.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ad.521024.cn

TS:   s.split(",")
来源：http://kz.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xy.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mp.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://vu.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sr.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://wz.szxytkj.cn

Py:   ",".join(items)
来源：http://yy.lnxyls.cn

PHP:  implode(",", $items);
来源：http://kn.yuntaijiaju.cn

JS:   items.join(",")
来源：http://nu.shtwfgs.cn

TS:   items.join(",")
来源：http://ph.bjjhwx.cn

Java: String.join(",", items)
来源：http://tp.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://jz.jctech888.com.cn

Ruby: items.join(",")
来源：http://fz.shxzukj.cn

C#:   string.Join(",", items)
来源：http://pd.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://md.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nl.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://du.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://cx.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ye.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://bh.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://si.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://na.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rg.hnjuh.cn


<!-- 参考信息 -->