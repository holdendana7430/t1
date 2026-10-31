代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ml.asd995.cn

Java: list.add(0, 0);
来源：http://rw.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xv.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://so.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://rf.shtwfgs.cn

[D04] 删除元素
来源：http://ww.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cj.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iw.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rt.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://fz.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://el.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tb.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rw.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tj.chemitech.net.cn

[D05] 访问与修改元素
来源：http://va.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bk.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vf.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://le.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://iu.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://jh.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://lw.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://un.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ty.szsharing.cn

[D06] 数组长度
来源：http://pl.jianghongdianzi.cn

Py:   len(arr)
来源：http://jt.huixiangedu.cn

PHP:  count($arr);
来源：http://zc.asd995.cn

JS:   arr.length
来源：http://ww.lnxyls.cn

TS:   arr.length
来源：http://qa.haigaiapp.cn

Java: list.size();
来源：http://oo.asd995.cn

Go:   len(arr)
来源：http://rx.9csxet.cn

Ruby: arr.length; arr.size
来源：http://cw.bookmarksfly.cn

C#:   list.Count;
来源：http://ub.newstarts.cn

[D07] 切片 / 取子数组
来源：http://jn.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://go.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rb.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://zj.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://xi.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ff.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://qq.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://rs.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ts.nicolike.cn

[D08] 合并两个数组
来源：http://ni.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://rz.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://tm.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yu.huanxung.cn

TS:   [...a, ...b];
来源：http://xl.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://od.asd995.cn

Go:   append(a, b...)
来源：http://go.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://wm.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://dt.szsharing.cn

[D09] 排序（升序）
来源：http://uh.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://xc.shxzukj.cn

PHP:  sort($arr);
来源：http://ok.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fo.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hr.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lv.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lp.haigaiapp.cn

Ruby: arr.sort
来源：http://vv.9csxet.cn

C#:   list.Sort();
来源：http://qs.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kw.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cq.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://et.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rl.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bl.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eg.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fs.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bl.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qz.panjiajie.cn

[D11] 反转数组
来源：http://jf.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://la.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://wb.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cq.9csxet.cn

TS:   [...arr].reverse();
来源：http://sq.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://dq.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://cn.lnxyls.cn

Ruby: arr.reverse
来源：http://wn.huixiangedu.cn

C#:   list.Reverse();
来源：http://my.shtwfgs.cn

[D12] 查找元素下标
来源：http://nz.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://bw.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vz.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wk.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://or.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rc.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://wx.9csxet.cn

Ruby: arr.index(x)
来源：http://gy.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://oz.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://xh.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ur.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hs.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://az.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ca.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gv.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eo.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iq.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kg.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://am.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jd.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yx.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://bs.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://fb.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wz.huanxung.cn

Go:   // 手写循环
来源：http://wi.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jw.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wv.huanxung.cn

[D15] 去重
来源：http://uz.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ia.newstarts.cn

PHP:  array_unique($arr);
来源：http://fh.colortex.cn

JS:   [...new Set(arr)]
来源：http://gq.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://cy.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ma.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vj.shtwfgs.cn

Ruby: arr.uniq
来源：http://nr.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://mb.szsharing.cn

[D16] 求和与平均值
来源：http://mz.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fj.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yr.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ut.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nu.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uu.shtwfgs.cn

Go:   // 手写循环累加
来源：http://lx.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oi.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://hf.muxihuayi.cn

[D17] 最大值与最小值
来源：http://kz.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://ss.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://kn.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wq.gzmigu.cn

TS:   Math.max(...arr);
来源：http://bn.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ti.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://bd.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://qq.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://hf.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zp.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://vi.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mx.nicolike.cn

TS:   nested.flat();
来源：http://ss.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ht.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://pz.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://lq.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zg.chemitech.net.cn

[D19] 按字段分组
来源：http://mv.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xr.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qa.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ox.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xb.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mu.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://rz.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://km.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://iv.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://ua.hahajie.cn

