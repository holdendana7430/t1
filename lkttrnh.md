代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://qp.gzmigu.cn

Java: list.add(0, 0);
来源：http://ns.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nv.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wd.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://gr.jianghongdianzi.cn

[D04] 删除元素
来源：http://ge.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sw.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mn.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ea.521024.cn

TS:   arr.splice(0, 1);
来源：http://il.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dp.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gg.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://va.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yg.wgjwhj.cn

[D05] 访问与修改元素
来源：http://zv.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iz.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zc.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vq.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://lr.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://jb.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://kw.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://su.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aa.colortex.cn

[D06] 数组长度
来源：http://sk.bjjhwx.cn

Py:   len(arr)
来源：http://nz.huanxung.cn

PHP:  count($arr);
来源：http://gb.haigaiapp.cn

JS:   arr.length
来源：http://rz.9csxet.cn

TS:   arr.length
来源：http://la.muxihuayi.cn

Java: list.size();
来源：http://zs.hahajie.cn

Go:   len(arr)
来源：http://di.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://xl.wgjwhj.cn

C#:   list.Count;
来源：http://wx.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://da.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jp.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vy.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://bp.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://if.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://hj.newstarts.cn

Go:   arr[1:4]
来源：http://vn.asd995.cn

Ruby: arr[1, 3]
来源：http://ag.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://nu.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://if.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://ad.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://nx.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ex.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://uy.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fq.muxihuayi.cn

Go:   append(a, b...)
来源：http://dg.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://ie.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://yq.szsharing.cn

[D09] 排序（升序）
来源：http://hl.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://hs.shxzukj.cn

PHP:  sort($arr);
来源：http://rl.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jq.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://op.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cf.yuntaijiaju.cn

Ruby: arr.sort
来源：http://nv.521024.cn

C#:   list.Sort();
来源：http://kx.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pl.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yz.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zv.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gb.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pw.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kn.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vr.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://np.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jn.newstarts.cn

[D11] 反转数组
来源：http://iw.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ex.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://nc.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lt.shxzukj.cn

TS:   [...arr].reverse();
来源：http://he.shxzskj.cn

Java: Collections.reverse(list);
来源：http://rt.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://uv.bookmarksfly.cn

Ruby: arr.reverse
来源：http://tj.huanxung.cn

C#:   list.Reverse();
来源：http://zn.9csxet.cn

[D12] 查找元素下标
来源：http://fh.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://cy.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uz.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fq.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sc.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://mz.panjiajie.cn

Ruby: arr.index(x)
来源：http://rn.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://vz.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://xm.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ej.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sk.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://gs.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://dt.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ds.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uq.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oa.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fy.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://gl.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ii.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eg.521024.cn

JS:   arr.map(x => x * 2)
来源：http://yl.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://gr.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wl.9csxet.cn

Go:   // 手写循环
来源：http://bn.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qm.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ld.lnxyls.cn

[D15] 去重
来源：http://qi.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pt.panjiajie.cn

PHP:  array_unique($arr);
来源：http://bs.newstarts.cn

JS:   [...new Set(arr)]
来源：http://jw.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://qw.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ln.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fw.bjjhwx.cn

Ruby: arr.uniq
来源：http://pj.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://bu.wgjwhj.cn

[D16] 求和与平均值
来源：http://hm.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oj.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://av.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ud.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lk.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xc.jctech888.com.cn

Go:   // 手写循环累加
来源：http://ho.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pv.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://hh.nszjky.cn

[D17] 最大值与最小值
来源：http://we.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://rb.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://mu.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eu.521024.cn

TS:   Math.max(...arr);
来源：http://us.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zs.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://og.asd995.cn

Ruby: arr.max;  arr.min
来源：http://gv.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://ks.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://rx.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://od.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://pr.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mz.jianghongdianzi.cn

TS:   nested.flat();
来源：http://tf.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bw.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://wc.hahajie.cn

Ruby: nested.flatten
来源：http://fl.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bv.lnxyls.cn

