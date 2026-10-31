代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://td.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://kk.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lv.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://ok.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://do.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://om.shxzukj.cn

JS:   arr.push(4);
来源：http://nl.szxytkj.cn

TS:   arr.push(4);
来源：http://ay.colortex.cn

Java: list.add(4);
来源：http://gf.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://qq.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://tz.521024.cn

C#:   list.Add(4);
来源：http://cs.colortex.cn

[D03] 在指定位置插入元素
来源：http://jk.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://jt.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yh.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lv.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://qt.lnxyls.cn

Java: list.add(0, 0);
来源：http://ly.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pm.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jd.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://xf.huixinmuqiang.cn

[D04] 删除元素
来源：http://sw.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ni.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://os.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://no.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://tr.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jx.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kc.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ln.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yg.gzmigu.cn

[D05] 访问与修改元素
来源：http://mi.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qu.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ql.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://cg.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://ab.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://fi.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://md.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tt.huanxung.cn

[D06] 数组长度
来源：http://re.chemitech.net.cn

Py:   len(arr)
来源：http://nn.bjjhwx.cn

PHP:  count($arr);
来源：http://lr.huixinmuqiang.cn

JS:   arr.length
来源：http://dh.jctech888.com.cn

TS:   arr.length
来源：http://pm.asd995.cn

Java: list.size();
来源：http://vz.gzmigu.cn

Go:   len(arr)
来源：http://av.nszjky.cn

Ruby: arr.length; arr.size
来源：http://if.muxihuayi.cn

C#:   list.Count;
来源：http://vx.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://by.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vs.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pt.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ut.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://ij.shxzukj.cn

Java: list.subList(1, 4);
来源：http://pj.szxytkj.cn

Go:   arr[1:4]
来源：http://ef.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://iu.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://je.wgjwhj.cn

[D08] 合并两个数组
来源：http://tx.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://lg.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://tp.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fq.hahajie.cn

TS:   [...a, ...b];
来源：http://ax.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yl.colortex.cn

Go:   append(a, b...)
来源：http://lu.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://do.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://kw.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://aj.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://cu.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yo.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://da.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ra.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rq.gzmigu.cn

Ruby: arr.sort
来源：http://mc.hahajie.cn

C#:   list.Sort();
来源：http://fa.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kb.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zb.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tc.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rk.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ch.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bh.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://st.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tc.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ox.521024.cn

[D11] 反转数组
来源：http://jw.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://by.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://to.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tg.hahajie.cn

TS:   [...arr].reverse();
来源：http://qb.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://kd.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://sv.huanxung.cn

Ruby: arr.reverse
来源：http://eb.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://bk.muxihuayi.cn

[D12] 查找元素下标
来源：http://ds.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ew.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dp.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mq.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nm.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://la.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://ya.newstarts.cn

Ruby: arr.index(x)
来源：http://wx.colortex.cn

C#:   list.IndexOf(x);
来源：http://as.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://yk.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fv.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qe.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://zx.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ad.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ly.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zb.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zd.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://za.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://jl.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zq.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mx.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://qe.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://yv.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fc.szxytkj.cn

Go:   // 手写循环
来源：http://fx.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://id.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rv.bjjhwx.cn

[D15] 去重
来源：http://ga.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qp.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://az.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://ug.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://wl.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ay.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cb.chemitech.net.cn

Ruby: arr.uniq
来源：http://ir.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://bm.521024.cn

[D16] 求和与平均值
来源：http://eq.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rl.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nl.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bi.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cz.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ro.colortex.cn

Go:   // 手写循环累加
来源：http://es.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kv.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://tm.lnxyls.cn

[D17] 最大值与最小值
来源：http://zf.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://qw.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://bj.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vb.szxytkj.cn

TS:   Math.max(...arr);
来源：http://th.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jn.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pg.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://xd.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://ww.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ye.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xc.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ls.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cy.colortex.cn

TS:   nested.flat();
来源：http://cy.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dc.panjiajie.cn

Go:   // 手写双层循环
来源：http://pj.shxzskj.cn

