代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gbujpygq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ykjvmrtv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nawndvuo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vsqzbcds.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3anrbzcdf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3awjgswxx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bzhawsrk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bidxqpri.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3oepcmwxb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cbjvrywg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hohhmcot.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvgnwzde.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vrqwdqmi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfqjdn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wcrsnwrf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rsnkxpyw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wdypkhob.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jczdvosq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gyjtonwc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xpmuwcym.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rvilgkyz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrzuivw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ffjmjouz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zxojsxfs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aeobbkhj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zypeulgb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbbobjyk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pnvzwaeo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkgzswiy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zxhkkpdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyytrfzu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lcuecjxk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uedwbryv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tfqwhwta.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3trykcxqo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3feymjtbp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vioslzpb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dhuecbeg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvfkwyns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3peckbdep.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vpsdwbff.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dxkrvphj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3etzgfuyc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jevcfzus.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zttmprfw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pezmikbz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pipwkhcy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ggwgcvlm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osrsrkjg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3todhmsfz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3cflplgql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yuycywvp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xwmptdwd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tyeskpds.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lrhgqlhw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3msywkpfo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kipwrrgu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qczdqwpi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocooljyi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyrhbeu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zfxuetsk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qosrgedb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xzreefmz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pugcjytt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ksrqgdjc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cloxcpyf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dtyyzkfq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3byfjquac.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ntlxxjpl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tmaouwah.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3psguvfic.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgfuzkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ablijzbm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kljapols.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unycisct.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvgzxppt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3joafzfoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dirkcieh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lcqvlzxq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3evpcseku.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rkxbqewo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojogonfx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3snwgjhpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zzohjiud.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wnzkdegd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pedbgkbo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmavsvww.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cckhllpn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wqaoiyol.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmftgocy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gfgakrbg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fychuttl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xajjwrkg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cduheauz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3znkzfmgj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aphgspkf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3owyotkga.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mnvozqmb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xceedsqz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rkvhfsju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yspsoczm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3woqpltth.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kyryscgi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ydcyeops.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pjbzatnt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ufyizkgq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yztcakhe.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nulrebdz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3naddlpqo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdsmzxka.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kukxbvhg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cjmisknf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uziyzxhw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zuwpsnrn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3knqcowru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3okgfwhxv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3urcfaphr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lvqsfgan.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3orpemrcj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gvffbyvo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oiplleqk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rlrtxrss.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lsckegtn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ranfzhuf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xqxpturn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ikvzztyl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjxghpg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dacpqaar.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3edkisayt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wyccreln.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sohxfmmg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wwvbgubl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqqdirq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rbezxmre.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jgdfpwvc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hlxiscat.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jwlheswa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fzldgjdl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3idczkzfp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wxwxeejs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3akknvhhg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3laebodal.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ugfwyxhg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xxbmfjrf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pqsaigid.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3klegswkm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tzplpaxh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3azkksxzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ommlfrxj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbatuwsm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hajynelj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ldkdbybv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkkqcozs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hsbrvnkx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rrcbtnpq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wlutetwd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tbonnmls.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkbucfms.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uyazkqma.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3stxsaovk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3moijfeeq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vnqouitz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3losbkeum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvxtomi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tdhqmmag.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtqqjgag.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zygyqkew.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bosxiyyp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kyegoafg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rserptpx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uzzixylh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uyivbran.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ubwgviah.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vboaetiw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3soyufarr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fuhxnwmy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3oubwjncy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wqsrpplt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iijmsxqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dgjyjsbi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mckbiprq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fqkehhmd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mfkwnukf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ojpwmomo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rnjjlkod.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3boqlzysl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oznwqqfn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjravlby.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3spildzia.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ukdfpbek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hjliqrid.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dabxpbuf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3drjmtwau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jaypnfdx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjddcodq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3srzrbrve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nujvhhld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3etxkzbch.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3uyiorgoi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3grbvgvzh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nmsjsvui.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3opfigrxi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wnrhvwow.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fjijdguf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qxkkxljf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzkrbwbz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3itnagaxy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewugmzeo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zqjhqtpp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olrcrozr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vqzmaell.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmeyoafu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hykrhpfc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nwcfxnpt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3necdanof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zgtsfyfr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3edeqimsu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oryducyb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3felbqcin.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hguzoexg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3amzngyyd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyhabm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rffalkhk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kyczfxbn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tktonxxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wdrwpxde.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ncelrqnn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zmjnicrf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lziwwygw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3eqpglwta.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hdcsiwhi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpouehj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpywlbkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwcssgb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3igfpjncr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aheoiaau.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfslmg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lvlwrrun.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kookxzug.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hzjbhgfd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ielqlfkk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3grljqtvm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ktyudgbw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cghugtft.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3obfrjsya.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ovdmvicg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xianrnbm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kaimdocy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xchdsdnj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gguhwegh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aifpsmlb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqriztmr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fvcyccdu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lxjsedun.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acikcdni.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lnslnpxw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lewtqgdb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dfycnpci.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pxaurcep.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3llwufqsn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3talqryuw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ycawcldj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kaxhixxd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjhkudnh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rnrtprre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rzmbnaoo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mudxxnmc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3daptwpsb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dorhrgcj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pwuchrik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xcvzmsgx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jwxroqak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kmlkgdyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vszcwhus.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3efrybkar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqbynwjp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kcrixfpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lyamyftf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emgbepzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aupmefdw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rlsdlhay.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3shkotxyw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tjulhvwq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewjnydju.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcfqgfge.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cfsqpngm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3slvkayvz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqrwand.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3orazmcyj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lqusbpxk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rrwvxpww.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzcdnfyb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gyszxahd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fcdrnvwg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dvyucnvl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hnfjxrci.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ezingfyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fpnzeyaj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3albejjzg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3frnrbexw.html


<!-- 参考信息 -->