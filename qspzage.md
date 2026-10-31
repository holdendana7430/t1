代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zd.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://at.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://uu.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ze.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://tt.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ps.yuexingan06.cn

[D06] 数组长度
来源：http://uc.hnjuh.cn

Py:   len(arr)
来源：http://ac.newstarts.cn

PHP:  count($arr);
来源：http://to.nicolike.cn

JS:   arr.length
来源：http://vl.521024.cn

TS:   arr.length
来源：http://le.nicolike.cn

Java: list.size();
来源：http://rv.szxytkj.cn

Go:   len(arr)
来源：http://pw.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://wa.muxihuayi.cn

C#:   list.Count;
来源：http://ty.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://bi.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fq.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zf.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://nk.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://yu.newstarts.cn

Java: list.subList(1, 4);
来源：http://sc.huixiangedu.cn

Go:   arr[1:4]
来源：http://my.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://ix.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://zi.chemitech.net.cn

[D08] 合并两个数组
来源：http://cr.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://vh.colortex.cn

PHP:  array_merge($a, $b);
来源：http://jg.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zq.9csxet.cn

TS:   [...a, ...b];
来源：http://er.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yr.asd995.cn

Go:   append(a, b...)
来源：http://ok.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://bq.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://mq.hnjuh.cn

[D09] 排序（升序）
来源：http://mx.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://bt.yuexingan06.cn

PHP:  sort($arr);
来源：http://kt.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mj.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dj.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://od.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dm.huanxung.cn

Ruby: arr.sort
来源：http://gc.yuntaijiaju.cn

C#:   list.Sort();
来源：http://jz.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cu.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ip.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qz.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vo.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gx.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vj.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gx.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ui.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.bookmarksfly.cn

[D11] 反转数组
来源：http://kg.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dx.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://vg.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xu.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://zg.huanxung.cn

Java: Collections.reverse(list);
来源：http://nx.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://eq.newstarts.cn

Ruby: arr.reverse
来源：http://af.wgjwhj.cn

C#:   list.Reverse();
来源：http://eu.wgjwhj.cn

[D12] 查找元素下标
来源：http://zn.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://cs.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lc.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dw.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ov.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ob.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://xu.nicolike.cn

Ruby: arr.index(x)
来源：http://bg.9csxet.cn

C#:   list.IndexOf(x);
来源：http://fm.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://kj.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nd.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ts.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://am.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ke.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yr.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uu.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xc.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lu.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://tw.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sw.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fi.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://gs.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://qq.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yw.gzmigu.cn

Go:   // 手写循环
来源：http://sk.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://by.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sy.asd995.cn

[D15] 去重
来源：http://oi.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://az.nszjky.cn

PHP:  array_unique($arr);
来源：http://rd.9csxet.cn

JS:   [...new Set(arr)]
来源：http://xi.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://lp.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://en.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yv.huixiangedu.cn

Ruby: arr.uniq
来源：http://ia.asd995.cn

C#:   list.Distinct().ToList()
来源：http://zc.muxihuayi.cn

[D16] 求和与平均值
来源：http://ky.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ym.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cm.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yo.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zt.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tf.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://xe.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zt.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://la.hnjuh.cn

[D17] 最大值与最小值
来源：http://xv.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ju.521024.cn

PHP:  max($arr);  min($arr);
来源：http://qf.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yp.asd995.cn

TS:   Math.max(...arr);
来源：http://hp.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fk.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tv.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://ik.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://yp.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://aq.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zn.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://zq.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zn.hnjuh.cn

TS:   nested.flat();
来源：http://af.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vk.hahajie.cn

Go:   // 手写双层循环
来源：http://is.shtwfgs.cn

Ruby: nested.flatten
来源：http://qa.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hp.muxihuayi.cn

[D19] 按字段分组
来源：http://yp.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sy.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qs.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ld.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ec.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wy.colortex.cn

Go:   // 手写 map[string][]T
来源：http://fv.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://be.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qo.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ut.chemitech.net.cn

Py:   Counter(arr)
来源：http://ni.szsharing.cn

PHP:  array_count_values($arr);
来源：http://qo.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sw.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jp.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pn.szsharing.cn

Go:   // 手写 map[T]int
来源：http://yb.huanxung.cn

Ruby: arr.tally
来源：http://ay.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.nicolike.cn

[D21] 判断是否包含某元素
来源：http://ca.521024.cn

Py:   x in arr
来源：http://ia.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://sg.shtwfgs.cn

JS:   arr.includes(x)
来源：http://fk.szxytkj.cn

