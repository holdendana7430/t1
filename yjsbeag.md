代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://bh.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yz.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://br.hnjuh.cn

[D06] 数组长度
来源：http://ea.shtwfgs.cn

Py:   len(arr)
来源：http://xr.jianghongdianzi.cn

PHP:  count($arr);
来源：http://nw.jianghongdianzi.cn

JS:   arr.length
来源：http://lp.newstarts.cn

TS:   arr.length
来源：http://lw.szsharing.cn

Java: list.size();
来源：http://bn.nszjky.cn

Go:   len(arr)
来源：http://rg.colortex.cn

Ruby: arr.length; arr.size
来源：http://qw.jianghongdianzi.cn

C#:   list.Count;
来源：http://ib.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://je.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zx.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nz.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://kd.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://io.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://li.nszjky.cn

Go:   arr[1:4]
来源：http://yf.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://xz.521024.cn

C#:   list.GetRange(1, 3);
来源：http://vf.shtwfgs.cn

[D08] 合并两个数组
来源：http://bf.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://xv.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://gi.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xi.lnxyls.cn

TS:   [...a, ...b];
来源：http://sp.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rz.haigaiapp.cn

Go:   append(a, b...)
来源：http://ys.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://tv.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://xh.haigaiapp.cn

[D09] 排序（升序）
来源：http://fp.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://sy.asd995.cn

PHP:  sort($arr);
来源：http://gd.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vw.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hi.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kz.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mc.huanxung.cn

Ruby: arr.sort
来源：http://ku.shxzskj.cn

C#:   list.Sort();
来源：http://jg.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rs.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bm.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qu.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://us.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bz.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hf.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qd.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wb.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lz.9csxet.cn

[D11] 反转数组
来源：http://up.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tm.asd995.cn

PHP:  array_reverse($arr);
来源：http://rn.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fc.newstarts.cn

TS:   [...arr].reverse();
来源：http://zp.nicolike.cn

Java: Collections.reverse(list);
来源：http://sl.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://qk.521024.cn

Ruby: arr.reverse
来源：http://kb.asd995.cn

C#:   list.Reverse();
来源：http://gr.9csxet.cn

[D12] 查找元素下标
来源：http://wh.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://sn.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rk.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lp.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ve.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vv.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://zt.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://es.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://eo.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://fh.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ww.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://js.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ws.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://do.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fj.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oo.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fj.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ub.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://zt.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lz.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wu.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://aj.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://cv.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ea.huixiangedu.cn

Go:   // 手写循环
来源：http://jg.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ne.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jo.hnjuh.cn

[D15] 去重
来源：http://om.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oh.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://zo.nszjky.cn

JS:   [...new Set(arr)]
来源：http://ia.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://wp.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bu.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lx.yuexingan06.cn

Ruby: arr.uniq
来源：http://lv.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://bg.gzmigu.cn

[D16] 求和与平均值
来源：http://yo.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://da.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cn.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lq.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cf.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xu.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://bx.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kl.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://xp.shxzukj.cn

[D17] 最大值与最小值
来源：http://cn.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://xh.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ci.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ba.521024.cn

TS:   Math.max(...arr);
来源：http://io.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ug.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ck.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://nx.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://bh.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://lt.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xo.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ps.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nx.nszjky.cn

TS:   nested.flat();
来源：http://yn.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xe.yuexingan06.cn

Go:   // 手写双层循环
来源：http://kw.shtwfgs.cn

Ruby: nested.flatten
来源：http://ge.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vf.newstarts.cn

[D19] 按字段分组
来源：http://bt.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wt.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kq.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mv.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gm.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://om.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://km.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bb.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hf.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://bv.chemitech.net.cn

Py:   Counter(arr)
来源：http://np.newstarts.cn

PHP:  array_count_values($arr);
来源：http://uw.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hj.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://la.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wg.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ih.shtwfgs.cn

Ruby: arr.tally
来源：http://xe.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cg.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://xn.hnjuh.cn

Py:   x in arr
来源：http://uj.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://mj.chemitech.net.cn

