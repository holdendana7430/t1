代发 wailian999

Java: list.add(4);
来源：http://dl.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://oo.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ni.szsharing.cn

C#:   list.Add(4);
来源：http://iv.colortex.cn

[D03] 在指定位置插入元素
来源：http://xw.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://lg.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://di.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pj.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://co.wgjwhj.cn

Java: list.add(0, 0);
来源：http://oo.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bz.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yk.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://qq.szsharing.cn

[D04] 删除元素
来源：http://rh.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ly.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wy.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://tp.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bi.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cc.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cz.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nl.hnjuh.cn

[D05] 访问与修改元素
来源：http://dt.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://op.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cg.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ff.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ts.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://oi.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://oo.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vs.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gx.jianghongdianzi.cn

[D06] 数组长度
来源：http://zk.chemitech.net.cn

Py:   len(arr)
来源：http://mo.chemitech.net.cn

PHP:  count($arr);
来源：http://ma.shxzukj.cn

JS:   arr.length
来源：http://kd.bookmarksfly.cn

TS:   arr.length
来源：http://am.gzmigu.cn

Java: list.size();
来源：http://zj.haigaiapp.cn

Go:   len(arr)
来源：http://iy.szsharing.cn

Ruby: arr.length; arr.size
来源：http://zi.huanxung.cn

C#:   list.Count;
来源：http://oe.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://ai.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jq.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oj.colortex.cn

JS:   arr.slice(1, 4);
来源：http://hg.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://kp.shxzukj.cn

Java: list.subList(1, 4);
来源：http://iq.szxytkj.cn

Go:   arr[1:4]
来源：http://to.nicolike.cn

Ruby: arr[1, 3]
来源：http://nn.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://qm.yuexingan06.cn

[D08] 合并两个数组
来源：http://qe.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://ez.521024.cn

PHP:  array_merge($a, $b);
来源：http://fs.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://id.huanxung.cn

TS:   [...a, ...b];
来源：http://eu.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kr.bjjhwx.cn

Go:   append(a, b...)
来源：http://jn.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://tr.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://aw.bookmarksfly.cn

[D09] 排序（升序）
来源：http://xq.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.shxzskj.cn

PHP:  sort($arr);
来源：http://tq.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hk.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tp.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dz.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ko.yuexingan06.cn

Ruby: arr.sort
来源：http://bq.asd995.cn

C#:   list.Sort();
来源：http://kz.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://et.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bb.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ks.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dr.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ss.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wn.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ub.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yq.521024.cn

[D11] 反转数组
来源：http://oh.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pj.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://tz.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ji.nszjky.cn

TS:   [...arr].reverse();
来源：http://eg.nicolike.cn

Java: Collections.reverse(list);
来源：http://hk.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ia.jctech888.com.cn

Ruby: arr.reverse
来源：http://ch.bookmarksfly.cn

C#:   list.Reverse();
来源：http://ud.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://gc.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://pr.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sh.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ui.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://al.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://oo.hnjuh.cn

Ruby: arr.index(x)
来源：http://jl.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://zw.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://me.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gb.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ki.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://nn.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://xe.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://km.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sr.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zh.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lj.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://xh.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yo.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://td.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://tq.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://np.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hd.jianghongdianzi.cn

Go:   // 手写循环
来源：http://se.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iq.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hj.colortex.cn

[D15] 去重
来源：http://rt.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tf.gzmigu.cn

PHP:  array_unique($arr);
来源：http://gb.huanxung.cn

JS:   [...new Set(arr)]
来源：http://to.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://th.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qn.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oc.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://bd.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://kk.shtwfgs.cn

[D16] 求和与平均值
来源：http://sh.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sc.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eu.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yk.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fx.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://or.chemitech.net.cn

Go:   // 手写循环累加
来源：http://na.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nb.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://ep.yuexingan06.cn

[D17] 最大值与最小值
来源：http://jx.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://zq.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://od.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ca.nszjky.cn

TS:   Math.max(...arr);
来源：http://pv.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mk.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hl.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://sd.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://zd.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://xc.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cb.521024.cn

PHP:  array_merge(...$nested);
来源：http://ha.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nx.muxihuayi.cn

TS:   nested.flat();
来源：http://sd.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vr.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://wh.chemitech.net.cn

