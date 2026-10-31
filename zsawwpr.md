代发 wailian999

Java: list.add(4);
来源：http://gz.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://cr.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://he.gzmigu.cn

C#:   list.Add(4);
来源：http://xb.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://mk.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://fb.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ai.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ct.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://tk.haigaiapp.cn

Java: list.add(0, 0);
来源：http://wb.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vi.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bf.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://gp.bjjhwx.cn

[D04] 删除元素
来源：http://lr.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lv.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://on.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tb.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://xe.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fr.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uo.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xd.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://er.newstarts.cn

[D05] 访问与修改元素
来源：http://mg.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sn.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aq.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ke.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://pb.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://aw.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://iq.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kj.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kp.wgjwhj.cn

[D06] 数组长度
来源：http://dn.haigaiapp.cn

Py:   len(arr)
来源：http://ua.wgjwhj.cn

PHP:  count($arr);
来源：http://xv.bjjhwx.cn

JS:   arr.length
来源：http://kh.chemitech.net.cn

TS:   arr.length
来源：http://kg.shxzukj.cn

Java: list.size();
来源：http://zd.521024.cn

Go:   len(arr)
来源：http://ak.nicolike.cn

Ruby: arr.length; arr.size
来源：http://kp.haigaiapp.cn

C#:   list.Count;
来源：http://ji.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://pn.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ko.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://em.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://wv.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://bv.asd995.cn

Java: list.subList(1, 4);
来源：http://je.bjjhwx.cn

Go:   arr[1:4]
来源：http://co.asd995.cn

Ruby: arr[1, 3]
来源：http://wf.521024.cn

C#:   list.GetRange(1, 3);
来源：http://zc.wgjwhj.cn

[D08] 合并两个数组
来源：http://qz.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://nj.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://op.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aj.gzmigu.cn

TS:   [...a, ...b];
来源：http://sa.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ss.hahajie.cn

Go:   append(a, b...)
来源：http://tg.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://um.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://gd.haigaiapp.cn

[D09] 排序（升序）
来源：http://ac.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://rb.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ea.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ov.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rz.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://es.nicolike.cn

Ruby: arr.sort
来源：http://mi.lnxyls.cn

C#:   list.Sort();
来源：http://wz.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://im.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cu.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sa.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rz.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://co.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fn.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ph.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xb.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://da.lnxyls.cn

[D11] 反转数组
来源：http://mx.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yv.nszjky.cn

PHP:  array_reverse($arr);
来源：http://va.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ty.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ru.colortex.cn

Java: Collections.reverse(list);
来源：http://uq.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://oa.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://zd.nszjky.cn

C#:   list.Reverse();
来源：http://ds.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://lg.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://tu.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bp.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cn.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ax.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ng.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://qr.jctech888.com.cn

Ruby: arr.index(x)
来源：http://py.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://qf.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://br.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pw.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vs.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://wr.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://tn.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ps.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lr.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xd.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yz.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://aa.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rj.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://np.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://jp.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://nj.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ll.wgjwhj.cn

Go:   // 手写循环
来源：http://mm.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tk.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jr.huanxung.cn

[D15] 去重
来源：http://yf.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ly.shxzskj.cn

PHP:  array_unique($arr);
来源：http://im.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://nq.nszjky.cn

TS:   [...new Set(arr)]
来源：http://yy.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xm.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gt.asd995.cn

Ruby: arr.uniq
来源：http://gv.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://wk.panjiajie.cn

[D16] 求和与平均值
来源：http://na.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bg.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hl.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yp.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fs.szxytkj.cn

Go:   // 手写循环累加
来源：http://nj.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jj.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://yp.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://kg.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://sc.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://qc.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hj.521024.cn

TS:   Math.max(...arr);
来源：http://oh.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sx.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ov.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://iv.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://zp.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://yk.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jn.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://un.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ie.huixinmuqiang.cn

TS:   nested.flat();
来源：http://fn.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qh.wgjwhj.cn

