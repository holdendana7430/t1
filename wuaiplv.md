代发 wailian999

PHP:  // 无重载
来源：http://ug.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ed.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://io.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://js.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://jw.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://hp.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ub.colortex.cn

================================================================================
来源：http://wm.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ja.hahajie.cn

================================================================================
来源：http://zs.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://kq.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qy.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jd.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oq.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nm.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bh.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://cu.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ci.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vj.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://ow.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mj.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hs.chemitech.net.cn

JS:   arr.push(4);
来源：http://hj.szsharing.cn

TS:   arr.push(4);
来源：http://xh.szxytkj.cn

Java: list.add(4);
来源：http://lq.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://se.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ty.shxzskj.cn

C#:   list.Add(4);
来源：http://ye.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://kd.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://fu.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oj.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bf.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://zy.shxzukj.cn

Java: list.add(0, 0);
来源：http://on.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lk.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vo.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://qx.521024.cn

[D04] 删除元素
来源：http://dt.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xl.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uk.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://xg.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sa.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nt.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ay.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iu.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://jx.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qs.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vz.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://bv.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://sh.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pk.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bj.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mt.hnjuh.cn

[D06] 数组长度
来源：http://er.colortex.cn

Py:   len(arr)
来源：http://xz.huixiangedu.cn

PHP:  count($arr);
来源：http://ss.jctech888.com.cn

JS:   arr.length
来源：http://cn.colortex.cn

TS:   arr.length
来源：http://hz.bjjhwx.cn

Java: list.size();
来源：http://gu.9csxet.cn

Go:   len(arr)
来源：http://mj.hahajie.cn

Ruby: arr.length; arr.size
来源：http://dx.lnxyls.cn

C#:   list.Count;
来源：http://yj.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ls.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bp.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ud.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://qf.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://df.hnjuh.cn

Java: list.subList(1, 4);
来源：http://sk.9csxet.cn

Go:   arr[1:4]
来源：http://yv.panjiajie.cn

Ruby: arr[1, 3]
来源：http://zl.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://lm.wgjwhj.cn

[D08] 合并两个数组
来源：http://mg.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://uh.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://ng.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dp.shtwfgs.cn

TS:   [...a, ...b];
来源：http://qy.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wi.521024.cn

Go:   append(a, b...)
来源：http://yh.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ox.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://yd.shtwfgs.cn

[D09] 排序（升序）
来源：http://wc.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://my.panjiajie.cn

PHP:  sort($arr);
来源：http://ak.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://je.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tb.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hd.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://um.hahajie.cn

Ruby: arr.sort
来源：http://hk.asd995.cn

C#:   list.Sort();
来源：http://bq.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://el.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://px.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mk.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ma.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ag.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ed.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ek.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pz.bookmarksfly.cn

[D11] 反转数组
来源：http://vs.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dn.huanxung.cn

PHP:  array_reverse($arr);
来源：http://yy.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zz.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://xt.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://zd.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://yc.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ys.wgjwhj.cn

C#:   list.Reverse();
来源：http://nc.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://vz.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://jt.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yy.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xt.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nx.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zr.colortex.cn

Go:   slices.Index(arr, x)
来源：http://zg.nszjky.cn

Ruby: arr.index(x)
来源：http://up.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://qg.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://vf.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pi.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tv.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://bn.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://ls.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vc.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ak.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xx.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lg.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://ws.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nc.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tr.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://va.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://qf.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://de.jianghongdianzi.cn

Go:   // 手写循环
来源：http://cw.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ly.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lp.hahajie.cn

[D15] 去重
来源：http://zq.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bz.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://qt.521024.cn

JS:   [...new Set(arr)]
来源：http://jj.521024.cn

TS:   [...new Set(arr)]
来源：http://ny.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uh.szxytkj.cn

Ruby: arr.uniq
来源：http://ye.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://ti.muxihuayi.cn

[D16] 求和与平均值
来源：http://df.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://re.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qj.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://je.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jy.szxytkj.cn

Go:   // 手写循环累加
来源：http://rf.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yq.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://gd.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://rd.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://en.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://ms.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cl.shxzukj.cn

TS:   Math.max(...arr);
来源：http://dd.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ks.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ss.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://ot.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://nt.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://vx.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ak.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://kj.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ni.szxytkj.cn

TS:   nested.flat();
来源：http://jg.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nx.panjiajie.cn

Go:   // 手写双层循环
来源：http://ym.521024.cn

Ruby: nested.flatten
来源：http://ln.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eu.szsharing.cn

[D19] 按字段分组
来源：http://tt.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yc.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pl.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aq.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eb.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bg.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ou.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oi.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kn.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://lg.521024.cn

Py:   Counter(arr)
来源：http://oe.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://kz.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cb.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bg.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gd.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ne.521024.cn

Ruby: arr.tally
来源：http://mg.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gn.521024.cn

[D21] 判断是否包含某元素
来源：http://gd.shtwfgs.cn

Py:   x in arr
来源：http://yw.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://ip.nicolike.cn

JS:   arr.includes(x)
来源：http://pq.wgjwhj.cn

TS:   arr.includes(x)
来源：http://qq.chemitech.net.cn

Java: list.contains(x)
来源：http://kb.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://nh.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://az.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://rh.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://fr.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pp.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zi.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cj.huanxung.cn

TS:   [...arr];
来源：http://zp.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://ef.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bu.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://bg.yuexingan06.cn

C#:   new List<int>(list);
来源：http://ll.szsharing.cn

[D23] reduce 累积计算
来源：http://gz.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mk.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vn.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qv.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nz.9csxet.cn

Go:   // 手写循环
来源：http://ru.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lm.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ha.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://eh.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ka.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pi.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ug.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ae.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ct.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xt.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kw.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jb.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://qm.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cf.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://os.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://un.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fh.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jr.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tj.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zi.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bb.hahajie.cn

[D26] 数组转字符串
来源：http://yx.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://pl.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ab.shxzskj.cn

JS:   arr.join(", ")
来源：http://mi.panjiajie.cn

TS:   arr.join(", ")
来源：http://va.szsharing.cn

Java: String.join(", ", list)
来源：http://hh.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://jv.521024.cn

Ruby: arr.join(", ")
来源：http://dm.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://sj.gzmigu.cn

================================================================================
来源：http://bx.yuexingan06.cn

E. 字符串处理
来源：http://oe.haigaiapp.cn

================================================================================
来源：http://qt.nicolike.cn

[E01] 拼接字符串
来源：http://xh.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hg.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aa.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cw.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ni.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sz.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vk.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hk.panjiajie.cn

[E02] 重复字符串
来源：http://fv.bjjhwx.cn

Py:   "ab" * 3
来源：http://dq.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://gt.huanxung.cn

JS:   "ab".repeat(3)
来源：http://nj.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://zg.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://id.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://dc.haigaiapp.cn

Ruby: "ab" * 3
来源：http://pr.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kx.colortex.cn

[E03] 截取子串
来源：http://cs.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ua.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pq.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ei.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://zx.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://by.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kn.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pg.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://dd.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://ed.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://zr.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://jb.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ef.9csxet.cn

TS:   s.indexOf("x")
来源：http://wi.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://hc.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://kl.chemitech.net.cn

Ruby: s.index("x")
来源：http://hh.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://bh.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ed.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://se.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ou.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mg.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zo.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wa.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ps.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bh.bjjhwx.cn

[E06] 替换子串
来源：http://nl.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fd.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://dq.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vy.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://sm.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sz.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ok.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ng.nszjky.cn


<!-- 参考信息 -->