代发 wailian999

[D07] 切片 / 取子数组
来源：http://qw.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sn.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yu.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://vv.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ur.asd995.cn

Java: list.subList(1, 4);
来源：http://bn.colortex.cn

Go:   arr[1:4]
来源：http://sv.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://xi.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://wl.9csxet.cn

[D08] 合并两个数组
来源：http://eh.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://wg.colortex.cn

PHP:  array_merge($a, $b);
来源：http://hx.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rx.haigaiapp.cn

TS:   [...a, ...b];
来源：http://oj.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rb.colortex.cn

Go:   append(a, b...)
来源：http://xc.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://xd.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://rl.newstarts.cn

[D09] 排序（升序）
来源：http://kf.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://xy.muxihuayi.cn

PHP:  sort($arr);
来源：http://bs.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kt.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://df.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ck.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dc.huixiangedu.cn

Ruby: arr.sort
来源：http://kk.newstarts.cn

C#:   list.Sort();
来源：http://cr.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://he.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xe.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rh.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kj.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wv.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bx.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://td.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ac.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bf.bjjhwx.cn

[D11] 反转数组
来源：http://uc.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://na.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://nx.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ys.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://xz.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://jl.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://ut.hahajie.cn

Ruby: arr.reverse
来源：http://fz.521024.cn

C#:   list.Reverse();
来源：http://pb.bjjhwx.cn

[D12] 查找元素下标
来源：http://lm.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://is.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jo.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://da.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pc.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sj.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://oc.shxzukj.cn

Ruby: arr.index(x)
来源：http://tn.521024.cn

C#:   list.IndexOf(x);
来源：http://vy.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://gh.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jk.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ff.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://nn.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://lg.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pv.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://og.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qr.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://es.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://tw.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kh.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eh.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://mf.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://sv.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jb.lnxyls.cn

Go:   // 手写循环
来源：http://wu.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://es.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yx.panjiajie.cn

[D15] 去重
来源：http://jw.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ra.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://vm.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://om.colortex.cn

TS:   [...new Set(arr)]
来源：http://jq.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fc.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xz.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://si.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ia.shtwfgs.cn

[D16] 求和与平均值
来源：http://zz.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tq.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zn.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qx.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://io.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://id.newstarts.cn

Go:   // 手写循环累加
来源：http://xi.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cr.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://lk.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://hd.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://ti.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://km.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uw.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://cz.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cb.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://do.asd995.cn

Ruby: arr.max;  arr.min
来源：http://vd.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://bd.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://so.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rk.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://vd.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://um.nszjky.cn

TS:   nested.flat();
来源：http://jd.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fl.yuexingan06.cn

Go:   // 手写双层循环
来源：http://sq.huanxung.cn

Ruby: nested.flatten
来源：http://ll.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gt.yuntaijiaju.cn

[D19] 按字段分组
来源：http://lv.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ue.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jz.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gg.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qd.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sr.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://ne.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ek.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xs.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ml.nicolike.cn

Py:   Counter(arr)
来源：http://je.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://uw.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fv.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pg.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://ri.huixiangedu.cn

Ruby: arr.tally
来源：http://mw.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nb.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://bt.wgjwhj.cn

Py:   x in arr
来源：http://az.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://sr.colortex.cn

JS:   arr.includes(x)
来源：http://ha.huanxung.cn

TS:   arr.includes(x)
来源：http://be.shxzskj.cn

Java: list.contains(x)
来源：http://qb.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://ts.gzmigu.cn

Ruby: arr.include?(x)
来源：http://mu.hahajie.cn

C#:   list.Contains(x)
来源：http://cf.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://es.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rb.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yh.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uv.gzmigu.cn

TS:   [...arr];
来源：http://gt.colortex.cn

Java: new ArrayList<>(list);
来源：http://yl.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xw.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://rf.muxihuayi.cn

C#:   new List<int>(list);
来源：http://yf.nszjky.cn

[D23] reduce 累积计算
来源：http://zb.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jn.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mw.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ez.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xj.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ge.nszjky.cn

Go:   // 手写循环
来源：http://bd.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ey.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zy.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ei.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hg.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qj.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fu.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gk.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oq.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sj.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ob.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xp.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://ew.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ui.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://go.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dt.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lq.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xf.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ia.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ga.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jm.521024.cn

[D26] 数组转字符串
来源：http://nq.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://wz.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://ki.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://xf.9csxet.cn

TS:   arr.join(", ")
来源：http://cb.hahajie.cn

Java: String.join(", ", list)
来源：http://vn.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://uo.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://mq.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://ge.huixinmuqiang.cn

================================================================================
来源：http://ta.nicolike.cn

E. 字符串处理
来源：http://hm.muxihuayi.cn

================================================================================
来源：http://gc.shtwfgs.cn

[E01] 拼接字符串
来源：http://fq.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xj.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lp.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sy.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bt.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yz.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uc.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sa.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fu.asd995.cn

[E02] 重复字符串
来源：http://pq.huixiangedu.cn

Py:   "ab" * 3
来源：http://lz.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://nf.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://gi.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://xg.9csxet.cn

Java: "ab".repeat(3)
来源：http://af.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://yz.muxihuayi.cn

Ruby: "ab" * 3
来源：http://fx.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sd.521024.cn

[E03] 截取子串
来源：http://ei.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dg.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bf.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kk.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://lw.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ls.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fi.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pv.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://xz.chemitech.net.cn

[E04] 查找子串位置
来源：http://qx.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://yc.nszjky.cn

PHP:  strpos($s, "x");
来源：http://nm.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kv.asd995.cn

TS:   s.indexOf("x")
来源：http://wh.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://af.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://ve.wgjwhj.cn

Ruby: s.index("x")
来源：http://ev.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ge.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fy.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ai.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://or.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cw.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ac.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pm.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ja.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dg.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ue.521024.cn

[E06] 替换子串
来源：http://zs.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://od.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://un.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ss.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ow.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wd.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mz.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jq.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://tl.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://dn.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yh.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wh.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://es.hnjuh.cn

TS:   s.split(",")
来源：http://hw.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://it.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bo.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://cz.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uq.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://xm.lnxyls.cn

Py:   ",".join(items)
来源：http://nm.colortex.cn

PHP:  implode(",", $items);
来源：http://qc.yuntaijiaju.cn

JS:   items.join(",")
来源：http://dg.shtwfgs.cn

TS:   items.join(",")
来源：http://qj.huanxung.cn

Java: String.join(",", items)
来源：http://ou.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ua.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://tt.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ym.panjiajie.cn

[E09] 去除所有空白字符
来源：http://ny.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://os.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zo.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ml.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://fq.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gd.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uj.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vs.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uk.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://ik.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vi.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://re.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://tp.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://us.9csxet.cn

Java: String.format("%03d", 7)
来源：http://ye.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bh.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pr.szsharing.cn

[E11] 反转字符串
来源：http://tt.wgjwhj.cn

Py:   s[::-1]
来源：http://oi.asd995.cn

PHP:  strrev($s);
来源：http://kk.asd995.cn

JS:   [...s].reverse().join("")
来源：http://de.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://at.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rz.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xt.hnjuh.cn

Ruby: s.reverse
来源：http://ob.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ha.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://dc.panjiajie.cn

Py:   s.count("a")
来源：http://bb.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://vp.nszjky.cn

JS:   s.split("a").length - 1
来源：http://nh.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://gs.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yw.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://dx.newstarts.cn

Ruby: s.count("a")
来源：http://yx.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://gk.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://jr.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ts.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eo.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sd.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://el.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kj.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yl.shxzskj.cn


<!-- 参考信息 -->