Ruby: nested.flatten
来源：http://kw.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mn.shxzskj.cn

[D19] 按字段分组
来源：http://fx.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kc.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jm.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vj.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yh.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qd.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://tn.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jj.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qj.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zb.nicolike.cn

Py:   Counter(arr)
来源：http://pf.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://yn.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qs.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nw.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://fm.gzmigu.cn

Ruby: arr.tally
来源：http://ts.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ow.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://xs.hnjuh.cn

Py:   x in arr
来源：http://vd.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://xn.szxytkj.cn

JS:   arr.includes(x)
来源：http://hr.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://we.bookmarksfly.cn

Java: list.contains(x)
来源：http://xy.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://ji.szsharing.cn

Ruby: arr.include?(x)
来源：http://cv.jctech888.com.cn

C#:   list.Contains(x)
来源：http://zy.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://qg.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tj.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://er.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vw.colortex.cn

TS:   [...arr];
来源：http://ss.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://sa.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://px.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://am.yuexingan06.cn

C#:   new List<int>(list);
来源：http://ya.shxzukj.cn

[D23] reduce 累积计算
来源：http://nn.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bt.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ax.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://to.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xz.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://av.shxzukj.cn

Go:   // 手写循环
来源：http://et.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dx.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://il.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://mc.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oh.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qp.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xi.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bu.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fq.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sa.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lu.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ij.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://db.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eb.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eo.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cg.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uv.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dh.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uz.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nr.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zb.haigaiapp.cn

[D26] 数组转字符串
来源：http://rq.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://xm.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://fr.nszjky.cn

JS:   arr.join(", ")
来源：http://no.bjjhwx.cn

TS:   arr.join(", ")
来源：http://xs.bjjhwx.cn

Java: String.join(", ", list)
来源：http://fq.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://tx.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://wn.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ga.huixinmuqiang.cn

================================================================================
来源：http://sb.chemitech.net.cn

E. 字符串处理
来源：http://yn.nicolike.cn

================================================================================
来源：http://vs.muxihuayi.cn

[E01] 拼接字符串
来源：http://rj.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wr.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qc.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vl.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vr.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ty.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aj.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zi.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xs.shxzskj.cn

[E02] 重复字符串
来源：http://xq.gzmigu.cn

Py:   "ab" * 3
来源：http://ls.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://oc.nicolike.cn

JS:   "ab".repeat(3)
来源：http://pc.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://nt.asd995.cn

Java: "ab".repeat(3)
来源：http://ck.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://va.colortex.cn

Ruby: "ab" * 3
来源：http://yv.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bw.jctech888.com.cn

[E03] 截取子串
来源：http://cg.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cn.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vx.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://la.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://sz.szxytkj.cn

Java: s.substring(1, 4)
来源：http://iz.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jk.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ei.colortex.cn

C#:   s.Substring(1, 3)
来源：http://kc.muxihuayi.cn

[E04] 查找子串位置
来源：http://wb.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://ze.asd995.cn

PHP:  strpos($s, "x");
来源：http://up.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ow.szsharing.cn

TS:   s.indexOf("x")
来源：http://ai.9csxet.cn

Java: s.indexOf("x")
来源：http://cq.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://mm.hnjuh.cn

Ruby: s.index("x")
来源：http://on.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://al.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yu.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ui.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qr.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uh.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eg.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ir.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dl.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kg.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ns.haigaiapp.cn

[E06] 替换子串
来源：http://wm.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uz.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://vt.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rr.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ko.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rx.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qj.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qz.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://co.asd995.cn

[E07] 按分隔符拆分
来源：http://gt.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gc.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bk.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vy.yuexingan06.cn

TS:   s.split(",")
来源：http://oz.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qw.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wq.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://et.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wc.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://uy.colortex.cn

Py:   ",".join(items)
来源：http://pf.shxzskj.cn

PHP:  implode(",", $items);
来源：http://su.hahajie.cn

JS:   items.join(",")
来源：http://mj.yuntaijiaju.cn

TS:   items.join(",")
来源：http://nm.colortex.cn

Java: String.join(",", items)
来源：http://qu.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://ka.shxzskj.cn

Ruby: items.join(",")
来源：http://ek.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ny.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://jv.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cf.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ak.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://ed.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://kb.szxytkj.cn


<!-- 参考信息 -->