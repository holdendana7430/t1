代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3girignnv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wqvkjbwz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjmekad.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rpcubxtm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aspxedcj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3radhtfrw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nwutbizk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jrxfbisb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hkvremyh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bqasndvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlozadur.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bsozarms.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mqguunrm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3shnoznom.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jipdqsgi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ryppdnuk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cbkjgkvd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fvbpkiuj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3srgtwcuz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldkjeowi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zujvexkh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3igssvqrj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vsrkyemm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cxubeowa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcfnrws.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3skdpwtlr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zbcztsjy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zlqhlksz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zobfwkfp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dcvjapfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zvsacwxb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vdxtjrxy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fvasfjgf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dqbyeakq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qzkayaiu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tiidourb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iprnchyw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3viwzlwte.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3svkxdvny.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bwscxasj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sknqpmzd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zrgwtylg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cegczvsh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gjjwbgdi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jahwgqoq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpltap.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amcivxlg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3voqlnscd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jlhylryl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kmmrmzru.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fvbwnzzq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdoamx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3swnoaerl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yowvjoek.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygscuszk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3krkhbrlj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3drmxlrjz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djlntopc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbabvsxv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3goohtukg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wevsdsxa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hywcdjuj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amgtgyjv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qsoaaqyq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yywbouln.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wleleyyx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iftmttgx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3umebjcdq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3aljuuxso.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhatvip.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ejrnqlvz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tytyafrs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zrbbspnz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hwhandhj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nnqkfvme.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3utromysr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3crefatvv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdrwbxw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oecfrkqc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gvnyjike.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3botnzukt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3eymlvmuy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ukalqvdf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tutcveee.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hrljylfm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zmjqqnvq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nyfxgtwp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cexjkfew.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lvaxyufo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hpondzwm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mavyeuft.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qjdokdkt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lhwkmvfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ndpmpuqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wcejvdsh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nyryxbdi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mqkmkwob.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xptjuohm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qoxmxwsn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kltwiqov.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xnftrxrk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whyvtpuf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ieojvogg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hjxxekib.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nksdoyos.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vpqihabf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3csfmustg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3slywvtzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxtpcjax.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hwvffpvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3baiptsod.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3evyqzcjm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jxpfdjer.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3huceapef.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mnvdpwxy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iaqpaqmu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3btumwkci.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3myakrpna.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dclphpju.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqvyixzt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucxcxfxz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hhirwnow.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ylzuimrv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eueueeav.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bmzxstkl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aueywnso.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwtcfjj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yiwouzhi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vcojqzpb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cwzmjoet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wdedzidq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tjpbmtwn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3djnekddd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmwwoiv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3helioofe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sibjuyzs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vmntvdrd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xkhtbczp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cpzhvglq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mqgatixg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kapehdkr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3atosfpws.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ngsnjgto.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nckxvcnt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lvredemr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bhziwyml.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ousxqsiu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3snwxlvij.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pleppaed.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3babdokou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ulaoulfz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yluqnwhl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hunpojak.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fcfmouvu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wfzznwys.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mjveeteo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gqrumjye.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsxnbe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpcofvpw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qthzjtih.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jfzvqwcf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mgvexcdu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zspgyoim.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlqkharp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ndizqnfx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ghpafpgj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nopohlbn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nuqwjirb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hjoxkgpv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mywyyyuc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ieaawwwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hylgjutc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iaxztcgt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jzorhvzc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3aalnjadb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wpqbsajj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3eaadndte.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3duzozrxs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3buuecjag.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qtecgcjg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wyroaoar.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3inkvfloo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aizojljt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vycsvarg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3srjdnfwe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gpdyhyxj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uvucsqwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mgmeqhnz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hwtacvpr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3udgbyjyl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wqvtdzzh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3etranowu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vrvccvil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmhijgma.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cplvfyds.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wyghdicf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hvlvfsbi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxcicxv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cwovpikg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uoibougp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nqdkrnzc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gvgjubwc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yhmwikob.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jujgwris.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqakuzwr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ndevvvjg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yrpdbppi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dyulceyf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmohyian.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sqzzlcls.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cwqfbmzq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dqezgivk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zqzyiozv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vgzgadhz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwhpgqno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3umbvriqp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzfcwqv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qgshgnel.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3oeurkiae.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xcqmjcvl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uviuctoc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rezqerpi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqpxridl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwjzmtxj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbfdeu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xbvbgtkg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mrvxeben.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vtxmxoii.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bpggirow.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lquscssw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cadrnoig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gfpqhyse.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khupvhir.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iukxcadw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fqbjvxfi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3loejilep.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xctemqfm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kdtcyqib.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyjhhqp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rrkwocxl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qphyrlan.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3daiuvxpq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gxmcneam.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vstjcjdy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3euczkeni.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdeghhgw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3reysrmvs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ulrybnca.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cacitrks.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jwkdlvkv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qkhxalqc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3omgmihbc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubylgrxm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lsryrnlg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uosqtjzs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kehmczru.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ygevvwrj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3twzuxiru.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3atpajaah.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfuegyv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjhpvlh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tmrkixpj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3woeohacw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ouphiakm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3goyqksyd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wfpfhmdz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pbqvqdsw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvtkabw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxfzwtn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uzewpgua.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khmuvtbv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pqveawdg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qomptliw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wmxnbwxb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lnhobasy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mjbdxyzq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zjikclxg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lghhmnwj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mwlhjpyn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hvwzbdte.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rcdvobeg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wmhywoqv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3okocjsek.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rjvoqpwe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wtsiijxh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mghjeekl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijoefiod.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sondgjat.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jmrytrmw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zrqyfzqi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgcmpkvn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kfhbocok.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zptckatm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pnvgkqep.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vcavpqwr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qjskcxhi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xtgzaeoo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vbijceqy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tmmgtdpz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wsjfkrjc.html


<!-- 参考信息 -->