代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hy.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ax.hnjuh.cn

Java: // 无解构
来源：http://jt.hahajie.cn

Go:   // 无解构
来源：http://mo.shtwfgs.cn

Ruby: a, b = pair
来源：http://me.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://xk.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://fe.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dv.newstarts.cn

PHP:  // 无重载
来源：http://hu.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qh.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ko.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mo.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://fh.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://cw.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ij.lnxyls.cn

================================================================================
来源：http://ag.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://sk.panjiajie.cn

================================================================================
来源：http://tc.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://wg.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ok.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mx.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cw.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sk.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iq.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://te.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://oq.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tf.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://es.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ry.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rj.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://um.jctech888.com.cn

TS:   arr.push(4);
来源：http://wi.huixiangedu.cn

Java: list.add(4);
来源：http://ny.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://vi.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ie.9csxet.cn

C#:   list.Add(4);
来源：http://zk.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://mz.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://xq.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lr.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cb.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://mk.jctech888.com.cn

Java: list.add(0, 0);
来源：http://dc.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ls.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://db.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://hv.haigaiapp.cn

[D04] 删除元素
来源：http://lv.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ai.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ov.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nt.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://sl.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dr.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zv.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jh.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kn.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://pj.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gc.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gj.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ds.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://za.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://el.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://cy.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gw.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lr.huixinmuqiang.cn

[D06] 数组长度
来源：http://kb.bookmarksfly.cn

Py:   len(arr)
来源：http://vw.bookmarksfly.cn

PHP:  count($arr);
来源：http://su.chemitech.net.cn

JS:   arr.length
来源：http://vs.nszjky.cn

TS:   arr.length
来源：http://jq.muxihuayi.cn

Java: list.size();
来源：http://yb.huixiangedu.cn

Go:   len(arr)
来源：http://kq.nicolike.cn

Ruby: arr.length; arr.size
来源：http://ts.hahajie.cn

C#:   list.Count;
来源：http://ta.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://yc.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yq.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rw.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://dk.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ia.shxzskj.cn

Java: list.subList(1, 4);
来源：http://oi.hnjuh.cn

Go:   arr[1:4]
来源：http://dv.nicolike.cn

Ruby: arr[1, 3]
来源：http://yw.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://lg.haigaiapp.cn

[D08] 合并两个数组
来源：http://bl.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://ph.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://of.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ha.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ef.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ey.szsharing.cn

Go:   append(a, b...)
来源：http://ug.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://eb.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://ti.huanxung.cn

[D09] 排序（升序）
来源：http://oh.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ey.yuexingan06.cn

PHP:  sort($arr);
来源：http://kj.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://if.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ds.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ox.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ep.panjiajie.cn

Ruby: arr.sort
来源：http://aq.hahajie.cn

C#:   list.Sort();
来源：http://xg.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://br.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zq.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://il.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zv.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qa.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xu.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nb.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xd.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aw.panjiajie.cn

[D11] 反转数组
来源：http://sx.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cc.asd995.cn

PHP:  array_reverse($arr);
来源：http://vd.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ud.huanxung.cn

TS:   [...arr].reverse();
来源：http://gr.9csxet.cn

Java: Collections.reverse(list);
来源：http://qm.colortex.cn

Go:   slices.Reverse(arr)
来源：http://gu.hnjuh.cn

Ruby: arr.reverse
来源：http://qp.521024.cn

C#:   list.Reverse();
来源：http://hg.wgjwhj.cn

[D12] 查找元素下标
来源：http://oi.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://gn.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nq.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ec.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zf.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jb.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://lb.nicolike.cn

Ruby: arr.index(x)
来源：http://lt.colortex.cn

C#:   list.IndexOf(x);
来源：http://gw.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://js.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wf.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ji.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://ns.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ii.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tm.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kf.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://og.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oa.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://nq.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lt.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://km.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://rb.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://ns.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ku.lnxyls.cn

Go:   // 手写循环
来源：http://vi.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zf.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vq.asd995.cn

