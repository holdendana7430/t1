代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ks.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://ab.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hj.hahajie.cn

[D02] 追加元素到末尾
来源：http://zk.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vz.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tc.nicolike.cn

JS:   arr.push(4);
来源：http://bm.asd995.cn

TS:   arr.push(4);
来源：http://uu.szxytkj.cn

Java: list.add(4);
来源：http://ls.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://iy.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://ez.asd995.cn

C#:   list.Add(4);
来源：http://ui.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://yz.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://hv.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pv.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fw.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://cz.gzmigu.cn

Java: list.add(0, 0);
来源：http://lf.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ew.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xu.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://rs.nszjky.cn

[D04] 删除元素
来源：http://eu.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pc.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jd.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mm.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://kx.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ru.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mj.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://so.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yo.jctech888.com.cn

[D05] 访问与修改元素
来源：http://kd.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ry.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gj.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fe.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://mt.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://ho.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://tj.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gw.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nl.nszjky.cn

[D06] 数组长度
来源：http://fh.huanxung.cn

Py:   len(arr)
来源：http://kb.521024.cn

PHP:  count($arr);
来源：http://ck.nicolike.cn

JS:   arr.length
来源：http://da.shxzskj.cn

TS:   arr.length
来源：http://xt.shxzukj.cn

Java: list.size();
来源：http://ux.asd995.cn

Go:   len(arr)
来源：http://me.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://sd.asd995.cn

C#:   list.Count;
来源：http://bw.521024.cn

[D07] 切片 / 取子数组
来源：http://ll.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nb.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dv.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://co.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ir.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://gn.jctech888.com.cn

Go:   arr[1:4]
来源：http://ua.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://qp.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://qf.9csxet.cn

[D08] 合并两个数组
来源：http://jb.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://kw.asd995.cn

PHP:  array_merge($a, $b);
来源：http://aj.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wy.gzmigu.cn

TS:   [...a, ...b];
来源：http://hc.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://un.jctech888.com.cn

Go:   append(a, b...)
来源：http://bk.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://sx.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://dw.nszjky.cn

[D09] 排序（升序）
来源：http://ll.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ko.colortex.cn

PHP:  sort($arr);
来源：http://mf.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sx.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gu.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ii.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ux.colortex.cn

Ruby: arr.sort
来源：http://hy.nicolike.cn

C#:   list.Sort();
来源：http://gj.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bo.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dw.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pi.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aq.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xx.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ck.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ug.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uc.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sq.bjjhwx.cn

[D11] 反转数组
来源：http://oj.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://au.szsharing.cn

PHP:  array_reverse($arr);
来源：http://lf.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ut.newstarts.cn

TS:   [...arr].reverse();
来源：http://cj.hnjuh.cn

Java: Collections.reverse(list);
来源：http://kp.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://ry.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://go.huixiangedu.cn

C#:   list.Reverse();
来源：http://qy.bookmarksfly.cn

[D12] 查找元素下标
来源：http://pa.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://ns.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qw.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xw.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://il.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wy.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://tn.wgjwhj.cn

Ruby: arr.index(x)
来源：http://jf.521024.cn

C#:   list.IndexOf(x);
来源：http://ra.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://ae.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tb.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bs.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://xg.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://ln.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uv.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qt.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yx.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ns.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://di.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qg.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://li.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://mq.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://zd.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cp.hahajie.cn

Go:   // 手写循环
来源：http://de.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yo.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ca.huixinmuqiang.cn

[D15] 去重
来源：http://ii.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pg.hnjuh.cn

PHP:  array_unique($arr);
来源：http://zp.nszjky.cn

JS:   [...new Set(arr)]
来源：http://jn.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://mu.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://be.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lo.colortex.cn

Ruby: arr.uniq
来源：http://zh.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://hr.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://tu.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cf.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mg.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sn.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gj.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://dl.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wu.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://wu.9csxet.cn

[D17] 最大值与最小值
来源：http://qx.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://pu.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://nj.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wj.hahajie.cn

