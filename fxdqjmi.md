代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://zl.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://pt.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zz.panjiajie.cn

Go:   append(a, b...)
来源：http://se.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://op.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://zk.gzmigu.cn

[D09] 排序（升序）
来源：http://re.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://gb.jctech888.com.cn

PHP:  sort($arr);
来源：http://pr.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bw.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cx.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uo.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fc.panjiajie.cn

Ruby: arr.sort
来源：http://ip.huixiangedu.cn

C#:   list.Sort();
来源：http://bf.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wb.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ap.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qk.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lo.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rj.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ok.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oe.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ju.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uw.bookmarksfly.cn

[D11] 反转数组
来源：http://qp.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tw.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ze.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gq.panjiajie.cn

TS:   [...arr].reverse();
来源：http://xk.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://uf.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://ha.szsharing.cn

Ruby: arr.reverse
来源：http://ll.shxzskj.cn

C#:   list.Reverse();
来源：http://oc.muxihuayi.cn

[D12] 查找元素下标
来源：http://tc.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://mr.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zg.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lx.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ya.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hk.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://mz.szxytkj.cn

Ruby: arr.index(x)
来源：http://ob.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://oz.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://ku.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zs.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sc.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://ep.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://uz.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bq.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ky.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fx.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pn.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://aa.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ju.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fs.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://bj.521024.cn

TS:   arr.map(x => x * 2)
来源：http://wn.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://am.asd995.cn

Go:   // 手写循环
来源：http://sa.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ns.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ax.haigaiapp.cn

[D15] 去重
来源：http://ld.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ey.shxzskj.cn

PHP:  array_unique($arr);
来源：http://ib.hahajie.cn

JS:   [...new Set(arr)]
来源：http://wv.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://az.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vi.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qh.wgjwhj.cn

Ruby: arr.uniq
来源：http://le.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://zm.shxzukj.cn

[D16] 求和与平均值
来源：http://xu.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ts.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ej.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cr.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vw.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gk.nszjky.cn

Go:   // 手写循环累加
来源：http://qx.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oa.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://tk.nszjky.cn

[D17] 最大值与最小值
来源：http://hw.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://hf.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://es.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vj.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://jq.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zj.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pa.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ls.asd995.cn

C#:   list.Max();  list.Min()
来源：http://tw.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://cp.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tr.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://tq.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ot.yuntaijiaju.cn

TS:   nested.flat();
来源：http://sb.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zs.newstarts.cn

Go:   // 手写双层循环
来源：http://tz.hahajie.cn

Ruby: nested.flatten
来源：http://na.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xw.bookmarksfly.cn

[D19] 按字段分组
来源：http://vu.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://at.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://od.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nq.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dx.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gu.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://kq.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sv.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://os.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://vs.chemitech.net.cn

Py:   Counter(arr)
来源：http://lo.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://gm.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qe.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dg.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://ye.bookmarksfly.cn

Ruby: arr.tally
来源：http://us.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oz.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://fd.nicolike.cn

Py:   x in arr
来源：http://bz.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://np.bjjhwx.cn

JS:   arr.includes(x)
来源：http://kg.hnjuh.cn

TS:   arr.includes(x)
来源：http://kz.szsharing.cn

Java: list.contains(x)
来源：http://qk.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://ek.9csxet.cn

Ruby: arr.include?(x)
来源：http://ne.yuexingan06.cn

C#:   list.Contains(x)
来源：http://xn.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://bw.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ho.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://im.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tk.nicolike.cn

TS:   [...arr];
来源：http://ey.9csxet.cn

Java: new ArrayList<>(list);
来源：http://gb.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vq.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://cm.colortex.cn

C#:   new List<int>(list);
来源：http://re.huixiangedu.cn

[D23] reduce 累积计算
来源：http://yr.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rc.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ss.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ro.bjjhwx.cn

Go:   // 手写循环
来源：http://iy.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ws.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://az.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://aw.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oi.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://km.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://by.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ky.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://as.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bb.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kc.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lt.asd995.cn

