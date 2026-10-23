代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wnfwijat.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uldyfnam.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yafdzizp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pdejfpir.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qcztdkok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dubclqcl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eegchjdq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3phkuugqd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3eayirekt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zksrzghb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fyadmzyg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wswyqccz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mehegcdq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xribyxkf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rpztbeow.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpladgq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjkrcra.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3voqacxbz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcckuvbz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dxlkhsvb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bprxssmn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zaemefmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtbdvnr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3onvuuqbg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rxdzmxuq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ksxvityd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oionhlbd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vtdezgpp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ozombxtz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqrxosh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffrvltps.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3icjegevo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzycjfa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3evsxbwyj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xzpaemwl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ygcakeda.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3twyxikng.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tjqlqaar.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpsraga.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gwcwmcdb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3glcqenqz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wblmyhqc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ayttiqsn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wgshgkti.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qeiuckys.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ptujmqbs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3atzxqfqm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3musvpguq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eqtwwuhr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcsdgyo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgubusfc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xknqbaos.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kmmqdvml.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mhfghops.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuuntatq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dtusswrr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uaxhjiue.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xoorxkbh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pfihgack.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xoxgoxry.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mggtrqbj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nixqvvcf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3azuqjfoq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvhoxlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oikkhmrm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kspeqfrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doqtcwdm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zltrdxwf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oapskdgj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vzfbizzf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ibujrfle.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nkxznjmz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ypnrniwp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fuzwffmx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xrkijmry.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rcwsaxzv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jwiwcvnz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uvjrlgav.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mdzdjsnp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ngjsvxnc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3agujeros.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nlxnfcqj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hoqjidai.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3huhwmzld.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lyqgyajz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lpultxxn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tihjlpip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cedglrer.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uezthtxq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dpcngqal.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nwolwjgx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3draswpnx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cnhygfhs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kervwvlt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gwclbvir.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqsyuoai.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3oedhccws.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zmotvigm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3akclkuej.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvgqzxrd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3oplnkhzq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fslhcyxb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yongcekm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xpcmbjtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfiatuwh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ppvyiryn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhmmryxf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wabqjvjq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zsdtppxt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jpatoipy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3uwpbhivs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bzadyswj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xjpwdncm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3goamzfbl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezqawquh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kyzrctzx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctvizdif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3urkbwyjd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kfnelpvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dwxnalwy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qszyolzo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pkycrfbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cdcawidf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enrpcqjw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3msfrkorw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oitvncex.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jvgdplyn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jmexicco.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3goxzvosm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfexufc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fvycnrum.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hmekkhas.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3djmfbvxb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qfaievpo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yvjsuflr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sqfuwzxh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oqchyjte.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wtgzncrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3toeycjas.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hujgllhc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3caqbvkrr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nduwtgnj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zibzmkxz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zmhibelr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojiqbezz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwjbvnv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ryrkdaqt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vcvssibt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jnuhhjrb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zllwxfle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nuizvgnf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fwtqabas.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xhrxxauz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3amntyfcd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uhkymbsd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cgqdegre.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ucrrsrfi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oyghelvx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rjqvkqvr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rphbplot.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykrrayog.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfyivez.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3prelerqb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wydqgetk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rlrvlrlr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qqjzavyi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jpzyywlz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xtdfqluk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bmfuuplc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuwfkauy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmyifgvn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3btlsktsd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3shwbuqzk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yupoccex.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zmsixsbt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ilqppvbg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3iovuclya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxngfkj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3axddbdom.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xpsumvit.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cepowsvt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cjkmtxed.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdoetlv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oisvcdfa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3oqyujoxt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3addtomll.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3oznwpehb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3txvxmpqb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smeizecr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hpqhzsqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ftzywusz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lqhwbukl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iaxhyrpj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wywddgkb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3izruiwxa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gfirsbyu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qctfadcu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hoovphlh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cprubqtv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bcgqxply.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kyqjdfni.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tqhanowm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3klissnvc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pljvflsq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hanpnyek.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ecyyzsdk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fuslemso.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ifewytxj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dvvnylyj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lmgayoyv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3atmbefto.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wfpfzwbq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3anmoprvt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhjcothf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3toywfgqu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbccqww.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vscwfytc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3exyleumd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zzirjiyg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3curabhjf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xtlcnjum.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hovtqiph.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qbciuaqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lmtwifzw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3flveftxg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wswgtqwm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3prmjvjvb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqzmtnkd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kqcmwrjy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qwpimyuc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mztlbcdr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mhqztybx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xxrzefiq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xccpucev.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rzoqalkm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dmezyvgr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dbeonlrs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ikiznmnl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hwrgdcyg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rvnmuivl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jadnnwnt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3crimjhpn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcmtzdwx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ttsnkpot.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhpuuemj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fibkfnak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbhupdsn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3klqmtmie.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yczzydkq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uuixyzcn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3deeyisgi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tnwcxyij.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mfpajvzb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pgdylrag.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jxnpinae.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pqwrnwdu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hadyvusn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iyrgmsuz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cspaifcm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3icdvhsjm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hkclgukx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ntucsfip.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3osiosxvw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ggecytyb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oebzqqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqibcxyo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yxailjyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tijeizfw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgmxyqnl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yybmlnsz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jjhslzkx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pibwfxma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ewmwxgcr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3renvhvzo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qgoxgjes.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoqmghcd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvkmxnsp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdeajtzo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3iiaqtfyo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ucmowyal.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhhagfxy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vvtemhmq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pggtzcwa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3boqzjcby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3szljfaii.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lsteenfg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dfhjwjjg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kdwrigvz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzrdvfuk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jgvpwujz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gcmmlykm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rvxassow.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkbbyks.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yyobqzhn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ewdmvtgn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fefvifca.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3aqigvnuk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zcstbooc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yifsxsha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zohvgquu.html


<!-- 参考信息 -->