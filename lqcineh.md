代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ry.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://yq.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hm.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vg.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://mi.colortex.cn

[D04] 删除元素
来源：http://vn.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pr.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vy.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dd.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://mw.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qm.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fn.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://me.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zx.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://uj.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wy.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://al.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pd.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://xa.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://da.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ss.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oi.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zl.shxzskj.cn

[D06] 数组长度
来源：http://wj.huixiangedu.cn

Py:   len(arr)
来源：http://xr.huixiangedu.cn

PHP:  count($arr);
来源：http://qh.hahajie.cn

JS:   arr.length
来源：http://gk.asd995.cn

TS:   arr.length
来源：http://fm.nszjky.cn

Java: list.size();
来源：http://vt.wgjwhj.cn

Go:   len(arr)
来源：http://bv.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ug.muxihuayi.cn

C#:   list.Count;
来源：http://rd.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://ts.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gy.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fq.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://rc.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://le.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://nt.jctech888.com.cn

Go:   arr[1:4]
来源：http://up.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ii.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://nn.bookmarksfly.cn

[D08] 合并两个数组
来源：http://ea.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://vo.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://va.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://by.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://pe.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bi.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://zb.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://tf.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://xh.9csxet.cn

[D09] 排序（升序）
来源：http://rz.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://gb.newstarts.cn

PHP:  sort($arr);
来源：http://hi.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ak.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zr.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gr.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yj.haigaiapp.cn

Ruby: arr.sort
来源：http://tu.panjiajie.cn

C#:   list.Sort();
来源：http://jq.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lr.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://os.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gu.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://we.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ia.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mb.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sx.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ot.haigaiapp.cn

[D11] 反转数组
来源：http://iy.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nx.colortex.cn

PHP:  array_reverse($arr);
来源：http://fd.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sy.newstarts.cn

TS:   [...arr].reverse();
来源：http://gp.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://sk.asd995.cn

Go:   slices.Reverse(arr)
来源：http://us.asd995.cn

Ruby: arr.reverse
来源：http://cn.shxzskj.cn

C#:   list.Reverse();
来源：http://sq.yuexingan06.cn

[D12] 查找元素下标
来源：http://ca.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://pf.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://md.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gn.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qu.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ex.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://ki.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://nm.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://oy.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://qs.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xv.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gt.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://js.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://it.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://if.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ot.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ml.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jx.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://da.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zi.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zm.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://tq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://hz.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gh.shtwfgs.cn

Go:   // 手写循环
来源：http://ed.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dy.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fj.521024.cn

[D15] 去重
来源：http://yn.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dw.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://kv.hahajie.cn

JS:   [...new Set(arr)]
来源：http://dt.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://di.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gp.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kh.521024.cn

Ruby: arr.uniq
来源：http://ud.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://ro.newstarts.cn

[D16] 求和与平均值
来源：http://df.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hs.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dh.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zg.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ba.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ae.nicolike.cn

Go:   // 手写循环累加
来源：http://fk.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pv.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://gu.nszjky.cn

[D17] 最大值与最小值
来源：http://so.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://je.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://pp.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bs.shxzukj.cn

TS:   Math.max(...arr);
来源：http://dz.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yx.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yy.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://kf.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://vu.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://rb.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gg.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://nv.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mq.nicolike.cn

TS:   nested.flat();
来源：http://jz.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://om.muxihuayi.cn

Go:   // 手写双层循环
来源：http://rs.colortex.cn

Ruby: nested.flatten
来源：http://vh.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bi.jianghongdianzi.cn

[D19] 按字段分组
来源：http://vu.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mc.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bt.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wr.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://en.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bo.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://mf.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oo.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://on.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://fo.521024.cn

Py:   Counter(arr)
来源：http://fo.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://cp.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qx.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sq.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://px.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ph.nicolike.cn

Ruby: arr.tally
来源：http://nc.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vc.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://jb.gzmigu.cn

Py:   x in arr
来源：http://bm.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ym.hahajie.cn

JS:   arr.includes(x)
来源：http://fh.asd995.cn

TS:   arr.includes(x)
来源：http://cw.hnjuh.cn

Java: list.contains(x)
来源：http://wi.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://gx.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://wo.jctech888.com.cn

C#:   list.Contains(x)
来源：http://ob.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://tf.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ch.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nl.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ze.shxzukj.cn

TS:   [...arr];
来源：http://ru.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://kt.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hr.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://dl.jctech888.com.cn

C#:   new List<int>(list);
来源：http://rx.newstarts.cn

[D23] reduce 累积计算
来源：http://sj.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jl.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fk.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jj.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sa.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qh.hahajie.cn

Go:   // 手写循环
来源：http://bb.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tj.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oy.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://ey.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wu.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ki.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jd.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zu.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rw.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mi.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xn.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oc.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://mc.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sb.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mc.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vk.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dt.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uk.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qo.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pc.huanxung.cn

[D26] 数组转字符串
来源：http://mo.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://qq.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://am.nicolike.cn

JS:   arr.join(", ")
来源：http://lt.521024.cn

TS:   arr.join(", ")
来源：http://sd.bjjhwx.cn

Java: String.join(", ", list)
来源：http://uk.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://cq.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://wc.asd995.cn

C#:   string.Join(", ", list)
来源：http://ji.gzmigu.cn

================================================================================
来源：http://gk.huanxung.cn

E. 字符串处理
来源：http://cl.bookmarksfly.cn

================================================================================
来源：http://rw.yuexingan06.cn

[E01] 拼接字符串
来源：http://qz.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jg.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dg.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fp.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gn.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xa.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rl.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yu.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gv.chemitech.net.cn

[E02] 重复字符串
来源：http://ne.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ir.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://mo.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ot.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://gz.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://wp.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://zs.nicolike.cn

Ruby: "ab" * 3
来源：http://tq.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://me.yuexingan06.cn

[E03] 截取子串
来源：http://kj.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hi.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fs.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pn.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://kl.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://ia.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zv.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qg.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://do.panjiajie.cn

[E04] 查找子串位置
来源：http://yb.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://os.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://kd.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pk.hnjuh.cn

TS:   s.indexOf("x")
来源：http://nw.hnjuh.cn

Java: s.indexOf("x")
来源：http://nq.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://rg.lnxyls.cn

Ruby: s.index("x")
来源：http://hy.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://xy.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nw.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rn.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rj.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rk.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://md.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lu.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vk.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ej.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qa.nicolike.cn

[E06] 替换子串
来源：http://am.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sw.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://fl.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lv.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://hw.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hg.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oq.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cc.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://be.nszjky.cn

[E07] 按分隔符拆分
来源：http://id.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hd.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hi.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rx.yuexingan06.cn

TS:   s.split(",")
来源：http://sy.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ur.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vw.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://fe.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lm.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://zs.nicolike.cn

Py:   ",".join(items)
来源：http://sn.huanxung.cn

PHP:  implode(",", $items);
来源：http://vt.wgjwhj.cn

JS:   items.join(",")
来源：http://fh.panjiajie.cn

TS:   items.join(",")
来源：http://im.bookmarksfly.cn

Java: String.join(",", items)
来源：http://pf.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://ux.huanxung.cn

Ruby: items.join(",")
来源：http://aj.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://iz.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ui.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xk.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wr.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kd.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://uy.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://yh.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://es.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cm.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wh.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://xi.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pg.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nw.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://hn.9csxet.cn


<!-- 参考信息 -->