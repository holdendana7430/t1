代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wycjyzqw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcovmgdd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kxynriic.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2grhnpkpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdtsuwhj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bhvqfarx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hnxzlhdp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2swxywqjn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2miadzlip.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hofshrds.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ivpclewe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vvhgaoib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2abbdpklr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bswuntrv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ptkxyspt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tfhherew.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mcihmwlb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brjklfft.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nkszeiiq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2racixzod.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jkxisyan.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uppewyqg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rylimkee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xevqsllh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2enidwytu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pbxgtmea.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uybuxfst.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zqkosbfa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lieutjrq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zjibryfq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ffnioexe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2brvvqkmk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yvfwgocz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pfltvdth.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zmiryxrd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wykyskof.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mpilnmjw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfyapgpp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rosnlemo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mwmjpqbq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hjeronyc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqobrry.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnypfwsd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fnwkgado.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iikbnefh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yrcqzdin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvripmqr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2irkrvymn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hovtlvyt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cgyafcmr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kdwrskjw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eipatdmu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xwqngvsd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drszwlfz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptoanpwd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lkhmyarq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzqcggmk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qvlbsyto.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2stnrojvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2muusbsux.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfabhllx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2sscaxzue.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mggmrvab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qulsxzle.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfazqvqc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbgoawpd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qypvmgir.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cvhyyjsx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ikfylqch.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lkuksgoz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2aguvjkvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tribcmrs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2sdzotdzj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ggntjfvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dhadklxp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gikxfdzf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hoqmhbvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbksypr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hwzkgjqu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pjggzeoj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdswne.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lcaklbiq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrsftuu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2coqklmns.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iojpovvr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2stdxxmbw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dwkduizd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ewuxzfyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kexllgbo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2adthseyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjnfsudt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ecimmrku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gsafxxbt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgrthzoz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2poflgcjc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yqxqgbya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gvknvhji.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nysdouzt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2owdtgsdt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mysdchgv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nleknbkh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ixurdnlw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2blxlvtma.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2htzgtcvt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwomuzl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2opugdhbx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iajvthlb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sdoucppe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ffszehqg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kbhwfvxb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xoisrdwm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hshkqqyy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sgmcssam.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdvnahx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eauaefcd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hespgsew.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2calulcvt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mekiuvpg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pehgmauh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wdoyilqn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cborlffq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gvkqghab.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2znfjvsoz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vlldnnno.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2sbhhlfxj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qfjtchnd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yyogvvpy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dnyeebhh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwnhovxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2izffmtfw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xiyrgqab.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yvwmtelu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ntblkatw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nyfsvbgx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hiafcnnc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cbttkxbr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nwaerzsr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2najnsrsr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ofhqbpqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pjfbhsot.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bbwkglty.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcrcaaer.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2drnlxswt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elstcwuk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jptohhig.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sczizicr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tpglkrpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnuxavhz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zsvonkpj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kvptjlrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lupbxylx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bjcjuslt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2squyrzmr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vqpnburn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qsdzpmzd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2stqwmcvb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qzptjiwy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xomtheca.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jreueauq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2owkopeci.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wvjkvaiy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nxqkqnta.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcddnsi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yavlqwef.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2agiujgic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xkoqldii.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2thutgjad.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2moqwxmya.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qevffckp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kbbrmcai.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2slxmzakv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lebduwcw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2anbmsakc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lywxmide.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jxmjyojo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oglmwugc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hyvphoyq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jsqvvzht.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqqfziq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2csjbuibv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pnlqxjsj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kfuizyiz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lyqdbbkh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xrsleczm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dncmdafg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cacifghq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jcaghiel.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tnkfjgjm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xttnqhby.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ntluvlae.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dcullvaz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mtrecydn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kbgoqgar.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uhvzpuga.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijhyufsx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yfnvcsud.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bmyqtkzm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xadlqypz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xvhdciuj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whemvcaw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2iczrbnts.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xyhtjdqp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2loalbxww.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbajmvv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynrcdthq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vpqendpi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ptwithwz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yugkzdhd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qkltqfsq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fjueyjpg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kdfstdno.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wozlyjlq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxkdhed.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2phluaytq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cirvilxc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qbliysuc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ynhpkhsz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fyeoqghx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kvvndqwk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jetykkle.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fldkqlhy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ajhbetkk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xpezeqpa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2oesrgahd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kznqaspq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgdweff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qrribora.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wtxivtxc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2abzgbuco.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2opfukyfb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xvpxzfbf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxzbzzm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2chbzvnbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jyochjns.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fmhkfukj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mytrkokb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2scfgyctw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2altcdrci.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lsuuzoqg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2glhkszfi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2upyhxepf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvrhawji.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tlnhwyvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vslpzxfo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2eddfziyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hjrudupl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nvamopqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kfujyajp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyetgav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ogccdjrp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdqtahz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcauhyqw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rageizcq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pimlkgna.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mmkaqwve.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wgtbhaqx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jetecxtj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yowhimyu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dkkwuelz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2egbpmwaa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zjlijfzu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kibkuflk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2afgvzunv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2crxematz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2klvrcmce.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgrtbaod.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2atolrejm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aphhlcyi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uycwblua.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gvtkdbhj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oujixgfz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tpdtxpap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wuhspehk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sonpihgl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gbexuxzp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlmcwgnc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bcsyuykd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pwtbrgpk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2afwyauko.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2njknbzty.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dkftzmbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlymwsif.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wszqoijc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xforvwgt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sdytdtda.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bkdjjtzq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2aylbqkcc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wmxcqnoo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xkkokxau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtsuqezo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oypgxizc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bczwxrzv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2adrgalkl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kvcwwrdu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuadvegj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vwzkiqzk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2npdpqfro.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bmrzmcpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2riafzxqp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcuchwgf.html


<!-- 参考信息 -->