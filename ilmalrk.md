代发 wailian999

[D07] 切片 / 取子数组
来源：http://ye.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mu.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hu.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://ns.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://bk.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://dl.wgjwhj.cn

Go:   arr[1:4]
来源：http://uy.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ug.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://db.9csxet.cn

[D08] 合并两个数组
来源：http://vv.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://wb.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://iy.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hh.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://qr.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zo.asd995.cn

Go:   append(a, b...)
来源：http://wi.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://fh.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://qm.lnxyls.cn

[D09] 排序（升序）
来源：http://sz.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://tg.jctech888.com.cn

PHP:  sort($arr);
来源：http://ja.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zd.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tg.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sf.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qd.chemitech.net.cn

Ruby: arr.sort
来源：http://oo.haigaiapp.cn

C#:   list.Sort();
来源：http://kt.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cj.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dj.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ug.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yj.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dp.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ww.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zm.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://se.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ul.szsharing.cn

[D11] 反转数组
来源：http://uf.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pg.nszjky.cn

PHP:  array_reverse($arr);
来源：http://za.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bd.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://cb.nicolike.cn

Java: Collections.reverse(list);
来源：http://cj.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://pc.haigaiapp.cn

Ruby: arr.reverse
来源：http://if.lnxyls.cn

C#:   list.Reverse();
来源：http://hl.shxzskj.cn

[D12] 查找元素下标
来源：http://ki.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://xa.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sy.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bx.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dh.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mw.asd995.cn

Go:   slices.Index(arr, x)
来源：http://oh.nicolike.cn

Ruby: arr.index(x)
来源：http://pz.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://bq.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://eb.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qo.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ni.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://bi.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://zb.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bk.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ub.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://im.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cb.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://el.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ne.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ax.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://im.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://jo.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qb.521024.cn

Go:   // 手写循环
来源：http://ka.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cg.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jg.jianghongdianzi.cn

[D15] 去重
来源：http://co.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ma.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://tj.9csxet.cn

JS:   [...new Set(arr)]
来源：http://on.newstarts.cn

TS:   [...new Set(arr)]
来源：http://vd.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sy.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ua.hahajie.cn

Ruby: arr.uniq
来源：http://jp.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://mr.9csxet.cn

[D16] 求和与平均值
来源：http://ft.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ri.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qw.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nu.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dz.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xm.szxytkj.cn

Go:   // 手写循环累加
来源：http://uu.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pr.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://ia.wgjwhj.cn

[D17] 最大值与最小值
来源：http://bw.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://ha.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://uy.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qr.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://ys.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kr.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bn.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://yp.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://gq.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://sf.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hj.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://jl.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vy.yuntaijiaju.cn

TS:   nested.flat();
来源：http://zt.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wj.jctech888.com.cn

Go:   // 手写双层循环
来源：http://jb.shtwfgs.cn

Ruby: nested.flatten
来源：http://oz.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fs.colortex.cn

[D19] 按字段分组
来源：http://gf.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://su.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bq.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ce.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://po.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xb.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://kx.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yq.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wf.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://bo.9csxet.cn

Py:   Counter(arr)
来源：http://uv.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://qi.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sf.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mj.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://px.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://qk.nszjky.cn

Ruby: arr.tally
来源：http://gw.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jd.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://la.521024.cn

Py:   x in arr
来源：http://qd.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://tv.huanxung.cn

JS:   arr.includes(x)
来源：http://vc.gzmigu.cn

TS:   arr.includes(x)
来源：http://ti.newstarts.cn

Java: list.contains(x)
来源：http://oc.521024.cn

Go:   slices.Contains(arr, x)
来源：http://mc.colortex.cn

Ruby: arr.include?(x)
来源：http://ge.huixiangedu.cn

C#:   list.Contains(x)
来源：http://oq.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://zu.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vf.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jy.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gl.hahajie.cn

TS:   [...arr];
来源：http://ec.521024.cn

Java: new ArrayList<>(list);
来源：http://vc.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wa.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://is.colortex.cn

C#:   new List<int>(list);
来源：http://pf.chemitech.net.cn

