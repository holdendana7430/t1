代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://oy.bjjhwx.cn

Java: list.add(0, 0);
来源：http://wt.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vs.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ip.panjiajie.cn

[D04] 删除元素
来源：http://sn.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jx.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dx.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xm.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://vk.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wc.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nm.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://od.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://au.hnjuh.cn

[D05] 访问与修改元素
来源：http://nz.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lo.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iy.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://it.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://yg.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yi.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://gb.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lf.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ej.szsharing.cn

[D06] 数组长度
来源：http://ip.jctech888.com.cn

Py:   len(arr)
来源：http://ju.lnxyls.cn

PHP:  count($arr);
来源：http://rr.shtwfgs.cn

JS:   arr.length
来源：http://mw.jctech888.com.cn

TS:   arr.length
来源：http://tv.newstarts.cn

Java: list.size();
来源：http://lw.lnxyls.cn

Go:   len(arr)
来源：http://dj.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://in.521024.cn

C#:   list.Count;
来源：http://op.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ia.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zt.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yl.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://vb.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://lz.newstarts.cn

Java: list.subList(1, 4);
来源：http://nh.szxytkj.cn

Go:   arr[1:4]
来源：http://ri.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://zq.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://eo.shxzukj.cn

[D08] 合并两个数组
来源：http://te.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://sr.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://ig.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://px.haigaiapp.cn

TS:   [...a, ...b];
来源：http://cz.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vi.szxytkj.cn

Go:   append(a, b...)
来源：http://vr.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://rs.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://nt.hnjuh.cn

[D09] 排序（升序）
来源：http://xv.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://zi.shxzukj.cn

PHP:  sort($arr);
来源：http://km.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nk.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uz.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wa.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dz.wgjwhj.cn

Ruby: arr.sort
来源：http://mp.hahajie.cn

C#:   list.Sort();
来源：http://le.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gr.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ph.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kp.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xy.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tm.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ft.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bu.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ln.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ac.shxzskj.cn

[D11] 反转数组
来源：http://pr.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://er.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://tu.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gs.lnxyls.cn

TS:   [...arr].reverse();
来源：http://se.asd995.cn

Java: Collections.reverse(list);
来源：http://wm.521024.cn

Go:   slices.Reverse(arr)
来源：http://oe.haigaiapp.cn

Ruby: arr.reverse
来源：http://qq.muxihuayi.cn

C#:   list.Reverse();
来源：http://sj.wgjwhj.cn

[D12] 查找元素下标
来源：http://gg.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://oo.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kh.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ga.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hl.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://oa.9csxet.cn

Ruby: arr.index(x)
来源：http://ie.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://cy.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://rw.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fc.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://az.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://kf.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://mq.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wd.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bs.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wa.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wn.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://op.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xl.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gk.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://rb.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://zv.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://le.colortex.cn

Go:   // 手写循环
来源：http://qx.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jq.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cm.panjiajie.cn

[D15] 去重
来源：http://yq.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qg.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://tt.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://kv.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://av.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xy.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://we.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://os.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://tw.shxzskj.cn

[D16] 求和与平均值
来源：http://if.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fq.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://os.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tx.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mc.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fd.muxihuayi.cn

Go:   // 手写循环累加
来源：http://bp.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ok.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://ic.wgjwhj.cn

[D17] 最大值与最小值
来源：http://el.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://lm.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://vq.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hx.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://fu.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yg.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wq.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://sf.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://vr.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://ki.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fs.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://po.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bc.bjjhwx.cn

TS:   nested.flat();
来源：http://jd.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lp.bjjhwx.cn

Go:   // 手写双层循环
来源：http://zf.shtwfgs.cn

Ruby: nested.flatten
来源：http://or.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ho.jianghongdianzi.cn

[D19] 按字段分组
来源：http://vx.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://du.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jr.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bt.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xu.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pq.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://qo.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zq.colortex.cn

[D20] 统计每个元素出现次数
来源：http://vl.newstarts.cn

Py:   Counter(arr)
来源：http://wu.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://sv.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pn.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fr.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ip.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ty.huixinmuqiang.cn

Ruby: arr.tally
来源：http://kv.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yr.9csxet.cn

