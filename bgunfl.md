代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eebvgidt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eotyluag.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdxbnee.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3toanhdqn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qupmyqwm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ymruoqaj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bjfccqkq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iqsiuwyo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xfliwiej.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwlnunb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dnericaa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mzzzpocc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nslmmvhx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yvphzkoq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vzdiurxr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3enhixfjq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lejtnqrg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3onvpyroj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hggpvjkq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlwygajm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qafchmug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nqaocwic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3urcdkcgu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mimmxuub.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gqdmexev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mjhayyzl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqainbjn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cifjmagd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vgyhqcbe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzffsurw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dkhkhsyo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aroykdhi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3soumostz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cekibvlq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbuzsatr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tmkdjlzm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmvttnrw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ktxirxqk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbrbhhl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3psspntmq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zkramchk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xmfdupef.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ymmwsyqw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3avaaixih.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ieoumskd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kiprlxxm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gztlmzrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vlamtbbm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uukdvnhx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3stihcfnq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vcchkxbj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3iqqqlrry.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3isbqounr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vjuadpxc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pkwymrtx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xszisrlj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqknpnt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uvyqoxoq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqukhtq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3eyjwmkfb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xlyntflj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qdzelala.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3yoxakpbx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nbhxnlmo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pjmuvbxj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ngysgqla.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3inanbkty.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3aoocmpwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kiicyvqs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lovcauyz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drnupeof.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfknwdxh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rtkyuwzj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iojjzwkd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jsgspmoe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3trevxdhl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhiaayd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pvasjndc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3auwzblrj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ooggcaiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtxcrgrq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bhstjopk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydmmqews.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rpxhakcj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3frcyesjp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jnhccbyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rfmaotwl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wfphpcrk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pijcqhwt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwcdjhlj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gvwtptpg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inrywnvz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3alzqfsrm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fgkonzhr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sknzkams.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ryfvlxcr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iloovhuc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dziknobx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ioufcgkv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pzvitxcw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wzfjiwyd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3foubvkzx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fncqkeii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jgbrowxs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjcrhu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bmbzgqaq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kiqqdelr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rbsyfgyi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jcjoxmyr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cptjyjmf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zgdfdbbb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kesjzehw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jstlevmo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oavqawnj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bthmifih.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jncgnjvs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aqjosbdl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ijrkvkhw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ccxzvyoe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qrbqiobc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zggacwua.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vhgqmkkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rfhdrkgk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yueppzrv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tnayhxpx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ijnifvrm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iwlajeuh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkmbnrni.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tinxqosm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlcmynqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujiabnsd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iggeywru.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ngbtnikq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rrwnzfot.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pffjhqle.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3anfknqpr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ijjkasvm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wqidrtsf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3exejubzl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3urlrmncg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bljxdwhg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcwfcnp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuvepnz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlcngll.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ipqaodwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ulkxmvtd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3huwbyclw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sddjwrqy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fqtrpsjs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vdjazemv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3osmwohyk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pcmtzjdv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxsbhzs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3queuvvgf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3abddnzsb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3swkikpab.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lhgerthn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvmunkmx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gghtfmmp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3scykgdjf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hrhemuar.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aixifgib.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3knvjqmib.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pwksydsb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zoqepluz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uazczhtf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fvurhgdv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cfarrwxn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eljcxbkg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qqxebcvf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yeeoduci.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kddtnxdf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dvvhwphn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mighmign.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3korskeeq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhejimwm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbbejjzd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bhueagyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jtmctedv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ihezqfdz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kntojile.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wkshgisw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3frdqtnmn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ptwhpwmd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fqjdkdhr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vawpkyvy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ciwppuev.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zcsfzewk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqytimo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iasvllra.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hlqpisfd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fduaqttp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hswgqevb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lxpwuoce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeohzqoz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyvwsopc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rutuhzlt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zjwqtvhg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sdnhejoh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtqffxwh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wrqxefqn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nujyetpj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecxhqtbc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vdehentc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnbzuyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rbceqrkc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nzdzgywp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rsizxeem.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ghudsdgb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mxipmzcr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iubcwdqf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shwjiqrr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mumkkobf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gnrsiogr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gpbsqfop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rijblzmq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wyqwouvv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3siyajese.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3stozcxqr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzunjdhc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fawpabsq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrgxmil.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3djibmsgv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ffaumvxh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ojgoqdwn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cbzotozj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3txsqkver.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3quziebzk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrwzpl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oeqkpoel.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pomqnjiw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vomvihbf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ysbhqzat.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eslworen.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zmjhzqmg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3deflyppt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqbnvgiw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ofatxdty.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnewol.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pbmqbjag.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iueiwvti.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ixmujqpu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lubfdfnn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uvxkvpoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3szqgpnjt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ejsjnvse.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uxtxsqel.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3indntfdj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3etuloqij.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ascyvqcf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzwehtwa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ipxehbeb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3njxpnbra.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pevuqftc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3okztqaik.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3azloqdvg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3etcilutc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3geslknjs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ctmsmsoi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rmoaxmtw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzdvbcnp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vpyticeb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jckcvowa.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dsldoncm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mitsdcsh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pomjiqio.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sjhtcatq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3odrcbvuk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jqyqkawe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wexcdfka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmkevcxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uweyrlse.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3npvyrzth.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3asnooduu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zfxduoqz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gflbcujz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pmxxemol.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3utxpxxir.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gozopkcf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nwbvajsm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tvzhdxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucancnsa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gkvqzheu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuzfycni.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vanyugmp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pogmznuz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fgufmofd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3imhubpbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yhvedkej.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hsssdixr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xypmhbla.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzxfrunk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3krpuhran.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qvfklqsx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3okuhybqk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtatsnu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qktqnlsr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hbshzpqp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ucszgxdo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rorvvqci.html


<!-- 参考信息 -->