[D25] Set 集合去重与交并差
来源：http://fb.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://je.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mp.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pn.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dp.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uu.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mr.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sw.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cc.gzmigu.cn

[D26] 数组转字符串
来源：http://fb.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ne.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://aa.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://pc.wgjwhj.cn

TS:   arr.join(", ")
来源：http://pn.yuexingan06.cn

Java: String.join(", ", list)
来源：http://jg.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://wv.nicolike.cn

Ruby: arr.join(", ")
来源：http://ge.szsharing.cn

C#:   string.Join(", ", list)
来源：http://wc.shxzukj.cn

================================================================================
来源：http://oc.lnxyls.cn

E. 字符串处理
来源：http://nw.huixiangedu.cn

================================================================================
来源：http://xf.huixiangedu.cn

[E01] 拼接字符串
来源：http://st.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ut.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ha.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yw.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xy.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fv.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nh.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ig.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gc.haigaiapp.cn

[E02] 重复字符串
来源：http://hk.nicolike.cn

Py:   "ab" * 3
来源：http://zq.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://jo.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://cj.newstarts.cn

TS:   "ab".repeat(3)
来源：http://xn.asd995.cn

Java: "ab".repeat(3)
来源：http://qs.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://fm.szxytkj.cn

Ruby: "ab" * 3
来源：http://tm.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cf.shxzskj.cn

[E03] 截取子串
来源：http://nt.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yw.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bp.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bd.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://rl.hnjuh.cn

Java: s.substring(1, 4)
来源：http://ar.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wm.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ws.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://to.521024.cn

[E04] 查找子串位置
来源：http://ob.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://kw.asd995.cn

PHP:  strpos($s, "x");
来源：http://vs.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ky.hnjuh.cn

TS:   s.indexOf("x")
来源：http://ra.huanxung.cn

Java: s.indexOf("x")
来源：http://yl.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://dz.szxytkj.cn

Ruby: s.index("x")
来源：http://vb.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://oa.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zn.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mn.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kn.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nx.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kc.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zx.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ug.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ie.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nc.jianghongdianzi.cn

[E06] 替换子串
来源：http://ko.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wk.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://xl.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kr.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://au.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ml.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lu.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://th.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://en.newstarts.cn

[E07] 按分隔符拆分
来源：http://qy.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qy.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hb.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pu.huanxung.cn

TS:   s.split(",")
来源：http://uc.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eg.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uc.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://hi.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ci.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://bo.newstarts.cn

Py:   ",".join(items)
来源：http://ki.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://gc.nszjky.cn

JS:   items.join(",")
来源：http://gu.jctech888.com.cn

TS:   items.join(",")
来源：http://ck.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://zz.colortex.cn

Go:   strings.Join(items, ",")
来源：http://bp.shxzskj.cn

Ruby: items.join(",")
来源：http://sa.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://we.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://am.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mt.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ow.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://zo.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://pu.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://za.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ol.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cq.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://ts.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ev.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ci.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://rf.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://od.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://fq.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nx.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iq.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ot.yuntaijiaju.cn

[E11] 反转字符串
来源：http://by.521024.cn

Py:   s[::-1]
来源：http://jn.szsharing.cn

PHP:  strrev($s);
来源：http://vj.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://zc.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://kh.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gx.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ko.huanxung.cn

Ruby: s.reverse
来源：http://vq.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qq.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://pk.huixiangedu.cn

Py:   s.count("a")
来源：http://hu.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://lc.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://eq.szsharing.cn

TS:   s.split("a").length - 1
来源：http://fm.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zu.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://fk.wgjwhj.cn

Ruby: s.count("a")
来源：http://ct.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://wd.jctech888.com.cn

[E13] 逐字符遍历
来源：http://wp.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://wg.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tv.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://da.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tp.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vp.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gu.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vj.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qa.asd995.cn

[E14] URL 编码与 Base64
来源：http://kc.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lz.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://za.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cf.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nf.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kv.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ch.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nj.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://sa.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pj.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vi.chemitech.net.cn


<!-- 参考信息 -->