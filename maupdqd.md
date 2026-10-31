代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://fh.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://cf.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ll.jctech888.com.cn

================================================================================
来源：http://mf.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://na.wgjwhj.cn

================================================================================
来源：http://hz.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://ig.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ln.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qp.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dk.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ss.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dn.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://is.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://ky.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vi.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://qk.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rb.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://so.9csxet.cn

JS:   arr.push(4);
来源：http://jh.huanxung.cn

TS:   arr.push(4);
来源：http://gp.nszjky.cn

Java: list.add(4);
来源：http://my.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://qo.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://nf.lnxyls.cn

C#:   list.Add(4);
来源：http://hj.nszjky.cn

[D03] 在指定位置插入元素
来源：http://ki.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://mv.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ba.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xo.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ol.shxzukj.cn

Java: list.add(0, 0);
来源：http://kd.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dn.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kd.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://cr.huixiangedu.cn

[D04] 删除元素
来源：http://hm.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lh.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qu.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ou.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://pw.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pl.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://po.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mx.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bs.jctech888.com.cn

[D05] 访问与修改元素
来源：http://mt.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yq.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tz.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ge.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://es.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://am.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://va.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sa.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://io.shxzukj.cn

[D06] 数组长度
来源：http://nv.asd995.cn

Py:   len(arr)
来源：http://kt.nszjky.cn

PHP:  count($arr);
来源：http://fi.panjiajie.cn

JS:   arr.length
来源：http://fw.jctech888.com.cn

TS:   arr.length
来源：http://zl.nszjky.cn

Java: list.size();
来源：http://to.gzmigu.cn

Go:   len(arr)
来源：http://mu.9csxet.cn

Ruby: arr.length; arr.size
来源：http://qe.szxytkj.cn

C#:   list.Count;
来源：http://sf.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://xv.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jm.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gh.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://wq.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://bb.shxzskj.cn

Java: list.subList(1, 4);
来源：http://pg.newstarts.cn

Go:   arr[1:4]
来源：http://bc.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://op.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://rv.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://re.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://fv.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://jo.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sn.9csxet.cn

TS:   [...a, ...b];
来源：http://ni.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ou.lnxyls.cn

Go:   append(a, b...)
来源：http://qx.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://lh.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://rx.asd995.cn

[D09] 排序（升序）
来源：http://rq.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.shxzukj.cn

PHP:  sort($arr);
来源：http://ul.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dv.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ym.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hs.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pb.gzmigu.cn

Ruby: arr.sort
来源：http://qk.muxihuayi.cn

C#:   list.Sort();
来源：http://qd.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bw.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dp.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mj.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jl.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tc.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tn.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://il.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pc.chemitech.net.cn

[D11] 反转数组
来源：http://bx.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fh.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://fr.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bz.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://nn.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://mm.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://jo.wgjwhj.cn

Ruby: arr.reverse
来源：http://cq.lnxyls.cn

C#:   list.Reverse();
来源：http://dv.521024.cn

[D12] 查找元素下标
来源：http://hg.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://wr.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rx.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qp.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zl.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://cj.nicolike.cn

Ruby: arr.index(x)
来源：http://xy.nicolike.cn

C#:   list.IndexOf(x);
来源：http://hw.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ki.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mg.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bd.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://yg.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://nl.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ps.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hl.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://of.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://oi.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ch.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zz.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://wn.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://me.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tz.chemitech.net.cn

Go:   // 手写循环
来源：http://bx.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://su.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kl.chemitech.net.cn

[D15] 去重
来源：http://fd.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tb.huanxung.cn

PHP:  array_unique($arr);
来源：http://zu.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://eg.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://kx.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vv.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cx.shxzukj.cn

Ruby: arr.uniq
来源：http://eh.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://op.gzmigu.cn

[D16] 求和与平均值
来源：http://uh.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://md.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://re.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yn.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ii.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uo.panjiajie.cn

Go:   // 手写循环累加
来源：http://ob.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fy.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ck.hahajie.cn

