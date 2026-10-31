代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pm.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ne.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vg.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://te.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://rx.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://lr.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cu.521024.cn

[D02] 追加元素到末尾
来源：http://kx.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fe.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yh.szxytkj.cn

JS:   arr.push(4);
来源：http://sx.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://ux.huixiangedu.cn

Java: list.add(4);
来源：http://ca.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://xv.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://ao.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://or.szsharing.cn

[D03] 在指定位置插入元素
来源：http://iu.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://lk.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kj.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zb.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://pp.huanxung.cn

Java: list.add(0, 0);
来源：http://hp.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mu.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rr.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://ub.szxytkj.cn

[D04] 删除元素
来源：http://hh.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zu.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ex.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sa.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://ku.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rs.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pr.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aq.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fh.9csxet.cn

[D05] 访问与修改元素
来源：http://yu.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ho.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wx.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zd.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://du.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://ad.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://sw.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xw.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jm.newstarts.cn

[D06] 数组长度
来源：http://iq.panjiajie.cn

Py:   len(arr)
来源：http://iw.newstarts.cn

PHP:  count($arr);
来源：http://zb.lnxyls.cn

JS:   arr.length
来源：http://qi.bookmarksfly.cn

TS:   arr.length
来源：http://wn.bookmarksfly.cn

Java: list.size();
来源：http://sr.jctech888.com.cn

Go:   len(arr)
来源：http://jl.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://ym.nicolike.cn

C#:   list.Count;
来源：http://nw.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://kx.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kh.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hn.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://kp.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://nr.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://pp.gzmigu.cn

Go:   arr[1:4]
来源：http://gn.gzmigu.cn

Ruby: arr[1, 3]
来源：http://ev.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://uh.yuexingan06.cn

[D08] 合并两个数组
来源：http://jd.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://sf.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://xb.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ef.asd995.cn

TS:   [...a, ...b];
来源：http://ft.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bs.nicolike.cn

Go:   append(a, b...)
来源：http://vy.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://qf.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ei.szxytkj.cn

[D09] 排序（升序）
来源：http://ik.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://tf.jctech888.com.cn

PHP:  sort($arr);
来源：http://ur.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mq.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jz.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://er.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ok.huixinmuqiang.cn

Ruby: arr.sort
来源：http://lo.9csxet.cn

C#:   list.Sort();
来源：http://zt.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iq.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://et.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jo.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mm.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hl.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nr.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xd.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yc.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wr.huanxung.cn

[D11] 反转数组
来源：http://wg.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bn.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://yu.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ql.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://dn.colortex.cn

Java: Collections.reverse(list);
来源：http://js.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://jl.lnxyls.cn

Ruby: arr.reverse
来源：http://dd.nszjky.cn

C#:   list.Reverse();
来源：http://by.shtwfgs.cn

[D12] 查找元素下标
来源：http://cx.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ol.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cj.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lk.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://is.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xs.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://zz.521024.cn

Ruby: arr.index(x)
来源：http://ru.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://zh.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://xc.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kl.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wr.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://lf.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://zk.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zu.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yo.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vd.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://if.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://wl.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cz.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jw.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://di.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://xi.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jp.panjiajie.cn

Go:   // 手写循环
来源：http://eu.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://id.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bz.newstarts.cn

[D15] 去重
来源：http://gq.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tm.gzmigu.cn

PHP:  array_unique($arr);
来源：http://xg.colortex.cn

JS:   [...new Set(arr)]
来源：http://qw.szsharing.cn

TS:   [...new Set(arr)]
来源：http://yc.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fe.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://dg.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://yg.shxzskj.cn

[D16] 求和与平均值
来源：http://kz.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sm.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ua.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xs.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nt.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iu.gzmigu.cn

Go:   // 手写循环累加
来源：http://hu.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ak.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://kt.521024.cn

[D17] 最大值与最小值
来源：http://hi.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://uh.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://gb.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nn.hnjuh.cn

TS:   Math.max(...arr);
来源：http://zv.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qw.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pe.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://zl.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://wo.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://nc.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lg.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ec.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cz.shxzskj.cn

