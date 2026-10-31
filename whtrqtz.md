代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wd.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://ar.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ku.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://lh.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yr.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pu.yuntaijiaju.cn

Java: // 无解构
来源：http://ef.nicolike.cn

Go:   // 无解构
来源：http://tu.jctech888.com.cn

Ruby: a, b = pair
来源：http://vw.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://hz.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://aq.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sn.asd995.cn

PHP:  // 无重载
来源：http://oh.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bf.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yy.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zx.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://rw.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://fq.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nh.haigaiapp.cn

================================================================================
来源：http://rh.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://wu.gzmigu.cn

================================================================================
来源：http://dh.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://zu.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wd.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jw.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://an.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cy.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nk.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://do.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://zv.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ih.szsharing.cn

[D02] 追加元素到末尾
来源：http://gb.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://je.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fb.colortex.cn

JS:   arr.push(4);
来源：http://mj.bjjhwx.cn

TS:   arr.push(4);
来源：http://sa.hahajie.cn

Java: list.add(4);
来源：http://lm.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://mk.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ys.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://am.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://vo.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://jb.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ao.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rl.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://sz.521024.cn

Java: list.add(0, 0);
来源：http://tn.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xz.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://od.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://lt.hnjuh.cn

[D04] 删除元素
来源：http://ma.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://no.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qo.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cy.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://oz.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jj.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jz.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sw.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://be.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://uf.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wc.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ku.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ey.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ky.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://fw.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://hj.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zh.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sw.huixinmuqiang.cn

[D06] 数组长度
来源：http://hl.gzmigu.cn

Py:   len(arr)
来源：http://hv.colortex.cn

PHP:  count($arr);
来源：http://iw.521024.cn

JS:   arr.length
来源：http://wp.asd995.cn

TS:   arr.length
来源：http://mk.huixinmuqiang.cn

Java: list.size();
来源：http://af.huixinmuqiang.cn

Go:   len(arr)
来源：http://mp.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://rl.szsharing.cn

C#:   list.Count;
来源：http://dy.nszjky.cn

[D07] 切片 / 取子数组
来源：http://zg.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://br.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nf.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://vh.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://bv.nszjky.cn

Java: list.subList(1, 4);
来源：http://cr.9csxet.cn

Go:   arr[1:4]
来源：http://js.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://cm.521024.cn

C#:   list.GetRange(1, 3);
来源：http://db.szsharing.cn

[D08] 合并两个数组
来源：http://eo.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ae.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://oe.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oa.chemitech.net.cn

TS:   [...a, ...b];
来源：http://hl.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kl.panjiajie.cn

Go:   append(a, b...)
来源：http://tl.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://fq.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://eh.yuexingan06.cn

[D09] 排序（升序）
来源：http://we.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jm.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://qz.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lw.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qw.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tw.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ua.haigaiapp.cn

Ruby: arr.sort
来源：http://ew.newstarts.cn

C#:   list.Sort();
来源：http://vl.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pb.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ri.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ji.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hp.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fh.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tg.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yt.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fr.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.jctech888.com.cn

[D11] 反转数组
来源：http://mb.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gd.nicolike.cn

PHP:  array_reverse($arr);
来源：http://xn.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kr.colortex.cn

TS:   [...arr].reverse();
来源：http://xp.hahajie.cn

Java: Collections.reverse(list);
来源：http://tb.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://wq.panjiajie.cn

Ruby: arr.reverse
来源：http://db.haigaiapp.cn

C#:   list.Reverse();
来源：http://xl.yuexingan06.cn

[D12] 查找元素下标
来源：http://no.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://rl.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vs.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wo.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yg.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://mp.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ee.9csxet.cn

C#:   list.IndexOf(x);
来源：http://dk.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://vh.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rh.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gr.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://jn.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://kk.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jf.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wz.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://on.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eh.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://fh.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://me.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rh.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ed.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ne.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jo.szxytkj.cn

Go:   // 手写循环
来源：http://yx.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wb.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://da.lnxyls.cn

[D15] 去重
来源：http://ng.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://og.nicolike.cn

