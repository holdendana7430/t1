代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zj.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://or.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://te.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://eq.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://cy.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ys.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://ty.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dk.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zf.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://bg.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://jq.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rp.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uk.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uk.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kz.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://gc.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oq.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qk.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://qb.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://xa.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ug.asd995.cn

Go:   // 手写循环
来源：http://mm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fe.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://so.521024.cn

[D15] 去重
来源：http://kz.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cq.shxzskj.cn

PHP:  array_unique($arr);
来源：http://is.colortex.cn

JS:   [...new Set(arr)]
来源：http://uo.szsharing.cn

TS:   [...new Set(arr)]
来源：http://up.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://he.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://we.bjjhwx.cn

Ruby: arr.uniq
来源：http://nm.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ye.yuexingan06.cn

[D16] 求和与平均值
来源：http://xy.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wi.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://my.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xz.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ey.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sc.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://ao.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mk.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://lk.huanxung.cn

[D17] 最大值与最小值
来源：http://re.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://oy.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://vo.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gf.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://oh.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rg.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fi.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://vm.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://by.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://zq.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jw.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://yx.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mm.gzmigu.cn

TS:   nested.flat();
来源：http://mf.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ak.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ko.521024.cn

Ruby: nested.flatten
来源：http://aq.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gn.panjiajie.cn

[D19] 按字段分组
来源：http://fg.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ez.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://az.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kt.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kx.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mu.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://xd.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rf.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://im.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://yr.szsharing.cn

Py:   Counter(arr)
来源：http://cj.hahajie.cn

PHP:  array_count_values($arr);
来源：http://ei.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zu.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wb.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://zh.huixinmuqiang.cn

Ruby: arr.tally
来源：http://yf.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lu.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://vr.wgjwhj.cn

Py:   x in arr
来源：http://et.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://ku.hnjuh.cn

JS:   arr.includes(x)
来源：http://we.shxzukj.cn

TS:   arr.includes(x)
来源：http://db.yuexingan06.cn

Java: list.contains(x)
来源：http://nb.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://vx.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://nj.hahajie.cn

C#:   list.Contains(x)
来源：http://wz.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://sw.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oo.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sf.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hn.bookmarksfly.cn

TS:   [...arr];
来源：http://we.nicolike.cn

Java: new ArrayList<>(list);
来源：http://dn.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://os.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://cz.panjiajie.cn

C#:   new List<int>(list);
来源：http://on.gzmigu.cn

[D23] reduce 累积计算
来源：http://mn.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pk.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qg.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sp.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iv.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zv.gzmigu.cn

Go:   // 手写循环
来源：http://en.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sm.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sp.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://sq.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gp.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tl.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jv.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tx.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cg.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zi.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jh.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mt.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://fp.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gi.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wp.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vg.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bc.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zi.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pi.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nj.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iq.shxzskj.cn

[D26] 数组转字符串
来源：http://nl.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://fh.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://yw.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://kc.colortex.cn

TS:   arr.join(", ")
来源：http://tw.bjjhwx.cn

Java: String.join(", ", list)
来源：http://qn.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://rt.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://ia.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://wq.lnxyls.cn

================================================================================
来源：http://uf.hnjuh.cn

E. 字符串处理
来源：http://jw.jianghongdianzi.cn

================================================================================
来源：http://wm.521024.cn

[E01] 拼接字符串
来源：http://ex.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jf.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ui.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jy.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://di.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sx.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sc.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sb.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zt.521024.cn

[E02] 重复字符串
来源：http://tj.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://uj.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://yn.asd995.cn

TS:   "ab".repeat(3)
来源：http://wd.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://qe.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://sw.muxihuayi.cn

Ruby: "ab" * 3
来源：http://id.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hp.huixiangedu.cn

[E03] 截取子串
来源：http://mt.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fq.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nj.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wq.nszjky.cn

TS:   s.slice(1, 4)
来源：http://fd.nszjky.cn

Java: s.substring(1, 4)
来源：http://jf.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://up.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ph.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://av.haigaiapp.cn

[E04] 查找子串位置
来源：http://zv.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://is.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://jw.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ml.hahajie.cn

TS:   s.indexOf("x")
来源：http://cs.chemitech.net.cn

Java: s.indexOf("x")
来源：http://kf.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://ps.panjiajie.cn

Ruby: s.index("x")
来源：http://be.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://mo.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ex.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hp.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jj.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tv.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://az.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jd.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ml.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ma.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lh.nszjky.cn

[E06] 替换子串
来源：http://ey.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qp.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://mm.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://xu.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ce.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bu.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iu.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://ur.lnxyls.cn

[E07] 按分隔符拆分
来源：http://od.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ny.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ez.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hy.gzmigu.cn

TS:   s.split(",")
来源：http://lg.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wd.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://go.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://kx.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wq.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://gd.szsharing.cn

Py:   ",".join(items)
来源：http://xp.shxzskj.cn

PHP:  implode(",", $items);
来源：http://cp.haigaiapp.cn

JS:   items.join(",")
来源：http://oc.521024.cn

TS:   items.join(",")
来源：http://wm.lnxyls.cn

Java: String.join(",", items)
来源：http://pw.asd995.cn

Go:   strings.Join(items, ",")
来源：http://sx.newstarts.cn

Ruby: items.join(",")
来源：http://zh.lnxyls.cn

C#:   string.Join(",", items)
来源：http://de.asd995.cn

[E09] 去除所有空白字符
来源：http://os.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ec.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dn.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://oj.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://zk.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://nt.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ye.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ts.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pj.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://uh.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://os.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://na.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://kw.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://rl.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://fs.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rw.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ko.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gr.wgjwhj.cn

[E11] 反转字符串
来源：http://tm.shxzskj.cn

Py:   s[::-1]
来源：http://mg.lnxyls.cn

PHP:  strrev($s);
来源：http://hp.521024.cn

JS:   [...s].reverse().join("")
来源：http://uk.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://af.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://my.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tk.yuexingan06.cn

Ruby: s.reverse
来源：http://sr.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fo.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ql.shxzukj.cn

Py:   s.count("a")
来源：http://se.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://sv.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://dt.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://co.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wr.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ww.muxihuayi.cn

Ruby: s.count("a")
来源：http://dv.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://zb.bjjhwx.cn

[E13] 逐字符遍历
来源：http://pe.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://pn.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pi.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eo.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qv.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uf.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nw.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fm.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ih.nszjky.cn

[E14] URL 编码与 Base64
来源：http://jt.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uu.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jg.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rb.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wv.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sn.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gw.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kz.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ml.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://af.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yc.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bi.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vs.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wa.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mi.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mh.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jr.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://br.521024.cn

[E16] 数字千分位
来源：http://vz.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://hr.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://ub.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zq.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ll.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vp.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ae.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ho.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://gg.chemitech.net.cn

[E17] 首字母大写
来源：http://mu.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zz.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cc.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qt.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cb.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qx.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lk.haigaiapp.cn

Ruby: s.capitalize
来源：http://yw.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oq.9csxet.cn

[E18] 模板占位符替换
来源：http://ic.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kj.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://no.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jk.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ki.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ke.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kj.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qu.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://py.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://ji.szsharing.cn

Py:   s.splitlines()
来源：http://sc.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wt.newstarts.cn


<!-- 参考信息 -->