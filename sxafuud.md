代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ns.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tk.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wg.muxihuayi.cn

[D06] 数组长度
来源：http://sl.nicolike.cn

Py:   len(arr)
来源：http://xm.hahajie.cn

PHP:  count($arr);
来源：http://ds.szsharing.cn

JS:   arr.length
来源：http://em.9csxet.cn

TS:   arr.length
来源：http://lf.chemitech.net.cn

Java: list.size();
来源：http://tm.521024.cn

Go:   len(arr)
来源：http://wm.asd995.cn

Ruby: arr.length; arr.size
来源：http://vv.jctech888.com.cn

C#:   list.Count;
来源：http://pm.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://gv.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ac.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sv.asd995.cn

JS:   arr.slice(1, 4);
来源：http://dv.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://er.lnxyls.cn

Java: list.subList(1, 4);
来源：http://ro.haigaiapp.cn

Go:   arr[1:4]
来源：http://yw.lnxyls.cn

Ruby: arr[1, 3]
来源：http://ep.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://po.nszjky.cn

[D08] 合并两个数组
来源：http://qk.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://xl.521024.cn

PHP:  array_merge($a, $b);
来源：http://sm.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vg.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://mn.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gi.huanxung.cn

Go:   append(a, b...)
来源：http://sw.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://gq.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ll.shtwfgs.cn

[D09] 排序（升序）
来源：http://kw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://fz.521024.cn

PHP:  sort($arr);
来源：http://lk.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zd.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://va.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mg.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hv.yuexingan06.cn

Ruby: arr.sort
来源：http://hz.nszjky.cn

C#:   list.Sort();
来源：http://no.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wg.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cs.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pd.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ck.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://da.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oa.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wo.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://up.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hh.jctech888.com.cn

[D11] 反转数组
来源：http://mm.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ww.newstarts.cn

PHP:  array_reverse($arr);
来源：http://vm.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wx.szsharing.cn

TS:   [...arr].reverse();
来源：http://jz.newstarts.cn

Java: Collections.reverse(list);
来源：http://nh.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ac.colortex.cn

Ruby: arr.reverse
来源：http://ib.haigaiapp.cn

C#:   list.Reverse();
来源：http://ck.521024.cn

[D12] 查找元素下标
来源：http://dr.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://jc.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://df.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://on.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gc.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rd.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ke.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://eh.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ht.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://hb.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wv.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yk.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://te.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://dr.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fc.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ti.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ho.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://re.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://cp.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lv.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qd.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://jf.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://kj.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oe.huanxung.cn

Go:   // 手写循环
来源：http://yk.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yh.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pe.nszjky.cn

[D15] 去重
来源：http://sb.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gi.colortex.cn

PHP:  array_unique($arr);
来源：http://hy.asd995.cn

JS:   [...new Set(arr)]
来源：http://ao.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://lq.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ea.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xp.gzmigu.cn

Ruby: arr.uniq
来源：http://se.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://oh.yuexingan06.cn

[D16] 求和与平均值
来源：http://os.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ub.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wi.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cu.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ue.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jr.asd995.cn

Go:   // 手写循环累加
来源：http://iz.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gv.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://va.shxzukj.cn

[D17] 最大值与最小值
来源：http://un.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://ci.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://sm.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pf.gzmigu.cn

TS:   Math.max(...arr);
来源：http://tv.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mv.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zy.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://wv.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://bh.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://zk.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jm.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://wk.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eo.bookmarksfly.cn

TS:   nested.flat();
来源：http://lr.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gz.chemitech.net.cn

Go:   // 手写双层循环
来源：http://qx.muxihuayi.cn

Ruby: nested.flatten
来源：http://hp.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kd.huanxung.cn

[D19] 按字段分组
来源：http://to.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nw.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rf.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hf.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yo.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gk.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://pc.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://br.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iq.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://fe.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://ls.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://zs.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tn.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cm.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bx.colortex.cn

Go:   // 手写 map[T]int
来源：http://sv.huixinmuqiang.cn

Ruby: arr.tally
来源：http://lu.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fe.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://xg.bjjhwx.cn

Py:   x in arr
来源：http://px.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://hm.chemitech.net.cn

