代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://hw.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://td.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lt.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://oj.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hq.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ne.wgjwhj.cn

JS:   arr.push(4);
来源：http://ab.yuexingan06.cn

TS:   arr.push(4);
来源：http://ru.yuexingan06.cn

Java: list.add(4);
来源：http://qd.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://oe.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://uq.shxzskj.cn

C#:   list.Add(4);
来源：http://dt.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://us.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://gv.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ml.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ez.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://wc.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://gb.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pl.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rw.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ow.huixiangedu.cn

[D04] 删除元素
来源：http://gr.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bx.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ph.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rk.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://he.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yi.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oe.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://if.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://cs.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://no.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qm.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://me.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://im.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://jv.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://jw.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wt.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ul.bjjhwx.cn

[D06] 数组长度
来源：http://ut.chemitech.net.cn

Py:   len(arr)
来源：http://kb.huixinmuqiang.cn

PHP:  count($arr);
来源：http://if.521024.cn

JS:   arr.length
来源：http://pj.9csxet.cn

TS:   arr.length
来源：http://hl.nicolike.cn

Java: list.size();
来源：http://mo.bookmarksfly.cn

Go:   len(arr)
来源：http://sh.nszjky.cn

Ruby: arr.length; arr.size
来源：http://yh.huixiangedu.cn

C#:   list.Count;
来源：http://gq.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://lh.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vi.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ur.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://xg.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ms.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://fd.bjjhwx.cn

Go:   arr[1:4]
来源：http://jg.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://ee.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://ee.muxihuayi.cn

[D08] 合并两个数组
来源：http://nr.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://sp.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://va.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zk.muxihuayi.cn

TS:   [...a, ...b];
来源：http://gc.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fo.nszjky.cn

Go:   append(a, b...)
来源：http://qy.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://ws.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://fs.haigaiapp.cn

[D09] 排序（升序）
来源：http://tg.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ln.521024.cn

PHP:  sort($arr);
来源：http://lw.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rb.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lp.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://my.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cj.szxytkj.cn

Ruby: arr.sort
来源：http://dh.muxihuayi.cn

C#:   list.Sort();
来源：http://ga.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jl.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dk.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iq.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hd.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ex.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fi.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uc.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bm.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ci.chemitech.net.cn

[D11] 反转数组
来源：http://et.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gp.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://ql.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rz.huanxung.cn

TS:   [...arr].reverse();
来源：http://ge.521024.cn

Java: Collections.reverse(list);
来源：http://ue.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ig.521024.cn

Ruby: arr.reverse
来源：http://sr.bjjhwx.cn

C#:   list.Reverse();
来源：http://uk.nicolike.cn

[D12] 查找元素下标
来源：http://gv.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://ib.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jp.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iv.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://el.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qz.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://if.nicolike.cn

Ruby: arr.index(x)
来源：http://pi.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://bv.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://lm.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jn.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dw.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://re.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://nl.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xh.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hi.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qp.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://hg.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tw.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sq.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://sj.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://nb.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qf.gzmigu.cn

Go:   // 手写循环
来源：http://dn.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vt.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zu.shtwfgs.cn

[D15] 去重
来源：http://if.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kv.colortex.cn

PHP:  array_unique($arr);
来源：http://eb.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://ck.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ny.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nc.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dg.jctech888.com.cn

Ruby: arr.uniq
来源：http://wo.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://oo.haigaiapp.cn

[D16] 求和与平均值
来源：http://nv.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aj.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ns.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bh.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uv.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://vf.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zt.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ni.521024.cn

[D17] 最大值与最小值
来源：http://fu.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://iv.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://bb.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://on.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://la.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ce.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qe.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://pl.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://hd.asd995.cn

[D18] 扁平化嵌套数组
来源：http://jo.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kd.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://qf.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://la.muxihuayi.cn

TS:   nested.flat();
来源：http://sf.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kz.shtwfgs.cn