JS:   arr.includes(x)
来源：http://hv.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://cc.521024.cn

Java: list.contains(x)
来源：http://dw.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://lm.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://hl.lnxyls.cn

C#:   list.Contains(x)
来源：http://ye.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ky.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vb.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qe.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.hahajie.cn

TS:   [...arr];
来源：http://fu.nszjky.cn

Java: new ArrayList<>(list);
来源：http://kw.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jh.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://dc.lnxyls.cn

C#:   new List<int>(list);
来源：http://wo.panjiajie.cn

[D23] reduce 累积计算
来源：http://qo.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qi.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hu.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ah.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wv.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://la.huanxung.cn

Go:   // 手写循环
来源：http://mm.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eo.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dg.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://ev.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zy.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uh.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://br.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://im.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://op.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mr.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qy.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kk.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://lg.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kb.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xo.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lq.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ph.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ot.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wc.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gi.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://un.hahajie.cn

[D26] 数组转字符串
来源：http://tg.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://dw.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://bz.shxzukj.cn

JS:   arr.join(", ")
来源：http://jz.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://hb.newstarts.cn

Java: String.join(", ", list)
来源：http://yx.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ge.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://mn.huanxung.cn

C#:   string.Join(", ", list)
来源：http://at.wgjwhj.cn

================================================================================
来源：http://rq.huanxung.cn

E. 字符串处理
来源：http://yt.jctech888.com.cn

================================================================================
来源：http://of.haigaiapp.cn

[E01] 拼接字符串
来源：http://lw.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ua.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sz.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lb.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xb.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yw.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ya.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gg.muxihuayi.cn

[E02] 重复字符串
来源：http://ls.hnjuh.cn

Py:   "ab" * 3
来源：http://gj.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://yk.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://rz.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://bo.lnxyls.cn

Java: "ab".repeat(3)
来源：http://pd.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://rw.hnjuh.cn

Ruby: "ab" * 3
来源：http://is.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uf.bjjhwx.cn

[E03] 截取子串
来源：http://qg.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ww.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fr.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ko.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://hk.lnxyls.cn

Java: s.substring(1, 4)
来源：http://xt.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dn.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xs.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://kg.jctech888.com.cn

[E04] 查找子串位置
来源：http://cb.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://nn.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://cs.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vf.hnjuh.cn

TS:   s.indexOf("x")
来源：http://ff.szxytkj.cn

Java: s.indexOf("x")
来源：http://ri.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://kw.szsharing.cn

Ruby: s.index("x")
来源：http://vj.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://yl.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gr.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://of.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qf.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://od.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://um.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fl.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kt.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://va.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kx.hahajie.cn

[E06] 替换子串
来源：http://dz.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kp.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ty.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://up.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://il.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://km.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dk.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kt.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://sr.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://md.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kh.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hy.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rc.wgjwhj.cn

TS:   s.split(",")
来源：http://gy.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gt.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lh.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://ew.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sr.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://di.nszjky.cn

Py:   ",".join(items)
来源：http://ti.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://gd.yuntaijiaju.cn

JS:   items.join(",")
来源：http://vf.panjiajie.cn

TS:   items.join(",")
来源：http://zu.bookmarksfly.cn

Java: String.join(",", items)
来源：http://wr.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://dt.shtwfgs.cn

Ruby: items.join(",")
来源：http://ct.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://xb.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://av.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zu.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://st.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://go.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://og.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://xo.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bz.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cd.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ve.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://aq.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://so.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rc.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://wt.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://po.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://ki.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gz.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oo.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fm.huanxung.cn

[E11] 反转字符串
来源：http://uj.huixinmuqiang.cn

Py:   s[::-1]
来源：http://qw.521024.cn

PHP:  strrev($s);
来源：http://it.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://be.521024.cn

TS:   [...s].reverse().join("")
来源：http://zd.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nx.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rd.bjjhwx.cn

Ruby: s.reverse
来源：http://sx.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qf.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://hu.hahajie.cn

Py:   s.count("a")
来源：http://wv.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://bz.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://yl.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://uf.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bx.shxzukj.cn


<!-- 参考信息 -->