代发 wailian999

[D03] 在指定位置插入元素
来源：http://xe.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://jv.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jx.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rw.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://sc.shxzukj.cn

Java: list.add(0, 0);
来源：http://it.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ks.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.521024.cn

C#:   list.Insert(0, 0);
来源：http://eg.nicolike.cn

[D04] 删除元素
来源：http://tl.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pu.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vn.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ad.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://am.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qv.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cp.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yt.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tg.panjiajie.cn

[D05] 访问与修改元素
来源：http://xq.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sd.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qe.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zh.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://qf.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://ui.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://bz.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yt.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vj.shtwfgs.cn

[D06] 数组长度
来源：http://uz.yuntaijiaju.cn

Py:   len(arr)
来源：http://td.shtwfgs.cn

PHP:  count($arr);
来源：http://ap.nszjky.cn

JS:   arr.length
来源：http://nc.nicolike.cn

TS:   arr.length
来源：http://bk.nszjky.cn

Java: list.size();
来源：http://mk.wgjwhj.cn

Go:   len(arr)
来源：http://hi.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ep.shxzskj.cn

C#:   list.Count;
来源：http://ip.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://zn.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qx.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ot.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://dj.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://nv.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://jd.colortex.cn

Go:   arr[1:4]
来源：http://cb.szxytkj.cn

Ruby: arr[1, 3]
来源：http://qr.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://ly.gzmigu.cn

[D08] 合并两个数组
来源：http://tx.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://wt.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://rz.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sz.nicolike.cn

TS:   [...a, ...b];
来源：http://pi.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yd.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ir.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://vl.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://kt.newstarts.cn

[D09] 排序（升序）
来源：http://qo.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://rr.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://up.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ht.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uq.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ux.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qf.newstarts.cn

Ruby: arr.sort
来源：http://yf.hnjuh.cn

C#:   list.Sort();
来源：http://xt.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lp.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cd.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ji.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dw.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hd.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ji.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wj.haigaiapp.cn

[D11] 反转数组
来源：http://bn.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xc.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://yb.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hu.nicolike.cn

TS:   [...arr].reverse();
来源：http://qc.nszjky.cn

Java: Collections.reverse(list);
来源：http://vm.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://fd.newstarts.cn

Ruby: arr.reverse
来源：http://kj.asd995.cn

C#:   list.Reverse();
来源：http://xv.huanxung.cn

[D12] 查找元素下标
来源：http://fd.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://dd.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rg.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bc.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eu.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fm.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://cy.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://em.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://le.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://jq.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pa.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rp.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://qm.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://mq.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yi.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://au.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fn.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yb.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://nj.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pv.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ms.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://qr.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://tx.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cg.jianghongdianzi.cn

Go:   // 手写循环
来源：http://on.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://up.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zq.nicolike.cn

[D15] 去重
来源：http://re.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vr.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://mu.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xv.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://qk.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yo.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pe.huixiangedu.cn

Ruby: arr.uniq
来源：http://hg.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://oa.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://jo.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ua.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cb.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nw.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ej.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ss.haigaiapp.cn

Go:   // 手写循环累加
来源：http://sa.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jt.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ll.asd995.cn

[D17] 最大值与最小值
来源：http://xi.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://qv.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://zm.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vv.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://rz.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jc.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ym.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://az.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://wa.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://rl.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ca.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://ih.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cb.chemitech.net.cn

TS:   nested.flat();
来源：http://ac.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://im.hnjuh.cn

Go:   // 手写双层循环
来源：http://hp.bookmarksfly.cn

Ruby: nested.flatten
来源：http://yn.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fk.szxytkj.cn

[D19] 按字段分组
来源：http://bn.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rw.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ay.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tl.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yr.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gp.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://lz.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jd.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tt.colortex.cn

[D20] 统计每个元素出现次数
来源：http://fs.hahajie.cn

Py:   Counter(arr)
来源：http://ah.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://si.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yi.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qh.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zn.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://sr.haigaiapp.cn

Ruby: arr.tally
来源：http://mi.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://js.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://ge.szsharing.cn