[D17] 最大值与最小值
来源：http://qt.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://rp.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://in.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kf.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://je.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xq.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tr.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://jn.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://ru.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://kt.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fu.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://kv.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ad.wgjwhj.cn

TS:   nested.flat();
来源：http://ov.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yj.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ti.szsharing.cn

Ruby: nested.flatten
来源：http://mj.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lj.shxzskj.cn

[D19] 按字段分组
来源：http://id.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mi.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tz.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pc.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tf.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://js.asd995.cn

Go:   // 手写 map[string][]T
来源：http://yr.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vo.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tu.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://aj.521024.cn

Py:   Counter(arr)
来源：http://xe.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://eg.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hm.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cz.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xu.newstarts.cn

Go:   // 手写 map[T]int
来源：http://ok.nicolike.cn

Ruby: arr.tally
来源：http://xa.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ax.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://br.jctech888.com.cn

Py:   x in arr
来源：http://os.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://fc.jctech888.com.cn

JS:   arr.includes(x)
来源：http://qs.9csxet.cn

TS:   arr.includes(x)
来源：http://fc.gzmigu.cn

Java: list.contains(x)
来源：http://tl.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://hu.521024.cn

Ruby: arr.include?(x)
来源：http://rb.lnxyls.cn

C#:   list.Contains(x)
来源：http://to.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://vj.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qd.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ax.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vt.9csxet.cn

TS:   [...arr];
来源：http://zp.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://wa.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jh.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://zb.521024.cn

C#:   new List<int>(list);
来源：http://zs.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://ql.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ca.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xn.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kb.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nd.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ye.huixiangedu.cn

Go:   // 手写循环
来源：http://do.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tu.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xx.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://fa.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lz.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vx.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xz.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xv.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gt.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://os.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lr.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hg.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://zx.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bj.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xu.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cb.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://il.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nb.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pg.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hb.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zw.asd995.cn

[D26] 数组转字符串
来源：http://sk.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://oj.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://wc.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ah.shxzskj.cn

TS:   arr.join(", ")
来源：http://um.asd995.cn

Java: String.join(", ", list)
来源：http://ks.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://mz.newstarts.cn

Ruby: arr.join(", ")
来源：http://zx.hahajie.cn

C#:   string.Join(", ", list)
来源：http://sg.panjiajie.cn

================================================================================
来源：http://wy.panjiajie.cn

E. 字符串处理
来源：http://yj.shxzskj.cn

================================================================================
来源：http://rh.nszjky.cn

[E01] 拼接字符串
来源：http://ka.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sr.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tu.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dp.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fm.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ae.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mm.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lr.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nb.chemitech.net.cn

[E02] 重复字符串
来源：http://wu.newstarts.cn

Py:   "ab" * 3
来源：http://ph.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://gy.asd995.cn

JS:   "ab".repeat(3)
来源：http://py.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://kw.nszjky.cn

Java: "ab".repeat(3)
来源：http://pc.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://cb.hahajie.cn

Ruby: "ab" * 3
来源：http://yv.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oi.nicolike.cn

[E03] 截取子串
来源：http://te.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gf.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cj.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ni.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ku.newstarts.cn

Java: s.substring(1, 4)
来源：http://gk.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mg.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rm.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://at.nicolike.cn

[E04] 查找子串位置
来源：http://di.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://lf.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://id.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sp.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ha.yuexingan06.cn

Java: s.indexOf("x")
来源：http://av.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://ly.asd995.cn

Ruby: s.index("x")
来源：http://nx.asd995.cn

C#:   s.IndexOf("x")
来源：http://qj.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://je.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zr.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nq.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wd.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hv.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xt.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fy.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bc.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mo.chemitech.net.cn

[E06] 替换子串
来源：http://dh.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fl.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://rj.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qc.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://xe.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ux.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://di.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://at.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://lk.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://oa.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bv.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sg.colortex.cn


<!-- 参考信息 -->