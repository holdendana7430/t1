代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wm.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://we.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sc.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hy.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qv.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ix.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ln.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://co.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cs.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://dg.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bx.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ru.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tn.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ff.huanxung.cn

[D06] 数组长度
来源：http://be.nicolike.cn

Py:   len(arr)
来源：http://or.521024.cn

PHP:  count($arr);
来源：http://jv.jctech888.com.cn

JS:   arr.length
来源：http://fm.huanxung.cn

TS:   arr.length
来源：http://jt.newstarts.cn

Java: list.size();
来源：http://ch.9csxet.cn

Go:   len(arr)
来源：http://yr.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://tm.chemitech.net.cn

C#:   list.Count;
来源：http://jq.hahajie.cn

[D07] 切片 / 取子数组
来源：http://nq.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wu.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ri.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://nf.asd995.cn

TS:   arr.slice(1, 4);
来源：http://zx.szxytkj.cn

Java: list.subList(1, 4);
来源：http://io.521024.cn

Go:   arr[1:4]
来源：http://mz.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://re.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://gs.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://rn.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ly.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://rj.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yl.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ce.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hl.jctech888.com.cn

Go:   append(a, b...)
来源：http://bl.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://ze.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://en.wgjwhj.cn

[D09] 排序（升序）
来源：http://ux.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://bx.colortex.cn

PHP:  sort($arr);
来源：http://us.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qj.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hb.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://et.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ql.hnjuh.cn

Ruby: arr.sort
来源：http://ew.hnjuh.cn

C#:   list.Sort();
来源：http://cs.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wq.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qd.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ax.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qc.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bu.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pf.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dq.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rz.nszjky.cn

[D11] 反转数组
来源：http://pp.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yg.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://dk.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pu.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://gw.asd995.cn

Java: Collections.reverse(list);
来源：http://ys.521024.cn

Go:   slices.Reverse(arr)
来源：http://tf.newstarts.cn

Ruby: arr.reverse
来源：http://sh.panjiajie.cn

C#:   list.Reverse();
来源：http://nn.hnjuh.cn

[D12] 查找元素下标
来源：http://sa.521024.cn

Py:   arr.index(x);  x in arr
来源：http://fa.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zu.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fv.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ua.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gu.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://nw.jctech888.com.cn

Ruby: arr.index(x)
来源：http://rx.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://sn.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://tb.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pm.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fy.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://qv.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ke.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vk.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dq.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://is.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vm.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://mj.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ur.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xk.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://ai.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://nd.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sa.bookmarksfly.cn

Go:   // 手写循环
来源：http://yb.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cx.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kc.jctech888.com.cn

[D15] 去重
来源：http://us.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wv.9csxet.cn

PHP:  array_unique($arr);
来源：http://rz.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://hq.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://kt.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gt.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ej.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://lz.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ke.lnxyls.cn

[D16] 求和与平均值
来源：http://ky.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cc.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yu.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pj.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kx.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xx.jctech888.com.cn

Go:   // 手写循环累加
来源：http://xk.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dg.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://go.shtwfgs.cn

[D17] 最大值与最小值
来源：http://ro.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://qw.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://nu.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yl.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://ec.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://af.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://os.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://qw.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://qs.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ns.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ti.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://lk.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ct.yuntaijiaju.cn

TS:   nested.flat();
来源：http://qz.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nf.wgjwhj.cn

Go:   // 手写双层循环
来源：http://gh.shxzukj.cn

Ruby: nested.flatten
来源：http://id.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ll.gzmigu.cn

[D19] 按字段分组
来源：http://hj.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wh.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zc.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jb.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yz.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nk.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://bh.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tj.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fp.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://gm.chemitech.net.cn

Py:   Counter(arr)
来源：http://am.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://co.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uo.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ll.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qg.nicolike.cn

Go:   // 手写 map[T]int
来源：http://nd.yuntaijiaju.cn

Ruby: arr.tally
来源：http://wj.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rz.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://hh.szxytkj.cn

