代发 wailian999

TS:   [...arr].reverse();
来源：http://to.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://tl.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://vz.panjiajie.cn

Ruby: arr.reverse
来源：http://ld.nszjky.cn

C#:   list.Reverse();
来源：http://zs.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://me.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://lo.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://we.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mw.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://my.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ft.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://tb.szxytkj.cn

Ruby: arr.index(x)
来源：http://pv.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://gw.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://bl.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ug.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zq.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://kc.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://fa.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tm.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fe.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://up.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gf.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ay.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qa.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ck.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://ys.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://uy.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jm.huixiangedu.cn

Go:   // 手写循环
来源：http://nf.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://an.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kq.szxytkj.cn

[D15] 去重
来源：http://ft.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oj.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://zg.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://vw.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://vg.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ew.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yy.panjiajie.cn

Ruby: arr.uniq
来源：http://mu.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://tf.haigaiapp.cn

[D16] 求和与平均值
来源：http://fk.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pg.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gx.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://io.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hv.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vq.hahajie.cn

Go:   // 手写循环累加
来源：http://gi.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cw.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://bs.bjjhwx.cn

[D17] 最大值与最小值
来源：http://tb.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://vc.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://vc.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ns.newstarts.cn

TS:   Math.max(...arr);
来源：http://qi.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://od.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ol.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://ks.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://ro.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ch.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lj.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://ek.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ab.muxihuayi.cn

TS:   nested.flat();
来源：http://ba.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jo.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://sa.shtwfgs.cn

Ruby: nested.flatten
来源：http://wv.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mv.huixiangedu.cn

[D19] 按字段分组
来源：http://nc.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ib.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zd.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rs.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hl.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jf.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://ck.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ko.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oe.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://yg.newstarts.cn

Py:   Counter(arr)
来源：http://zv.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://an.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ad.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nz.hahajie.cn

Go:   // 手写 map[T]int
来源：http://yq.wgjwhj.cn

Ruby: arr.tally
来源：http://og.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jh.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://tx.huixinmuqiang.cn

Py:   x in arr
来源：http://jf.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://fs.szsharing.cn

JS:   arr.includes(x)
来源：http://yx.chemitech.net.cn

TS:   arr.includes(x)
来源：http://pe.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ef.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://zd.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://ns.szxytkj.cn

C#:   list.Contains(x)
来源：http://bz.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://yf.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pt.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sc.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gx.shxzukj.cn

TS:   [...arr];
来源：http://hw.521024.cn

Java: new ArrayList<>(list);
来源：http://zu.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gu.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://kv.huixiangedu.cn

C#:   new List<int>(list);
来源：http://rg.shxzukj.cn

[D23] reduce 累积计算
来源：http://dk.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aj.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lw.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vc.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ex.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kr.newstarts.cn

Go:   // 手写循环
来源：http://ng.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jd.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vu.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://cb.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tz.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zr.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aj.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://br.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ql.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vv.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jl.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ke.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://gh.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://in.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gf.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dq.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ca.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yo.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ok.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gu.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ef.asd995.cn

[D26] 数组转字符串
来源：http://oq.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://qm.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ug.9csxet.cn

JS:   arr.join(", ")
来源：http://ee.muxihuayi.cn

TS:   arr.join(", ")
来源：http://dn.colortex.cn

Java: String.join(", ", list)
来源：http://gf.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://ok.hnjuh.cn

Ruby: arr.join(", ")
来源：http://xv.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://sp.wgjwhj.cn

================================================================================
来源：http://rp.panjiajie.cn

E. 字符串处理
来源：http://in.jctech888.com.cn

================================================================================
来源：http://sf.bookmarksfly.cn

[E01] 拼接字符串
来源：http://sn.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ia.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://km.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fw.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dz.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mn.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ef.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://or.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pm.yuntaijiaju.cn

[E02] 重复字符串
来源：http://gb.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://pc.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://xq.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://mq.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://xy.nicolike.cn

Java: "ab".repeat(3)
来源：http://ep.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://fa.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ly.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bt.panjiajie.cn

[E03] 截取子串
来源：http://ck.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ay.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qw.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pg.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://in.huanxung.cn

Java: s.substring(1, 4)
来源：http://tt.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://et.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ju.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://kx.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://pt.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://vn.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://nf.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wf.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://yg.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://vn.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://yz.huanxung.cn

Ruby: s.index("x")
来源：http://hj.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://lw.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uu.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ea.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hf.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qo.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eu.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kh.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ot.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zc.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wn.huixinmuqiang.cn

[E06] 替换子串
来源：http://wa.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yc.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://pk.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gy.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://dp.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bz.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ht.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ta.colortex.cn

C#:   s.Replace("a", "b")
来源：http://wm.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://wo.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://je.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fp.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rw.521024.cn

TS:   s.split(",")
来源：http://gu.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wh.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lt.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://ql.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kn.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ds.hahajie.cn

Py:   ",".join(items)
来源：http://xt.szsharing.cn

PHP:  implode(",", $items);
来源：http://xv.jianghongdianzi.cn

JS:   items.join(",")
来源：http://mz.huanxung.cn

TS:   items.join(",")
来源：http://uh.hahajie.cn

Java: String.join(",", items)
来源：http://ds.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://mo.nicolike.cn

Ruby: items.join(",")
来源：http://zo.asd995.cn

C#:   string.Join(",", items)
来源：http://ks.hahajie.cn

[E09] 去除所有空白字符
来源：http://os.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xp.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rx.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://tx.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ii.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://jj.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bm.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cr.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jo.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://xy.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bn.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ky.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://ns.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://jk.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://gy.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ag.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nc.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xd.9csxet.cn

[E11] 反转字符串
来源：http://hs.nicolike.cn

Py:   s[::-1]
来源：http://ou.yuexingan06.cn

PHP:  strrev($s);
来源：http://at.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://mq.colortex.cn

TS:   [...s].reverse().join("")
来源：http://js.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fa.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://if.wgjwhj.cn

Ruby: s.reverse
来源：http://pv.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fl.hahajie.cn

[E12] 统计某字符出现次数
来源：http://lt.colortex.cn

Py:   s.count("a")
来源：http://wq.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://fs.nszjky.cn

JS:   s.split("a").length - 1
来源：http://xo.newstarts.cn

TS:   s.split("a").length - 1
来源：http://rx.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hf.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://ui.huixiangedu.cn

Ruby: s.count("a")
来源：http://ac.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ix.newstarts.cn

[E13] 逐字符遍历
来源：http://zk.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://pb.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cm.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yx.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ic.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tu.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://li.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://re.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ev.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://rp.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yd.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wu.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ur.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uj.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uw.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ac.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oi.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://pj.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ct.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ow.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wd.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vr.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fj.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xl.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ss.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rm.hnjuh.cn

[E16] 数字千分位
来源：http://uc.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://xw.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://dz.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rl.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vf.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://po.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xb.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gj.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ij.lnxyls.cn

[E17] 首字母大写
来源：http://zn.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://am.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ru.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wc.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kk.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cm.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://di.nicolike.cn

Ruby: s.capitalize
来源：http://ox.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ac.nicolike.cn

[E18] 模板占位符替换
来源：http://vm.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://by.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ng.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fh.colortex.cn


<!-- 参考信息 -->