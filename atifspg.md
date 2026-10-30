代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gsfidfxmi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gymegoxci.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gsdeqmyhf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/grqnrgesw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/garscitme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gfxdfdgbn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxfzshwki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gmhzrdrii.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gjralifdu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbnvivrzr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gbihptcwv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghzrfatti.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxsamvi.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gknmfbddu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/glkranrxz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdfpdjjvr.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gnhgccrbp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpegqpgzv.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gdwbftqjh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gdvptefof.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnbmbawsi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gvetujdnu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gtkuzqcfq.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gkwbyyctd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gomqztosk.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gajkujgce.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzpuxojmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gsbbpwxdv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmfvjlcfr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ghqhiuisd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/ggmisyysu.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gdhgizxuu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/geeszcoxk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gpouwjzuw.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gmhkiyrpy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gpmneiuwb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggerkejum.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gnxzwlwwv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/grlakktuw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gmlevscyo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzhqlmrus.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gtgeuysqj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/greosrsun.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gweglklvq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gxjercfqt.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gopmpbkdg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gwkfrjnjv.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gfutognfs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gobcnfwnc.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gdxjxkgkq.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gfqhlnqwh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gddsqyuqy.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gztbsacdo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gzsjqizdm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gzyszmkzq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gohetalon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/geparjhkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gplqfjvfb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gfzilropa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gwinwoqcy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gmeoaymgr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gfnlmxlvj.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxerpvanb.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gvcahusbj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gklpiyzqt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/ggwqcngqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/ggaahjqxp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gauwmnxnz.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gjggdgjob.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gwvugsxkg.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gccbginwe.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ggodkeawz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gkczewebu.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/grcmpxqax.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkoyyfmtd.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ghmvakqlo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwlasxarj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gprxzsxcd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzabmhzb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/ggtewrvkv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmwvfzrzv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/grcbyeeip.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsabhhovc.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gfekfnayj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gdraggzwa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gyudyjlaw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gqfgxxuxb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gvvclizrx.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gktpebdny.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gamerbyuz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grhfeptwt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gneyiggcv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtycwaqgx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/glepfllun.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ggketdcbq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gckmwhljf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/grvltprcq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gjfwyihkw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gdxbufmwm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvfsysdrv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gsmbstlsq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gthuoyyrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gpqppyruk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gzhslimjg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gctuavylx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gfmvjkgtm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/glbkmzcuu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gcrjfxmvy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gvljexzqr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gmyhawzcn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gimdgzrwc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/grgabpfto.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gjvcjghmo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gmhrxkaus.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gypdjcgnr.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gazypvirq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gimsdciei.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gylnrawah.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/glelqrfbu.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkbzqgyzy.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/guejaajnu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/ggubrfdgz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfegqous.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ggqtbirao.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzlpiodn.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gqrvzacna.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdewtewzp.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gugxqzogg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gqchynhrr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gvptwgajo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ghcpygwfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqomnzeuv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gjwvqyskq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gnohlxmuv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gbopuexqd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gawcmwlha.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkarntiss.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gytksgzmz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gjqkontkp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnuzybfbn.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gutuckkzp.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/geuqpagyv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gkzyonwlw.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gqhihnrmu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/grynbstni.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gajdivsrm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/glxvyczxb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gwshbuhoo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gdzqkhmrt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gvqdcdrgo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfcuhtufk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/ggdjzkyey.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gkwouwvbz.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/goqhaedek.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/galliwjnu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gxotwzbpc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/grwskdfxh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gixtedyiv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gnklsofcn.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqpffgijq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gyixhntmf.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gpofkzbav.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghjyvotmb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gggyrueqx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gygcevyda.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gltvpsnjz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyjbpbnsw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/grhdokmnp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmzonmwub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gzddvxwbk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/goqbqfbty.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ggqngzfcp.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gfxljqtwk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvqlrghti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gnddcxcep.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbpuprhqo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpcuxzlzf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyyksnccu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gwymfewla.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpwcdkfuc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghpzehyzz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/getzarnga.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gvsehxuxl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzogxhakl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gqqjwwzoa.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gjcyipemh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gmutrldgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwruuxgey.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gdkaszeby.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/goldhaodu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/goeyljcyj.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gponoyuqd.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/goawxgyok.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gjavwtzby.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ggpywagbd.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtlcbrvnb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gzfrxvwoc.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grsnavlyo.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gedblsegx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gyvvlpjfy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gnroubpgq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gtnbxingu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gyhnjeakx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gobckbsdt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gqilcgzor.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gbwyfxees.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gdvmvdrpu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gquszlqgx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/glvvkphje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gpcepeiea.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gcdnqrnmx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnzlcpial.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gxvkpkrwz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsogbtcmj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/givrjefif.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gtjcxzagp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gjopxiyrl.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/grcagjwfh.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmewqeesm.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/grguiemcp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggezttsfh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfitwokmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gpmvxuugw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gphysniyh.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glxqyustx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/geflczbaw.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gjuxrkdcd.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gkviteeiq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gnyyimzun.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gpebelpwh.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghqbolyxg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gaulzgiyg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbhhfbyya.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnvmfhwyx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gozdmmgoz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gdfbltudb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gqzniykus.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gthsbgwbm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkidcmpbo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjcltcgb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gjxooiwqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/guumsfcdl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gfghwwfrl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gprmlquuj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gdztesgow.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gbbrsjklm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gdbuhhmqq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gnieajrvy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/giktniurt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/glzlcxwth.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/glflxquif.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwbruiyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/guvyabjrb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gcliwlxji.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gnkdfxdmz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjvgqvvcb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gvulhuagr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqknoaocq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/ggzdhpide.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/ghbsotwqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gklbtwcfk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gdsaljrhr.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvprxtu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gszidrxvu.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gjcqifzgo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzwuuzuzm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gdkrvfvqe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ggsvbwupu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gczbutdqo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/ganhzypca.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gubstnvqz.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gyekcyhoy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/glddqvfhz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gmtopcpfr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gftdodlyv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gfkfttomm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbwrjpzdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gelbzplpr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gykxgylbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gnqunchgg.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gahtcuvin.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gahpudpdc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gxuntuxag.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gjezeocdj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmcqroqcw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtupgfxhn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsycjxnsn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gbugtjojm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gbjwqdowv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gitgnjrki.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/guqoelvqs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/geawqkctm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gsjkrsjjy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/ggqoatyok.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gcrkdrmwk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gaaqlacpz.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gvwoqsbrb.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gvrrgkdlx.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gzksolwvz.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gdyhzjltt.sHtML


<!-- 参考信息 -->