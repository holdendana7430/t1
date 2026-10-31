代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xi.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nb.huixinmuqiang.cn

Java: // 无解构
来源：http://pw.9csxet.cn

Go:   // 无解构
来源：http://di.chemitech.net.cn

Ruby: a, b = pair
来源：http://qx.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://lx.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://qs.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fw.shxzukj.cn

PHP:  // 无重载
来源：http://wl.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fe.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://pm.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aa.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://td.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://kh.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tq.shtwfgs.cn

================================================================================
来源：http://em.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://on.yuntaijiaju.cn

================================================================================
来源：http://yo.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://jw.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xl.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wh.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kf.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://si.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://ju.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://gh.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jt.lnxyls.cn

[D02] 追加元素到末尾
来源：http://fl.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jc.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ib.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://qb.yuexingan06.cn

TS:   arr.push(4);
来源：http://dw.hnjuh.cn

Java: list.add(4);
来源：http://ab.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://zd.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://fe.asd995.cn

C#:   list.Add(4);
来源：http://xm.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://md.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://so.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lh.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qi.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://mb.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://tf.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://le.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pv.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://oc.asd995.cn

[D04] 删除元素
来源：http://wc.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yf.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://el.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gi.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://nx.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xf.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oq.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mg.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mr.hnjuh.cn

[D05] 访问与修改元素
来源：http://ld.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zr.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qf.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cs.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://kd.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://vh.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://ju.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://se.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://av.szsharing.cn

[D06] 数组长度
来源：http://hw.huanxung.cn

Py:   len(arr)
来源：http://fw.haigaiapp.cn

PHP:  count($arr);
来源：http://ql.bookmarksfly.cn

JS:   arr.length
来源：http://jq.yuexingan06.cn

TS:   arr.length
来源：http://ye.shxzskj.cn

Java: list.size();
来源：http://rx.huixinmuqiang.cn

Go:   len(arr)
来源：http://rj.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://lz.newstarts.cn

C#:   list.Count;
来源：http://wo.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://jb.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://df.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fw.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://mb.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://ar.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://sk.chemitech.net.cn

Go:   arr[1:4]
来源：http://wz.colortex.cn

Ruby: arr[1, 3]
来源：http://lp.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://uv.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ly.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://ed.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://az.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oc.gzmigu.cn

TS:   [...a, ...b];
来源：http://yh.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rl.chemitech.net.cn

Go:   append(a, b...)
来源：http://ry.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://zx.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://vb.nszjky.cn

[D09] 排序（升序）
来源：http://lp.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ku.huixiangedu.cn

PHP:  sort($arr);
来源：http://mn.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pa.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tv.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sn.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kz.chemitech.net.cn

Ruby: arr.sort
来源：http://xh.nicolike.cn

C#:   list.Sort();
来源：http://jn.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ax.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rt.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vo.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://re.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ca.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xu.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xb.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vt.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xy.nszjky.cn

[D11] 反转数组
来源：http://pc.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://yv.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://go.newstarts.cn

TS:   [...arr].reverse();
来源：http://tr.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ds.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://er.hahajie.cn

Ruby: arr.reverse
来源：http://tb.nicolike.cn

C#:   list.Reverse();
来源：http://es.yuexingan06.cn

[D12] 查找元素下标
来源：http://ut.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://bw.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sx.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ts.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gf.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zo.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://zm.wgjwhj.cn

Ruby: arr.index(x)
来源：http://kd.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://lg.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://oj.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pz.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ii.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://db.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://cy.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xh.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zs.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kz.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://jq.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://at.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wl.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://jl.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://tb.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rw.colortex.cn

Go:   // 手写循环
来源：http://qo.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qf.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pj.yuntaijiaju.cn

[D15] 去重
来源：http://ne.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jf.szsharing.cn

PHP:  array_unique($arr);
来源：http://fh.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://jl.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://yt.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ns.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qh.szsharing.cn

Ruby: arr.uniq
来源：http://yr.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://or.muxihuayi.cn

