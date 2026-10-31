代发 wailian999

[D07] 切片 / 取子数组
来源：http://lh.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://un.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tf.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://ac.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://xk.newstarts.cn

Java: list.subList(1, 4);
来源：http://fm.gzmigu.cn

Go:   arr[1:4]
来源：http://wr.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://yg.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://qj.shxzukj.cn

[D08] 合并两个数组
来源：http://eh.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ea.asd995.cn

PHP:  array_merge($a, $b);
来源：http://vs.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wy.newstarts.cn

TS:   [...a, ...b];
来源：http://is.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wr.szxytkj.cn

Go:   append(a, b...)
来源：http://qq.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://xl.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://im.nszjky.cn

[D09] 排序（升序）
来源：http://dh.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://hw.yuexingan06.cn

PHP:  sort($arr);
来源：http://tw.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mj.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lr.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wt.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jp.wgjwhj.cn

Ruby: arr.sort
来源：http://fa.muxihuayi.cn

C#:   list.Sort();
来源：http://ae.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ev.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ji.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ho.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://na.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xo.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ay.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zo.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cs.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vl.huanxung.cn

[D11] 反转数组
来源：http://jy.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jc.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://sy.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sb.hnjuh.cn

TS:   [...arr].reverse();
来源：http://wf.hahajie.cn

Java: Collections.reverse(list);
来源：http://xo.colortex.cn

Go:   slices.Reverse(arr)
来源：http://ks.nicolike.cn

Ruby: arr.reverse
来源：http://wd.nszjky.cn

C#:   list.Reverse();
来源：http://fr.jctech888.com.cn

[D12] 查找元素下标
来源：http://om.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://hh.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yx.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lk.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nc.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qz.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://mr.nicolike.cn

Ruby: arr.index(x)
来源：http://xk.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://ko.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://gv.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vv.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tn.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://fm.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://wt.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zp.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ji.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xc.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zi.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://qk.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wf.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ip.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://px.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://ox.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ze.lnxyls.cn

Go:   // 手写循环
来源：http://vl.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xq.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lg.nicolike.cn

[D15] 去重
来源：http://eq.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rs.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ww.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://lv.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://ea.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rk.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hh.nicolike.cn

Ruby: arr.uniq
来源：http://ur.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://fv.newstarts.cn

[D16] 求和与平均值
来源：http://zt.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ql.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tq.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yp.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ug.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yh.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://vp.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jd.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://fp.panjiajie.cn

[D17] 最大值与最小值
来源：http://ja.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://tx.521024.cn

PHP:  max($arr);  min($arr);
来源：http://vn.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sp.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://wy.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fd.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nm.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://it.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://tt.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://gs.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lo.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://cy.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tj.nszjky.cn

TS:   nested.flat();
来源：http://uh.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dv.chemitech.net.cn

Go:   // 手写双层循环
来源：http://bt.szsharing.cn

Ruby: nested.flatten
来源：http://es.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uy.9csxet.cn

[D19] 按字段分组
来源：http://zn.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nv.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lg.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kc.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zm.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oq.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://uw.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kc.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bn.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://la.521024.cn

Py:   Counter(arr)
来源：http://aq.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://ne.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rz.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tw.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://he.nszjky.cn

Go:   // 手写 map[T]int
来源：http://rr.newstarts.cn

Ruby: arr.tally
来源：http://qj.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yu.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://ds.szsharing.cn

Py:   x in arr
来源：http://as.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://zp.nszjky.cn

JS:   arr.includes(x)
来源：http://ut.bjjhwx.cn

TS:   arr.includes(x)
来源：http://py.colortex.cn

Java: list.contains(x)
来源：http://fy.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://xe.szxytkj.cn

Ruby: arr.include?(x)
来源：http://tz.yuexingan06.cn

C#:   list.Contains(x)
来源：http://gu.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://vj.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tb.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wm.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dl.colortex.cn

TS:   [...arr];
来源：http://tk.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://rj.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nl.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ct.colortex.cn

