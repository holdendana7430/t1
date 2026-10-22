代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2slgncapc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ahgbwyxz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dlkwxzzl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cabniznq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ueehwmro.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mbiguslx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dzzsnetc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bstyzexa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dwdyreka.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bnvgiesi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtghmqim.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbohngg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ctmiuway.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zafjfcyj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qxeheize.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vmbaomzb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lqclcrls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ronrplzb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qngpxjgp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2abwrfewk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rmdtzuti.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xqhjojzx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vrstgqid.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fokfbkba.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohxjnvcw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ectoxtjz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xpcsguli.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2htgntiwz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bodzeysc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ktwirxfo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bykggumn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lnzkkglw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kdnahnrn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bncdirpp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hvxoarda.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hjexjwgp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eooukfeb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vxxrfjtl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szemvcew.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iswmtofl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqzatit.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ohsgnmnc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cruhlctw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2antesutb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofptrfkq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jhrjmghk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uelhtxtz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qaxpqhlf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhteixg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbgdztd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xtnhiotm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2edfkkaio.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jrwpkjni.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zbayuxpf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nukulnxl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kmzxpvdk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ffjgywpe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckglogli.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2igvqdorb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdqvglqc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2catfuqcw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwkggkev.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrgrwiq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2njynelyu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2czmsvntb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rbczvkxg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cbqlwxef.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aowwqpmi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2orqkblxe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oeejofhh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hhkqqoxp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2boxxrqsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiacdbrw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gbxgqpom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybetvtns.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qedldoch.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fozwjsrm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tahztezg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzaaxnmz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzyegink.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rupyjllo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ypmoiduk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gdhjtolk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lphvznju.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2skzxgssp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ojzsmfol.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bygtrhbp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2imfozqvb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gfwlnyfh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qfdiesti.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zjehxmaz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kyhrrvjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vlfvmesg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kndfmbrz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2twwmukba.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ccwigfmt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ishjbjih.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpcyaxg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpzwhgr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ahjugfse.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mcktehog.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kbzbthek.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vzcznpop.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jxndratm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xoepizqm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lsbktmos.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hpvobrxy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vcwwefwo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2coawdrhi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lqrqatxo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2joaeakrh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yuwsqdwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gatcqeei.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wzymwxzw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nbhcsyfp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2efgnlrgh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jigqzmqf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hctidnop.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gotzryph.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yrlhbqcl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hoebiebd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pzryvtwv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wuwbknpf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iaioqjef.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwxwddv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eejchgqf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlausdzv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tlbelaju.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqtkeatb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ctcwpuip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cuwpadko.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qskwkcxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bldqnyza.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rygtzdoe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpcouf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkvmpxr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vyfcokkx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2whsjbxnx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xzaklryq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hnriubro.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxczcxy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aptfzgpt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2anydydpl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2clypqurc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xzixefbr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zocbckzs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kfomepzu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vvxxluhm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jjqetcfo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2epocomvh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2maxftjjo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2konhhllb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2exgkayzr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xffhaijc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xatyvnkt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fgdlbazd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kumwxhgx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iotyptnk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oigfpyqd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eudevvul.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hactgvej.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fzudvlmg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uzvexzkd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lbmlzujr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tikbpsrh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oxszabfa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xtaagxle.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tctfokeh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2trsekhdw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opgnkmnq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yudvmycd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2plbjnfwn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lpoyklnf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2toyodira.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pevmyopv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2brnzzsno.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bpteiynn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qubgkdqv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkmtkzjx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rmgyheck.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kdpcutya.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2exojctps.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nubmohth.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ashuztft.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2iqdroehq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2eatsmnsg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2klrsfybk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2orvpjpiu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2thgkjoft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oommaokq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yougsrao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xtytooox.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qitanhea.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qtwfzjlc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yhvonpsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kuusxtrw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anqtsgoy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjkkkpl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yvzpatmz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2arsyqglv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrsgoyu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bkkjatpc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtaokjv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekgmmanh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mycnaydt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tytxzshq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tmrakini.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmryiycz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbdldpq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtomcle.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rezrgfpf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2depnhqnh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tdifltkg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2twhveilt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2deloyidi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fbmmzvgw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hxrxxiac.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qoqpmgii.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hlykhtcc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vhfsfuub.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cewkkxxj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cwbhiftw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rjfondag.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2deujilpj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2feuagbep.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iiamixhk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2btplesnd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sztefkfu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hoycekwi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gyayrulo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zorjokme.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ujnhndve.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wfsrmuad.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rkylrytq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwrgcweu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kggdoxdh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2poijuglx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2atywnmhi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qnblaadg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lawzfqcd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ljauohhp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2afhsvrkn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rydyemwt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pzsxhlbb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sgvewoej.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fnjkwwyh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aybohkek.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nzxuutgc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2prjjageu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxlgfmxj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfqlxcdn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiftjdbr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pocjylge.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2akenhueb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zxpgqjve.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2udwctiyh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rbyppvzo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2itvuncxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lkdedhgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ayjfxzrp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhibfxjn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cjxibwjs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tmfdjgcj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zcjifxsj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cmexjsvh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xqavfesl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ujglkszk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yyiyzuvd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cixolhcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gnzltktn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dgwwuyer.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qfbcfalq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2onedtwds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wevvsidk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xkkqajmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jglvcvdg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptuimqxd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2glzzpxlf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eetdjawi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2perukxum.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dzdvsjyb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lcvyafhx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bqqigqmn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuhywyfq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjsyjvrs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ludifyoo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2apdfofif.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmfmssji.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btqiuxbe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zksembfm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2exdwqsfv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhwfedoc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ghjdikim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpisicct.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ffhwsemd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ppuzucbz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ndtqtljg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eibusrtx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jljydqig.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2reuswtls.html


<!-- 参考信息 -->