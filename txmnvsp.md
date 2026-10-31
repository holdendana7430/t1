代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jh.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uc.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bc.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qx.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://dd.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://cy.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tr.nszjky.cn

[D02] 追加元素到末尾
来源：http://av.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dy.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sw.szsharing.cn

JS:   arr.push(4);
来源：http://ow.shxzskj.cn

TS:   arr.push(4);
来源：http://jz.yuntaijiaju.cn

Java: list.add(4);
来源：http://ft.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://oc.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://mu.chemitech.net.cn

C#:   list.Add(4);
来源：http://wf.hahajie.cn

[D03] 在指定位置插入元素
来源：http://lg.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://aq.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gt.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uo.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://dt.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://re.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oj.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gk.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://po.colortex.cn

[D04] 删除元素
来源：http://zt.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oo.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bi.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eu.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://fj.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dy.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eo.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://je.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bu.shxzukj.cn

[D05] 访问与修改元素
来源：http://vm.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mb.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ca.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wz.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://gh.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bq.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://mb.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mq.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mo.jctech888.com.cn

[D06] 数组长度
来源：http://ak.shtwfgs.cn

Py:   len(arr)
来源：http://qg.shxzukj.cn

PHP:  count($arr);
来源：http://tf.521024.cn

JS:   arr.length
来源：http://oz.haigaiapp.cn

TS:   arr.length
来源：http://zw.asd995.cn

Java: list.size();
来源：http://xo.chemitech.net.cn

Go:   len(arr)
来源：http://wr.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ii.nicolike.cn

C#:   list.Count;
来源：http://pi.huanxung.cn

[D07] 切片 / 取子数组
来源：http://yk.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nq.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ov.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://dj.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://yf.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://dm.colortex.cn

Go:   arr[1:4]
来源：http://bi.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://te.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://nz.bookmarksfly.cn

[D08] 合并两个数组
来源：http://jo.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://mx.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://bt.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lf.jctech888.com.cn

TS:   [...a, ...b];
来源：http://rj.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zw.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://sr.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://hf.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://fh.nszjky.cn

[D09] 排序（升序）
来源：http://sh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://wf.521024.cn

PHP:  sort($arr);
来源：http://bi.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pg.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cx.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zd.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xv.gzmigu.cn

Ruby: arr.sort
来源：http://ye.chemitech.net.cn

C#:   list.Sort();
来源：http://ci.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tt.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xv.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rk.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lm.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kc.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ga.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://et.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zg.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://us.gzmigu.cn

[D11] 反转数组
来源：http://rg.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pn.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://py.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ln.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ny.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://sq.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://zs.shxzskj.cn

Ruby: arr.reverse
来源：http://eo.shxzskj.cn

C#:   list.Reverse();
来源：http://nd.hnjuh.cn

[D12] 查找元素下标
来源：http://ya.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://uu.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ft.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://up.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rm.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cr.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://tt.chemitech.net.cn

Ruby: arr.index(x)
来源：http://gi.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ab.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://ts.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gb.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dn.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://hs.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://iz.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yq.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fb.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nm.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kj.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://pv.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hp.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://la.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://qi.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://kk.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cz.shxzukj.cn

Go:   // 手写循环
来源：http://kp.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cc.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pu.521024.cn

[D15] 去重
来源：http://cq.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yq.asd995.cn

PHP:  array_unique($arr);
来源：http://xi.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://at.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://vb.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gw.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qr.hahajie.cn

Ruby: arr.uniq
来源：http://jf.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://uh.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://qb.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ul.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tr.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ht.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bo.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jg.shxzskj.cn

Go:   // 手写循环累加
来源：http://me.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lq.521024.cn

C#:   list.Sum();  list.Average()
来源：http://ak.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://gi.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://lk.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://fg.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rm.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://zy.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vf.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wt.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://yn.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://wd.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://wz.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fy.521024.cn

PHP:  array_merge(...$nested);
来源：http://gd.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uw.muxihuayi.cn