TS:   arr.includes(x)
来源：http://sq.shtwfgs.cn

Java: list.contains(x)
来源：http://iz.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://xx.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://pm.colortex.cn

C#:   list.Contains(x)
来源：http://fm.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://bk.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ez.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rb.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fa.bjjhwx.cn

TS:   [...arr];
来源：http://vy.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://yg.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mb.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://tl.panjiajie.cn

C#:   new List<int>(list);
来源：http://ki.panjiajie.cn

[D23] reduce 累积计算
来源：http://bq.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zu.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bu.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lu.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fk.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ev.panjiajie.cn

Go:   // 手写循环
来源：http://rm.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ln.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ux.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://bq.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pe.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ak.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gg.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cn.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://si.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://te.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jl.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ij.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://bz.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://td.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ks.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ns.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jw.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ln.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wx.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hb.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://he.jctech888.com.cn

[D26] 数组转字符串
来源：http://ui.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://wm.521024.cn

PHP:  implode(", ", $arr);
来源：http://nv.nicolike.cn

JS:   arr.join(", ")
来源：http://cu.huanxung.cn

TS:   arr.join(", ")
来源：http://zy.shxzukj.cn

Java: String.join(", ", list)
来源：http://pt.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://em.hahajie.cn

Ruby: arr.join(", ")
来源：http://we.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://ud.bookmarksfly.cn

================================================================================
来源：http://xv.newstarts.cn

E. 字符串处理
来源：http://km.lnxyls.cn

================================================================================
来源：http://tq.newstarts.cn

[E01] 拼接字符串
来源：http://bm.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pm.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ue.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ib.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://at.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zu.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rc.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rh.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aw.chemitech.net.cn

[E02] 重复字符串
来源：http://rb.szsharing.cn

Py:   "ab" * 3
来源：http://ib.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://qu.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://jg.9csxet.cn

TS:   "ab".repeat(3)
来源：http://oa.hahajie.cn

Java: "ab".repeat(3)
来源：http://xv.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://vb.huanxung.cn

Ruby: "ab" * 3
来源：http://nt.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ny.jianghongdianzi.cn

[E03] 截取子串
来源：http://cj.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ef.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tc.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cb.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://tw.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://si.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ak.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jo.colortex.cn

C#:   s.Substring(1, 3)
来源：http://ru.9csxet.cn

[E04] 查找子串位置
来源：http://el.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://lq.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://cg.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jq.shxzukj.cn

TS:   s.indexOf("x")
来源：http://wk.gzmigu.cn

Java: s.indexOf("x")
来源：http://gj.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://wj.newstarts.cn

Ruby: s.index("x")
来源：http://ao.asd995.cn

C#:   s.IndexOf("x")
来源：http://fs.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kq.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ho.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bg.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uz.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://of.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nh.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eb.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ye.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vc.shxzskj.cn

[E06] 替换子串
来源：http://wb.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rj.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://gm.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tm.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://cm.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://la.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bz.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eq.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://is.nszjky.cn

[E07] 按分隔符拆分
来源：http://or.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yu.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ao.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vr.bjjhwx.cn

TS:   s.split(",")
来源：http://rr.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ah.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dj.521024.cn

Ruby: s.split(",");  s.split
来源：http://ar.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ph.nszjky.cn

[E08] 数组按分隔符合并
来源：http://ro.shtwfgs.cn

Py:   ",".join(items)
来源：http://rm.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://wb.jianghongdianzi.cn

JS:   items.join(",")
来源：http://oq.huixinmuqiang.cn

TS:   items.join(",")
来源：http://su.521024.cn

Java: String.join(",", items)
来源：http://yn.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://dz.szxytkj.cn

Ruby: items.join(",")
来源：http://ns.colortex.cn

C#:   string.Join(",", items)
来源：http://vm.nicolike.cn

[E09] 去除所有空白字符
来源：http://mp.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ht.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dm.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://mc.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://hw.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://em.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vv.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://or.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://zt.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ie.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ja.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://yi.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://cr.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://lv.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kk.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sh.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://na.shxzukj.cn

[E11] 反转字符串
来源：http://sw.hnjuh.cn

Py:   s[::-1]
来源：http://qv.huixiangedu.cn

PHP:  strrev($s);
来源：http://bj.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://sm.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://cl.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uo.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ie.nszjky.cn

Ruby: s.reverse
来源：http://nr.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hl.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://eu.jianghongdianzi.cn

Py:   s.count("a")
来源：http://qj.szsharing.cn


<!-- 参考信息 -->