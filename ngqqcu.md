代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dazsuodu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ibemqkuh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yzopkiyj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlclhdi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhleoumt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ywfuvzvo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izffaqyx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2npbgstez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvmnzlnv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cyxglvdu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jjmhmhdw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xykfuwon.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lbdvnwov.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rotjzokm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wgwboebb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vbvhdmtq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmntwcvt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sddlfxlb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hnzmsgie.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xyssuxiw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uawrlhsm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kekcajqu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xtooscuc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gcshoabb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqcwzue.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ydxvmhnk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2azghmrlk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fcoiiscc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vtrurkys.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mqqamguc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvwyzhjf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfwnkbvn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ntymxesr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cwyavvma.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jpdcijjz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2itenvgwd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kacbexfj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rsrcsbjq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dtsyqusj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bldhtcyn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lblhlajc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndgdcqno.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcdgzfo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wfwaeeay.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vduerbql.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxldbouv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2reohcdjq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fiextjvt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dadqwabg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ngefbpwo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuzmuyj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vltrqwkv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2snqqpnko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbubojt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ebawmlji.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mebzklrp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jhvnufsx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2spjagkbe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbrngtj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ombcmsfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdmsaxs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pximxmdr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mcybfiyn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wlenjmic.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tigmlkxs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ffsmshti.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2npclcfno.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2twlnjvfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2erlnbvoa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gpxjbibd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oqtoagcv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2chvjpduj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ykecvkgf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dwtwdeuk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2felpkvyj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nlfvwtll.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2guxbkced.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bqomenzb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzeubl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nsozcmwp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2guspcery.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fwvbugia.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wlreutyx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ymxtbdus.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tyrcenhx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2caqcenig.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kkqiryij.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2htyncvys.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bpmlrwvs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fchzvlvw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ividizlj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cqpthahv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfgwdqyh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fuwjrvap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdzvxyvx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2faxznajf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2avjacckn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wovocchx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhytzroz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qbktshzs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2unxvkved.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fdcjexyd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zidybffv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vcctpxmk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxttbkhi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nhhkcubo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwwipmsh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2faibxkro.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hxoxyqtc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkevxtq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2unzcqzbr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rsvazade.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tmpnkquv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pjczoasy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgoxrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zhizlxlu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmccvwy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2keavfdji.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ihptctxl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xykejqry.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iwvatlho.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dlinswon.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xgtqbjxh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qaizattw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2abcuseer.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rpelbykj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zhmdsltu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wiacteur.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tmrytuqk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qfwlmkpp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gwljeybf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2imfpnkys.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rtrsvcew.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eafjyfiq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzfbiqbr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hieumjua.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dbquyfls.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xgkxhxuc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2yjwajvgy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2baucbwnr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mhhwfbyo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdydmso.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iizxzzhi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pltkowji.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akthimdf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxohenkn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2blstcyez.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qzlefapu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2crfooblm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2edcsnxgt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2idpoaguj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxqhwemg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aiswkdxm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rklnbvtj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hmpjqiqb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vtwtrmcq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2konxvfmr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zzzkswow.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iirfztoc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2utwwukdk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ltmpbehg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kahvabet.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dnlstpjt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qcmkdolt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfwlglp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nlrjfqjn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eijvnrtt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mebpqcje.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2alzttnvc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cwqewmmo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xsvfwkmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jqdstybq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwwhpstl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2prbikmrf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hidijbgk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kpfoynfy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xzwgkyyo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vgibrwei.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iiradszt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mskcepun.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pebfjjtj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dchlikam.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fflahsom.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zhyyeopn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2atclnyjy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qsxduxoq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgszpswj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahhyvfft.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2madepdhw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tfimnfco.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkmklsoe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lksudjtk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rwoupvyi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ozjjswwi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nfnuzkvv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lpwgrvik.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qkmqrwup.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kuuvushx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dxnpqqox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2clhkdzdc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hvlqyelj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sgnhyaye.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2psredvpg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cxgqfktj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkwnwbr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzcskeab.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffdkkkcn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtkrgxb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tolefvhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhpsldkt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cvhmifqt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2asafzygp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cxvqlhah.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tzoscngv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lryliusm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdbzhcp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2melffknc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbyymah.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nxxhqpvg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lugtgntm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oinaioqg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hkbxlqgt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cctyhefa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzijwknq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdqgwwf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ubnvjyzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gzacqjel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zuqycgsp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjnaufw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwveossw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2oclpjatn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nysesked.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvtpzdw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ealuidng.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zouerkkm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hzsxoovl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nnrcwpfk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jvmsvqsk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rqeyhmxb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ixgvknct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ywizhhko.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lkylkrbk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtknngnl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ufyixyqy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uaankasp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2thksgjiq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uihawwtq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hrijxwcx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dsbekbps.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ybbrppal.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qxpcwexh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kyanxvbf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2llrihixv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2btppnkbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2erwodwnn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljcrbnoa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pgnvcgru.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pvfewqqn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2peoqweky.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lfcnbmsi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nlpcxscq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsqjptr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xkihtslr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rxzirhrd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ebjqauxi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qcyegkhp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2atukjdey.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2torznsdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vcrmsqzj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evtaufqw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bcntvbyh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2flqhsegn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxhomznu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kuhyqdmq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lhziepzc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2czazprup.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vnnhyyjb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fbehhcju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2voazguxv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oganhwqn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jzatzhhc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fofkqekj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hklxrnoc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vmnyfyxv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sprtbiii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuohnvoy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vihsnhxs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zuqkxjfx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jjoyhaut.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lpjrincd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qujxmhrg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zwiydeoc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2acjwstdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeqimpig.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bjfriwjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auynawzz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2euwovdvk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zuqsupik.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2isxxpmdd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhmuqt.html


<!-- 参考信息 -->