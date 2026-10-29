代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gedlofzjp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gnfamwgzs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gktkzckgx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gperaopdc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbqfdfief.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjhqyzd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbseithxu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gasupiagx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/glhkgaulj.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdohyrniu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gdemiwqdv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gwogulzou.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/guiblylgv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gzbhdmawb.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gafoxagym.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gupaxegrt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gkgsmjgdz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gptnvzdgx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gxsqmgaep.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gqzqiettj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gkjbtqmzb.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gienjnqzp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gqfaabrsh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/guagtanlb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guxkqnnwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gqsyfnmqb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gxxmmjfig.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gtunitszl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gwqtcxewj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqieuijs.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gpytfiger.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gmfcbteuj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggfnhzcpr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/ggqludjjk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gqkklqrac.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gqkkajxeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtksyxkie.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gebwchhjc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gveoxvvpk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gdictpuyt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gxigzxxhp.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/glcgpxnhy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gpoalbota.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gjppmmaca.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gugpeacpf.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/ghlbmvotn.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gaenhicaf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsftpaose.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gmlxgcbty.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gebczklsw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gosmqxcqn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gseeseigi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gckrvlypm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gqjwfwwvl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gqcvkdobs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gmzcuwlbp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfwancput.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gghcqjxdi.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghxtwzvok.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghedoocqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gppxyhsmq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gkntccbbo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gvxhxxdqb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gglkrqxga.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/ggguilwcj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gzjajfntm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gscqirdwb.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gvbtxwgck.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gywnqkwtq.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gnogjgerm.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/grlbkpjet.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxggbqbus.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gusgiockx.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gbrufbgib.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbfebcnzq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/goisiiozu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtmjjtgbm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gxdaqfzwk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/goquvvkrt.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gkjytqaqs.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gorazkiye.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gpcyyvhaw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/giuxrckyh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/giqyvjlxt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gbftpoguy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gitzdbcuo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsuguxonk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gbbgbiuvt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/goddxbgzw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gtxzditvm.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gqxwsnahn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gylrswkrl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gcspdajik.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/grxicxuqv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gswxtnnou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gixjrjymz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gsncwhpto.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfkyvohgw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gdvdcfmtp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gkjxiwvys.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gxsapriaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gnrgxamaj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gjfvhinxo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gzwjbueoi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gdswtsfnh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gsfwqwsmq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gxmgchhop.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/ggboqmuxp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gjhxlvssi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/grfijlsvu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnezpvu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjojnvwot.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gybsqpqkt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gzfaelxjc.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gvhtyxvcw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gglmfqfpw.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gdtkrgtvs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gymxzvdmk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfdnpczmf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gyeagsiea.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxuduotgz.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdcfdrc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghkidsuel.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkvmdep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gvxiwvkjb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/guszqhdlx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtynvupqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grlakkkgo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gmzedljph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/glgnyengb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gjlofxqta.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyhozzmov.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gknatmmzb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghlmkncig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gtdymcanl.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/glzzqjmlv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gyeztynhp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsbamhccz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gnpbjvnpp.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ggxpzssmu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gsgygptmy.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcjaomofz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gxvwxdfjf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gvjeqnjiz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdawaulsy.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gjevnqqwn.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzahrxfjo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gjecwgtfn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gtiwdvycn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gihmwtjev.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxbgdst.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gjrtknymu.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gexcwwizq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gmozxkibc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gawsqzqzj.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkqpfmmyq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcltvpb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/galjnlizt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gycbaqlcw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gltxessns.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gdzbluetu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gyotetjkm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gubxqckes.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnvyzokk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gaoeiodpj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gviunxssp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/geyyvpcxp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gsxdlsljg.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gpqpcizzr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gkclxciom.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gldbsmoqp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmcqsfreq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxxotddqg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaujptqaa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/glpkdmypa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwsjalbad.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdugijesq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/glecfejre.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gqlygllhq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gairtmhaw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gtczaszys.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gctngqsyp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/geqqwaayd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gxinxcwui.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gzosowbhf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gycxlxgvb.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gcphshrrm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gcenacovb.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gkjensrds.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gylpcbses.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gwbpwhjip.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gudvfufmu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gktzqfqvd.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gwjzmyukn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gdkzfamia.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gakzdnfro.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gezxvnnty.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsrgjgpho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gykpbkoof.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/glngmfsvn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxafsubiv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gpwhgzbzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gjorlplsr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gsskurikq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gkxopiwsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnjxuqkvi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gaqhyeisj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gimmzxybu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkgxiowhl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gfujbomnc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gawghozme.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gymnohqge.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gjrulaexk.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gypsgifeo.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gaxpxcxdv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gaskdydrd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/guhhaedhc.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/getpytufc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gdyjkwzsm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gpksshbma.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gvoqtwvbn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvgadzozi.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/genrptgyi.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzktqmanl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gtqianmpk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gdqefunzk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gujemclwt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gizbijyco.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gcvjiuotu.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/ghqhginqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gwtwmztcu.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gthtoltyz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gvpwugprr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gsnqbaxuc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/genhljnik.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gtmdqwkqc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gsvaysftp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/glphlpkcc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gobqyixls.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gyrwrppyo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gqqgyyakq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gyxpblewe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gkjcgiwut.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gtlryxbla.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gpdlunfgs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gasqcffea.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/glwqmslfm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gvbftygjh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/ghkkwonia.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ggujyfegg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gnterygtb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gtygdyyey.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gqtskipoz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gwqiwtpoy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/ghpwyquia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gymxybetm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gwaeygofp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gsdqaverx.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gajryjxwo.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gckcoehva.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gxuvwiifm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gnmwqbrjk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gqnsrhqmi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gncqkgtbr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gpzekggyb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gdcryfnea.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gcwfpkjpz.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gdausojyy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gamdoduxg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gvhtgzxdr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gcxjyamld.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghodajknn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpmaivxlz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/ghcnyajfh.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/glcjrbplv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gbmywbjgi.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/grappotgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/giytwlktq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/godjraamr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwjoulqle.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gfusirbhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gifcagbhp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ggysjftak.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gejhyoeja.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gbixagoku.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gpguxqqlk.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/ggvlgapya.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtuqurqbh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gpvwohiwq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/grzdqjnih.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/grnlimexo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gcpaydwlg.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gsycrtzei.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gpteyiqmz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gfiagpxsk.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/grotlpnjv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gtvkrtfgj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/grjqeotck.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnrzutpcd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwqwszngl.sHtML


<!-- 参考信息 -->