TS:   nested.flat();
来源：http://zt.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pf.wgjwhj.cn

Go:   // 手写双层循环
来源：http://pm.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://jn.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fn.bjjhwx.cn

[D19] 按字段分组
来源：http://be.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dc.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ll.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zs.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fu.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zd.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://op.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eq.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fy.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://hy.521024.cn

Py:   Counter(arr)
来源：http://sg.asd995.cn

PHP:  array_count_values($arr);
来源：http://nz.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cx.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mq.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://qa.bookmarksfly.cn

Ruby: arr.tally
来源：http://zh.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zv.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://mu.shtwfgs.cn

Py:   x in arr
来源：http://md.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://li.wgjwhj.cn

JS:   arr.includes(x)
来源：http://up.wgjwhj.cn

TS:   arr.includes(x)
来源：http://mv.lnxyls.cn

Java: list.contains(x)
来源：http://ki.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://do.shxzskj.cn

Ruby: arr.include?(x)
来源：http://py.asd995.cn

C#:   list.Contains(x)
来源：http://eq.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://wt.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qe.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gx.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://md.szxytkj.cn

TS:   [...arr];
来源：http://av.szsharing.cn

Java: new ArrayList<>(list);
来源：http://gh.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mb.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://gv.hnjuh.cn

C#:   new List<int>(list);
来源：http://cy.muxihuayi.cn

[D23] reduce 累积计算
来源：http://fs.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wg.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mq.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cs.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vo.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ti.szxytkj.cn

Go:   // 手写循环
来源：http://gh.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jm.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ga.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://nn.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rm.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dt.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dq.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rq.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://na.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jc.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://js.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jb.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://wf.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cz.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fw.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ys.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zk.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://io.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cm.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://li.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nv.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ow.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://kl.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://sm.521024.cn

JS:   arr.join(", ")
来源：http://uu.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ao.nicolike.cn

Java: String.join(", ", list)
来源：http://ve.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://uy.shxzskj.cn

Ruby: arr.join(", ")
来源：http://pr.asd995.cn

C#:   string.Join(", ", list)
来源：http://hf.yuntaijiaju.cn

================================================================================
来源：http://zt.huixiangedu.cn

E. 字符串处理
来源：http://wz.nicolike.cn

================================================================================
来源：http://lr.9csxet.cn

[E01] 拼接字符串
来源：http://yt.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gd.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bq.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rx.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ho.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mm.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ws.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rh.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wh.szxytkj.cn

[E02] 重复字符串
来源：http://fq.huanxung.cn

Py:   "ab" * 3
来源：http://le.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://gp.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://yz.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ny.shxzukj.cn

Java: "ab".repeat(3)
来源：http://vs.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://ca.huanxung.cn

Ruby: "ab" * 3
来源：http://oe.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cr.shxzskj.cn

[E03] 截取子串
来源：http://sx.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hd.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vq.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sj.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://sk.hnjuh.cn

Java: s.substring(1, 4)
来源：http://od.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xu.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://un.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://zr.gzmigu.cn

[E04] 查找子串位置
来源：http://jn.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://rz.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://sn.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bf.hahajie.cn

TS:   s.indexOf("x")
来源：http://bx.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ul.asd995.cn

Go:   strings.Index(s, "x")
来源：http://xh.521024.cn

Ruby: s.index("x")
来源：http://uc.asd995.cn

C#:   s.IndexOf("x")
来源：http://fh.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sg.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tb.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gs.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://na.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kt.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rf.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://df.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hs.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ix.jctech888.com.cn

[E06] 替换子串
来源：http://bc.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oi.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://nx.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fe.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://qx.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rm.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://av.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ek.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://jc.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://hp.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yg.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fm.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ol.yuexingan06.cn

TS:   s.split(",")
来源：http://fp.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zy.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aq.521024.cn

Ruby: s.split(",");  s.split
来源：http://rw.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ba.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://dt.huanxung.cn

Py:   ",".join(items)
来源：http://zf.haigaiapp.cn


<!-- 参考信息 -->