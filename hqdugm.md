代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwiaulqd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vhzvurfr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jcohhhwp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rqxmgkbs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dkhzjizs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ssshbaxg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3eheoxuzg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zseogazl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rcrjpaao.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxzklkdr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3clvrjgyx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eiyncjix.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yxvszlzx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mpbckckw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uqcfgojp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dhhkmosu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3urdaarvf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fjgqvzkt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ujjwsicz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3buveroqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wrujhsvi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3czxnsgej.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpejqeix.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfgconym.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sjyijtat.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yuoafopz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wwvhmtix.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ebxeaiut.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3subunvwa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zmoxhagm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kossefft.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ypcrfaxf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3khulohcn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkterpf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tylfupex.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mvacihxd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iiavpbjj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hjkdvyfb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkaounvt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mwnspwnh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3oriirxqa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cjamjqpy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhquhpdo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hqkbpxxg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zvpftxuq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3slfalwoq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cdqmhmdf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3evivnofh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qjboplub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pwlqtqfb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gaeynybx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrjkhnel.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbpwosj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqfeifo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jnsnomaz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uuvsjkmi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3noiaokfl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fxoqthrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3euosrddz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vebszseg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3txdmbbtv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xozbjsmo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ygxwtins.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bfvrggzt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pjurpcxt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kdittwyz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dfkjqdmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvrinv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3phpngxhn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyitramj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtzhewqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hplxgocr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uydwkamz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmdkykg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sidjtlmc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdiboqau.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvvsglsw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ckpozfkt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ufqzcemy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mqhnatzt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iraxvvna.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bnqpsmqa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nfnlawum.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nycvwuge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbhqdwvp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cuvcwsle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drjdhidm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kwgndlbh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3endedbmu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gvcdrtjy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfnxymwi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tgqqseie.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tydrpiba.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hdsiprcz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zsoauvbj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwgtlczw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvmobayo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ovhgsybl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwkvamke.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zuivyeeq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qximcbye.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fozfmelu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yawwtwwf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3orldovlj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3svoezhkk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zvxzvjyk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3szrfhict.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijidspan.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwthjxq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nrevuunz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ocuquoio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kmiudvok.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ganwfydf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mlyrroku.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nmtntowz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eycjryyb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vygvxyha.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gfywfoqc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3scrcskqa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qehdsqdv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nsxneqgd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dvpwrdil.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fgjjvryp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3iqpyxbmh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cjohpesb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lpzqczby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddsygwch.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmxjyr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ytbfjegf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lgozeyvz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mmdsxkny.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dfvawhct.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qjbrqpvs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vfhsqsrp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qwlcjwhm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3toceccdn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jtxfovyl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mxdsrxrz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaczvfqj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uplmrlez.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxhcbtxb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ngbitygj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mvzmqjrp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zikpiubm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oyolfujj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wrqusjpl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rslvhosh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gofwfpgs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pufzhhct.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqshbua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tlpfmugp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3avfjajlk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ysemvazm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jnfzkgdh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ymrshoyv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vnxzasqb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qzufvajj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3awyotdaj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3llycdxjr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nqseloxc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcctfgxd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwztxuvq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uziibbty.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ogyqbxha.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bnaibonr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmhwduko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzcwkzdd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3soimrxie.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zbzycwid.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nlaioczd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hgxtvlna.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wqkadrwq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iggqmfmu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxzkaz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3patkhlvy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpxkifu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mrzdrzmc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brzrokeq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3poxflanf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bxmqvbby.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3skwgtdwz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clqzsgwx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3anqesjjq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rkbadydb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wbetwmld.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ctamicyd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cuxumifj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dhhvslqf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dgbywkxx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwibhqzt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lweiyyxa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3eazjduir.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3otlrcfff.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gpabjgkn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3soqjxugq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dpgaahiw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3atoyiblg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cfktsefz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqxfgvw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ephhjfal.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zudxload.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xbcwnong.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nienvzhq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhxjdcgl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3elgveaop.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qfccqbek.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ikppjbou.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xwmzuodq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atiyujqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wusctqgg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3flwkbsyz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xszzlaro.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3khvvbzyi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dpuzegpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lncxifef.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tboqtnyc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ewefigtn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rnnixcpf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mtloadcc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjgkml.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bwroeyle.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxujjcfn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dwxaervk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkhmeexp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eqijiehr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3afpjkrnz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kjppgeud.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgvdrlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3eckosmws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cmbtilav.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3byebzvad.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nixsgrpm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jarrouuk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvivkrck.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qlwnyeff.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvjchhs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iprdbkio.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dbowxbzw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iumnswjc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bbqprisl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eejiwswa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jhijrcne.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwpssua.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gasisles.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vovcromz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eejinxbu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3epvbppko.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zofdtrwr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vuybroza.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gbomckrt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uvvbxywp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ojvvjwuy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3irfujmxh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vfhewojt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wslmnqru.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jbxvmnqq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3aywscyda.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jhuhgxbj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nuwzncke.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pjecpkpp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xaikbwsu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snsgpxng.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjeoymll.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvvpscpu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mkhvhuca.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ezfzkjhu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3geqmouvv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fbqzenbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wjuyennj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vqzjwipr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qnoirdwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3opsqqzjk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qzscossi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdhzzb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewwiczdu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3txdysylh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hussoktw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yijwqdlq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pfcjrwlx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kycmldva.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oenjapyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tlmqbctu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jmmngmxq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pbemsaex.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jpdqvrqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxmlheop.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3weutejiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwtyivrm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqdirzwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gapjdzxf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odevugxg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wyspoojh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jltbaesi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rzjpkjut.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3slrzulmm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmtasulc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfvwbiqr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3achybsyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rgiynvtg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkzvyru.html


<!-- 参考信息 -->