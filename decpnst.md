代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gn.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xc.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://wc.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://fg.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://up.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pb.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zv.bjjhwx.cn

[D06] 数组长度
来源：http://xw.shtwfgs.cn

Py:   len(arr)
来源：http://nq.jctech888.com.cn

PHP:  count($arr);
来源：http://nd.yuexingan06.cn

JS:   arr.length
来源：http://no.asd995.cn

TS:   arr.length
来源：http://ym.jctech888.com.cn

Java: list.size();
来源：http://xk.521024.cn

Go:   len(arr)
来源：http://iy.nicolike.cn

Ruby: arr.length; arr.size
来源：http://xt.shtwfgs.cn

C#:   list.Count;
来源：http://tq.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://vz.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yk.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bw.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ve.colortex.cn

TS:   arr.slice(1, 4);
来源：http://xv.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://bp.bjjhwx.cn

Go:   arr[1:4]
来源：http://ej.szxytkj.cn

Ruby: arr[1, 3]
来源：http://uc.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://fx.bjjhwx.cn

[D08] 合并两个数组
来源：http://dq.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://pp.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://pm.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ul.newstarts.cn

TS:   [...a, ...b];
来源：http://ff.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://el.huixiangedu.cn

Go:   append(a, b...)
来源：http://kv.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://jf.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://kl.521024.cn

[D09] 排序（升序）
来源：http://ik.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.bookmarksfly.cn

PHP:  sort($arr);
来源：http://vb.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rd.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iz.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yf.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zs.nszjky.cn

Ruby: arr.sort
来源：http://vh.wgjwhj.cn

C#:   list.Sort();
来源：http://no.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rz.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yz.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qv.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://so.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://po.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qc.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rv.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yk.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uo.chemitech.net.cn

[D11] 反转数组
来源：http://jo.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://au.newstarts.cn

PHP:  array_reverse($arr);
来源：http://nx.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iq.hnjuh.cn

TS:   [...arr].reverse();
来源：http://rl.hnjuh.cn

Java: Collections.reverse(list);
来源：http://mx.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ow.9csxet.cn

Ruby: arr.reverse
来源：http://om.nszjky.cn

C#:   list.Reverse();
来源：http://zl.hnjuh.cn

[D12] 查找元素下标
来源：http://vm.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://xe.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zf.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ow.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wd.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://da.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ec.haigaiapp.cn

Ruby: arr.index(x)
来源：http://dd.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://jt.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://ai.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://it.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tu.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://yi.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://iu.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xv.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wb.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fr.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nv.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://lp.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://na.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rr.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ju.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://hg.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lp.muxihuayi.cn

Go:   // 手写循环
来源：http://dr.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ji.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wk.shxzskj.cn

[D15] 去重
来源：http://ce.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jk.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://uv.9csxet.cn

JS:   [...new Set(arr)]
来源：http://od.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://pe.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://el.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lm.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://fe.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://wb.gzmigu.cn

[D16] 求和与平均值
来源：http://zr.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://id.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fl.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ne.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dr.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uy.shxzskj.cn

Go:   // 手写循环累加
来源：http://wh.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qg.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://tm.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ii.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://jw.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://ov.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kc.huanxung.cn

TS:   Math.max(...arr);
来源：http://na.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qd.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ql.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://oh.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://mr.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://uo.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fy.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://rj.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xp.lnxyls.cn

TS:   nested.flat();
来源：http://qj.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pi.szsharing.cn

Go:   // 手写双层循环
来源：http://gr.bookmarksfly.cn

Ruby: nested.flatten
来源：http://jr.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mp.panjiajie.cn

[D19] 按字段分组
来源：http://ov.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wn.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sv.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qv.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ap.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iw.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://bs.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qz.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://co.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://rt.chemitech.net.cn

Py:   Counter(arr)
来源：http://vl.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://re.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nt.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uv.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://lt.gzmigu.cn

Ruby: arr.tally
来源：http://eo.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mn.9csxet.cn

[D21] 判断是否包含某元素
来源：http://tp.newstarts.cn

Py:   x in arr
来源：http://ku.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://kx.szxytkj.cn

JS:   arr.includes(x)
来源：http://ve.shtwfgs.cn

