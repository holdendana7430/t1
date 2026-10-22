代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qrcispxv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vqatclzb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xwrwotbu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvckonla.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2frskykgt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtoawdol.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zyaxvlww.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wdvyigpo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sopvlxjx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cgglsopv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2deluzcvw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gnnlhmag.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2umapvigm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2licprlbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnpxvds.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cfgwrgec.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ufrydzmy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nrdfhkfh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ijajehmi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxkurcgs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nodltbbf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mbtfhgla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2khjywuzr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2koaivrpl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2viyniguc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ornqikfh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mnopgpsz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nvyovvqg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wvgwgmzt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2psoumyyu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvllrfzd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lyhwlknk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ilgzazdk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xfxkubkl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qehiwyym.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ycmfwojg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lvoratbg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fvzsyuee.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uuoevkkz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vdzrlrcu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mlofawwe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdjnikwq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2quiowcwi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2axiwkpwr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2csaqstrf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lnpfoacx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2edbvfpej.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vvhgzvvg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojcucsvz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nnpmcveb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcpktst.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pnodqxya.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dxwnchwr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xitslboq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kftvswuk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ukxxexey.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2riqtlbyw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwzqmhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hzopuaxa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rplrequk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ymwbgebq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hjoxetwe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eucpbeqm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gfedmjxo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mgoorlzw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yogflfbd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhepmtp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcqenppt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ootbikoq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezimaizn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jdtkdsba.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aiwtyerm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vayahvuy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jzxpupng.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fkcshtkj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2iahgrsqp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pchkgkey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2shccnpvg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jqzzruzy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajwueytl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wifxeign.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqyzjvdd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2amuvxoxd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvctqyhk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qgayxrpj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2otcpokly.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cnqvfhko.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ellcbiey.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uavupvku.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uptqytom.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hhrfidzs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fcczoygl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftcbmavt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmncftgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tunuhkdg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qqukseyb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xqxwwurl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtazlhrs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cbkgojyw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xmwpxusz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzcxnmii.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nyqbaivi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vexiahwh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktwjfanf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvschrhd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oikcbomt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vxvbsbtp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhluhpuz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ynpxlhck.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wapbkudi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqelqtsx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tnpvdffi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bwypngpv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2edtsxbwl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xucpqfjh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iuybjulj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kzzezoyg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2akeywcie.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2whwsewrj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jczmmfhr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ugzqvamg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rcykwyqq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aovjyssi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jucrtrno.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cqswcawt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbhjlfg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gihrmsdd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xmdeiztv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2katlnucv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kbhpewyo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2quczkueg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ctykxbtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fzvcxvka.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zdncsytl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cbjtpsur.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aopflait.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tkokqgry.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2guvpwzjx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjxicao.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2apfymqbz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jtreobzi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jhvhmdlz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gzusewgg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxihetwa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rkkuzdhq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ntmlussj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fxwchand.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gvrbqlom.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wwbuwios.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2crrmmqlh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ooxtqpok.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bstlexpi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhcvysot.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mushdeyw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvqard.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrblypof.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rbepopxh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kvpskqkd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dutmjhbl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ixdzihxf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jsfsvgcr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tfkqaxsk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uvdxcffy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ixwzhwfj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lfliucah.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ngskbvrn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ohepjhct.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bcztafqm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhaozfv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ysdndedv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhkbhcvg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fszcaouq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2inoubpag.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2inyekhpu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kktmmqrw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2obpnniub.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kxpatdvp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hvddblce.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jygcbdzb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vukobdhb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ipsbbidl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tcttlzsj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vcsyxboj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tlgyylnp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rgwehilt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dyfsbixn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2phckteyc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ezbzlzsn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rsurnclv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfxtzwsq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dfwxmlxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xzonsrlk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2equdjxfs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kimbrhug.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kfuvowod.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nxwhkqhw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2woxsaqhx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bxfumalg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zpoasdvj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2siafralz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvxetbbc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nzlactnc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ndsxbxby.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fytudqxy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hmpqxiih.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zzdfayvf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2crtqpgnn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2shlwtbvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2esmkdzfm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zseizcdy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uzdozple.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nzyjvpdw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rkyewbcf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2oejfclpb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfdedbzz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iceapeje.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wlxomxlj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjnkxru.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxkpyn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cgkvmxim.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jepgmpad.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2voufbwgp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vstlmxog.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fqlfctrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clvuiiwp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vztyiouc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ccbsrage.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lgutaqzt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akzfyjsv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gwlhulre.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cyonojyn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2engevitf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nxyicjvn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dgkwitxg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdytaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vvnqipww.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gnbiznqe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ttraxqbk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wkfuhswv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ibjdjiud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tdfpdsji.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gvcmfttg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pxggvfem.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zulhscsp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2akfkpgex.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bnzgfvuw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hyvvyhlx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jcacyfwp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2drsdaqwa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xlyzjgde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uhnfmisj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bcdxckcr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lskugjni.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ublotbiz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yiaultkf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rjxtcqbt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gfihixtx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qviewazz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ytucubqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjvlehg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gdnyodvt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jdusnngm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uhvboxeb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdgbnhz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ccrwclve.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xtzfxgpk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cvczkxkt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2thxhxwph.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kcjctkhh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tgzjcvxf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvwuzmyv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbwpvncl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcfamgxc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwczoq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mgguwolb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qaodcxju.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cjkbwunu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gzofzxjr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ejzivsmo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ecydylex.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2udrvmgbe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hlbsilpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mkukatwf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cixaolxa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hkovaewo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmyemgm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2syxbrhrj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptbzbzic.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rdtulmoz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pbtemdpl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2geqkddhv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tkzcicsy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ntssopbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kspwhaxw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kjjqppty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkzjelre.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2peikgoth.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tzayrstg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ianuqpkt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bdmlyoce.html


<!-- 参考信息 -->