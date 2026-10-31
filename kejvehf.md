代发 wailian999

Java: list.add(4);
来源：http://hy.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://qm.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://wi.szxytkj.cn

C#:   list.Add(4);
来源：http://ow.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://tu.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://tv.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fm.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zs.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://zx.szsharing.cn

Java: list.add(0, 0);
来源：http://ro.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fq.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vn.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://du.yuexingan06.cn

[D04] 删除元素
来源：http://zs.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ue.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gn.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fs.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://wa.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mh.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://la.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hx.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hi.shtwfgs.cn

[D05] 访问与修改元素
来源：http://qm.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nm.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nd.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xl.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://rh.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://wd.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://zk.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uk.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cc.nicolike.cn

[D06] 数组长度
来源：http://aa.hahajie.cn

Py:   len(arr)
来源：http://es.shxzukj.cn

PHP:  count($arr);
来源：http://uf.bookmarksfly.cn

JS:   arr.length
来源：http://ri.haigaiapp.cn

TS:   arr.length
来源：http://tp.shxzskj.cn

Java: list.size();
来源：http://ts.wgjwhj.cn

Go:   len(arr)
来源：http://bl.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://yg.muxihuayi.cn

C#:   list.Count;
来源：http://sx.huanxung.cn

[D07] 切片 / 取子数组
来源：http://pc.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tv.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hq.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://xj.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://xl.szsharing.cn

Java: list.subList(1, 4);
来源：http://zs.yuexingan06.cn

Go:   arr[1:4]
来源：http://kf.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://zx.521024.cn

C#:   list.GetRange(1, 3);
来源：http://xp.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://eh.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://jt.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://pz.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oi.muxihuayi.cn

TS:   [...a, ...b];
来源：http://mq.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://om.gzmigu.cn

Go:   append(a, b...)
来源：http://jx.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://wp.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://bl.muxihuayi.cn

[D09] 排序（升序）
来源：http://lx.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://rr.asd995.cn

PHP:  sort($arr);
来源：http://sz.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://se.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dn.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://la.haigaiapp.cn

Ruby: arr.sort
来源：http://pe.muxihuayi.cn

C#:   list.Sort();
来源：http://xf.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zs.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gz.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lu.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pq.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zb.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rk.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oj.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cf.newstarts.cn

[D11] 反转数组
来源：http://wa.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bm.9csxet.cn

PHP:  array_reverse($arr);
来源：http://mp.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ot.szxytkj.cn

TS:   [...arr].reverse();
来源：http://mz.asd995.cn

Java: Collections.reverse(list);
来源：http://ko.521024.cn

Go:   slices.Reverse(arr)
来源：http://me.lnxyls.cn

Ruby: arr.reverse
来源：http://fa.shxzskj.cn

C#:   list.Reverse();
来源：http://dm.bookmarksfly.cn

[D12] 查找元素下标
来源：http://gu.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://rc.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jv.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tg.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yu.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sp.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://gn.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://lb.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://vi.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://jo.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dt.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kl.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://yt.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://fy.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fs.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bm.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cb.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pd.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://be.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fo.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rt.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://am.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://kq.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qu.9csxet.cn

Go:   // 手写循环
来源：http://nu.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xo.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xm.huanxung.cn

[D15] 去重
来源：http://la.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://zd.asd995.cn

JS:   [...new Set(arr)]
来源：http://nq.nicolike.cn

TS:   [...new Set(arr)]
来源：http://sf.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bg.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tx.newstarts.cn

Ruby: arr.uniq
来源：http://ix.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://dl.chemitech.net.cn

[D16] 求和与平均值
来源：http://jq.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pf.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ra.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zg.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://om.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mv.newstarts.cn

Go:   // 手写循环累加
来源：http://nz.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rs.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://bc.szsharing.cn

[D17] 最大值与最小值
来源：http://rh.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://mh.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://pq.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ak.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://og.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://um.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ak.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ap.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://cv.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://et.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lm.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://rg.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tq.bjjhwx.cn

TS:   nested.flat();
来源：http://ls.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nw.nszjky.cn

Go:   // 手写双层循环
来源：http://ul.panjiajie.cn