Go:   // 手写双层循环
来源：http://cm.521024.cn

Ruby: nested.flatten
来源：http://uu.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://px.muxihuayi.cn

[D19] 按字段分组
来源：http://sq.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kn.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aa.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xc.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ph.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://na.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://fl.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fd.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hu.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://vf.nszjky.cn

Py:   Counter(arr)
来源：http://hw.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://qt.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ad.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oa.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ub.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://hs.shxzskj.cn

Ruby: arr.tally
来源：http://ur.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fc.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://xx.colortex.cn

Py:   x in arr
来源：http://qb.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://qq.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://se.9csxet.cn

TS:   arr.includes(x)
来源：http://ed.asd995.cn

Java: list.contains(x)
来源：http://xm.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://cp.newstarts.cn

Ruby: arr.include?(x)
来源：http://bf.huanxung.cn

C#:   list.Contains(x)
来源：http://ae.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://kv.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cs.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zk.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oq.521024.cn

TS:   [...arr];
来源：http://lc.nicolike.cn

Java: new ArrayList<>(list);
来源：http://wa.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ln.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://fz.hnjuh.cn

C#:   new List<int>(list);
来源：http://za.huanxung.cn

[D23] reduce 累积计算
来源：http://ww.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pu.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ax.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kp.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pz.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://to.hahajie.cn

Go:   // 手写循环
来源：http://xw.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gd.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ts.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://oo.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jl.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qz.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zz.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pf.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lj.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qs.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kk.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pd.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://vg.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qf.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jh.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fk.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://js.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rz.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pi.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fd.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ix.huixiangedu.cn

[D26] 数组转字符串
来源：http://lw.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://gu.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://fk.colortex.cn

JS:   arr.join(", ")
来源：http://jp.hnjuh.cn

TS:   arr.join(", ")
来源：http://fk.newstarts.cn

Java: String.join(", ", list)
来源：http://jd.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://vv.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ud.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://kx.muxihuayi.cn

================================================================================
来源：http://gj.jianghongdianzi.cn

E. 字符串处理
来源：http://os.panjiajie.cn

================================================================================
来源：http://pi.haigaiapp.cn

[E01] 拼接字符串
来源：http://ds.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lr.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xp.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ss.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rj.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dt.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gw.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lw.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tx.yuntaijiaju.cn

[E02] 重复字符串
来源：http://jn.521024.cn

Py:   "ab" * 3
来源：http://pz.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://mi.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://dy.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://bx.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ih.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://qc.yuexingan06.cn

Ruby: "ab" * 3
来源：http://zh.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://br.hahajie.cn

[E03] 截取子串
来源：http://wh.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mk.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ko.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fj.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://us.shxzukj.cn

Java: s.substring(1, 4)
来源：http://fx.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cy.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fn.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://vn.colortex.cn

[E04] 查找子串位置
来源：http://po.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ab.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://xj.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lp.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://fi.newstarts.cn

Java: s.indexOf("x")
来源：http://po.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://pe.szxytkj.cn

Ruby: s.index("x")
来源：http://ia.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://nh.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kn.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ss.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fq.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zd.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zi.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ze.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://il.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ap.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pw.521024.cn

[E06] 替换子串
来源：http://yw.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://an.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://yy.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ly.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://si.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ba.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wh.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://xu.szsharing.cn

[E07] 按分隔符拆分
来源：http://nh.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mt.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pd.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qb.wgjwhj.cn

TS:   s.split(",")
来源：http://qf.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xq.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ix.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://vq.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lo.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://rf.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://fx.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://zn.szsharing.cn

JS:   items.join(",")
来源：http://nq.hnjuh.cn

TS:   items.join(",")
来源：http://yp.jctech888.com.cn

Java: String.join(",", items)
来源：http://vx.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ak.szxytkj.cn

Ruby: items.join(",")
来源：http://cq.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ss.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://nb.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gv.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mw.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://tm.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://aw.hnjuh.cn


<!-- 参考信息 -->