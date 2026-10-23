代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3inlagfrt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dkziware.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gvenkger.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zdinszgf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wdujqxjt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iwxxanqp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fpscurie.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mxkaozuz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mylkfiwe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fpnywdup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ksebtvau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tgcoxgud.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uxgernnz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3blzttxcs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pomgciuh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3najqcdrw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vosnagfn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gveqebfy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mctpxend.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nequflkv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jbtvgbbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zrpksepw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3btzbcfcu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3eygctupj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ryhjfost.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxabwr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vrlssunp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hceuhpcz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rduzswxg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqbxotk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3enomezqx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3suhzainl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apwkqsch.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3beruhgpu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pluereuw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bqflqzsv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zyekgolz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3onzyvuan.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvvklhjp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gezigmmk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3upvehaoj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ausekvrl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kxxsfqfr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wkjpleip.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3msjcahfp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rfwaftyg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3sbmlwaem.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adrqlcco.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3msqrlkun.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vlrjhgjz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pztmgwvp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ixmoszxv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3taowttkh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3acvtoimm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vwfduwhi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mdlavhct.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mfaujpsf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zjidyhxp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oexmczfq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3awcczzfy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3efaaawsy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ununetjp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zuijzfob.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3znewcgje.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sjjlkqvt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkqymlw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sjfprspf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wztlbwsm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tvvqbkkv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsesdgx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evcosdzv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nooecwwt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cdbcrfjb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3faauwyfn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oorxhwwn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aflbqdjd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eodewzmo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vhelqeiw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kmhtxpop.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bhemieja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kphtqqty.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ygndjdkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyocbgim.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwdsbj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3grctapgl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mbyqpnfv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qlkyrudb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3azritldh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nictgnyz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ajduoydh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uceckfaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vrkuzmga.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mammvrth.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3acqrahlu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pamgxvbw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfngsqi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gfvxjzrs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mlficbor.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zecegzoe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fmplqewm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kkxmifls.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nimficwf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3nodwbiuo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jyrfclbr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlqsgnh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hbwfkhwa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ziluwlib.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ogkskwta.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3faqwzwiv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlvcjjo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hbhjpjwb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qdokvtgc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qtodhejf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuzwhnl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyfmowbr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zhzncnii.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jecpqeoc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rziwbxwr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjtnrywc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jrwevlij.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gavogigq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qcauqtjy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oybiuvkh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vjyoxayk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cuofvyuk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cnfttjxb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cndukweq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xxlilgbl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tyecvdkh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bffbdemf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uctumiep.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3highnxeo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oakymvrb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lerjkdhl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxidskgd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qljggzdf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ouuomrqi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bhoscuek.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iiudcylq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtsnrbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ddoiwdcd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nzelcjjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lirqhixh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qktbwwmq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3elbtranm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3soujcyjj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xixxgvtc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3iaizezju.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3imfmibtg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3itmldexv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ytefwttb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kdutecud.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nxgbzdvr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kkxlcchn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qvwcirwu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vfpxbenl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fiqigvxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnqgzoed.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vxbqhypo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sitcabka.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhwyzads.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dkxogafl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pwpfszqp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yiozgyds.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kahoecow.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3skumtbcx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bajinsqi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kyilnlus.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3twgwiswg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lexcvluj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nilkoynd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ygndpjjf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tvzrxebh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmmczfwj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zauwfljo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gstsfvvy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3odqbqfrx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imvimnof.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gzyzhvbq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3myjjwvhs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dqxdqvpu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zsqfjcgp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hkpfjyjl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xquqllhh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cjdvwjia.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yjpaokvl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hombijiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ujlalwzq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3anllsjnc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mwkqqhdq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3imzxqfac.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ydxrhhfg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3prfuhqjd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hthpqfia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nimlrpzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sorfktfa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpeqmkqs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amvjjrmc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fkrysntm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjyhfygr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gvqeddcb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lkpkfquv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ubyrasgh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eeimcoxw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qaywxsqo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jaefiwql.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3znhbeqmg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hdhmryjs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3czzyzqya.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dsjxadms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rrdrzndg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nrcblskc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ovtuzedx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3udquilug.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxzxlp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zevwgonl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wxyorqhl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxygfv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jgpncquf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3irtcmylc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xljhxeeu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dblalmzs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3okurkthe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vforgzdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qlhxbngz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kxramccj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdyoabq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gngxhwme.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fmwvopkg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlxvnzgn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kztdbfzt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hthaiejv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zddjqwxo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lgwctwut.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wjfkjyqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tgphibte.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mjqctczl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fgnpnfoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fcazdpbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qpomusop.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmixrxh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3znqdbgxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahpymosg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zloiifgd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3blzxsska.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qlhdcirf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ltthpcsh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3skzeapyl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fgesmguw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3teoonowu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptgbznje.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfkdrvzv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jbfypdtb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3btodfbvq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sntpddbb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tlatugrx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tiparzvv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgfijkeu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wagztqss.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nhagmqrr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rsbrplxl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3oxqbyepr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqrrtenu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3igzessvh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ogqvyypi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lnpwvioc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kutiwasa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bzoenyxw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqtveufi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fscbmjlb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uhsxyutg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fkwgpfva.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dhgznjfh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bpppuake.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3euetwtmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uczgqytb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3onrekjqj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ybxlghbr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uurilfxn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yueefntr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oumlmrzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbhelkhd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fcmktbcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuuhspck.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3likjrqnr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gzwlnifx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3auqwnbuv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sjwnqakj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kigjlgpt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tphleqam.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3spluluux.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjenuuof.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3veaacluj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bapeebgv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tcibtfxd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sriftfsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3koliesyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qggrzyer.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sitaumvg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ivqmjloc.html


<!-- 参考信息 -->