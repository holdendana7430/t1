代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kg.521024.cn

TS:   arr.splice(0, 1);
来源：http://ef.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pn.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ex.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mx.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://ep.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nv.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sc.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vf.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ul.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://we.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://xk.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gy.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xc.huixiangedu.cn

[D06] 数组长度
来源：http://bi.9csxet.cn

Py:   len(arr)
来源：http://ci.newstarts.cn

PHP:  count($arr);
来源：http://ic.huanxung.cn

JS:   arr.length
来源：http://pw.yuexingan06.cn

TS:   arr.length
来源：http://ro.hahajie.cn

Java: list.size();
来源：http://iq.newstarts.cn

Go:   len(arr)
来源：http://us.szsharing.cn

Ruby: arr.length; arr.size
来源：http://lh.huanxung.cn

C#:   list.Count;
来源：http://mn.nszjky.cn

[D07] 切片 / 取子数组
来源：http://xe.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://px.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ct.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ci.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://du.shxzukj.cn

Java: list.subList(1, 4);
来源：http://ny.bookmarksfly.cn

Go:   arr[1:4]
来源：http://zb.lnxyls.cn

Ruby: arr[1, 3]
来源：http://et.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://zn.yuexingan06.cn

[D08] 合并两个数组
来源：http://lq.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://tb.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://dg.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rl.asd995.cn

TS:   [...a, ...b];
来源：http://xm.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qq.gzmigu.cn

Go:   append(a, b...)
来源：http://qf.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://mg.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://kx.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://gr.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ho.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://ch.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uh.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lx.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://al.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sz.yuexingan06.cn

Ruby: arr.sort
来源：http://tt.szsharing.cn

C#:   list.Sort();
来源：http://mo.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ao.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qj.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fk.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gm.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rm.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zp.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wx.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zx.jctech888.com.cn

[D11] 反转数组
来源：http://kv.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ft.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://iu.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bn.huanxung.cn

TS:   [...arr].reverse();
来源：http://le.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://bm.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://yh.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ve.wgjwhj.cn

C#:   list.Reverse();
来源：http://cj.asd995.cn

[D12] 查找元素下标
来源：http://au.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://tq.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xs.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gh.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wi.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ja.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ge.muxihuayi.cn

Ruby: arr.index(x)
来源：http://mz.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://em.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://vv.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vs.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yr.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://vi.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://zz.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tb.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nl.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gx.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tu.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://cs.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tp.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uf.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://pw.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://za.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uk.huixinmuqiang.cn

Go:   // 手写循环
来源：http://iu.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dd.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ke.hnjuh.cn

[D15] 去重
来源：http://wk.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ye.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://ra.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://tc.asd995.cn

TS:   [...new Set(arr)]
来源：http://rn.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gk.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zi.wgjwhj.cn

Ruby: arr.uniq
来源：http://lm.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://wr.hnjuh.cn

[D16] 求和与平均值
来源：http://li.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aw.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fa.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yz.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ng.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pz.chemitech.net.cn

Go:   // 手写循环累加
来源：http://bf.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ze.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://mo.asd995.cn

[D17] 最大值与最小值
来源：http://zd.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://fn.521024.cn

PHP:  max($arr);  min($arr);
来源：http://tn.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lx.shxzukj.cn

TS:   Math.max(...arr);
来源：http://eo.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sn.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xa.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://kw.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ko.asd995.cn

[D18] 扁平化嵌套数组
来源：http://eb.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cj.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ca.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tf.yuntaijiaju.cn

TS:   nested.flat();
来源：http://lp.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qm.chemitech.net.cn

Go:   // 手写双层循环
来源：http://pl.szxytkj.cn

Ruby: nested.flatten
来源：http://xv.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oe.bookmarksfly.cn

[D19] 按字段分组
来源：http://oi.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oa.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eg.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qc.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tb.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vu.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://bh.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ej.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ya.521024.cn

[D20] 统计每个元素出现次数
来源：http://lg.nszjky.cn

Py:   Counter(arr)
来源：http://qt.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://wj.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yg.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ha.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uz.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://kt.szxytkj.cn

Ruby: arr.tally
来源：http://fu.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xd.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://fu.haigaiapp.cn

Py:   x in arr
来源：http://lh.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://fc.chemitech.net.cn

JS:   arr.includes(x)
来源：http://zt.bjjhwx.cn