[D23] reduce 累积计算
来源：http://fw.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fj.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fs.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pj.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fc.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://do.muxihuayi.cn

Go:   // 手写循环
来源：http://es.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ax.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sn.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://sh.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lk.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vr.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://at.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yi.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://js.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ld.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gf.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ac.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://lz.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cd.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nl.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hn.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yx.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rz.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dl.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xl.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qb.szsharing.cn

[D26] 数组转字符串
来源：http://ih.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://og.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://tn.lnxyls.cn

JS:   arr.join(", ")
来源：http://lg.huanxung.cn

TS:   arr.join(", ")
来源：http://wd.shtwfgs.cn

Java: String.join(", ", list)
来源：http://wi.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://qq.521024.cn

Ruby: arr.join(", ")
来源：http://dn.huanxung.cn

C#:   string.Join(", ", list)
来源：http://bu.haigaiapp.cn

================================================================================
来源：http://ji.asd995.cn

E. 字符串处理
来源：http://uw.panjiajie.cn

================================================================================
来源：http://sk.bookmarksfly.cn

[E01] 拼接字符串
来源：http://kj.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yz.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bs.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oe.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dd.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ye.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xp.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rj.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bq.huixinmuqiang.cn

[E02] 重复字符串
来源：http://zz.wgjwhj.cn

Py:   "ab" * 3
来源：http://zx.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://pm.newstarts.cn

JS:   "ab".repeat(3)
来源：http://tt.szsharing.cn

TS:   "ab".repeat(3)
来源：http://od.szsharing.cn

Java: "ab".repeat(3)
来源：http://ad.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nt.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://oj.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://on.jianghongdianzi.cn

[E03] 截取子串
来源：http://kl.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dy.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qu.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yo.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://im.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://wb.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bt.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lu.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://eb.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://hq.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://mk.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://wi.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fj.asd995.cn

TS:   s.indexOf("x")
来源：http://az.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ni.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://hs.colortex.cn

Ruby: s.index("x")
来源：http://ru.szsharing.cn

C#:   s.IndexOf("x")
来源：http://jx.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://td.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kd.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wr.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fj.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dj.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sj.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zt.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fx.jianghongdianzi.cn

[E06] 替换子串
来源：http://kf.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ji.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://qs.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jf.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://wy.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kl.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rx.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cx.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://xe.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://yf.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mo.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cu.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://we.nszjky.cn

TS:   s.split(",")
来源：http://px.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ft.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mu.colortex.cn

Ruby: s.split(",");  s.split
来源：http://wr.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vr.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://ij.newstarts.cn

Py:   ",".join(items)
来源：http://fg.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://mi.colortex.cn

JS:   items.join(",")
来源：http://fp.haigaiapp.cn

TS:   items.join(",")
来源：http://hk.521024.cn

Java: String.join(",", items)
来源：http://py.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ms.muxihuayi.cn

Ruby: items.join(",")
来源：http://rg.szsharing.cn

C#:   string.Join(",", items)
来源：http://lk.szxytkj.cn

[E09] 去除所有空白字符
来源：http://pj.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hf.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xg.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://qn.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://rp.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://ja.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ob.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nr.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vr.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://dd.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pg.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xw.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://pc.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://pr.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://zn.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xk.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kq.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vv.bjjhwx.cn

[E11] 反转字符串
来源：http://ed.hnjuh.cn

Py:   s[::-1]
来源：http://ee.hnjuh.cn

PHP:  strrev($s);
来源：http://kl.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://na.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://rn.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hg.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wg.wgjwhj.cn

Ruby: s.reverse
来源：http://jm.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ph.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://jz.colortex.cn

Py:   s.count("a")
来源：http://yi.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://re.newstarts.cn

JS:   s.split("a").length - 1
来源：http://vp.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://qu.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sf.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://sj.muxihuayi.cn

Ruby: s.count("a")
来源：http://qo.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://wx.gzmigu.cn

[E13] 逐字符遍历
来源：http://cl.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://wp.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mu.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qz.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dv.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oe.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xl.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zy.panjiajie.cn


<!-- 参考信息 -->