代发 wailian999

Java: list.add(4);
来源：http://mf.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://gx.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://yc.haigaiapp.cn

C#:   list.Add(4);
来源：http://xu.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://ir.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://hp.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vc.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fg.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ga.nicolike.cn

Java: list.add(0, 0);
来源：http://di.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xh.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yw.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://kp.hnjuh.cn

[D04] 删除元素
来源：http://om.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://en.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sj.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://lt.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wa.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eh.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rj.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gt.hnjuh.cn

[D05] 访问与修改元素
来源：http://vl.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jh.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lt.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cc.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://mw.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://qc.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://sp.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pc.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xf.9csxet.cn

[D06] 数组长度
来源：http://bh.newstarts.cn

Py:   len(arr)
来源：http://xs.huixiangedu.cn

PHP:  count($arr);
来源：http://uq.colortex.cn

JS:   arr.length
来源：http://xh.bjjhwx.cn

TS:   arr.length
来源：http://oe.muxihuayi.cn

Java: list.size();
来源：http://dz.yuexingan06.cn

Go:   len(arr)
来源：http://pr.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://hs.colortex.cn

C#:   list.Count;
来源：http://kk.hahajie.cn

[D07] 切片 / 取子数组
来源：http://bi.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rz.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kt.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://nn.asd995.cn

TS:   arr.slice(1, 4);
来源：http://nf.9csxet.cn

Java: list.subList(1, 4);
来源：http://jt.szxytkj.cn

Go:   arr[1:4]
来源：http://ym.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://bt.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://oy.lnxyls.cn

[D08] 合并两个数组
来源：http://ny.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://hc.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://gt.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zj.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://lq.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fn.shxzskj.cn

Go:   append(a, b...)
来源：http://td.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://gr.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ro.521024.cn

[D09] 排序（升序）
来源：http://sh.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ik.haigaiapp.cn

PHP:  sort($arr);
来源：http://ou.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qh.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fi.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rt.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bw.colortex.cn

Ruby: arr.sort
来源：http://xa.huixiangedu.cn

C#:   list.Sort();
来源：http://oi.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xr.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bi.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kn.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://er.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pw.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bx.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ni.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lu.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hg.colortex.cn

[D11] 反转数组
来源：http://bq.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lf.colortex.cn

PHP:  array_reverse($arr);
来源：http://pc.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tr.szxytkj.cn

TS:   [...arr].reverse();
来源：http://zk.lnxyls.cn

Java: Collections.reverse(list);
来源：http://no.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ts.panjiajie.cn

Ruby: arr.reverse
来源：http://jb.hnjuh.cn

C#:   list.Reverse();
来源：http://xx.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://vu.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ex.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ui.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tj.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bd.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kj.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://bs.yuexingan06.cn

Ruby: arr.index(x)
来源：http://kj.szsharing.cn

C#:   list.IndexOf(x);
来源：http://vs.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ly.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gy.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://na.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://qf.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://co.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rt.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sb.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jx.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://in.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://fo.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mo.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qk.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://qw.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://yh.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rg.yuntaijiaju.cn

Go:   // 手写循环
来源：http://yw.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gq.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gs.shxzukj.cn

[D15] 去重
来源：http://ph.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kx.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://yr.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://rx.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://sp.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oq.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://to.muxihuayi.cn

Ruby: arr.uniq
来源：http://oh.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://wo.wgjwhj.cn

[D16] 求和与平均值
来源：http://jf.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rh.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://up.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fz.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ym.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hp.szxytkj.cn

Go:   // 手写循环累加
来源：http://aq.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ka.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://wf.521024.cn

[D17] 最大值与最小值
来源：http://qb.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://bq.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://xu.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eg.9csxet.cn

TS:   Math.max(...arr);
来源：http://dn.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jz.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ey.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://af.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://uq.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://yh.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mr.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://zm.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.panjiajie.cn

TS:   nested.flat();
来源：http://ei.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vt.huixiangedu.cn

Go:   // 手写双层循环
来源：http://wo.asd995.cn

