代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://zq.lnxyls.cn

[D08] 合并两个数组
来源：http://zp.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://uk.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://aa.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://el.521024.cn

TS:   [...a, ...b];
来源：http://ot.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mb.shxzukj.cn

Go:   append(a, b...)
来源：http://mq.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://iz.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://cn.shxzukj.cn

[D09] 排序（升序）
来源：http://lz.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://lx.hnjuh.cn

PHP:  sort($arr);
来源：http://ha.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vv.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fr.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ef.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qu.521024.cn

Ruby: arr.sort
来源：http://bv.panjiajie.cn

C#:   list.Sort();
来源：http://ze.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zs.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sc.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://na.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wt.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fe.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pz.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lh.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jl.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bk.szsharing.cn

[D11] 反转数组
来源：http://cg.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qp.9csxet.cn

PHP:  array_reverse($arr);
来源：http://py.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rp.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://zf.gzmigu.cn

Java: Collections.reverse(list);
来源：http://iz.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://re.gzmigu.cn

Ruby: arr.reverse
来源：http://yz.hnjuh.cn

C#:   list.Reverse();
来源：http://lp.chemitech.net.cn

[D12] 查找元素下标
来源：http://fi.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://gz.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ye.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hv.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bp.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://jc.lnxyls.cn

Ruby: arr.index(x)
来源：http://gl.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ld.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://bw.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aa.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://df.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://og.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ey.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kr.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zf.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tq.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eq.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://aa.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ld.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ta.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://lx.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://rj.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vm.shxzukj.cn

Go:   // 手写循环
来源：http://qd.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mw.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ra.jianghongdianzi.cn

[D15] 去重
来源：http://fr.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dw.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ay.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://ox.521024.cn

TS:   [...new Set(arr)]
来源：http://cu.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hi.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yr.chemitech.net.cn

Ruby: arr.uniq
来源：http://gs.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://vi.wgjwhj.cn

[D16] 求和与平均值
来源：http://gd.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nu.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bl.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ek.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bg.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sl.9csxet.cn

Go:   // 手写循环累加
来源：http://ha.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hd.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://si.huanxung.cn

[D17] 最大值与最小值
来源：http://gb.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://so.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://bz.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ci.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://tw.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uj.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xs.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://kj.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://vk.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://yz.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ph.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://cd.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qw.yuntaijiaju.cn

TS:   nested.flat();
来源：http://gj.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jt.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://oh.lnxyls.cn

Ruby: nested.flatten
来源：http://rl.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tl.nszjky.cn

[D19] 按字段分组
来源：http://qk.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ak.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ex.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sw.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://or.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://do.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://gu.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yp.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://at.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://xe.lnxyls.cn

Py:   Counter(arr)
来源：http://ue.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://yo.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hk.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xd.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ll.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://xm.huanxung.cn

Ruby: arr.tally
来源：http://lh.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tw.nszjky.cn

[D21] 判断是否包含某元素
来源：http://uw.hnjuh.cn

Py:   x in arr
来源：http://wm.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://vn.colortex.cn

JS:   arr.includes(x)
来源：http://qc.wgjwhj.cn

TS:   arr.includes(x)
来源：http://pd.jctech888.com.cn

Java: list.contains(x)
来源：http://in.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://kt.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://av.9csxet.cn

C#:   list.Contains(x)
来源：http://yy.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://pz.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ud.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hh.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jk.9csxet.cn

TS:   [...arr];
来源：http://zx.newstarts.cn

Java: new ArrayList<>(list);
来源：http://qs.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ni.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://ny.szxytkj.cn

C#:   new List<int>(list);
来源：http://rs.nicolike.cn

[D23] reduce 累积计算
来源：http://nw.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bu.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zp.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hw.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ad.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zh.521024.cn

