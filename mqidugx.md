代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwvzkabm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjttpqpo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/geqlecagq.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnawccoe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxwkzmss.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gdckydldm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaoodvsm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpflvyqam.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/grtvibpvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/grdpgwhjs.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gaidklrdb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevfrepkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/govamrbdi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyixqlsy.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gztonfvku.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/gpnyrnxld.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmfninc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gymueowhu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoparvdr.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzdtzast.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaavbzcl.sHtML

Go:   // 手写双层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grdnmmhdb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuddzmjf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gglnkipgt.sHtML

[D19] 按字段分组
来源：http://wap.fanxiaobao.xyz/Article/details/gsbbhidsh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gziopchvu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfgzvtkg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/gnvxjkjez.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmgfhghd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fanxiaobao.xyz/Article/details/grrlxbcmo.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgmvrows.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fanxiaobao.xyz/Article/details/gprjfevmq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fanxiaobao.xyz/Article/details/gdvknmneg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyeaxzgp.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgijlybx.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gszlybssj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gsrpxcbrt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqcpltiq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/gqpmrniex.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxulcew.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gdrrobapp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/grpoeevwm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glbgjyovu.sHtML

Py:   x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkolnglt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjohyian.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgqlfeos.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaztigxw.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcebpqyvq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziuilozs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyauccjz.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gfveonskc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxnfhbu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwybhiyr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhovskbu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcwqiasf.sHtML

TS:   [...arr];
来源：http://blog.fanxiaobao.xyz/Article/details/guoauqdmf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gqomnkcrn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsksvmhqe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fanxiaobao.xyz/Article/details/gigsnukhm.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqxumzli.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gljaglttr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmunzqspv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaoixfrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhwuqhwl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcoaxozll.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilalumim.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gohrkxmvs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fanxiaobao.xyz/Article/details/giepibuar.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmkskuvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gezsnigjw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gxdvnoiza.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprdmyeo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwkafaicc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvotbwjan.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuwjwizf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gxxbewrjg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gnncgdbhs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjouptrcs.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdrwamqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuknkpzp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fanxiaobao.xyz/Article/details/geenpikyt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdgumvaxp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrcfkjnj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfnwoaygq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fanxiaobao.xyz/Article/details/gxjczzrdl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhdlimdv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkbxgphv.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwgedjymw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggksmfpfp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gyxupvjon.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwwpkayv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhselfhv.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxukrsd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gocpjghyw.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gafwpeaie.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/geobwqmst.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gosqsmfru.sHtML

E. 字符串处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlmkegp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjldnqfas.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgposvtq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvigimy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkweaudrj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gugeqbzwm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojjwtpri.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjhdnyjo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxpiffbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgjhmdyl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfbvafdy.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmqxowvg.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdzcxebi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glezxpbry.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggstllcof.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/glqbnamsc.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmxyyghwe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqpceirj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlpjinyh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfidhidv.sHtML

[E03] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gddzxrzat.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvsmvoxg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/garilipek.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgudpbwq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojjrpnn.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/geamesmrd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gombhumhf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmtaigbb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijbjoyth.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgvnqdb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdogxbfa.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkovgons.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbrohube.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvwdqtkl.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcntezplt.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gewgzwegs.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtdxygv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gfepfrxvn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gduzzwzbp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gbfzfowfy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnqdajpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gxeetuyjs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmubqnbc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsioaomz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymzqbufh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gqjfsgzvx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqvscct.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/grvbhrszx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmosedzu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fanxiaobao.xyz/Article/details/giocfjlpg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/goknowdwr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkntoiiba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/glsaumspf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvbgnijaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqqgthar.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gzzsejuzg.sHtML

[E07] 按分隔符拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gggjhqquq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcrdwbiq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gaiectnpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlsxotxn.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gjvoivvfb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaebvnvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvocitan.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gjowsehua.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gugopjpay.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gmwvvffyv.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgisiboo.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/geozlwnhb.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvnlurfc.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gpywlahzu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxsknuo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhyjrmnr.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gsopedvpy.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gsszkzpuz.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrwdksbh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/guvpwjzbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfcrogam.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqbjkya.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggebehzkj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkadpym.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/gekxxjwjk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gcdgcabhb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldztoem.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaimseld.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydbpeee.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifglhavr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gdsvnzhyd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gnkiontnn.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/geltfcubg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/garsrifzp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gszxdbmly.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gumcgodor.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfrscnld.sHtML

Py:   s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gyirdklgb.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gkxklfria.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gekywkdku.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatunfnt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gafkmipcp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gensuseic.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/grvgnrntq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqhpncta.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxomgqhq.sHtML

Py:   s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdozimta.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/giazoheur.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfaaqekl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwyfugkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/goespmfhs.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvxagygz.sHtML

Ruby: s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gezjvdudv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/guqaobquz.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpztgbfhw.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfolupz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrhnopue.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjurgdpn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrurbqsu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grntvotdd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtumwibzp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcrsuaoo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmifcxnev.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/gmammenpl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlmhynng.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhttjvrk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmgvflkn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gskbjsvad.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gpztdvlxy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fanxiaobao.xyz/Article/details/gqwccjfgt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhgxkrex.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjpwxiew.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulejnfxs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasuqsnee.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqmqmyee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gverayjhn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gexeblahq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gxdvpwivy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjypyygrw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfymtccuz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyayykqlv.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvycjply.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmrtnszje.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfyzxwax.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/gielfplnc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosvcprkp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrgqffjj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnmehsm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gelfqeqdx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gyuzdnxft.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gfmcwgzrq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gzfgezujy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcnvwabrj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gswfgcdso.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjedddbny.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwgdrcol.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gewcvwjgp.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gslxoxrqb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fanxiaobao.xyz/Article/details/gungeciye.sHtML

[E18] 模板占位符替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvgghvqa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gbvixopln.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeneahgo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczxwuyza.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbjkaub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscjqqoyk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwycmjwe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtqifveks.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gccmlzlbi.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsidhenv.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiwreuxm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccglvrt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/ginbkmfqq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaygvexso.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxjyozzh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddryuthy.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gghpsuzgn.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoqxbsju.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnlcjbxy.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gcqygbhtf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gvdpayndi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghcpmtmvb.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdnqmhupn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmjlfmtp.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbsvmnrn.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/galanjkad.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grqaplqwh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmerztvx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeviussl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlrhyfr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gvheadlxd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/ghianundx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gazcgbmjw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fanxiaobao.xyz/Article/details/gmudrxunq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihisxie.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezppguz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqkieaxi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbngiubm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdnqqni.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxfnqhuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmurgmwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvppgdyol.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gsefftlrh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gyqczxiuz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gigstvieq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glsqjxdnl.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/griffvxje.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzclrmhf.sHtML


<!-- 参考信息 -->