Go:   // 手写双层循环
来源：http://wl.gzmigu.cn

Ruby: nested.flatten
来源：http://rz.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://df.nicolike.cn

[D19] 按字段分组
来源：http://wm.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fv.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xo.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jv.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://an.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kn.asd995.cn

Go:   // 手写 map[string][]T
来源：http://lq.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ma.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kd.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://zp.hnjuh.cn

Py:   Counter(arr)
来源：http://hl.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://yh.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dt.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xh.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ou.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://xb.newstarts.cn

Ruby: arr.tally
来源：http://cp.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ve.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://sq.shxzukj.cn

Py:   x in arr
来源：http://vr.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://fl.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://pl.lnxyls.cn

TS:   arr.includes(x)
来源：http://hm.nicolike.cn

Java: list.contains(x)
来源：http://yy.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://lw.shxzukj.cn

Ruby: arr.include?(x)
来源：http://ta.yuexingan06.cn

C#:   list.Contains(x)
来源：http://bh.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://eo.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cd.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jc.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zr.shxzukj.cn

TS:   [...arr];
来源：http://ty.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://bf.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dt.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://cu.hnjuh.cn

C#:   new List<int>(list);
来源：http://xu.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://uu.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oh.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pm.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oa.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rz.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wc.muxihuayi.cn

Go:   // 手写循环
来源：http://il.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hu.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nh.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://wq.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cp.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fm.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ka.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ai.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dx.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://in.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ti.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hs.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://dn.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zc.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yu.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zm.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lh.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://km.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sx.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qe.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jr.gzmigu.cn

[D26] 数组转字符串
来源：http://ew.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://jw.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://xw.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://lx.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://xy.newstarts.cn

Java: String.join(", ", list)
来源：http://lz.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://ux.szxytkj.cn

Ruby: arr.join(", ")
来源：http://bf.nszjky.cn

C#:   string.Join(", ", list)
来源：http://qh.newstarts.cn

================================================================================
来源：http://ht.521024.cn

E. 字符串处理
来源：http://sg.wgjwhj.cn

================================================================================
来源：http://sa.chemitech.net.cn

[E01] 拼接字符串
来源：http://oq.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uj.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pn.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vk.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jx.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oy.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lx.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qh.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yw.shxzskj.cn

[E02] 重复字符串
来源：http://as.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://fq.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://jw.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://id.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://pr.colortex.cn

Java: "ab".repeat(3)
来源：http://mo.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://bp.haigaiapp.cn

Ruby: "ab" * 3
来源：http://hn.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yb.gzmigu.cn

[E03] 截取子串
来源：http://al.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ui.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kp.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ow.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://xp.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ih.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wr.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://if.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://by.nicolike.cn

[E04] 查找子串位置
来源：http://on.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://fj.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://kx.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ih.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ia.521024.cn

Java: s.indexOf("x")
来源：http://dr.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://md.muxihuayi.cn

Ruby: s.index("x")
来源：http://qm.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://nl.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oq.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sv.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ae.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mh.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xw.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vd.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ga.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://to.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tk.colortex.cn

[E06] 替换子串
来源：http://cz.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eb.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://ec.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wl.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://et.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xm.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wv.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ft.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://mz.nicolike.cn

[E07] 按分隔符拆分
来源：http://ft.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wr.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xg.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fo.szsharing.cn

TS:   s.split(",")
来源：http://pk.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://be.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://th.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://nt.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tc.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://nb.chemitech.net.cn

Py:   ",".join(items)
来源：http://st.szsharing.cn

PHP:  implode(",", $items);
来源：http://bz.szsharing.cn

JS:   items.join(",")
来源：http://hh.shxzukj.cn

TS:   items.join(",")
来源：http://mw.shxzskj.cn

Java: String.join(",", items)
来源：http://cx.yuexingan06.cn


<!-- 参考信息 -->