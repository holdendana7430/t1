代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://qo.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ar.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tm.colortex.cn

[D06] 数组长度
来源：http://ys.muxihuayi.cn

Py:   len(arr)
来源：http://br.newstarts.cn

PHP:  count($arr);
来源：http://ga.chemitech.net.cn

JS:   arr.length
来源：http://ds.jctech888.com.cn

TS:   arr.length
来源：http://gz.bjjhwx.cn

Java: list.size();
来源：http://xh.bjjhwx.cn

Go:   len(arr)
来源：http://pt.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://hr.yuexingan06.cn

C#:   list.Count;
来源：http://my.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://is.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://er.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ew.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://sm.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://eq.nicolike.cn

Java: list.subList(1, 4);
来源：http://gb.huanxung.cn

Go:   arr[1:4]
来源：http://yp.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://bx.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://et.gzmigu.cn

[D08] 合并两个数组
来源：http://is.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://lc.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://xu.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dh.521024.cn

TS:   [...a, ...b];
来源：http://ra.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://du.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ww.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://ve.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://fd.huixiangedu.cn

[D09] 排序（升序）
来源：http://oz.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://rq.lnxyls.cn

PHP:  sort($arr);
来源：http://mt.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mb.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ns.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cm.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mr.muxihuayi.cn

Ruby: arr.sort
来源：http://kb.lnxyls.cn

C#:   list.Sort();
来源：http://hz.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pj.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ky.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ju.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qt.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aa.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xd.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://is.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yp.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.shxzskj.cn

[D11] 反转数组
来源：http://om.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cr.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://gs.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ns.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://qd.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://ve.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://cd.huixiangedu.cn

Ruby: arr.reverse
来源：http://je.bookmarksfly.cn

C#:   list.Reverse();
来源：http://mb.jctech888.com.cn

[D12] 查找元素下标
来源：http://yz.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ea.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vm.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aq.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xx.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://li.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://dw.newstarts.cn

Ruby: arr.index(x)
来源：http://pp.hahajie.cn

C#:   list.IndexOf(x);
来源：http://gh.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://vw.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uh.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fb.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://eu.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ll.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vs.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ot.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xx.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rv.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://ot.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lq.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sy.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://pm.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://zp.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oc.521024.cn

Go:   // 手写循环
来源：http://gh.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yl.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fc.wgjwhj.cn

[D15] 去重
来源：http://bm.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kb.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://zj.szsharing.cn

JS:   [...new Set(arr)]
来源：http://cy.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://lo.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jt.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lw.9csxet.cn

Ruby: arr.uniq
来源：http://nf.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://fs.muxihuayi.cn

[D16] 求和与平均值
来源：http://eo.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wo.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gm.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ux.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://db.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oe.muxihuayi.cn

Go:   // 手写循环累加
来源：http://yj.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jl.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://en.shxzskj.cn

[D17] 最大值与最小值
来源：http://cm.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ox.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://aq.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kk.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://lr.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gn.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zu.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://vs.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://vh.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://oe.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kh.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://la.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zd.bjjhwx.cn

TS:   nested.flat();
来源：http://zm.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tn.huanxung.cn

Go:   // 手写双层循环
来源：http://nb.colortex.cn

Ruby: nested.flatten
来源：http://re.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hy.huanxung.cn

[D19] 按字段分组
来源：http://bm.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://li.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lv.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hm.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uv.colortex.cn

Go:   // 手写 map[string][]T
来源：http://ld.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ul.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pz.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://yf.nicolike.cn

Py:   Counter(arr)
来源：http://kd.nszjky.cn

PHP:  array_count_values($arr);
来源：http://wo.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wr.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lm.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oe.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://ks.wgjwhj.cn

Ruby: arr.tally
来源：http://hi.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tn.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://mu.shtwfgs.cn

Py:   x in arr
来源：http://mq.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://rq.lnxyls.cn

JS:   arr.includes(x)
来源：http://hd.szsharing.cn

TS:   arr.includes(x)
来源：http://ym.wgjwhj.cn