C#:   new List<int>(list);
来源：http://vx.shxzukj.cn

[D23] reduce 累积计算
来源：http://bv.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yl.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://br.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://es.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gi.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hg.chemitech.net.cn

Go:   // 手写循环
来源：http://vk.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pv.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ke.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://gs.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ni.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jd.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ka.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lf.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ej.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kx.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qu.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xr.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ok.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ao.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://js.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uh.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://un.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nj.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uq.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ri.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://me.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://ri.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://ta.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://qn.hahajie.cn

JS:   arr.join(", ")
来源：http://ee.wgjwhj.cn

TS:   arr.join(", ")
来源：http://qe.panjiajie.cn

Java: String.join(", ", list)
来源：http://lg.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ul.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://la.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://lt.jctech888.com.cn

================================================================================
来源：http://nw.gzmigu.cn

E. 字符串处理
来源：http://td.szxytkj.cn

================================================================================
来源：http://jv.asd995.cn

[E01] 拼接字符串
来源：http://du.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ia.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vo.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aj.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://va.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gt.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pb.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cy.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aq.muxihuayi.cn

[E02] 重复字符串
来源：http://dp.521024.cn

Py:   "ab" * 3
来源：http://hi.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://pz.9csxet.cn

JS:   "ab".repeat(3)
来源：http://rm.hahajie.cn

TS:   "ab".repeat(3)
来源：http://ig.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://hi.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://tv.chemitech.net.cn

Ruby: "ab" * 3
来源：http://pv.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mg.yuexingan06.cn

[E03] 截取子串
来源：http://ig.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://me.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hn.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pc.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://hb.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ii.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qt.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bg.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://gw.newstarts.cn

[E04] 查找子串位置
来源：http://uc.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://py.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://rt.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rw.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://hh.lnxyls.cn

Java: s.indexOf("x")
来源：http://xt.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://sz.newstarts.cn

Ruby: s.index("x")
来源：http://ec.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://yk.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xa.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kx.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nf.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lm.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ho.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dy.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oo.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yz.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vq.yuntaijiaju.cn

[E06] 替换子串
来源：http://jo.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nv.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://le.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://et.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://vs.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bt.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xo.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qv.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://jo.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://hu.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ba.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mw.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bz.nicolike.cn

TS:   s.split(",")
来源：http://kr.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ww.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rr.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://nf.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lx.nszjky.cn

[E08] 数组按分隔符合并
来源：http://qv.bjjhwx.cn

Py:   ",".join(items)
来源：http://hv.nszjky.cn

PHP:  implode(",", $items);
来源：http://lh.szsharing.cn

JS:   items.join(",")
来源：http://ik.haigaiapp.cn

TS:   items.join(",")
来源：http://aq.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://pz.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://hm.lnxyls.cn

Ruby: items.join(",")
来源：http://ox.shxzskj.cn

C#:   string.Join(",", items)
来源：http://xt.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://vq.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tm.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jb.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://cu.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://dj.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pn.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sq.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vn.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lv.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://vv.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ri.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wp.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://sa.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://xy.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://gk.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mz.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ow.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ac.huixiangedu.cn

[E11] 反转字符串
来源：http://fw.colortex.cn

Py:   s[::-1]
来源：http://dn.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://ja.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://pw.521024.cn

TS:   [...s].reverse().join("")
来源：http://ph.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ui.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gn.szsharing.cn

Ruby: s.reverse
来源：http://qu.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rm.newstarts.cn

[E12] 统计某字符出现次数
来源：http://fx.asd995.cn

Py:   s.count("a")
来源：http://xw.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://bo.szsharing.cn

JS:   s.split("a").length - 1
来源：http://mu.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://ck.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://om.521024.cn

Go:   strings.Count(s, "a")
来源：http://jx.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://fe.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://tj.haigaiapp.cn

[E13] 逐字符遍历
来源：http://pi.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://vv.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://if.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xv.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aj.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sk.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gg.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://af.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ex.shxzskj.cn


<!-- 参考信息 -->