[D21] 判断是否包含某元素
来源：http://hm.hahajie.cn

Py:   x in arr
来源：http://tv.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://th.9csxet.cn

JS:   arr.includes(x)
来源：http://wy.wgjwhj.cn

TS:   arr.includes(x)
来源：http://wn.chemitech.net.cn

Java: list.contains(x)
来源：http://zn.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://qg.9csxet.cn

Ruby: arr.include?(x)
来源：http://wo.nszjky.cn

C#:   list.Contains(x)
来源：http://ya.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://sy.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cm.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dv.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pg.huixiangedu.cn

TS:   [...arr];
来源：http://iu.huanxung.cn

Java: new ArrayList<>(list);
来源：http://nu.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mg.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://pg.nicolike.cn

C#:   new List<int>(list);
来源：http://ql.bjjhwx.cn

[D23] reduce 累积计算
来源：http://cw.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://np.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qj.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ul.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xx.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sf.nicolike.cn

Go:   // 手写循环
来源：http://dw.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nx.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mi.521024.cn

[D24] 字典 / Map 基本操作
来源：http://xv.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hi.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://we.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ct.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lq.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hb.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hi.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ic.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yi.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://ts.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gf.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ka.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fs.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ke.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mo.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pe.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zx.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bm.jctech888.com.cn

[D26] 数组转字符串
来源：http://go.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://ak.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://et.asd995.cn

JS:   arr.join(", ")
来源：http://om.gzmigu.cn

TS:   arr.join(", ")
来源：http://kq.bjjhwx.cn

Java: String.join(", ", list)
来源：http://df.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://jf.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://mj.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://dl.szsharing.cn

================================================================================
来源：http://id.asd995.cn

E. 字符串处理
来源：http://dk.hnjuh.cn

================================================================================
来源：http://rg.asd995.cn

[E01] 拼接字符串
来源：http://vb.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rf.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jb.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qs.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mu.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hs.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pa.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yz.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ih.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ml.hahajie.cn

Py:   "ab" * 3
来源：http://pg.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://dw.521024.cn

JS:   "ab".repeat(3)
来源：http://og.9csxet.cn

TS:   "ab".repeat(3)
来源：http://mg.huanxung.cn

Java: "ab".repeat(3)
来源：http://np.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://mg.newstarts.cn

Ruby: "ab" * 3
来源：http://eq.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uy.nszjky.cn

[E03] 截取子串
来源：http://jx.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sw.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dx.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ic.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ss.gzmigu.cn

Java: s.substring(1, 4)
来源：http://eb.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ie.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cx.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://jw.colortex.cn

[E04] 查找子串位置
来源：http://cb.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://op.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://xh.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ar.shxzskj.cn

TS:   s.indexOf("x")
来源：http://gn.asd995.cn

Java: s.indexOf("x")
来源：http://dq.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://aj.hahajie.cn

Ruby: s.index("x")
来源：http://tx.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://me.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uo.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://az.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hm.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cq.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jd.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://co.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sn.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fz.huanxung.cn

[E06] 替换子串
来源：http://fz.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://li.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://of.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wy.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://rp.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jt.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xo.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oj.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://xb.newstarts.cn

[E07] 按分隔符拆分
来源：http://gp.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jd.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://er.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ym.chemitech.net.cn

TS:   s.split(",")
来源：http://lp.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fn.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uz.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://qs.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xn.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://al.szsharing.cn

Py:   ",".join(items)
来源：http://ei.huanxung.cn

PHP:  implode(",", $items);
来源：http://qf.lnxyls.cn

JS:   items.join(",")
来源：http://tq.szsharing.cn

TS:   items.join(",")
来源：http://gr.bjjhwx.cn

Java: String.join(",", items)
来源：http://da.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://xt.hnjuh.cn

Ruby: items.join(",")
来源：http://xg.nicolike.cn

C#:   string.Join(",", items)
来源：http://ei.gzmigu.cn

[E09] 去除所有空白字符
来源：http://zw.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ga.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hc.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ie.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://uj.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://id.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rr.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iy.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gs.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://zd.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://su.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dm.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://bh.szxytkj.cn


<!-- 参考信息 -->