[D19] 按字段分组
来源：http://oj.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xa.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qh.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lb.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nz.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tw.521024.cn

Go:   // 手写 map[string][]T
来源：http://vw.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aa.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://br.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://jp.yuexingan06.cn

Py:   Counter(arr)
来源：http://tx.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://xe.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lw.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dz.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ei.haigaiapp.cn

Ruby: arr.tally
来源：http://vf.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://go.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ia.gzmigu.cn

Py:   x in arr
来源：http://xf.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://dm.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://av.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://kf.asd995.cn

Java: list.contains(x)
来源：http://kc.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://vx.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://ul.shxzskj.cn

C#:   list.Contains(x)
来源：http://vn.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ya.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eg.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ea.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://do.nszjky.cn

TS:   [...arr];
来源：http://mt.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://vr.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fa.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://ev.bjjhwx.cn

C#:   new List<int>(list);
来源：http://hl.szxytkj.cn

[D23] reduce 累积计算
来源：http://yb.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gn.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fe.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://se.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mf.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ih.gzmigu.cn

Go:   // 手写循环
来源：http://vb.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ox.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ll.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://yi.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ob.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dj.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jq.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ff.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qe.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://db.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fr.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vv.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://il.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ia.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nz.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sz.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://so.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zs.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wk.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cg.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ia.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://tv.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://px.asd995.cn

PHP:  implode(", ", $arr);
来源：http://qn.gzmigu.cn

JS:   arr.join(", ")
来源：http://is.hahajie.cn

TS:   arr.join(", ")
来源：http://pp.haigaiapp.cn

Java: String.join(", ", list)
来源：http://gh.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://em.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://zm.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://zj.shxzskj.cn

================================================================================
来源：http://kv.jctech888.com.cn

E. 字符串处理
来源：http://xg.shtwfgs.cn

================================================================================
来源：http://du.gzmigu.cn

[E01] 拼接字符串
来源：http://uc.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rb.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://li.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zw.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xu.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vq.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rf.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ho.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gq.hnjuh.cn

[E02] 重复字符串
来源：http://ph.9csxet.cn

Py:   "ab" * 3
来源：http://bu.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://uq.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://dc.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://pg.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://vo.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ti.shtwfgs.cn

Ruby: "ab" * 3
来源：http://dq.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rv.yuexingan06.cn

[E03] 截取子串
来源：http://yy.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dg.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yh.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ek.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ry.521024.cn

Java: s.substring(1, 4)
来源：http://dr.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wf.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uz.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://cn.lnxyls.cn

[E04] 查找子串位置
来源：http://qy.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ip.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://ou.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oe.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://tn.szsharing.cn

Java: s.indexOf("x")
来源：http://hz.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://mv.huixiangedu.cn

Ruby: s.index("x")
来源：http://gm.nicolike.cn

C#:   s.IndexOf("x")
来源：http://ah.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zs.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cb.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vn.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ra.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ij.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hl.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://br.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ht.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fp.colortex.cn

[E06] 替换子串
来源：http://pu.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ty.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://dg.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ac.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ln.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://is.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pw.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aj.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://pp.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://dt.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pj.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aw.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bj.gzmigu.cn

TS:   s.split(",")
来源：http://jj.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jy.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sb.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://gn.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dm.nszjky.cn

[E08] 数组按分隔符合并
来源：http://em.colortex.cn

Py:   ",".join(items)
来源：http://zs.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://vi.muxihuayi.cn

JS:   items.join(",")
来源：http://gz.haigaiapp.cn

TS:   items.join(",")
来源：http://fm.nszjky.cn

Java: String.join(",", items)
来源：http://vf.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://wv.colortex.cn

Ruby: items.join(",")
来源：http://of.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://hb.colortex.cn

[E09] 去除所有空白字符
来源：http://oh.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gu.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sm.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://vt.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://mm.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://cj.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gr.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ty.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hr.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://gd.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kx.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yh.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://to.newstarts.cn


<!-- 参考信息 -->