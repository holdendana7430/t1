代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozawjqlj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3eirmrjct.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nfktdnea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nhbazaqs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wuitdzhu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3uvzxlzye.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3siidckij.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uyoququq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3veashnzs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cqlhfxgo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pouhmrld.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oupvpeil.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xanjmgrh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqdswtc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3eclcmywr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3guxysgji.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmzmekg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3frwjqvdh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ktdxjkta.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wqwpfbth.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uarngbzl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bzltsjnb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpbzfnax.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnuaybzq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3okzkgwor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hdmoqiuz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3riqugphy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3njguxlic.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tagvmmfb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nrufelzr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3imjwvapy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wsrqyogh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3unwxikfm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bplkedde.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmtqdeh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pysfwiao.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cenvzjne.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bstpvupk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qnbtwcxx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pokotvac.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsoxqse.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yqanbaoa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imwqrsan.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kamtcukd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lvyofqry.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ceofeerg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ijeirkfl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbkojh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dqdnzvck.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oqmaozri.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wahuybha.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3krsbajgr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqkplxxl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgimpih.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jwiusefc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nhhnmmty.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xoilavep.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qnwdaapc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kkuwvsua.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvzvdmih.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3apngqept.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gucahunt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3malurtys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3embkdhcw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bxqrapsz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rxatwcof.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bmqhjens.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mfxwfoyw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yzmutecv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwvjfzv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3phfaesmm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igzhzjoq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3truwvmkb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lftylgyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gkhkbybd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mktnhojc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3blczcgkz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iqefduwz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xqhhdgvx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3unrxstzh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwyyqua.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wfbrylqd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gpedbgzw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qgdtjuxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aiqrpequ.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ssujdhcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrdxmdjr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxmuexvp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zjrgdtce.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3frstacgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pntxnptk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ldiatqhq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hrvehqtz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qedvswrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3eufkgcup.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zkgcixne.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edbbofhd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wdvwirzt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dbfvpuzk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfjltqo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsaoicn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzqablsv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vpioacsg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bxvgtvae.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ekmyhbit.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3njyrihvt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vrzcvyna.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yrlbcrpg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mirvnaps.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ydouavlu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhvpvpr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gdvhmzdp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ifcdqtwr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3juchvqqc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ljkgshab.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wmklhvxw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qtsnbkgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oxiglskc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nxotsjnx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3udbanlgc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ttbjdblf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aovkopqw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3swqomwbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zcvwtoha.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3giddygfp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nqljkoxe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgkglcra.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qiyngeii.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yqrgkroq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3weurscla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qapoomyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nrlindzc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3agjikasn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hnqqagyu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uvxpoxcd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fxcaxtfs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tseykhre.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3byulfgrs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcuagkso.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cyujjpwh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uimygsvf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bowoefsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rdntfzth.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ybjbcmaw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfoohql.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tuybzfju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wvnzkguu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zykerkaf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3poksdhcj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hhqucgqs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lewfkyib.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yeoxflui.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iqyhpuvv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sxiijfmc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gyemjnqt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nbocdpdm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dumdxfgt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3flkmxuvo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hzbfcvbl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3idxywdii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fczsqqlx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgcfoowb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ffetzoak.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xddxaayb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3edldzfag.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcareeoa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lbgrhqxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kbfqbowi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3juxvlpxw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3osfxestg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tdalllex.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vunljedg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ucyapxjs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mtnnvmbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3azlzgufb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3meungvcx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xhsnvmjt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oyktmory.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qpctzzdw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmgsstlz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wjmzsylq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kqgqvxjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ofzzssot.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pihkpids.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3effgzkds.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3picmhrjv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vlptedyn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsposldo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lppmsqby.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohkcirus.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgarwvmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kyujpjoh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hnzpdzkn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oszlolwu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yldudrxe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgfroqqf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dxyxqiei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvfkyw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvmmkpx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ihdgjaqe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wxahvetz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ayojqwat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tzfphcsi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzkeshj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3znmrmorm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nemmxddk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dcfaefau.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mfjaklfz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ilkkyhgl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rvmwzsqi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3moccmncc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xxaoyjyo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfpidn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3eomorapl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjqidepy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qgnndnck.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zhhavcal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3figrzrbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tyuvyegc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3njkuxfbl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nidvwwfm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wamgxiol.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hjfboqyq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gscezoet.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ocjbieko.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kjdgglrr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jlpjjzvr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbgtfjr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3syvqnmbf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3uegmygtf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wqygnnfa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lffwozeg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfejpqt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qrkuqvox.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3orlqtjnv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iawaoiea.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vvqqlokm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hmfuzqzg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qvqpltxu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bxcrkgly.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqopwuni.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pulxwclq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wtulqclu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qturtxji.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3becuadon.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnsawqbj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbleeovz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ijchdrxd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3btihnkba.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qvjihsda.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3klsxqkuh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pphksibn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rxewwwke.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wmpquzzo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkzrovmm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3slthpmaz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kjnogsvv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cxdifwrm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bvvomvfr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gudwtiug.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ddbldrje.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qypqmwhs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3picrboov.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fckkzfaw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rqkhpcvj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gdberufw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btimmznd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3phcnidzq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ppmvgzma.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kxpoqetg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3liucmwhi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jpzigvkj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tlauycsm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kvhjmpuj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qwzoprbb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtpzjoox.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gmftnahr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vddiabdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ubhrneze.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lfsjspox.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hlxzbhht.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ludkhfbt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3llwrozdd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pfvtieag.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bfkyhrvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggoalhsi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xnzfpjdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aikpjepo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jeptrige.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pjujisfw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfkcnrhb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jaheeszq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xhiwfxbp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3giprbyjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dneczqio.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwczdlon.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qqeobxlc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jygxjpvj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ckekovbk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qqfqyahj.html


<!-- 参考信息 -->