TS:   arr.includes(x)
来源：http://mg.newstarts.cn

Java: list.contains(x)
来源：http://hy.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://qc.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://lp.huanxung.cn

C#:   list.Contains(x)
来源：http://rk.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ou.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xf.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rr.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xj.muxihuayi.cn

TS:   [...arr];
来源：http://pf.colortex.cn

Java: new ArrayList<>(list);
来源：http://oj.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ga.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://lt.newstarts.cn

C#:   new List<int>(list);
来源：http://xr.haigaiapp.cn

[D23] reduce 累积计算
来源：http://rm.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vu.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bm.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kb.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dd.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ra.szxytkj.cn

Go:   // 手写循环
来源：http://pm.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mq.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ao.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://go.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sa.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qj.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cl.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fp.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ex.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://og.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ci.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pf.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://bq.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://os.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ut.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://va.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cj.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sl.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nf.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://od.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sa.jctech888.com.cn

[D26] 数组转字符串
来源：http://uo.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://uw.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://cl.newstarts.cn

JS:   arr.join(", ")
来源：http://hy.wgjwhj.cn

TS:   arr.join(", ")
来源：http://lk.asd995.cn

Java: String.join(", ", list)
来源：http://uj.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ao.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://hz.521024.cn

C#:   string.Join(", ", list)
来源：http://le.lnxyls.cn

================================================================================
来源：http://dl.huixinmuqiang.cn

E. 字符串处理
来源：http://le.gzmigu.cn

================================================================================
来源：http://zs.bjjhwx.cn

[E01] 拼接字符串
来源：http://el.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yg.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tv.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ob.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://op.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gy.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pa.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gp.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vz.hahajie.cn

[E02] 重复字符串
来源：http://fz.shxzskj.cn

Py:   "ab" * 3
来源：http://uh.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://qp.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://kw.huanxung.cn

TS:   "ab".repeat(3)
来源：http://ik.szsharing.cn

Java: "ab".repeat(3)
来源：http://tm.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://qq.shxzukj.cn

Ruby: "ab" * 3
来源：http://pm.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sh.bookmarksfly.cn

[E03] 截取子串
来源：http://vm.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vt.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://us.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gv.szsharing.cn

TS:   s.slice(1, 4)
来源：http://vb.newstarts.cn

Java: s.substring(1, 4)
来源：http://oi.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lx.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eh.colortex.cn

C#:   s.Substring(1, 3)
来源：http://om.shtwfgs.cn

[E04] 查找子串位置
来源：http://bw.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://kp.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://do.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nt.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://pm.panjiajie.cn

Java: s.indexOf("x")
来源：http://og.521024.cn

Go:   strings.Index(s, "x")
来源：http://wq.szxytkj.cn

Ruby: s.index("x")
来源：http://qy.colortex.cn

C#:   s.IndexOf("x")
来源：http://dd.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ka.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bi.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eb.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ew.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iq.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lx.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lc.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qn.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://et.9csxet.cn

[E06] 替换子串
来源：http://pl.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ug.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://gs.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iy.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://ka.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pv.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kg.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ri.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://yo.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://uh.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://id.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ol.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dq.asd995.cn

TS:   s.split(",")
来源：http://wv.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ls.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oe.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://is.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gv.9csxet.cn

[E08] 数组按分隔符合并
来源：http://om.nicolike.cn

Py:   ",".join(items)
来源：http://gn.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ht.bookmarksfly.cn

JS:   items.join(",")
来源：http://uy.chemitech.net.cn

TS:   items.join(",")
来源：http://yi.shxzskj.cn

Java: String.join(",", items)
来源：http://zf.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://no.shxzukj.cn

Ruby: items.join(",")
来源：http://dl.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://ye.9csxet.cn

[E09] 去除所有空白字符
来源：http://dv.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bm.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ox.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://nk.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://yz.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://xv.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rx.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cr.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zt.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://hv.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://se.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ta.521024.cn

JS:   "7".padStart(3, "0")
来源：http://gr.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://bt.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://cy.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lz.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hi.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tj.huanxung.cn

[E11] 反转字符串
来源：http://wr.521024.cn

Py:   s[::-1]
来源：http://tz.chemitech.net.cn

PHP:  strrev($s);
来源：http://ob.szxytkj.cn


<!-- 参考信息 -->