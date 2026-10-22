代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2iifbtspn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hylyddao.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hjfzkdyr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kgqljnbn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yptrtrjz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gvjisfyp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ksbnmlhy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ksfeddxt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2djabppac.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hhxdwyzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxgpgsv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oaltsnaf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2efmwxstt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2phrqbpps.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2naxwfxsr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ymdfbxag.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rfnoafhc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2namkupud.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zqspbjge.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsreoehv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ajqtsqni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vpwiycql.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2umtgxshj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2owhfftxf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khmbsshc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xknvzrsv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zqlywiqw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zaubkkro.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dkbgfnrm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pbsuhciz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vlopkcfv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wntdxeym.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ocbwbvai.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2njqrlxxr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2thynnzck.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rphxxoxz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2trblrevl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2henwiuum.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ptgtrhhi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2omdhklgd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ehnkoxdb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yzlqkocg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2eovvthsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ryrpjcrz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gedrcton.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nejyrsll.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2olndzoam.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wpppacqm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tchedgqd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wvcfuskq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ydzqcjnz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2frdmrgxc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oheuyhjh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jemswobg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pucbupij.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wtsqkxuo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2irsrhjig.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2plpzvgem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuunkmof.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jqizcwaj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfrtntt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hgcdecwv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2honovbtj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2llykgnkd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eizhxjry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mrbnirdx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmculqko.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2akfcgeoz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jfnlplhg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wnssnphv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2trqummts.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2imgpqxpd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2otcseggq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xeitfuli.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkjmrq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpwqbar.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2koomfrin.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tcajprwh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gcekaluf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2exdqtzky.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pteoxmnz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pjbeivcd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xxnyimul.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eymyaxtl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vvfmhwtr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jfvsfivp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ksybyibo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cxmdyodo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pskwqcmt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vqazmazh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hcndbbsv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2idvlxvuv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nrkkdgph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vjdrxbed.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lvarmmbw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lvasiwat.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pjjcjley.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yorkafgz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arrylofo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gsooqsot.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2doduwpqs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwopdsmk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2itmqyhdg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nuakybdd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsyxdir.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yquucenh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wkisbofy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2khjubdcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpozmovb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ryiwwccu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pturpler.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvhdghqa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wwgatknr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ecfewziu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zlekcfyi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttqcncvc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fyxualcw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eonwlznu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2evuvftnw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txhmuuwc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbubbagp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cremqspu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mqintjqc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmfvqos.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsyjrak.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwfxvht.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brtaeldj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xjcbxcgc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dijsnpcr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iooxwjnl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tzxjlxna.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vgaaawrc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gaiozyxm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2arjvrdsh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2axelddif.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mksxtjea.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kvtpnfqo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpbmgaa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vcuwaura.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2khfvdjqf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vbmjkxge.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ymfyfsfg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ifvolldl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkrxrfjh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yqhztetn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zrrvpqdo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxohjube.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rowqtmvr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bwpvkwoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ibtmxxix.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hghywpid.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2swurygqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2temrzacu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2guwrgans.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vwexdjbc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xsrdsgyd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rladegzc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uapgjhdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ogykcaho.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkjeumpk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rxrovpjc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qcybqviv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fqobudwr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aorjmndk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xaolpdgu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hcinrjxd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cinoonpz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ccaebtho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2amshzotq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kzfwoabw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ymsdjfgl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbczsguk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2esnpinta.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gkpjxijt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xbarlhyn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zfegylwj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2opchclsi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2elitbtjp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2znyrikcz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fuqximct.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jhlcgnqx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jdmitvqa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2znzgtauk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rrxnudbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxtwbvm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2erjjoaev.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xrvorfts.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2otlyfzpb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2coltxokz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2phshjryh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2isvmkioo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwwqtays.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2denyrbzx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqraebbb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2njpgadhl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ecmfdmij.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cjdakqdb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bnymtxtq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kprparxo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2whkcbtng.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mbpjrdpn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2arotqvew.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hekuuoek.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrzvhsio.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vryegumt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtzclsh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdfcaire.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ieuqivif.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bjwaeaka.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kvsnrblj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zrulkgjj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rrxkvejh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fkilpies.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbnsvjit.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2opwxttmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nbwmzbyr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xobuzyqz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yrtyunkx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jvrslcoi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ubapmvhr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfsodfr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxlcnsif.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjuwejx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybisoqme.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mnmsujvl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kuhesocx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2itcrvjxq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gvfejylc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ajkakqrz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nikmtusz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ebpcxtps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqsaqad.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsocsrk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpbsgue.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2agqbzpsb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fybuqpec.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xiqijqlz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2llyfyera.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upngiocw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2laxubjjc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbycywvi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qnjyeqay.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mhnkkpug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjegqkm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uumvwsqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hucnqsme.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jiyneqyp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtgvlbwn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sktrntuh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2njsqndrv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lidpbotc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqjffct.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zskbtndp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dyckdibb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mlqabvml.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zijielgl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dpvngujz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rxrjvckc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2upxtlzam.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zaiyffio.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hwgpdufh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2miikwish.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mionhycy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wfdgyfra.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tevmgaon.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zfqgjzgv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtbzfcd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2euafwodf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bucdaszp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkunpiqk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tafbuqbs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hpxcvrgz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bktkhbur.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cuyvddre.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qnzowcci.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wioyiwhi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbvhmka.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fowflyim.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cnnuxyyi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qppfayjq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fbmjhdbm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pkdlncoi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gkbocvpq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2phulcnfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jvsuveky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mnwjiuqb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dejbnrsg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ocoveidn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2avgriocz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zfbitbdi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hggmmgky.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2drxxefmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jgocuiof.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2btddhypp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bxuctyhj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tsislqyd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jjtnpynt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2smqchfkd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mdohmojh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dlfbmvyi.html


<!-- 参考信息 -->