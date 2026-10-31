代发 wailian999

[D11] 反转数组
来源：http://hu.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ne.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://gn.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://te.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://xl.gzmigu.cn

Java: Collections.reverse(list);
来源：http://rq.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://yw.newstarts.cn

Ruby: arr.reverse
来源：http://wb.shxzukj.cn

C#:   list.Reverse();
来源：http://pj.nszjky.cn

[D12] 查找元素下标
来源：http://nl.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://sn.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yw.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jd.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://cb.chemitech.net.cn

Ruby: arr.index(x)
来源：http://rd.9csxet.cn

C#:   list.IndexOf(x);
来源：http://hv.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://at.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://an.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ud.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://ae.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://yu.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hd.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://by.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uq.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cs.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://vz.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hs.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ui.521024.cn

TS:   arr.map(x => x * 2)
来源：http://io.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jz.gzmigu.cn

Go:   // 手写循环
来源：http://sr.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aa.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ik.gzmigu.cn

[D15] 去重
来源：http://ty.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xv.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://kx.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://du.szsharing.cn

TS:   [...new Set(arr)]
来源：http://yl.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hd.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nq.shtwfgs.cn

Ruby: arr.uniq
来源：http://ir.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://yh.nicolike.cn

[D16] 求和与平均值
来源：http://dp.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hc.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dn.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bi.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lx.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ye.szsharing.cn

Go:   // 手写循环累加
来源：http://fw.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yt.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://eh.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://hl.colortex.cn

Py:   max(arr);  min(arr)
来源：http://qh.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://sp.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mi.9csxet.cn

TS:   Math.max(...arr);
来源：http://gc.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cl.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ts.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://hh.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://yo.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://xj.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://am.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://df.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://um.muxihuayi.cn

TS:   nested.flat();
来源：http://rd.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sq.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://ox.jctech888.com.cn

Ruby: nested.flatten
来源：http://px.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dr.colortex.cn

[D19] 按字段分组
来源：http://ss.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qe.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gm.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uw.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lu.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jt.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://xa.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vf.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pa.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://jx.hnjuh.cn

Py:   Counter(arr)
来源：http://py.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://be.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zm.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://it.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://uv.szsharing.cn

Ruby: arr.tally
来源：http://qv.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xu.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://af.shtwfgs.cn

Py:   x in arr
来源：http://xm.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://dh.huanxung.cn

JS:   arr.includes(x)
来源：http://ll.muxihuayi.cn

TS:   arr.includes(x)
来源：http://fc.9csxet.cn

Java: list.contains(x)
来源：http://yr.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://fe.521024.cn

Ruby: arr.include?(x)
来源：http://bg.szsharing.cn

C#:   list.Contains(x)
来源：http://fs.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://nj.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vt.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iw.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://up.jctech888.com.cn

TS:   [...arr];
来源：http://vu.newstarts.cn

Java: new ArrayList<>(list);
来源：http://qy.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fi.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://is.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://te.jctech888.com.cn

[D23] reduce 累积计算
来源：http://od.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ti.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://er.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hi.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tc.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gz.521024.cn

Go:   // 手写循环
来源：http://ju.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://op.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qr.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://um.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dq.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://th.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://br.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ew.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ow.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nw.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tb.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qg.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://bo.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://it.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ko.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zu.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ho.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tt.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ku.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qj.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fq.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://hw.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://dl.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://ef.nszjky.cn

JS:   arr.join(", ")
来源：http://bj.szsharing.cn

TS:   arr.join(", ")
来源：http://uo.9csxet.cn

Java: String.join(", ", list)
来源：http://md.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ch.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://mi.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://me.hnjuh.cn

================================================================================
来源：http://tr.shtwfgs.cn

E. 字符串处理
来源：http://ez.hahajie.cn

================================================================================
来源：http://kh.hnjuh.cn

[E01] 拼接字符串
来源：http://jj.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aj.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mt.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uc.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mx.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://va.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lv.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ro.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ma.colortex.cn

[E02] 重复字符串
来源：http://ga.huixiangedu.cn

Py:   "ab" * 3
来源：http://oq.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://yo.szsharing.cn

JS:   "ab".repeat(3)
来源：http://dm.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://nq.shxzukj.cn

Java: "ab".repeat(3)
来源：http://hf.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://zg.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://zl.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gr.nicolike.cn

[E03] 截取子串
来源：http://ia.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lx.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vm.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bn.szsharing.cn

TS:   s.slice(1, 4)
来源：http://xs.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://mh.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uh.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rc.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://dg.colortex.cn

[E04] 查找子串位置
来源：http://xq.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://va.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://op.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wz.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://aw.yuexingan06.cn

Java: s.indexOf("x")
来源：http://gl.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://or.hahajie.cn

Ruby: s.index("x")
来源：http://lg.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://fc.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qd.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ph.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kz.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://id.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kl.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dy.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jk.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://np.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://il.lnxyls.cn

[E06] 替换子串
来源：http://fc.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uq.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://xl.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ku.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://ey.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mw.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ps.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ni.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://mf.asd995.cn

[E07] 按分隔符拆分
来源：http://yl.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vz.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ox.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cb.huixinmuqiang.cn

TS:   s.split(",")
来源：http://fb.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cf.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ls.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://xi.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zc.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://aq.shtwfgs.cn

Py:   ",".join(items)
来源：http://xj.521024.cn

PHP:  implode(",", $items);
来源：http://fk.9csxet.cn

JS:   items.join(",")
来源：http://hz.haigaiapp.cn

TS:   items.join(",")
来源：http://qr.yuexingan06.cn

Java: String.join(",", items)
来源：http://jg.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://po.muxihuayi.cn

Ruby: items.join(",")
来源：http://og.lnxyls.cn

C#:   string.Join(",", items)
来源：http://my.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://hq.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sd.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://el.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://ds.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://pu.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://mw.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ob.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yz.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ct.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://fi.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zm.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jt.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://hy.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://uy.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ea.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tb.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cq.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vf.shxzskj.cn

[E11] 反转字符串
来源：http://fj.szsharing.cn

Py:   s[::-1]
来源：http://oo.gzmigu.cn

PHP:  strrev($s);
来源：http://eg.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://sj.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://js.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zd.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tm.gzmigu.cn

Ruby: s.reverse
来源：http://mj.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cj.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://zu.9csxet.cn

Py:   s.count("a")
来源：http://uc.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://bj.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://qf.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://cp.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://os.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://kj.jctech888.com.cn

Ruby: s.count("a")
来源：http://qz.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://rj.9csxet.cn

[E13] 逐字符遍历
来源：http://nc.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://hb.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bg.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cn.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cs.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nc.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ae.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://od.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gm.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://gs.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wv.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fq.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tq.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sh.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pe.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fv.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qz.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nc.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://rf.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kn.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sd.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kz.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gx.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ng.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://il.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ko.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yv.9csxet.cn

[E16] 数字千分位
来源：http://jf.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://dx.panjiajie.cn

PHP:  number_format(1234567);
来源：http://zg.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dv.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ju.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tf.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://an.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jn.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://hi.szsharing.cn

[E17] 首字母大写
来源：http://nv.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ae.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yn.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vb.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ig.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://me.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zx.muxihuayi.cn

Ruby: s.capitalize
来源：http://ry.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tn.huanxung.cn


<!-- 参考信息 -->