Go:   // 手写循环
来源：http://qc.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sb.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zh.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://ot.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ir.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bj.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ei.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vc.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rh.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://on.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eu.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tq.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://sx.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zm.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hr.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fu.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vt.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://py.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ub.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jl.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rk.szxytkj.cn

[D26] 数组转字符串
来源：http://kf.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://qg.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://ec.nszjky.cn

JS:   arr.join(", ")
来源：http://vc.521024.cn

TS:   arr.join(", ")
来源：http://vx.hahajie.cn

Java: String.join(", ", list)
来源：http://bg.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ao.shxzukj.cn

Ruby: arr.join(", ")
来源：http://iy.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://yp.jianghongdianzi.cn

================================================================================
来源：http://in.9csxet.cn

E. 字符串处理
来源：http://dr.521024.cn

================================================================================
来源：http://cr.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://hw.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rj.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wy.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xy.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ok.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wf.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zq.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.huixinmuqiang.cn

[E02] 重复字符串
来源：http://bm.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://el.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://vs.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ze.hahajie.cn

TS:   "ab".repeat(3)
来源：http://tk.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://uh.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://tx.lnxyls.cn

Ruby: "ab" * 3
来源：http://vq.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wd.nicolike.cn

[E03] 截取子串
来源：http://eu.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gx.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dv.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jj.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://jg.shxzskj.cn

Java: s.substring(1, 4)
来源：http://vj.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xc.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ao.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ea.muxihuayi.cn

[E04] 查找子串位置
来源：http://xj.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://li.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://sq.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uc.hahajie.cn

TS:   s.indexOf("x")
来源：http://td.lnxyls.cn

Java: s.indexOf("x")
来源：http://jf.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://tm.asd995.cn

Ruby: s.index("x")
来源：http://eu.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://wo.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sk.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ci.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hp.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ue.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://io.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uq.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xh.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qw.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ug.huixiangedu.cn

[E06] 替换子串
来源：http://vu.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://co.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://xa.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://qb.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wb.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cn.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kr.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://oz.hnjuh.cn

[E07] 按分隔符拆分
来源：http://nm.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ac.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vs.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kh.jctech888.com.cn

TS:   s.split(",")
来源：http://jz.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://au.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lc.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://dw.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pi.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://us.nszjky.cn

Py:   ",".join(items)
来源：http://eq.nszjky.cn

PHP:  implode(",", $items);
来源：http://jt.asd995.cn

JS:   items.join(",")
来源：http://iz.huanxung.cn

TS:   items.join(",")
来源：http://ht.hahajie.cn

Java: String.join(",", items)
来源：http://yi.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://wx.chemitech.net.cn

Ruby: items.join(",")
来源：http://zy.gzmigu.cn

C#:   string.Join(",", items)
来源：http://km.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://uv.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lt.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mm.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://pf.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://jg.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://jc.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ax.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lk.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ev.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://an.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ao.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pa.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://rv.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://mn.szsharing.cn

Java: String.format("%03d", 7)
来源：http://hg.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://je.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ha.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zo.bookmarksfly.cn

[E11] 反转字符串
来源：http://na.wgjwhj.cn

Py:   s[::-1]
来源：http://xs.lnxyls.cn

PHP:  strrev($s);
来源：http://lz.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://hg.521024.cn

TS:   [...s].reverse().join("")
来源：http://xl.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hb.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ne.colortex.cn

Ruby: s.reverse
来源：http://xk.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bz.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://jc.9csxet.cn

Py:   s.count("a")
来源：http://hm.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ud.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://di.9csxet.cn

TS:   s.split("a").length - 1
来源：http://kn.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://em.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://lr.shxzskj.cn

Ruby: s.count("a")
来源：http://pc.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://gl.szsharing.cn

[E13] 逐字符遍历
来源：http://pz.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ue.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zb.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bv.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dh.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yo.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fn.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rh.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fh.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://yr.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gr.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kq.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cz.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ae.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wn.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sw.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yp.gzmigu.cn


<!-- 参考信息 -->