PHP:  array_unique($arr);
来源：http://ih.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://eg.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://qb.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dr.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qc.muxihuayi.cn

Ruby: arr.uniq
来源：http://cs.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://uz.gzmigu.cn

[D16] 求和与平均值
来源：http://fv.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nj.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xd.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lk.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://js.yuexingan06.cn

Go:   // 手写循环累加
来源：http://nj.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sy.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://dk.lnxyls.cn

[D17] 最大值与最小值
来源：http://xo.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://px.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ip.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dp.hnjuh.cn

TS:   Math.max(...arr);
来源：http://th.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zy.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fp.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://pl.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://rv.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ii.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bq.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://wj.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://td.lnxyls.cn

TS:   nested.flat();
来源：http://xv.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oh.bjjhwx.cn

Go:   // 手写双层循环
来源：http://cy.lnxyls.cn

Ruby: nested.flatten
来源：http://tp.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rf.haigaiapp.cn

[D19] 按字段分组
来源：http://ao.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ep.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qj.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ui.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xw.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bt.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://dw.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ij.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ey.newstarts.cn

Py:   Counter(arr)
来源：http://ms.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://cr.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ww.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fl.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ce.hahajie.cn

Go:   // 手写 map[T]int
来源：http://xf.szxytkj.cn

Ruby: arr.tally
来源：http://oq.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://en.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://jf.521024.cn

Py:   x in arr
来源：http://mh.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://gv.gzmigu.cn

JS:   arr.includes(x)
来源：http://zm.muxihuayi.cn

TS:   arr.includes(x)
来源：http://lz.jctech888.com.cn

Java: list.contains(x)
来源：http://bj.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://pd.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://lt.bjjhwx.cn

C#:   list.Contains(x)
来源：http://hv.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://kz.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ae.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lu.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uj.gzmigu.cn

TS:   [...arr];
来源：http://nl.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://sk.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vy.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://bt.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://us.521024.cn

[D23] reduce 累积计算
来源：http://tu.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mx.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rt.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ri.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mi.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gj.hnjuh.cn

Go:   // 手写循环
来源：http://ff.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bd.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ua.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://lw.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ri.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xq.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rg.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sk.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zx.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gp.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zo.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ep.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://qd.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jm.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gk.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jo.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qu.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iu.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gt.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dy.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qr.panjiajie.cn

[D26] 数组转字符串
来源：http://ns.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://tf.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ph.muxihuayi.cn

JS:   arr.join(", ")
来源：http://uc.hahajie.cn

TS:   arr.join(", ")
来源：http://zp.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ad.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://pf.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://mm.asd995.cn

C#:   string.Join(", ", list)
来源：http://nd.szsharing.cn

================================================================================
来源：http://vm.nicolike.cn

E. 字符串处理
来源：http://ir.shtwfgs.cn

================================================================================
来源：http://vy.hahajie.cn

[E01] 拼接字符串
来源：http://vp.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://as.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ib.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vy.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sc.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xl.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ba.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rq.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vf.nicolike.cn

[E02] 重复字符串
来源：http://ee.szsharing.cn

Py:   "ab" * 3
来源：http://yj.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://qn.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://li.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://kg.nicolike.cn

Java: "ab".repeat(3)
来源：http://yi.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://rm.521024.cn

Ruby: "ab" * 3
来源：http://if.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nx.nicolike.cn

[E03] 截取子串
来源：http://vk.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://me.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jd.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://jp.gzmigu.cn

Java: s.substring(1, 4)
来源：http://df.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qe.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xw.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://en.gzmigu.cn

[E04] 查找子串位置
来源：http://qk.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://le.9csxet.cn

PHP:  strpos($s, "x");
来源：http://ct.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rc.szsharing.cn

TS:   s.indexOf("x")
来源：http://sy.jctech888.com.cn

Java: s.indexOf("x")
来源：http://pc.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://ng.shxzskj.cn

Ruby: s.index("x")
来源：http://bf.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://tw.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fo.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iv.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ck.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xe.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jr.hahajie.cn


<!-- 参考信息 -->