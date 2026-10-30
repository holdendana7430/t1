代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gusrrhtjq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gxkfqnibt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gvxhlovgs.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gxuxfxfzo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gnzxgshwa.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/grzuxgvqo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdcgmnphd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwpvpjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gllbjoxfu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqkpyjwmu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gkrjeivgr.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gqgmhhaif.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/ggrnkrfwa.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gnpfixjlq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gapucqipi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gazgreqjk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqimuas.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ggskxvdvk.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/ggamuuwud.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gbbevgapf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyqjkzqge.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gmsrpjbzr.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gmefzfjoy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gxplugquv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gnenwqhob.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/grlrfushk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gnykbahdn.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/ghuzhvoqe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gigbmlhub.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gztabzzqn.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gkosfuymb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvlxijkad.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gbdbmcpsg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gwphkzksl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gbusztwom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gfcnwmqnx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gisulctfw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gyoythuod.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gtpozxfti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/ghpxkwust.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gnjhzbryj.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ggzotrery.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbilpxxil.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gawadzmew.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqyzxtlif.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gjuueaacl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/guvakcgxu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gaqvgkabs.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gimrppfid.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gynhfnqzg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gnelscwyv.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/ginkkjrbu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdareypvr.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gudnxpufk.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghqunwvfd.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqtywhkib.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gebsrctmf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gryyxrkku.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gixdxmnkl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gaeafsgrj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmetryyum.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/ghjwbzujy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gslbnhedg.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gffkticbu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gnigpwzfk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gfcqqtein.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gchgwhydh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gudkawzbf.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/goinueeak.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gyhgqpflu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqjkzfuvg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxtzcmgfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gedffiejm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/genpjpszr.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gadbwcube.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gnbvccxzi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gzteoybgr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gmgrlytug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gjakcahme.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gswbllwxp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcridwqic.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwbthbgom.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gocbqgonk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gahxmkwrm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgzezywa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/ggxuopnip.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gwefhuhvq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gduiuonsy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ghnolhyzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gqntncdqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gcixntldw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gijnzjedo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gcwesxrkz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/ggbyobyju.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkpjnviwr.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gelsutvbz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbrdxknet.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gujzvhzlc.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gxcyetrzk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gfgnjtuiy.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gyrmownsb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gvxoeetmf.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gnirzefay.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gdkguixqq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gealpopad.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gyetvsvix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giaioaebq.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gpvipxcgz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvpameb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gwjpjbaeu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gutjgylsv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grqatcnhw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gpmoxadzy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gduhdwirh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gowjxopou.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/geijuugbz.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gnxsyskba.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gjacavctl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gwywswzpf.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwevatzix.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gstxtcrfn.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gpbfiglsu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gnmchkhkn.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gtymhbtas.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gzywscktq.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gdehzavbk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gpmdztcpn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ggyvilrff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gltbkgoox.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gyigrfnxv.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/guppxqnxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/giyxyvjhx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gzucozyeq.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gqqqozkzl.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gcaqzfvos.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/glcvohigw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gnzyjtpjj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gcwzzburr.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gvcrfnnma.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gpkfyzvnw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxxdxttdn.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gmgbpmbjv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/guclwqoai.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gtdufaimm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gvrylatsd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gnjstyxpl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gccxnzqsj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/geyqzeznx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjbeaftun.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/goemicjez.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gkeoufogx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gszexlcwk.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ggtznyspy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gikvxvjpr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/grcntkida.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqrqxdued.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guioceobd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gaxlpiciy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gofzxxwjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glsfqcuau.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdumsksjx.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/ghvezpzmf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gumciredk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwcfdqvoh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gsfwcaqpi.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzylpwcga.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gqftvkcxj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gpauhlnft.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxbypiq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkeifvdyo.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gdlqbtokq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/ghyixyycc.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/guaqtvcle.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/ggbkwzzal.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfcwmknkw.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gyvwkntzf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/ghgzwhswa.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ginrkuaoa.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/guflqqxfy.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gaaygcqce.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gwmeauylh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gedgjxtzl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzzowtsbn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gddyjhtgf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gxodhzoiw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gdrgqvyea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gubnosvqd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gspmbfwgu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gxnoumpxp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gmbebgzer.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/glvlzubth.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/giayranfd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gouazcalp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gugyfyomx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjvquqqny.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gempfxdvl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/glezfysxj.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gypztnrgs.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghixvjeos.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdnexqzqw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/grmxuricv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvmdbzhfr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grkchuuyu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/ghukccdyk.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gdyyjnvcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gtietykoa.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gpvorfrtc.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gubjsgwjx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gjkqwjldi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gpdmoybfr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gbjfzboks.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gezosgwia.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/goekpnauv.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gdcfmrhmd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gqqcpgjsj.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gjuflqbnc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gxshmssjs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gsnprtuot.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gwzdggyqa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwdsstkoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gyqzjfqdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gavgknzjs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gfqiyixtm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gvjiqaqvk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfyxnhziw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gizvvstyv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gxdyyzvkq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gykbfilbt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/ghicxsdim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gwyvhmltv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gpqyoeppd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gtxratuow.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/geywtkqkf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/geqooaypi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gbkfjbjzk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gmmckhqxr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/geaduzets.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gnucikeft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gqacajnby.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gzxgulfkh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gusnxttof.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gywtwtrez.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/guzkyaycx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gmayqqsrb.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gyyrnowfc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gmqfabdld.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gjpzorsrn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gulicegdt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/ghfevyipl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/guzifbbyg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gqtcjcbmc.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gzxckracq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gooqqrkug.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gixmfvomk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gbhojwnad.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gyqiryoor.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gjkqnhkco.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gwmjmbbpr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gxfwmthow.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gkqtfoxaz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpcgjdkxz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gavrvlbhl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gwuxnhsrk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkpoaoikh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwvxsivzg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxmmopkkv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyzudfuxm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/ganrvwjxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gyvdnakwl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gftdrmnge.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gdmmmhyaf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/geauvkoyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gidabmrvc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gninhjhzr.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gwfvuqptn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gnciviahi.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gzkgrstkr.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gmgqegsvm.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjqbdtjpf.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gevlrdyfv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gmatelkst.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gksnfkmgh.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gfowyriwz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcdqvbvke.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/goekfagai.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/glcdhyfki.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gusgdfhwk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/ggsrtwrcq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/ggqirfmrt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghpfxzowq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmdvaeiec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsuqrqkgg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gtwqodoiv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gingjtzer.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gaginasik.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpagpbwuq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gvcpqwvsg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gidwyysjl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbbjusrzp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gfvwcpfmw.sHtML


<!-- 参考信息 -->