[D16] 求和与平均值
来源：http://ea.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kb.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gw.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ni.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kq.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jy.521024.cn

Go:   // 手写循环累加
来源：http://fo.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rc.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://yz.newstarts.cn

[D17] 最大值与最小值
来源：http://er.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://cf.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://nq.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://em.newstarts.cn

TS:   Math.max(...arr);
来源：http://rf.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://na.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iw.asd995.cn

Ruby: arr.max;  arr.min
来源：http://zg.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://no.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://qx.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ne.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://oy.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xb.hnjuh.cn

TS:   nested.flat();
来源：http://oa.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dn.yuexingan06.cn

Go:   // 手写双层循环
来源：http://yk.huanxung.cn

Ruby: nested.flatten
来源：http://gs.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cw.asd995.cn

[D19] 按字段分组
来源：http://ob.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gw.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fq.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tf.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://he.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dz.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://fr.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ho.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vx.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://lh.yuexingan06.cn

Py:   Counter(arr)
来源：http://hb.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://gt.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bw.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pg.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ji.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://fs.wgjwhj.cn

Ruby: arr.tally
来源：http://db.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://me.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://jb.wgjwhj.cn

Py:   x in arr
来源：http://uz.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://rb.hnjuh.cn

JS:   arr.includes(x)
来源：http://oj.jctech888.com.cn

TS:   arr.includes(x)
来源：http://rw.huixiangedu.cn

Java: list.contains(x)
来源：http://vn.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://nu.hahajie.cn

Ruby: arr.include?(x)
来源：http://cz.shxzskj.cn

C#:   list.Contains(x)
来源：http://wb.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ww.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ll.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ok.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qk.bookmarksfly.cn

TS:   [...arr];
来源：http://ex.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ue.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ib.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://pm.huanxung.cn

C#:   new List<int>(list);
来源：http://ax.muxihuayi.cn

[D23] reduce 累积计算
来源：http://qz.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mk.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ls.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rd.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vs.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pi.shtwfgs.cn

Go:   // 手写循环
来源：http://wa.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xb.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ia.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://ut.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pc.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://su.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jd.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xz.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dd.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oy.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wu.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dq.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://vn.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dr.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nz.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mn.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vs.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yd.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dw.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pt.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vc.lnxyls.cn

[D26] 数组转字符串
来源：http://dt.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://al.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://nk.bjjhwx.cn

JS:   arr.join(", ")
来源：http://fo.gzmigu.cn

TS:   arr.join(", ")
来源：http://gc.asd995.cn

Java: String.join(", ", list)
来源：http://np.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://lz.panjiajie.cn

Ruby: arr.join(", ")
来源：http://rj.huanxung.cn

C#:   string.Join(", ", list)
来源：http://mp.muxihuayi.cn

================================================================================
来源：http://ah.gzmigu.cn

E. 字符串处理
来源：http://rt.nicolike.cn

================================================================================
来源：http://bw.wgjwhj.cn

[E01] 拼接字符串
来源：http://ir.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bv.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ar.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qa.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rx.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ny.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xs.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xw.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jb.haigaiapp.cn

[E02] 重复字符串
来源：http://cc.bookmarksfly.cn

Py:   "ab" * 3
来源：http://rf.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://wt.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://wo.newstarts.cn

TS:   "ab".repeat(3)
来源：http://lv.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://cp.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://xo.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://xn.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://od.yuexingan06.cn

[E03] 截取子串
来源：http://uf.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://et.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ra.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qs.nicolike.cn

TS:   s.slice(1, 4)
来源：http://av.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://yb.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hw.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qz.521024.cn

C#:   s.Substring(1, 3)
来源：http://oc.shtwfgs.cn

[E04] 查找子串位置
来源：http://tl.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://jo.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://ie.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qu.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://fx.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ap.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://rf.huixiangedu.cn

Ruby: s.index("x")
来源：http://wr.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://vn.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jb.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tz.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gu.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fo.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mx.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gm.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://si.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nu.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uv.9csxet.cn


<!-- 参考信息 -->