Ruby: nested.flatten
来源：http://sf.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ml.huixiangedu.cn

[D19] 按字段分组
来源：http://vg.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hf.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://si.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ax.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qv.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vp.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://lr.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yb.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://er.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://ef.9csxet.cn

Py:   Counter(arr)
来源：http://on.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ck.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://im.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://op.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bz.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://vh.lnxyls.cn

Ruby: arr.tally
来源：http://fn.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cl.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://xo.lnxyls.cn

Py:   x in arr
来源：http://qo.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://kf.huixiangedu.cn

JS:   arr.includes(x)
来源：http://cs.jctech888.com.cn

TS:   arr.includes(x)
来源：http://hq.9csxet.cn

Java: list.contains(x)
来源：http://ut.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ga.szsharing.cn

Ruby: arr.include?(x)
来源：http://gm.yuexingan06.cn

C#:   list.Contains(x)
来源：http://tn.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://jx.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ze.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cr.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lg.szxytkj.cn

TS:   [...arr];
来源：http://nt.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://av.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ss.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://xz.szsharing.cn

C#:   new List<int>(list);
来源：http://kn.shxzukj.cn

[D23] reduce 累积计算
来源：http://te.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://et.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://en.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ka.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tq.lnxyls.cn

Go:   // 手写循环
来源：http://yo.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hn.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vb.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://yt.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ah.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wy.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vy.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nf.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vg.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qd.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sb.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mr.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://tb.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wp.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zp.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://do.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ka.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vp.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vs.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tb.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pw.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://gh.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://zr.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://ld.panjiajie.cn

JS:   arr.join(", ")
来源：http://au.jctech888.com.cn

TS:   arr.join(", ")
来源：http://te.szxytkj.cn

Java: String.join(", ", list)
来源：http://oz.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://cy.nszjky.cn

Ruby: arr.join(", ")
来源：http://yy.nicolike.cn

C#:   string.Join(", ", list)
来源：http://uf.asd995.cn

================================================================================
来源：http://qk.panjiajie.cn

E. 字符串处理
来源：http://md.shxzskj.cn

================================================================================
来源：http://jv.nicolike.cn

[E01] 拼接字符串
来源：http://av.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cj.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vr.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ty.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oh.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gk.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dz.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mv.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ib.jianghongdianzi.cn

[E02] 重复字符串
来源：http://pj.jctech888.com.cn

Py:   "ab" * 3
来源：http://tv.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://es.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ai.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://db.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://fw.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://wf.jctech888.com.cn

Ruby: "ab" * 3
来源：http://lo.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nx.jianghongdianzi.cn

[E03] 截取子串
来源：http://tm.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rx.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cb.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://st.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ea.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://xb.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://id.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tv.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://wp.hahajie.cn

[E04] 查找子串位置
来源：http://xb.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://jo.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ze.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rr.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ou.asd995.cn

Java: s.indexOf("x")
来源：http://cq.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://my.panjiajie.cn

Ruby: s.index("x")
来源：http://gm.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://tm.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pt.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://on.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oq.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kg.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bw.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oa.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ob.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pm.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gt.yuntaijiaju.cn

[E06] 替换子串
来源：http://va.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ll.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ff.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://gu.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yd.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ll.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yk.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://on.panjiajie.cn

[E07] 按分隔符拆分
来源：http://fw.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ii.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jh.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://su.panjiajie.cn

TS:   s.split(",")
来源：http://lm.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wu.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xc.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://sq.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jk.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ld.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://ez.szsharing.cn

PHP:  implode(",", $items);
来源：http://ex.nicolike.cn

JS:   items.join(",")
来源：http://rn.gzmigu.cn

TS:   items.join(",")
来源：http://qk.shtwfgs.cn

Java: String.join(",", items)
来源：http://qw.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://tl.haigaiapp.cn

Ruby: items.join(",")
来源：http://wi.colortex.cn

C#:   string.Join(",", items)
来源：http://sq.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://qx.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cd.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gt.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://xw.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://sm.bjjhwx.cn


<!-- 参考信息 -->