Ruby: nested.flatten
来源：http://iz.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sq.shxzukj.cn

[D19] 按字段分组
来源：http://yt.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rj.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hr.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ya.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yu.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sd.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://sa.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rm.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wj.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://dn.szsharing.cn

Py:   Counter(arr)
来源：http://cd.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://bf.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jw.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yg.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nb.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://xf.jianghongdianzi.cn

Ruby: arr.tally
来源：http://yq.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uo.nszjky.cn

[D21] 判断是否包含某元素
来源：http://ia.lnxyls.cn

Py:   x in arr
来源：http://pe.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://vd.szsharing.cn

JS:   arr.includes(x)
来源：http://ok.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://so.muxihuayi.cn

Java: list.contains(x)
来源：http://jb.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://cw.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://dm.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://iq.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://nl.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qe.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lh.huanxung.cn

TS:   [...arr];
来源：http://av.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://mx.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://df.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://kz.nicolike.cn

C#:   new List<int>(list);
来源：http://cv.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://xm.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nb.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://op.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ap.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gb.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vk.shxzukj.cn

Go:   // 手写循环
来源：http://wc.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://su.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://io.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://re.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ce.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://by.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lg.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gc.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://op.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ov.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kl.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ah.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zi.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fo.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ba.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xq.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xs.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ue.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jd.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fh.hnjuh.cn

[D26] 数组转字符串
来源：http://px.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://rx.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://kt.hahajie.cn

JS:   arr.join(", ")
来源：http://tv.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ao.szxytkj.cn

Java: String.join(", ", list)
来源：http://jo.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://eo.521024.cn

Ruby: arr.join(", ")
来源：http://ov.nicolike.cn

C#:   string.Join(", ", list)
来源：http://le.asd995.cn

================================================================================
来源：http://vd.chemitech.net.cn

E. 字符串处理
来源：http://gm.haigaiapp.cn

================================================================================
来源：http://wa.jctech888.com.cn

[E01] 拼接字符串
来源：http://hx.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://az.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vp.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fw.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ad.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qa.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qz.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://li.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ta.bookmarksfly.cn

[E02] 重复字符串
来源：http://bv.shxzukj.cn

Py:   "ab" * 3
来源：http://bx.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://vq.colortex.cn

JS:   "ab".repeat(3)
来源：http://so.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://kp.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ap.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://ji.shxzukj.cn

Ruby: "ab" * 3
来源：http://re.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.panjiajie.cn

[E03] 截取子串
来源：http://fj.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iu.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yt.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cq.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://mm.hnjuh.cn

Java: s.substring(1, 4)
来源：http://me.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tj.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ey.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://dl.jctech888.com.cn

[E04] 查找子串位置
来源：http://ly.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://zs.nszjky.cn

PHP:  strpos($s, "x");
来源：http://yj.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iz.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://hv.hahajie.cn

Java: s.indexOf("x")
来源：http://ph.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://qv.szxytkj.cn

Ruby: s.index("x")
来源：http://cz.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://yq.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rq.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vu.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tx.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ul.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xd.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tm.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ve.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mx.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pz.asd995.cn

[E06] 替换子串
来源：http://du.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nv.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://pv.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lk.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://sk.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://em.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://de.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nk.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://cc.shxzskj.cn

[E07] 按分隔符拆分
来源：http://qh.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aw.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dx.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vf.jctech888.com.cn

TS:   s.split(",")
来源：http://rd.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yw.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cx.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://jv.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://we.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ld.panjiajie.cn

Py:   ",".join(items)
来源：http://dl.hnjuh.cn

PHP:  implode(",", $items);
来源：http://uw.lnxyls.cn

JS:   items.join(",")
来源：http://tz.jctech888.com.cn

TS:   items.join(",")
来源：http://tu.yuexingan06.cn

Java: String.join(",", items)
来源：http://fe.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://yh.huixiangedu.cn

Ruby: items.join(",")
来源：http://aq.newstarts.cn

C#:   string.Join(",", items)
来源：http://py.nszjky.cn

[E09] 去除所有空白字符
来源：http://ja.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://du.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xx.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://aq.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://oa.jianghongdianzi.cn


<!-- 参考信息 -->