TS:   nested.flat();
来源：http://rp.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xf.hahajie.cn

Go:   // 手写双层循环
来源：http://bh.bjjhwx.cn

Ruby: nested.flatten
来源：http://jn.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nt.huanxung.cn

[D19] 按字段分组
来源：http://ii.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ga.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dt.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rv.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cl.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bb.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://na.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xv.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dg.asd995.cn

[D20] 统计每个元素出现次数
来源：http://gt.yuexingan06.cn

Py:   Counter(arr)
来源：http://fh.521024.cn

PHP:  array_count_values($arr);
来源：http://jk.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ip.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kg.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://in.colortex.cn

Go:   // 手写 map[T]int
来源：http://zu.szsharing.cn

Ruby: arr.tally
来源：http://iq.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rt.colortex.cn

[D21] 判断是否包含某元素
来源：http://lj.asd995.cn

Py:   x in arr
来源：http://be.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://gv.szsharing.cn

JS:   arr.includes(x)
来源：http://vt.gzmigu.cn

TS:   arr.includes(x)
来源：http://df.gzmigu.cn

Java: list.contains(x)
来源：http://sy.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://ev.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://kx.chemitech.net.cn

C#:   list.Contains(x)
来源：http://wv.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://sh.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vh.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uv.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pu.huanxung.cn

TS:   [...arr];
来源：http://fo.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://lv.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wn.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://qy.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://kf.szxytkj.cn

[D23] reduce 累积计算
来源：http://yo.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lr.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qf.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fl.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hp.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ug.nszjky.cn

Go:   // 手写循环
来源：http://vk.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yk.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://hs.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yy.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vc.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kg.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sf.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://id.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zz.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oo.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xb.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ut.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gc.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pl.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qk.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cj.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wo.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kg.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tx.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ot.nicolike.cn

[D26] 数组转字符串
来源：http://rs.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://tu.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://ep.szsharing.cn

JS:   arr.join(", ")
来源：http://fb.haigaiapp.cn

TS:   arr.join(", ")
来源：http://sw.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://dp.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://sk.shxzukj.cn

Ruby: arr.join(", ")
来源：http://hx.szsharing.cn

C#:   string.Join(", ", list)
来源：http://lb.nicolike.cn

================================================================================
来源：http://ke.jctech888.com.cn

E. 字符串处理
来源：http://se.chemitech.net.cn

================================================================================
来源：http://dv.nszjky.cn

[E01] 拼接字符串
来源：http://gg.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lx.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jn.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://du.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sa.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jj.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zy.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qu.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gi.521024.cn

[E02] 重复字符串
来源：http://aa.jctech888.com.cn

Py:   "ab" * 3
来源：http://zu.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://bp.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://nr.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://qd.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://zm.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://tk.bjjhwx.cn

Ruby: "ab" * 3
来源：http://rn.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://on.bookmarksfly.cn

[E03] 截取子串
来源：http://ub.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oj.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eq.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ia.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://dz.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://gt.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ru.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wc.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://li.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://va.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://uh.szsharing.cn

PHP:  strpos($s, "x");
来源：http://sy.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tt.panjiajie.cn

TS:   s.indexOf("x")
来源：http://ka.shxzukj.cn

Java: s.indexOf("x")
来源：http://lf.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://oc.haigaiapp.cn

Ruby: s.index("x")
来源：http://gp.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://yc.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ha.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ik.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kq.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wv.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ks.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sm.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ge.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kf.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ks.jctech888.com.cn

[E06] 替换子串
来源：http://ad.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dx.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://nq.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xw.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ii.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hd.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bc.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vx.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://zm.9csxet.cn

[E07] 按分隔符拆分
来源：http://ep.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ee.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://th.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dj.yuexingan06.cn

TS:   s.split(",")
来源：http://le.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ee.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qr.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://bg.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ry.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://tk.panjiajie.cn

Py:   ",".join(items)
来源：http://mz.hnjuh.cn


<!-- 参考信息 -->