Py:   x in arr
来源：http://ak.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://qy.jctech888.com.cn

JS:   arr.includes(x)
来源：http://qp.wgjwhj.cn

TS:   arr.includes(x)
来源：http://br.yuexingan06.cn

Java: list.contains(x)
来源：http://nx.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://wx.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://yr.bjjhwx.cn

C#:   list.Contains(x)
来源：http://qm.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://rp.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tr.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dp.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yz.9csxet.cn

TS:   [...arr];
来源：http://kq.asd995.cn

Java: new ArrayList<>(list);
来源：http://pn.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mm.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ey.huanxung.cn

C#:   new List<int>(list);
来源：http://az.shxzukj.cn

[D23] reduce 累积计算
来源：http://er.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xr.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eg.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lq.shxzukj.cn

Go:   // 手写循环
来源：http://zu.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dr.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qa.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://hg.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ej.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xw.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gh.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eh.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lh.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ek.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://go.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dc.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://by.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bp.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cu.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jq.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ii.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://on.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qi.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://li.colortex.cn

[D26] 数组转字符串
来源：http://ih.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://fg.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://kx.shxzskj.cn

JS:   arr.join(", ")
来源：http://ki.huanxung.cn

TS:   arr.join(", ")
来源：http://nb.yuexingan06.cn

Java: String.join(", ", list)
来源：http://fh.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://nc.huanxung.cn

Ruby: arr.join(", ")
来源：http://zh.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://rd.yuntaijiaju.cn

================================================================================
来源：http://ez.asd995.cn

E. 字符串处理
来源：http://tp.jianghongdianzi.cn

================================================================================
来源：http://ay.huixiangedu.cn

[E01] 拼接字符串
来源：http://kx.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ay.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fy.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hf.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pk.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cy.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jv.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tn.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ak.asd995.cn

[E02] 重复字符串
来源：http://yd.colortex.cn

Py:   "ab" * 3
来源：http://ns.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://xc.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://ra.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://qf.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://wt.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ux.jctech888.com.cn

Ruby: "ab" * 3
来源：http://ke.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jt.bjjhwx.cn

[E03] 截取子串
来源：http://oh.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nu.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sn.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fy.nicolike.cn

TS:   s.slice(1, 4)
来源：http://xa.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://wj.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nw.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rg.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://na.gzmigu.cn

[E04] 查找子串位置
来源：http://oq.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://rr.hahajie.cn

PHP:  strpos($s, "x");
来源：http://rs.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nn.szxytkj.cn

TS:   s.indexOf("x")
来源：http://my.huixiangedu.cn

Java: s.indexOf("x")
来源：http://gv.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://iq.shxzukj.cn

Ruby: s.index("x")
来源：http://cu.nicolike.cn

C#:   s.IndexOf("x")
来源：http://nt.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bb.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mt.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xw.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hc.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jv.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ll.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bw.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ou.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kz.521024.cn

[E06] 替换子串
来源：http://kf.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zj.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://uh.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://gk.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jl.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bt.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eo.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://qy.521024.cn

[E07] 按分隔符拆分
来源：http://hv.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ab.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sk.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jk.nszjky.cn

TS:   s.split(",")
来源：http://iw.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mz.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kb.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://uj.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sl.newstarts.cn

[E08] 数组按分隔符合并
来源：http://dn.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://ag.szxytkj.cn

PHP:  implode(",", $items);
来源：http://eh.shxzukj.cn

JS:   items.join(",")
来源：http://ce.huixinmuqiang.cn

TS:   items.join(",")
来源：http://eb.szxytkj.cn

Java: String.join(",", items)
来源：http://nh.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://jz.jctech888.com.cn

Ruby: items.join(",")
来源：http://fa.huanxung.cn

C#:   string.Join(",", items)
来源：http://xe.panjiajie.cn

[E09] 去除所有空白字符
来源：http://oa.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fl.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gq.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://iz.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://xy.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://kp.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://et.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://td.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uw.yuexingan06.cn


<!-- 参考信息 -->