[D15] 去重
来源：http://jq.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cu.hahajie.cn

PHP:  array_unique($arr);
来源：http://hz.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://kg.9csxet.cn

TS:   [...new Set(arr)]
来源：http://zh.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ip.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cj.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://cy.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ji.shxzskj.cn

[D16] 求和与平均值
来源：http://an.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dv.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aj.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://om.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zr.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://br.huanxung.cn

Go:   // 手写循环累加
来源：http://fn.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cp.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://fk.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ec.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://gf.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ni.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://od.shxzukj.cn

TS:   Math.max(...arr);
来源：http://or.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xc.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iz.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://bx.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://ko.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://uk.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ho.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wq.panjiajie.cn

TS:   nested.flat();
来源：http://vs.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gh.nicolike.cn

Go:   // 手写双层循环
来源：http://eg.nszjky.cn

Ruby: nested.flatten
来源：http://nv.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sc.newstarts.cn

[D19] 按字段分组
来源：http://qd.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cl.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xe.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bc.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pt.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ur.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://ob.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ec.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yo.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://fn.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://og.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://gz.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gn.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://is.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://ki.gzmigu.cn

Ruby: arr.tally
来源：http://kl.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qm.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://qy.521024.cn

Py:   x in arr
来源：http://sg.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://aj.yuexingan06.cn

JS:   arr.includes(x)
来源：http://yp.shxzukj.cn

TS:   arr.includes(x)
来源：http://ts.yuntaijiaju.cn

Java: list.contains(x)
来源：http://tc.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://uj.nszjky.cn

Ruby: arr.include?(x)
来源：http://cf.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://ol.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://lw.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yk.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bv.yuexingan06.cn

TS:   [...arr];
来源：http://qp.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://ud.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bn.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://vy.muxihuayi.cn

C#:   new List<int>(list);
来源：http://og.huixiangedu.cn

[D23] reduce 累积计算
来源：http://zu.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wp.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ua.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cd.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pk.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sv.bjjhwx.cn

Go:   // 手写循环
来源：http://ow.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zt.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yc.521024.cn

[D24] 字典 / Map 基本操作
来源：http://jc.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ld.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yu.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gy.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pj.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cz.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fg.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ja.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rh.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://tg.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mi.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rl.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rn.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bj.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cu.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tm.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qd.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jm.newstarts.cn

[D26] 数组转字符串
来源：http://ff.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://hi.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://hi.colortex.cn

JS:   arr.join(", ")
来源：http://gb.panjiajie.cn

TS:   arr.join(", ")
来源：http://bz.shxzskj.cn

Java: String.join(", ", list)
来源：http://an.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://wb.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://zp.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://nj.shxzukj.cn

================================================================================
来源：http://xv.shxzukj.cn

E. 字符串处理
来源：http://xy.jctech888.com.cn

================================================================================
来源：http://up.wgjwhj.cn

[E01] 拼接字符串
来源：http://ek.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ce.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bg.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mu.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vf.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mi.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pt.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jx.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sb.9csxet.cn

[E02] 重复字符串
来源：http://gl.nszjky.cn

Py:   "ab" * 3
来源：http://xs.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://gk.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://pe.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://pw.szsharing.cn

Java: "ab".repeat(3)
来源：http://vz.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://vt.shxzukj.cn

Ruby: "ab" * 3
来源：http://vv.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lz.asd995.cn

[E03] 截取子串
来源：http://xn.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lp.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lo.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bo.szsharing.cn

TS:   s.slice(1, 4)
来源：http://fm.shxzskj.cn

Java: s.substring(1, 4)
来源：http://mh.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mh.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iw.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://nz.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://ea.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://cg.hahajie.cn

PHP:  strpos($s, "x");
来源：http://sp.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ds.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://vh.asd995.cn

Java: s.indexOf("x")
来源：http://ic.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://va.huanxung.cn

Ruby: s.index("x")
来源：http://dj.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://nm.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hh.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dl.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ar.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pl.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zf.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lm.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zy.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xx.nicolike.cn


<!-- 参考信息 -->