Ruby: nested.flatten
来源：http://fe.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vi.jctech888.com.cn

[D19] 按字段分组
来源：http://gk.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ua.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pd.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iu.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uu.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ie.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://yq.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ds.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tu.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://nj.521024.cn

Py:   Counter(arr)
来源：http://qz.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ch.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qq.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lu.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hc.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://lg.lnxyls.cn

Ruby: arr.tally
来源：http://fl.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xn.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://pn.newstarts.cn

Py:   x in arr
来源：http://lb.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://xb.wgjwhj.cn

JS:   arr.includes(x)
来源：http://yk.asd995.cn

TS:   arr.includes(x)
来源：http://pv.huixiangedu.cn

Java: list.contains(x)
来源：http://zu.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://dv.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://fr.nicolike.cn

C#:   list.Contains(x)
来源：http://ar.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://mi.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vi.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zv.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uh.asd995.cn

TS:   [...arr];
来源：http://ay.hahajie.cn

Java: new ArrayList<>(list);
来源：http://qg.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yj.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://dg.9csxet.cn

C#:   new List<int>(list);
来源：http://gg.nszjky.cn

[D23] reduce 累积计算
来源：http://hn.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://md.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mo.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ll.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xm.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wo.bookmarksfly.cn

Go:   // 手写循环
来源：http://uo.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fv.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bj.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://sm.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ud.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vk.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tf.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zs.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://md.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jr.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dg.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hq.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://cj.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yb.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dr.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://on.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ga.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ny.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aj.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://do.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hu.9csxet.cn

[D26] 数组转字符串
来源：http://zr.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://ym.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://fc.szxytkj.cn

JS:   arr.join(", ")
来源：http://hz.nicolike.cn

TS:   arr.join(", ")
来源：http://rx.shxzukj.cn

Java: String.join(", ", list)
来源：http://ty.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://uw.huanxung.cn

Ruby: arr.join(", ")
来源：http://fm.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://zu.nicolike.cn

================================================================================
来源：http://hf.yuntaijiaju.cn

E. 字符串处理
来源：http://wk.hnjuh.cn

================================================================================
来源：http://rm.wgjwhj.cn

[E01] 拼接字符串
来源：http://zr.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wo.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wf.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mi.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ty.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://if.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dn.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sc.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ob.hahajie.cn

[E02] 重复字符串
来源：http://pk.9csxet.cn

Py:   "ab" * 3
来源：http://uv.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://rm.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://wk.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ri.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://xv.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://hv.shxzskj.cn

Ruby: "ab" * 3
来源：http://ja.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hk.gzmigu.cn

[E03] 截取子串
来源：http://bq.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fw.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yc.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jk.521024.cn

TS:   s.slice(1, 4)
来源：http://lt.asd995.cn

Java: s.substring(1, 4)
来源：http://zp.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lh.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zy.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://eg.asd995.cn

[E04] 查找子串位置
来源：http://ad.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://wb.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://fe.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jx.huanxung.cn

TS:   s.indexOf("x")
来源：http://qn.nszjky.cn

Java: s.indexOf("x")
来源：http://jm.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://fm.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://vs.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://hk.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jx.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://st.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gy.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kn.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tp.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ms.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xr.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oy.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ha.gzmigu.cn

[E06] 替换子串
来源：http://gj.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vh.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://pq.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://qn.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aj.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://is.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://tr.shxzskj.cn

[E07] 按分隔符拆分
来源：http://aj.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gf.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yt.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pr.chemitech.net.cn

TS:   s.split(",")
来源：http://ko.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ht.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://py.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://ta.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fb.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ai.jctech888.com.cn

Py:   ",".join(items)
来源：http://cu.521024.cn

PHP:  implode(",", $items);
来源：http://uv.yuexingan06.cn

JS:   items.join(",")
来源：http://pn.muxihuayi.cn

TS:   items.join(",")
来源：http://ze.haigaiapp.cn

Java: String.join(",", items)
来源：http://yb.shxzukj.cn


<!-- 参考信息 -->