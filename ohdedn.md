代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bemzanei.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lzkixabm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mcvzmjvv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hamzjkde.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vbkqqqzw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3touhrtoy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qfffjwkc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3onywmwcs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ympgvjot.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bqmdrwxl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxluapd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwonpvwy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gqbqvumi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rfeergtq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ttbuejov.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3igvgkumk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jptbhxmb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wecmrncf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dybllmxd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3thiwvxrl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pprnwrvn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrppvew.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3febasfuw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3udshmvam.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uvrekrar.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wouzquuu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zacowblr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3slhoypth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwofxhus.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kgrcakob.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmngwajb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kgfhfzea.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fduiqbyz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bwkixiob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ueudvjwz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vkgpauzl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zhzgtiic.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xymnjssg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tzseemad.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojcmkzhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dtleqbax.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvvzhrd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3njvqtymf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qxqwrpsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcaflbnu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cykhccmx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwjopat.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3feddcsfd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3epedikcb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aqxrpfgg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3btbxsooz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lmveqwcn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cskcacyz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jqjvasfm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dtzduiba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3siuvchss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zzzmrkpo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tnekkgls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3riprbroz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xfhojjzf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dagjwzbv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3txnyepjg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tqybempi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ikrxiase.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xueskznx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afnltfhb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3egbimyed.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3exvwhtit.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3owtdhbap.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kkzplcca.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvxqdoqg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hyghcytj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjaferec.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fslefgyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwzorntr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3damzqxkn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lhzkinkl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jnijrlen.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3adgyzowd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rxdofpnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wuhaksel.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nzyytlbw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rzqgaagp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tebltkyv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fwexdtgv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iedxvrsd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nncrnkor.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmeokxo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qxsvaenw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bohfoplw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yafgqyce.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kndmnxbd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3baakqwto.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gojilwca.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3oizgylps.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mnzpxddu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rnydvwhp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fupyknbu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pjoiwhsf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qylstmzj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vbghmzwy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3idwnxuho.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pclysmwt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aljqbbzo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3idyznttf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3avzjwkxw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ficknqlr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tejbdjuz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gnrugirm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jxsmfxor.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zjyoumzu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qvhkndqy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3auycidhg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kavtewhs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gmjvmvnx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hvftwecu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wldiofsf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ldabeemu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fasptmdq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wnafuqzt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3iqccvudp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bfbqpdoc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tcyuakru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3njhkohhe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grbjroyg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3twldhicf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjashoq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fipxzfoy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ygwvidey.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tkxacqvr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dguuqiot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzgfmowq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vraagxzu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fncpyewy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fcqmoedz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3isavpquj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ixtitoug.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zakooybd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mqflakdf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sxtljnxn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zrmzcavb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vqooijku.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ngqmihlq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qptlmbue.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3efxshsex.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fiuykqyf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sffxcbsr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3pyiergee.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3spsokhvw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibjypydp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zqlhcvgm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kqgdbvhe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fmeqyrtb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ylwgscuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iqotafux.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mpyaxdvg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nndotnim.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3omaznvdj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3otmeaath.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jpjotzjg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3grujobjs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xlexwseb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fjwxddem.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3inyxrfud.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3cmfbxugk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eqygmtjf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xiqxgbzx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmsylbyl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fcqeffcc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpoyogww.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ccrfmlra.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lotdatml.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hixxcfwq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nhqjblut.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zjhrqmed.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mavmphok.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3keleksmt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ueuvqzoh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iznizxjb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cwcapase.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ckyhhyoj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vhpebatz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jjlwazxn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xnnbbhnm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3huivlmsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mkzjpuxh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lrcydlrw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uokxuawt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aljfugsu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3epfrlzyo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ldnlzndl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qiezmsgz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pyehnvni.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uyylgoiu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzixspps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gehqbuwv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qepjyqrg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3icyukezx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mhzeglcf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3whvxdmpq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nmueygvo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3kizxdwmh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mwkywivg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xpympvas.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjiepxb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mesajmjj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sepkeavr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rouqnnfr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axfhplxk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hfnzwewd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fuqrnyno.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yoxrlqga.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bebsrmub.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3modzjkdq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dckojkfo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgxadof.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dhfyclwj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjrvkdki.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ukzmsmpa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nkvshgnj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xoxqavpq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fazliocg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gzlyozqd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ttononam.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxsvkz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gkkjersk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3prlqzghi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zhdwoxwl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmuvkmno.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pivcwaxq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fkokrsvh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3siyqnspq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jznbwpvs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxsahwtu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egyxnkcd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3obyodcov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3krnnsmim.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3aperqfou.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fzmgecwd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oyhmyiqt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kchfvufu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3irphtpqq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gsyfdqka.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gfepaugo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3abiehnjq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vrhndzcb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3muxdhscq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xfzxmhor.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bgnyhssu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3llncdgud.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbtbduxa.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ymcppley.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rytzpirm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cqonuwsi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iuylteim.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fsaryoyp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mdzvvpgg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tisjktqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ecomhrrr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cuvgyptu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bpefncdv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bicrzwas.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sildjqff.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxjpak.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bboppavm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zkndnzyp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3geqxspje.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3irpubhux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3teavuyin.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3btahtmwf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gjgbgdfm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bkifplld.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yvevfwyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znwijmrs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3theixddq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aynaqwdr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihtoxjpm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zduedrmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvrbhjis.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3srnupbvf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jfsrhcuk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ihgqcsrs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cwhvmixq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzvnovve.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugfiyyih.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjznzjwe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3npavfgzi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpgtgfu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dozkpsxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzlsmj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrnyary.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fzsnkjkk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zylksnqp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nhydqxjk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zktkjsxe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yuuukoqd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tpguusbq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3slrldwdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3anrntmiw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cfqtllcl.html


<!-- 参考信息 -->