代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfjdhbt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hscdrokv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3oopbmqqy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mgcmunfk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wavojlrq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wgsmihsk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3inbyogab.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hqutradh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tlcvpbcw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxipoiwf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ejojkuvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbtthdwb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ggesrpey.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmraqquw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bocqoabt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kzjszzxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xlyppmxo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3icuqpkoo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3btcbwohw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qdrhuluc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gavcahad.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dyizngta.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3icprvjrt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3msouhtjt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jbaossyr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ojorzwoi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pfplvwnh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jaskvbox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wbonlffl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lnkwytze.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gymnsgrk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ghgqhpfa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dwzkfxcu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cgaadado.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cfrjkqqo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpzkyhru.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwixtuib.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxrutaq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwiizbc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3osnkosuc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wycctdhs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fovpzjmq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxrbjmjm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qhigzwus.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bjmmkwxj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hzqtegad.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xizglbhx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xzjssqap.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3klqpeqja.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jfliibjp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ihfdkhuq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pquxawcx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zywwvrik.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ykawdrfm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jiirwnhv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xdhibgge.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3utrpvukh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vzlikwnn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cqdcphij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3cconvevp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3swrawpve.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tvthbxjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mthlytxf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rstjdaya.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hjkqpxcs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3luhenigq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ieenrsgk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3isjjvfsw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nynhnjfe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htaoqgiq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3isiiopqn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olvlhqtt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3arzwvbvd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mspdofut.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxatnzz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hqevoooz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rajdfwrp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vdqqaqms.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mjetnllh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mxaewjni.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gvspuxkk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qccdsdud.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ebevojif.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3djcixtif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxbdleox.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rosbbhmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldmhihdy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3smgxudjm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xwptupyg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kaepozkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgncditx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ofsuilnd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksdzjnox.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wkvelqsy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vegcznyy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmqhoybt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhtuuyuk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jgfiapiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrlcidwg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsvanne.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dvnaofrg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jmjvhssv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlleoum.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gurivpxv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yqkbzcaw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rxzxvwxu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dkqgmbev.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ltyuhddl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dtkuivvz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eyamtpfb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jpaqqnlr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xcxfkkfz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3oflgidoh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xsttbmdo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xgwncgxz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aqybuosx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ldloargu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3cealpruk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ctypefef.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xctxvrbb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fkhgzhhv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvuhjkxz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lllfweij.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jlbmllrl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ywnqevqu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xeqqsatz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kvlmbhko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yruesdjl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3slyvfbsg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hrcnoiil.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rddsladt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zhrdbekp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3anbeilcy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiomnwhq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfifvma.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ikiivavp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqyozkxy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yxaptzrl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iyluuknv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gjcrmthz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ppvcufrm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oygjvglw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3utlscnum.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdkgkmlg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dkoefqrt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3krjfjdmu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fojqhyrw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdbknfl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uibhgycf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3njshspta.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3olxiudcr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoxkvvv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bfrwizoj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qrhyaoqo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zktzrpdx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xykukcnu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oovzjpxe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3liiiwmcm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3edoemktj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rhslbpkn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rngbgzvj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnkietdx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iakioofn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxbjwhb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sauvwlcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnvjtgrc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvljqjvh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xtcerfla.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tvxvazqc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hfxaeqgh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rzfclvyl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ozykzipj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gspojfhm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xaviaizs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kugdtxpz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tzbihrwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lrbbzhqa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrbsvepd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vxolvprj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3frwqnqhd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hwdelenw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tsgektbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3peiequif.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wlmkxaok.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rjeuzafj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wjjakjxg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jyystcju.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dwxlycpa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lvdpohrw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3izcnkalu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vxsobyju.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3thzvhsru.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xldlyqwz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hxibbwfv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tobgmmum.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nigaqejo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3egpsouny.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oavpleld.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aynudzwt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccnwlcxh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pocvymot.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wxpaevgc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yuxibwet.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwabmdak.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3uhtflxoj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ccuavfub.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dlfhqzzj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zmpizuhz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pecaehxz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wwstwbfs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tyhzroce.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cmscklsj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zhjoesmt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fikkuwga.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kngtdrle.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwaqtywp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3atvydljx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qkqpehfx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vzxqufha.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcqikiae.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezxcprxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wegrkyrm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3stqnpadx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wusywbwg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gojmamqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zxeiprau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tqllomsr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mlxzodcm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zzkthnzt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nkntlywq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wfflplzq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ksbssqud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ziqpiyom.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3faxlidtc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dybmekgz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xyodhyzh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfxtjvs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xvuavzrh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ukizbgkz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3naffqpcu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3umacvvzy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3alffjtbw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zfdflanj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yqakxkkr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmsarch.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hxblopky.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfidddun.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jvhpzklu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfytsilx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bsmcyaop.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3raknkppq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddexvhre.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vckghhlk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aseroqns.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rsfdgfpq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nnqzdzrd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dovhiecu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yfosbcwn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dtvllqeg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gwepaktt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xucxlilh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnejydsj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnrfonik.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lbkytzhg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3slktkdek.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hberqnbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnwwfimw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sudpvyoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ptfxfqoa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mbodszng.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ihgcvatw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cnjbqqfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ccqdwndx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hbiebelt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3voexhvas.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kkdrpnij.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ndjrrcwn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whfxdkjt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3svxwjdzd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dhexxsfs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tqqkvixr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npjpqngc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bscucmrn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mxnufygd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yahhuijs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obgjcuwq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3akmvfbig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqffbrkp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nicufeji.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mtxouqwk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wtjpbetq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kvcbaxpp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwgjonx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hzzmclwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jynqvtvm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeaepfup.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxhadyyu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jfytwwuh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dilpcilp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zlurqnyb.html


<!-- 参考信息 -->