PHP:  array_count_values($arr);
来源：http://qe.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jt.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xo.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cp.newstarts.cn

Go:   // 手写 map[T]int
来源：http://ow.hahajie.cn

Ruby: arr.tally
来源：http://wa.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nd.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://mg.huixinmuqiang.cn

Py:   x in arr
来源：http://yl.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://qm.asd995.cn

JS:   arr.includes(x)
来源：http://nv.jctech888.com.cn

TS:   arr.includes(x)
来源：http://mp.bjjhwx.cn

Java: list.contains(x)
来源：http://hb.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://by.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://px.9csxet.cn

C#:   list.Contains(x)
来源：http://as.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://os.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wd.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zv.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ng.huixiangedu.cn

TS:   [...arr];
来源：http://jg.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://yt.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pk.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://sc.newstarts.cn

C#:   new List<int>(list);
来源：http://jr.nszjky.cn

[D23] reduce 累积计算
来源：http://rn.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hh.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ys.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oc.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vv.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xd.shxzukj.cn

Go:   // 手写循环
来源：http://lo.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xn.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sh.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://jk.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nn.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cp.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kl.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ho.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://am.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ik.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rp.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bd.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://bd.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cw.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fy.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jr.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://al.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sa.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wv.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wf.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wo.colortex.cn

[D26] 数组转字符串
来源：http://nn.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://vc.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ly.asd995.cn

JS:   arr.join(", ")
来源：http://gu.nszjky.cn

TS:   arr.join(", ")
来源：http://ot.newstarts.cn

Java: String.join(", ", list)
来源：http://ag.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://cy.521024.cn

Ruby: arr.join(", ")
来源：http://bc.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ff.nicolike.cn

================================================================================
来源：http://bs.colortex.cn

E. 字符串处理
来源：http://zm.huixinmuqiang.cn

================================================================================
来源：http://sg.shxzukj.cn

[E01] 拼接字符串
来源：http://oi.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sd.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lb.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hc.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lb.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rt.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fd.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rj.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fu.shxzukj.cn

[E02] 重复字符串
来源：http://rp.szxytkj.cn

Py:   "ab" * 3
来源：http://pn.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://cf.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://uo.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://wx.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://va.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://ll.hnjuh.cn

Ruby: "ab" * 3
来源：http://wr.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ic.panjiajie.cn

[E03] 截取子串
来源：http://qt.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pi.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cs.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kg.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://rl.nszjky.cn

Java: s.substring(1, 4)
来源：http://yu.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ly.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://op.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://xm.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://ug.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://ao.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://zi.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zw.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://dx.chemitech.net.cn

Java: s.indexOf("x")
来源：http://uk.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://wc.muxihuayi.cn

Ruby: s.index("x")
来源：http://gi.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://rl.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ol.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qy.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://li.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rz.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sa.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hq.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://au.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ks.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ot.gzmigu.cn

[E06] 替换子串
来源：http://eb.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pk.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ad.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mk.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://an.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ti.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oy.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xq.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://cm.hahajie.cn

[E07] 按分隔符拆分
来源：http://hx.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://el.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://io.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fu.huixiangedu.cn

TS:   s.split(",")
来源：http://cn.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://za.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rs.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ld.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bi.newstarts.cn

[E08] 数组按分隔符合并
来源：http://yk.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://tg.newstarts.cn

PHP:  implode(",", $items);
来源：http://qx.newstarts.cn

JS:   items.join(",")
来源：http://xy.jctech888.com.cn

TS:   items.join(",")
来源：http://pq.521024.cn

Java: String.join(",", items)
来源：http://fp.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://yt.colortex.cn

Ruby: items.join(",")
来源：http://gm.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ew.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://oe.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hj.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zv.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://av.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://qd.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://qh.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://us.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kq.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tn.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://wk.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zq.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kl.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://hf.jianghongdianzi.cn


<!-- 参考信息 -->