JS:   arr.includes(x)
来源：http://wl.shtwfgs.cn

TS:   arr.includes(x)
来源：http://oq.newstarts.cn

Java: list.contains(x)
来源：http://tn.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://fi.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ql.asd995.cn

C#:   list.Contains(x)
来源：http://zq.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://da.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ud.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dm.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gs.szxytkj.cn

TS:   [...arr];
来源：http://oz.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://lo.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jz.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://uk.panjiajie.cn

C#:   new List<int>(list);
来源：http://ra.chemitech.net.cn

[D23] reduce 累积计算
来源：http://xa.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bb.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ke.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://px.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zd.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://on.newstarts.cn

Go:   // 手写循环
来源：http://hi.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yh.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xk.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ac.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bz.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bd.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ah.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kt.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nm.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://um.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vf.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://is.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bu.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ph.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jj.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mh.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nz.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tb.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cs.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lg.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://zh.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://xr.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://xz.bjjhwx.cn

JS:   arr.join(", ")
来源：http://ih.yuexingan06.cn

TS:   arr.join(", ")
来源：http://lh.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://bt.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://mx.nicolike.cn

Ruby: arr.join(", ")
来源：http://lr.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://xn.nicolike.cn

================================================================================
来源：http://rk.gzmigu.cn

E. 字符串处理
来源：http://xa.bookmarksfly.cn

================================================================================
来源：http://di.asd995.cn

[E01] 拼接字符串
来源：http://kk.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wk.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xw.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://te.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dw.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ve.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://et.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kv.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qn.bjjhwx.cn

[E02] 重复字符串
来源：http://dz.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://yo.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://wj.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://mf.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://gx.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ft.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://cd.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://dd.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yd.yuexingan06.cn

[E03] 截取子串
来源：http://cr.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cl.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iw.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pd.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://no.szxytkj.cn

Java: s.substring(1, 4)
来源：http://tc.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kh.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ga.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://xo.hnjuh.cn

[E04] 查找子串位置
来源：http://ne.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://lt.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://ja.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://po.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ww.colortex.cn

Java: s.indexOf("x")
来源：http://bx.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://kl.panjiajie.cn

Ruby: s.index("x")
来源：http://jq.szsharing.cn

C#:   s.IndexOf("x")
来源：http://kq.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iw.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jc.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hr.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ct.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sx.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qi.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rv.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cb.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rg.shxzskj.cn

[E06] 替换子串
来源：http://yz.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://st.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://fh.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ms.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://dz.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zy.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jk.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fw.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://se.panjiajie.cn

[E07] 按分隔符拆分
来源：http://mj.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uc.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ll.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cl.yuntaijiaju.cn

TS:   s.split(",")
来源：http://ol.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://al.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eq.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://tc.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ra.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://gd.bjjhwx.cn

Py:   ",".join(items)
来源：http://hb.nicolike.cn

PHP:  implode(",", $items);
来源：http://ja.9csxet.cn

JS:   items.join(",")
来源：http://ov.shxzukj.cn

TS:   items.join(",")
来源：http://dt.szxytkj.cn

Java: String.join(",", items)
来源：http://lg.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://tj.bookmarksfly.cn

Ruby: items.join(",")
来源：http://vb.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://td.newstarts.cn

[E09] 去除所有空白字符
来源：http://lg.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rq.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sy.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://sv.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ik.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://fn.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bq.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xt.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dg.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://vw.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tt.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dz.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://lx.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://wn.9csxet.cn

Java: String.format("%03d", 7)
来源：http://yy.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tp.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mx.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://es.bjjhwx.cn

[E11] 反转字符串
来源：http://od.yuntaijiaju.cn

Py:   s[::-1]
来源：http://xo.yuexingan06.cn

PHP:  strrev($s);
来源：http://fa.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://kg.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://co.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gl.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yb.muxihuayi.cn

Ruby: s.reverse
来源：http://yh.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ig.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://qm.wgjwhj.cn

Py:   s.count("a")
来源：http://cv.asd995.cn

PHP:  substr_count($s, "a");
来源：http://aq.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ai.szsharing.cn

TS:   s.split("a").length - 1
来源：http://qv.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://in.wgjwhj.cn


<!-- 参考信息 -->