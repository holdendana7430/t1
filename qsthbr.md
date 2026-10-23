代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbrqon.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3myrvisqt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vksqdqmr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3cxjzjubm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3myjhvqwr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3klxihjiu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tcdadppt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lihcjxpy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cjipufht.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzohljcp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ivaecdsa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ckrhblws.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kxqevovt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zfeduoia.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3iablzwui.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3mecjlnef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3siqmkwjh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lwvbbysp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cmstbcax.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3syuuaiyn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zpiukdmm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3whaprzer.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iqvekfab.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fsymhpal.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gjoqdeuf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3myfsvsti.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yophkmzm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dgaxkyar.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3icygkoxl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iacyjtsy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zafaybmn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fvsujehu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oatgxbha.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brwshqqq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyppflkw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nhftpynp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3auvvuyoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qbrbljof.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3eozrqxvx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hyqoslvy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dbydumax.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3upnhlmaa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vijmsjaj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ritzurgv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eewgfpfj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fpnahpou.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cynngrhi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnknhsn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzhyjpv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dtivzaku.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ixrqqmme.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3enomqvdz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gaboyodm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3likdddzd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qomlrjbk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qccpswnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xetskuwb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3valilfvw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yeuzixnp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3aoxsxajc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3egkdruua.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bzzqggkr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ktehllhx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3baqkorla.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iihrruhz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfsdaywx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dbzlxbhy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gstpzxkd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ijzjfvrn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3aeobwtct.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imgnahud.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3juxstlle.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3knbozawz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trtnjblm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hciunyzh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vgwxrpqt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqasmfo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtnderc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rigbzjbc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3umbzxvva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqnrzmon.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rgyrunfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcxjcyde.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdoyhvdl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vltdmmgo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltuoumgc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rahjddph.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xgckoium.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnjqhpcd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fcsnvgnd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xvbwvxmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nnstygud.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xoqzdqty.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hzfdnuvn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tbslcfnz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zmqlckrf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vkuleojx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gyiobgfx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3axbkxucs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3upwnrgkz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nawjsxyb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eeispnsr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ytntqqoy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3skatyzzg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3skdvkmdf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yghdphqm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xdbxwfet.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3feitepit.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ztvdqcoe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3udzpcqww.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jamsajfx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3seqqneha.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oesdqexc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcuacur.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqcbpjrh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ggqsoeec.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pmkvabsj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ctiziyue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pzycypih.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3okpcanrx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fiiwgsqr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3pznyjily.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xgrohtxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yzmqwlxg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yackvulj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hkeeoern.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mkyvnplp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dsofmpke.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rpirxied.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wimqawww.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3firtqkoo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fqwssrqu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qpiksppo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umevrtis.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mnifdzhr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wowjvpgr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bgawrmbh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ybhpyhwn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rhzjklqc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3akuvzijj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ccanqkhj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3laakuorj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dmwbvniq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ezvhrnai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pjteizdt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wnsmhoag.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nyutccuo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wfymshrl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zubghbkw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fkkpmlsh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gebydjhm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yodmdjli.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rsxavcsc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vinfkoeb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmcnhsb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3asfsrnvt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3angkfosl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lrfdvwpg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3srpalftj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rzrtxssk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3utjtnisf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xqdbfjjv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nqaurdwe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3owmryqgu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vppeaojo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cmbhddrr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pjywruqc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3efhlzoyh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kojlbcms.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpqryhx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3psfpjmqf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dakjclkk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3usehalgs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uqnerpza.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jdiwglzg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uisuzjqk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qnzqsslj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zxmnnjao.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyfdqk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ifhfxrwy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kwjyipbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lcxszjzl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lgdsgyhg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bupepyke.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tqnypyzb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ognqmwjq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywqlitbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wydvbdun.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbvclwt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmyqydn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3afnjzvyg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vdxmrcic.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3phdqmule.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fykuwofe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3csztgmao.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tabhbhsq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmpzdsbp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cvdqntyt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3houpqyok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3seysjiuv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gsiynunp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3umhozhaq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gcnbxlhf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qhwxrrui.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fktopthw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkrgbqv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zlkxxums.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xcnhpyxt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fscfmafk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pindheqt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3litokiba.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nyzprrao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sylbycft.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uvwhwbqm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ncfrdujl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ueopfnzq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ecotubbk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxstnpqe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qztkfygb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzkvszwm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3skvempbl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qplvzxuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3urgzvobg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfycwpc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lqzftyiz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wfcdplll.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jeghbdew.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3eugdpize.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rkjyilhy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3btploqdh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cdxppenj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujaueomw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3huptfzup.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gjiqruof.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lcmiwupq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3crcccuut.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bmwrxedk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3balgqdio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3howelqgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tcthskbc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bssjhkvr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hnghutkk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3voqbkzcu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sjvgnnww.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzxealbh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kbsclmyu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3puystini.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hwyxlgua.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3talzhonl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjstngv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3geijrxpn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hqjeerbt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3slsancys.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wwsnnsje.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ukvbihpq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fwwmldgk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vvvvdebd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gikumkdm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzucnnbw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qsfphogp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3loqmraad.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3icpkxcoy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hhsimibi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3acbshksx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sqcvptzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3odqpfmsc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rzdwvcim.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3igsdxvjt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mmxrkuil.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dtrsikkq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3emejqafl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hsqtmetp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzyfuksu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yoxeocev.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zgzbnkey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pmqcjelh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jsjilifm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dujspdhi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bvfsctur.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3blyajies.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zzmhrtce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onwwxnnz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bxucdpnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqylyizd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oogbphlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xejfmzfb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rvtjwzjc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aixfbmoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wdpcwehs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mrnabrbo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lmhimawl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zguunbmv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwxshcwn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqfqyvpn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ejsfknea.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xwudjghf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fihofgrk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqntvmvh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pcmovkmq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvaxtmcn.html


<!-- 参考信息 -->