Py:   x in arr
来源：http://ii.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://if.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://yl.panjiajie.cn

TS:   arr.includes(x)
来源：http://ut.wgjwhj.cn

Java: list.contains(x)
来源：http://oz.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://yc.shxzskj.cn

Ruby: arr.include?(x)
来源：http://nc.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://kh.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ju.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fx.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fx.bookmarksfly.cn

TS:   [...arr];
来源：http://me.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://kt.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rs.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://jv.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ep.huanxung.cn

[D23] reduce 累积计算
来源：http://ph.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xv.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://br.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tf.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ov.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gm.521024.cn

Go:   // 手写循环
来源：http://hl.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qv.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xi.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://mq.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nj.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gy.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zb.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nm.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dw.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cl.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hr.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ap.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://dz.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fj.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gu.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iy.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ml.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://un.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oe.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://na.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fq.hnjuh.cn

[D26] 数组转字符串
来源：http://yf.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://ww.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://pt.shtwfgs.cn

JS:   arr.join(", ")
来源：http://cg.gzmigu.cn

TS:   arr.join(", ")
来源：http://lc.9csxet.cn

Java: String.join(", ", list)
来源：http://rv.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://jk.shxzukj.cn

Ruby: arr.join(", ")
来源：http://lk.asd995.cn

C#:   string.Join(", ", list)
来源：http://io.hahajie.cn

================================================================================
来源：http://yy.shxzskj.cn

E. 字符串处理
来源：http://sc.panjiajie.cn

================================================================================
来源：http://ha.szxytkj.cn

[E01] 拼接字符串
来源：http://dk.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ri.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nh.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wg.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yr.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wt.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rl.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ht.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sf.yuexingan06.cn

[E02] 重复字符串
来源：http://rh.newstarts.cn

Py:   "ab" * 3
来源：http://rc.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://qf.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://nw.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://wg.asd995.cn

Java: "ab".repeat(3)
来源：http://gf.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://xm.lnxyls.cn

Ruby: "ab" * 3
来源：http://pp.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jz.bjjhwx.cn

[E03] 截取子串
来源：http://xr.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://go.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nb.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cz.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://mk.szsharing.cn

Java: s.substring(1, 4)
来源：http://ju.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gm.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nk.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ek.9csxet.cn

[E04] 查找子串位置
来源：http://sj.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://qj.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://jh.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lg.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://bs.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://ok.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://vb.nszjky.cn

Ruby: s.index("x")
来源：http://mo.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ua.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rv.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qj.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vu.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ra.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bp.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wr.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cn.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gr.hnjuh.cn

[E06] 替换子串
来源：http://dy.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ga.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://jf.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wv.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://bu.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oc.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uh.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ws.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://cm.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://jg.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aw.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cd.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xi.newstarts.cn

TS:   s.split(",")
来源：http://vd.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://id.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rz.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://rf.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ei.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://ld.newstarts.cn

Py:   ",".join(items)
来源：http://xf.asd995.cn

PHP:  implode(",", $items);
来源：http://zm.nicolike.cn

JS:   items.join(",")
来源：http://ol.hahajie.cn

TS:   items.join(",")
来源：http://hy.shxzskj.cn

Java: String.join(",", items)
来源：http://us.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://kw.chemitech.net.cn

Ruby: items.join(",")
来源：http://js.nszjky.cn

C#:   string.Join(",", items)
来源：http://gj.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://am.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nm.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fa.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://kj.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://fo.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://bn.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vl.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zf.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://je.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://ex.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://it.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ha.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://dk.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://cl.huanxung.cn

Java: String.format("%03d", 7)
来源：http://bt.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sw.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vc.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fz.lnxyls.cn

[E11] 反转字符串
来源：http://mt.panjiajie.cn

Py:   s[::-1]
来源：http://je.panjiajie.cn

PHP:  strrev($s);
来源：http://wo.bjjhwx.cn


<!-- 参考信息 -->