TS:   Math.max(...arr);
来源：http://lp.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oi.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xq.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://sv.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://dy.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://yy.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cm.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://hb.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ze.huanxung.cn

TS:   nested.flat();
来源：http://ih.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ts.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://cj.nicolike.cn

Ruby: nested.flatten
来源：http://ux.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dy.asd995.cn

[D19] 按字段分组
来源：http://jj.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wj.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yu.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://po.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ou.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xt.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://pt.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wb.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yr.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://qu.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://wy.9csxet.cn

PHP:  array_count_values($arr);
来源：http://mb.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wy.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sd.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wk.nicolike.cn

Go:   // 手写 map[T]int
来源：http://qy.wgjwhj.cn

Ruby: arr.tally
来源：http://lp.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vi.hahajie.cn

[D21] 判断是否包含某元素
来源：http://td.huixinmuqiang.cn

Py:   x in arr
来源：http://kv.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://rr.lnxyls.cn

JS:   arr.includes(x)
来源：http://zw.chemitech.net.cn

TS:   arr.includes(x)
来源：http://kc.jctech888.com.cn

Java: list.contains(x)
来源：http://kw.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://im.shxzukj.cn

Ruby: arr.include?(x)
来源：http://jc.shxzskj.cn

C#:   list.Contains(x)
来源：http://ft.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://id.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yi.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cp.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hw.gzmigu.cn

TS:   [...arr];
来源：http://xh.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://gk.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://my.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://co.hnjuh.cn

C#:   new List<int>(list);
来源：http://ub.chemitech.net.cn

[D23] reduce 累积计算
来源：http://gs.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://by.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tt.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ow.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ov.asd995.cn

Go:   // 手写循环
来源：http://fs.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uw.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iw.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ly.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kc.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ue.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mt.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fz.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fc.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wm.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kq.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://on.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://ye.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bu.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fm.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wf.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ct.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dy.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kl.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ab.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wc.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ua.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://rm.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://hl.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://hk.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ai.gzmigu.cn

Java: String.join(", ", list)
来源：http://ap.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://wu.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://cc.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ya.szsharing.cn

================================================================================
来源：http://re.shtwfgs.cn

E. 字符串处理
来源：http://fz.hnjuh.cn

================================================================================
来源：http://oz.shxzskj.cn

[E01] 拼接字符串
来源：http://os.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://td.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ac.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yr.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tv.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gz.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gq.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nw.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wr.newstarts.cn

[E02] 重复字符串
来源：http://hr.jctech888.com.cn

Py:   "ab" * 3
来源：http://cz.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://gl.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://bb.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://hy.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://tq.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://nu.huixiangedu.cn

Ruby: "ab" * 3
来源：http://yj.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eo.9csxet.cn

[E03] 截取子串
来源：http://yq.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kr.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tc.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mr.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://so.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://wu.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zr.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qr.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://hq.newstarts.cn

[E04] 查找子串位置
来源：http://jr.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://rd.521024.cn

PHP:  strpos($s, "x");
来源：http://hh.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vg.gzmigu.cn

TS:   s.indexOf("x")
来源：http://nw.colortex.cn

Java: s.indexOf("x")
来源：http://ba.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://eo.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://yk.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://yq.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yz.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xh.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wv.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ar.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sh.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yd.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lh.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lk.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vx.huixiangedu.cn

[E06] 替换子串
来源：http://wu.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yh.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://gk.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wl.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://so.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zw.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lv.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iu.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://sm.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://sv.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ev.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fp.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wz.hnjuh.cn

TS:   s.split(",")
来源：http://rc.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fy.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eb.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://er.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kl.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://ay.huixiangedu.cn

Py:   ",".join(items)
来源：http://gy.szsharing.cn

PHP:  implode(",", $items);
来源：http://ur.szsharing.cn

JS:   items.join(",")
来源：http://dl.muxihuayi.cn

TS:   items.join(",")
来源：http://cz.huanxung.cn

Java: String.join(",", items)
来源：http://cj.szsharing.cn


<!-- 参考信息 -->