Java: list.contains(x)
来源：http://fe.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://rk.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://uf.haigaiapp.cn

C#:   list.Contains(x)
来源：http://by.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://qx.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://me.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ah.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bn.nszjky.cn

TS:   [...arr];
来源：http://ly.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://em.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wx.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://mk.haigaiapp.cn

C#:   new List<int>(list);
来源：http://tc.shxzukj.cn

[D23] reduce 累积计算
来源：http://zb.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vy.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://az.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tz.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ub.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kn.shxzskj.cn

Go:   // 手写循环
来源：http://fp.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ie.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hr.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://eg.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wh.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tm.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ap.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qi.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cz.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rs.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gd.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ld.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://et.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ex.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nc.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fh.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ix.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ja.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qq.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bh.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wu.huixiangedu.cn

[D26] 数组转字符串
来源：http://zx.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://wi.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://gy.huixiangedu.cn

JS:   arr.join(", ")
来源：http://yl.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ia.haigaiapp.cn

Java: String.join(", ", list)
来源：http://mw.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://xi.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://iy.asd995.cn

C#:   string.Join(", ", list)
来源：http://he.lnxyls.cn

================================================================================
来源：http://gn.haigaiapp.cn

E. 字符串处理
来源：http://je.hahajie.cn

================================================================================
来源：http://ax.colortex.cn

[E01] 拼接字符串
来源：http://vp.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kr.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dm.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ef.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ie.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dv.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qd.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dx.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lv.haigaiapp.cn

[E02] 重复字符串
来源：http://xc.szsharing.cn

Py:   "ab" * 3
来源：http://im.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://fd.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://gw.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://ym.szsharing.cn

Java: "ab".repeat(3)
来源：http://je.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://tp.shtwfgs.cn

Ruby: "ab" * 3
来源：http://by.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zm.9csxet.cn

[E03] 截取子串
来源：http://qc.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zz.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sb.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ns.nszjky.cn

TS:   s.slice(1, 4)
来源：http://nh.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://da.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hf.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rp.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://dw.521024.cn

[E04] 查找子串位置
来源：http://ou.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://id.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://fq.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yi.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://dk.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ih.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://uk.newstarts.cn

Ruby: s.index("x")
来源：http://wv.newstarts.cn

C#:   s.IndexOf("x")
来源：http://fr.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ae.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dd.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yi.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ja.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mt.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yw.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dz.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nw.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://do.chemitech.net.cn

[E06] 替换子串
来源：http://af.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rt.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://rc.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yq.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://wn.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ci.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xw.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://rq.szsharing.cn

[E07] 按分隔符拆分
来源：http://rh.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nq.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://en.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lk.panjiajie.cn

TS:   s.split(",")
来源：http://vq.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pu.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wf.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://qz.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hx.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://kf.hnjuh.cn

Py:   ",".join(items)
来源：http://sf.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://br.szxytkj.cn

JS:   items.join(",")
来源：http://bt.asd995.cn

TS:   items.join(",")
来源：http://hi.haigaiapp.cn

Java: String.join(",", items)
来源：http://cp.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://jc.huixiangedu.cn

Ruby: items.join(",")
来源：http://hs.colortex.cn

C#:   string.Join(",", items)
来源：http://ix.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://sf.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xu.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ee.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://lx.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://ou.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://fi.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vr.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lq.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://em.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://xr.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zg.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tv.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://em.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://fw.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://vs.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fw.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://li.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://de.lnxyls.cn

[E11] 反转字符串
来源：http://tm.chemitech.net.cn

Py:   s[::-1]
来源：http://mt.hnjuh.cn

PHP:  strrev($s);
来源：http://qx.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://qc.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://bp.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wi.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lr.9csxet.cn

Ruby: s.reverse
来源：http://as.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://si.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://qs.bjjhwx.cn

Py:   s.count("a")
来源：http://zg.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://fp.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://to.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://qw.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ie.jianghongdianzi.cn


<!-- 参考信息 -->