TS:   arr.includes(x)
来源：http://ko.huanxung.cn

Java: list.contains(x)
来源：http://mk.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://bd.lnxyls.cn

Ruby: arr.include?(x)
来源：http://tt.shtwfgs.cn

C#:   list.Contains(x)
来源：http://xv.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://cu.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vn.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yd.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fs.521024.cn

TS:   [...arr];
来源：http://pn.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://on.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://at.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ww.521024.cn

C#:   new List<int>(list);
来源：http://ki.bjjhwx.cn

[D23] reduce 累积计算
来源：http://qd.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://av.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://im.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hd.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vz.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wq.nszjky.cn

Go:   // 手写循环
来源：http://tb.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jt.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://kg.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qs.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zk.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ga.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ko.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hw.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qt.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://az.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lm.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ts.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mp.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mo.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wy.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hc.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bc.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://si.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ym.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tz.gzmigu.cn

[D26] 数组转字符串
来源：http://sh.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://fn.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ud.shxzskj.cn

JS:   arr.join(", ")
来源：http://sd.muxihuayi.cn

TS:   arr.join(", ")
来源：http://ck.521024.cn

Java: String.join(", ", list)
来源：http://tz.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://mk.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://kr.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://uf.9csxet.cn

================================================================================
来源：http://np.hnjuh.cn

E. 字符串处理
来源：http://rx.wgjwhj.cn

================================================================================
来源：http://gl.chemitech.net.cn

[E01] 拼接字符串
来源：http://mb.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qy.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vj.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jv.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://he.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bs.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kq.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xy.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://os.gzmigu.cn

[E02] 重复字符串
来源：http://fu.newstarts.cn

Py:   "ab" * 3
来源：http://me.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://wg.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://vi.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://jb.shxzskj.cn

Java: "ab".repeat(3)
来源：http://bd.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://dq.hnjuh.cn

Ruby: "ab" * 3
来源：http://tu.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wo.szxytkj.cn

[E03] 截取子串
来源：http://qi.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qc.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wv.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qh.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://tu.newstarts.cn

Java: s.substring(1, 4)
来源：http://ft.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xu.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jl.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://kq.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://tj.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://tz.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://hn.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kv.asd995.cn

TS:   s.indexOf("x")
来源：http://vk.lnxyls.cn

Java: s.indexOf("x")
来源：http://gs.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://ec.shtwfgs.cn

Ruby: s.index("x")
来源：http://hr.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://gz.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ap.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pw.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yf.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ii.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vy.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ml.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tq.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ze.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kk.huixinmuqiang.cn

[E06] 替换子串
来源：http://xd.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mu.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://nd.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kp.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://cf.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qn.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vd.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bp.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://sk.hnjuh.cn

[E07] 按分隔符拆分
来源：http://xa.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sf.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ty.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://he.huanxung.cn

TS:   s.split(",")
来源：http://bc.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eg.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yr.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://dj.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gs.colortex.cn

[E08] 数组按分隔符合并
来源：http://ze.bjjhwx.cn

Py:   ",".join(items)
来源：http://hi.521024.cn

PHP:  implode(",", $items);
来源：http://pg.nicolike.cn

JS:   items.join(",")
来源：http://ck.nicolike.cn

TS:   items.join(",")
来源：http://hh.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ga.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://ws.huanxung.cn

Ruby: items.join(",")
来源：http://dq.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://rf.asd995.cn

[E09] 去除所有空白字符
来源：http://nl.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rc.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kb.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://qx.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://eo.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://dd.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ed.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aj.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://an.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://oq.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tj.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wj.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://ar.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://zh.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ot.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yo.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bd.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ga.jianghongdianzi.cn

[E11] 反转字符串
来源：http://qa.panjiajie.cn

Py:   s[::-1]
来源：http://ne.chemitech.net.cn

PHP:  strrev($s);
来源：http://ak.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://kj.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://hy.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ml.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://um.newstarts.cn

Ruby: s.reverse
来源：http://kp.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yy.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://px.huixinmuqiang.cn

Py:   s.count("a")
来源：http://jo.lnxyls.cn


<!-- 参考信息 -->