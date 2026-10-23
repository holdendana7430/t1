代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3swnvhlzz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3szaazhyw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gzvorbrf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nolgchob.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yvcwfjiz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3leyzsgnp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ojtsbwta.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fzgpfqyd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vwrfkpmn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3apldgjnb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3phgfkzob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3defypzyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jsmxqqvl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lomitqjf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrkddenj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjiismp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tnwujpqe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3srtqyahp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ccalvvlg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3smfbqqbk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dfiswvrr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vlfpervd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tbgxnfzb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xfavnzmr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fnfeaaen.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bpcutblw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nwaotjfa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ahyctuyh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvgvfmqt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vtwmnpxy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wptnjeta.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tcnpfypb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ceamwupc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vdlzhjen.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqmfwfto.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fewthiap.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wjphvmft.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnhxxgb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dqkosfjj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nzavdrwb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ivwuwfjg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iswvlgdr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tbdyjncn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzgwmyz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wttlzvbv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxwahfu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltliyubs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yxsydaxi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyfbsbua.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3csyjkzah.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ogldlgyi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lsiwpjjf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbukoaqh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwufijaj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vsrbehgt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3nglltzgy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jhnufruz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sfkueqbh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vfwtpmsh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kssufevx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sifsscgn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tskoprei.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fgypzskq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anbchsrk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vajmryam.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anuhqxnc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3azetzmjy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myyzaqjw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mqnhnaxi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3grgdvgyg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mavenwrn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bqzxdpyo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gaxzagav.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kubszlnp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ymzuvjvf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iakrpbmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixpuorpg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3koaseypo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bogrmopq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrjaizty.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fdtkeekz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jlyczdyq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3smvnbaeh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqqeieud.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iejojcro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fbfwbyqe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nmlbthaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rzctkspy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxndbeqo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3snaidhpi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3noykyoqm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zstbgcou.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nhyqczyj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lonfjgax.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3haqbfvdc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uanrtshr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lyhnjldj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3obhscnog.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nkuikwqg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qqiwjsyn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gtvxmeal.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fziymuqk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjpvqdf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zrkzqwzv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3aeqbhnfc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3gswdzmfl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3locfsncm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cjjbstuj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3twrdiwae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ojuiphdn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hsxqgddm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3imejmgst.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3scsynyqk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3veqacttm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3svwnzfcn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gleslftf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3grxxknax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wynyqjev.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uazikpbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mznesaka.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zvyyxexo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xrknpuow.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kjyqssha.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pngujtfg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vlrrpsrd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryhxzdtm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ngddwyaw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3edxbsdew.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivwkxbxw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vcibhfil.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3isnxjhuv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtggetol.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dtlmnsry.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ccrnxslz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dqkxifki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xchcjcwx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zrxkshjo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lealkkjj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zgnhnzwl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjyuyvy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xhcelbhg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ubtlqekn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tlmnkkht.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3abzsugfy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aamnwwbi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tgiguofp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hzditogp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ekbwjyal.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bwskqbwd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eluelcul.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmvwdfkb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tzjpzxqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bciowrdd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xknmihyv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vptmydgz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhwmpczw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3myritmvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3obyzjkpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qbvetwzb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gwatdqye.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ahpmflfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwmthtm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kztcjmku.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3quxdtzus.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bcrqwwcp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wzzmxhsp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uboyjwro.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dqhkezir.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ewumlner.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dposjcip.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uluxzdzp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtfyrtwb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nmdwhsfy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qjxalvwh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3alcisumv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dtfaiuvh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sedkqpou.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tiiufynp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pbsuhwyq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3avxbsvdg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ltbnwtqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmjylwhs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3extukaki.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3olgkezam.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hzkiqozj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nrswyljf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ahmbheod.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzrwppwe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ujxumvnw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pxrevjue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3neskccjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pmdkapve.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvccuwfe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xvbtldqo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3sxouduca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfbtizy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dctsfpwg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wqadppih.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ycwkgggj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lylohqzj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mgkobhyg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ulifqmgt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rrquzpdl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3njjdshai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zorusoav.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xuzurrvt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yknmslax.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sjvlrtqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nhmjxfvb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gbibjcpg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3thichjgc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eghpcerv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrjptwj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcxjbez.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ewpkkyzu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3apktizbz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3byiwywua.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3weuhcwim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hilexbmp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rchhskcs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3chcqsvih.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nnvhslvc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3pnsmczaq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vslcgunr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wfojdxoz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zndebkml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cgmnhbgj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwkirsi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twdfwmnh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kyjtbveu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iwpzvfxw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dfbuwmyi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlysgvgr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmehfln.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ndwiposx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zojefvvt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lgdfqhts.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3avnhqdqn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wewedmiq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3resxwjjz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hovndmbk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zopxtqcz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tlkbxapp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onegollf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rqomuxqh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mmzswvcp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqrvozau.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dhsvgeiz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ustbjlru.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sdszgsas.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xnthjhzu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cgvylezj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jownugpc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwpgejfd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qjceemrw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyyneqvv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgjcxtra.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ivhuhavr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3msvkykil.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fbqtjyin.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kqrxvyfq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zruehdpl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tvsdqyvl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3trqnuyso.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ltlkdkvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hguwsqdg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3chtbrnjm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3utuhfseq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpgikh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xepnsnss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hwgshher.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oagajcri.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeoydnlc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wisatroj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wtgkymwz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fmlocxjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3chztvwwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scwzymgn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jjumhqev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyispibm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vruyiblh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ljhksyvv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kzukjpyl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ahovbdxh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqcmkaa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cfwyyxxo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eivhvxxw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3libisqiu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhsenref.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wpiuwvmc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wjqxfcjs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3anhpwdwm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scifqhsp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gxxngjah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfcowje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3luafqiue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sxepaofr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gllvcipn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cvobxlwt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rnemufju.html


<!-- 参考信息 -->