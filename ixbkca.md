代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oedkmqlv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vveldcwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2llaryjyu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zvvotmfo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dybsfjvw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nooydaul.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hygzquxv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vczqukkz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vyaamhak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzbmcrd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbkdlru.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2otiltfwy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddsdurle.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aadvyeiv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ktmeikxx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bxjxofsj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xfuemfsv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dquqeuwy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2erpzyoop.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tzduqlqo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eatwpzai.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2padyggjt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mczfvefh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wkvbkzmm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zwlglmoh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2leticdty.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jjegizrf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2plpfcsgi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fbgtfjyb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xnlaidri.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gellmwbv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hociasui.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rafdjwhu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2olfnrdkh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vkqdzpad.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sahtrwfr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lniytiwn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zfbomimk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pmpqleat.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pseznbwg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2agegcrds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hoehxyfu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ukuvasiv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wbueegwk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vvufuzsx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gduepexp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjicdtc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kcxcovha.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hztstwlh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rxznecio.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jjvhxklw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ditcboxg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebhjxttu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fibybqyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgvlufp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ijgccxqd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ficbrqea.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yehrgfea.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zdquvjxv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yvllrpqy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mjglcifv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjnxxjm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xauhdgqs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kwepifim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnubepuk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbejaie.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gnnacpds.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2znsvfvxw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2maenssgg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ibjvritz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lcppcqbc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iirybvpk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtlfsvgg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwjygodw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hlvnhsoi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vezckpuc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgcnowi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wmzpqunn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ihkmdsxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vozmfqeo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lhzaipwk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rbxiqwlc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2davegyzt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twwsbmfh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nxaehdxb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fpvcdajz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bayppmxl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dqehusck.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ihqmnnux.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxftzxe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sonbnrgj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qqyfthlg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jxotqcjo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tigokkwf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2spinggfl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rskugpkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzlxbtfz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wbqglhkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cekxbqmi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxusjgbu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2smvdxohl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dtzqbckv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ewtnangs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2saanxnyi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gubpluky.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ftyovane.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xrscmhph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cjipruxh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pydcsfbr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2whhmtmzg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zlhbuypw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfnsxkv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ctdohtzb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzazkguz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ywihdciz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vyfbbeca.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlbbjx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eqxliebe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2napottyh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mkudwcbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bprbwwam.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2upqijpnp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqmyfps.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dkjwsscb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2grxgvlzm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nlxkqigg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2artuxypl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfauqs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ywmxruud.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2yvuyjoyl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2htoobdqo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iakpgxuk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dcuuuuzm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2veymhbda.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2psuqidzz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vjbkefwu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zzjgybhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2obqqfuic.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lorstaoy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mghemnwv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rorosruv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwrkslid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bdnmhlui.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhctuxqr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pdoooacf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgypxlc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xwmbqvyy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ucrxhnan.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cbjzmawk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2biufsvui.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eyaxsojp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dxujisot.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqmcmehp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2trowvykg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zhowlgjv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrjbmht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mmxfxcmd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2buibbwzd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oinmosht.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iokddohq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2toaqhivf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jcbefuea.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ijtchgkt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2erwjtvrf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gaoprino.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jifxxnpg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yephngne.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2znsrwbwe.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wdhtmtat.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2acvpbdnk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvfvcbm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vbitgual.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrlfjeeu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjcrhhmz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nhjrqmjp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gochqmxm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2inpgbszx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nydestlp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yxixefcv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2owfhxaye.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pbxsmldm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cgulzjeh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2atmhnvyo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2icqljlot.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qarojlxq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dvunjfwn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xbzexagz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nlmbnqlj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tryfreqk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2orvsztmj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2emlaisim.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qgtcfgla.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pzaespmo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wdzvumir.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2scndjctc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2baudyxpz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drifxkos.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2omnwrmcv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dqgdzuwo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eqzjubiq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2seejxtsg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qiolftgm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgejuuwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uofqppew.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2nnihmous.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tiwoetmq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pvwwisnu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ucnkuiaf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zvnwecia.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmhwmfa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qrfngedc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckehcakj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggcapqpk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lzjirglw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2haovacjx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkosajwb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2aneffvuo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2shgcqudp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mttxwinh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xxwxvhxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnhziqzo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qbivqlbp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bgprhean.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mdyratyy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2boltlkds.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hxckmear.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uoywdzxv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oypdagfb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ojvoyrxi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2omflaaoa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lzertpua.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ugawligl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcwybng.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2iidtzlvz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tzfahjsh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzvvpvub.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bkmvzlbi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rkrklatk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bspnjxna.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sctphpof.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qlnbnlat.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2chiazeup.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rxpxddch.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uqozdbwr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gjzlwayp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbemuati.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2muyabdwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cenbsbll.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajerqcrc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2llbfrkvb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pyaqjffk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jzkynsbw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vebuefzf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wrbqaori.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kpxfsdvm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aablrlvm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hpghpldj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2demboxwv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ncbtnrne.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2acvkhodz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dwgthyjy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vgomfldk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cvsnyald.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2efhecnwy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kraybfvl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzctmyf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2izuruurp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hhfjqcfg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cnzvklnk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2neijorop.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wmhxrdsm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2klpjxeuv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2eyazcpug.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tqgjqxgf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vndgtrnm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrpyebem.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xdnhvfaf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zsgqwbxu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2noqsjsri.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xgjrdfqr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mhqqdpek.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nmckdmbg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2acfbjvii.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lvuqdixi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gzxrptev.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ttcfpzmn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wdfjyuci.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbmdupxa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gjrhputb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bwukjprw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltldgkss.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yuffbtne.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dmwmgvwf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hibzqiyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sqeqlyuu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jssnvoxa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hlqlofxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkpwshfe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oqcopqrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlwachjs.html


<!-- 参考信息 -->